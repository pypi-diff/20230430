# Comparing `tmp/censoredsummarystats-1.0.1.tar.gz` & `tmp/censoredsummarystats-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-1.0.1.tar", max compression
+gzip compressed data, was "censoredsummarystats-1.1.0.tar", max compression
```

## Comparing `censoredsummarystats-1.0.1.tar` & `censoredsummarystats-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      588 2023-04-10 04:15:16.014879 censoredsummarystats-1.0.1/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0    54495 2023-04-21 01:24:00.486982 censoredsummarystats-1.0.1/censoredsummarystats/censoredsummarystats.py
--rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-1.0.1/LICENSE
--rw-r--r--   0        0        0      534 2023-04-21 01:26:56.290650 censoredsummarystats-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-1.0.1/README.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      256 2023-04-29 03:54:32.851141 censoredsummarystats-1.1.0/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0    50106 2023-04-29 23:52:07.081367 censoredsummarystats-1.1.0/censoredsummarystats/statistics.py
+-rw-r--r--   0        0        0     2291 2023-04-29 21:55:33.186386 censoredsummarystats-1.1.0/censoredsummarystats/utils.py
+-rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-1.1.0/LICENSE
+-rw-r--r--   0        0        0      558 2023-04-30 00:02:25.472559 censoredsummarystats-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-1.1.0/README.md
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 censoredsummarystats-1.1.0/PKG-INFO
```

### Comparing `censoredsummarystats-1.0.1/censoredsummarystats/censoredsummarystats.py` & `censoredsummarystats-1.1.0/censoredsummarystats/statistics.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,187 +2,119 @@
 """
 Created on Sun Mar 12 13:42:00 2023
 
 @author: KurtV
 """
 
 import numpy as np
+from utils import string_precision, numeric_precision
 
-#%% Utility Functions
+# Set default column names
+stat_col = 'Statistic'
+result_col = 'Result'
+censor_col = 'CensorComponent'
+numeric_col = 'NumericComponent'
+interval_col = 'Interval'
+left_boundary_col = '__LeftBoundary__'
+left_bound_col = '__LeftBound__'
+midpoint_col = '__MidPoint__'
+right_bound_col = '__RightBound__'
+right_boundary_col = '__RightBoundary__'
 
-#%%% Display
 
-def string_precision(value):
-    '''
-    A function that applies a specified rounding method that is value
-    dependent. This method is specifically designed to reflect the
-    typical measurement precision for water quality results. Depending on the
-    value, the rounding is either to a particular number of decimal places or
-    to a particular number of significant digits.
-
-    Parameters
-    ----------
-    value : float
-        Numeric value that will be rounded.
-
-    Returns
-    -------
-    string : string
-        The rounded value expressed as a string to the appropriate precision.
-
-    '''
-    
-    # Check for infinite values
-    if abs(value) == np.inf:
-        string = str(value)
-    # Values above 100 or are rounded to 100 should be expressed as integers
-    # with no more than 3 significant digits.
-    elif round(abs(value),1) >= 100:
-        string = str(int(float(f'{value:.3g}')))
-    # Values above 10 or are rounded to 10 should be rounded to 1 decimal place
-    elif round(abs(value),2) >= 10:
-        string = f'{value:.1f}'
-    # Values above 0.2 or are rounded to 0.2 should be rounded to 2 decimal places
-    elif round(abs(value),3) >= 0.2:
-        string = f'{value:.2f}'
-    # Values above 0.1 or are rounded to 0.1 should be rounded to 3 decimal places
-    elif round(abs(value),3) >= 0.1:
-        string = f'{value:.3f}'
-    # Values below 0.1 should be rounded to 2 significant digits
-    else:
-        string = f'{value:.2g}'
 
-    return string
+#%% Conversion between result and interval components
 
+#%%% Between result and censor/numeric components
 
-def numeric_precision(value):
-    '''
-    A function that returns a float data type from a rounding function instead
-    of a string data type.
-
-    Parameters
-    ----------
-    value : float
-        Float value that may have more decimal places or significant digits
-        than is appropriate
-
-    Returns
-    -------
-    float
-        Float value that is rounded appropriately
-
-    '''
-    
-    # Return the same rounded result as string_precision but as a float
-    return float(string_precision(value))
-
-def interval_notation(df, precision_rounding=True):
+def result_to_components(df,
+                         result_column):
     '''
-    This function creates a column that combines the interval components
-    into a single text notation for intervals.
+    A function that separates censors (<,≤,≥,>) from a result. Splitting the
+    censor component from the numeric component enables the use of numeric
+    data types. A result of <10 (string/text) is split into a censor component
+    of < (string/text) and a numeric component of 10 (float/decimal).
 
     Parameters
     ----------
     df : DataFrame
-        DataFrame containing columns for left/right bounds and boundaries
-    precision_rounding : boolean, optional
-        If True, a rounding method is applied to round results to have no more
-        decimals than what can be measured.
-        The default is True.
+        DataFrame containing a column to be split into components
+    result_column : string
+        Column name for the column that contains the results to be split
 
     Returns
     -------
     df : DataFrame
-        DataFrame identical to intput with additional column with combined
-        interval notation
+        Input DataFrame with two additional columns created for the censor
+        and numeric components
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
-    # Determine the left boundary symbol
-    df['Interval'] = np.where(df['LeftBoundary'] == 'Open', '(', '[')
-    
-    # Incorporate left and right bounds
-    if precision_rounding:
-        df['Interval'] += df['LeftBound'].apply(string_precision) + ', ' + df['RightBound'].apply(string_precision)
-    else:
-        df['Interval'] += df['LeftBound'].astype(str) + ', ' + df['RightBound'].astype(str)
+    # Ensure the value column is text/string data type.
+    df[result_column] = df[result_column].astype(str)
     
-    # Determine the right boundary symbol
-    df['Interval'] += np.where(df['RightBoundary'].isin(['Open']), ')', ']')
+    # Create censor and numeric columns from result column
+    df[censor_col] = df[result_column].str.extract(r'([<≤≥>])').fillna('')
+    df[numeric_col] = df[result_column].str.replace('<|≤|≥|>','',regex=True).astype(float)
     
     return df
 
-#%%% Convert between, results, components, intervals
-
-def result_to_components(df,
-                         value_column,
-                         censor_column = 'CensorComponent',
-                         numeric_column = 'NumericComponent'):
+def components_to_result(df,
+                         precision_rounding = True):
     '''
-    A function that separates censors (<,≤,≥,>) from a result. Splitting the
-    censor component from the numeric component enables the use of numeric
-    data types. A result of <10 (string/text) is split into a censor component
-    of < (string/text) and a numeric component of 10 (float/decimal).
+    A function that combines censor and numeric components into a combined
+    string/text result.
 
     Parameters
     ----------
     df : DataFrame
-        DataFrame containing a column to be split into components
-    value_column : string
-        Column name for the column that contains the results to be split
-    censor_column : string, optional
-        Column name that will be assigned to the censor component column
-        The default is 'CensorComponent'.
-    numeric_column : string, optional
-        Column name that will be assigned to the numeric component column
-        The default is 'NumericComponent'.
+        DataFrame containing censor and numeric columns that will be combined
+    precision_rounding : boolean, optional
+        If True, a rounding method is applied to round results to have no more
+        decimals than what can be measured.
+        The default is True.
 
     Returns
     -------
     df : DataFrame
-        Input DataFrame with two additional columns created for the censor
-        and numeric components
+        Input DataFrame that contains a new string/text column that combines
+        the censor and numeric components of a result
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
-    # Ensure the value column is text/string data type.
-    df[value_column] = df[value_column].astype(str)
-    
-    # Create censor and numeric columns from result column
-    df[censor_column] = df[value_column].str.extract(r'([<≤≥>])').fillna('')
-    df[numeric_column] = df[value_column].str.replace('<|≤|≥|>','',regex=True).astype(float)
+    # Combine the censor and numeric components to create a combined result
+    # Apply the appropriate rounding functions if precision_rounding is True
+    if precision_rounding:
+        df[result_col] = df[censor_col] + df[numeric_col].apply(string_precision,thousands_comma=True)
+        df[numeric_col] = df[numeric_col].apply(numeric_precision)
+    else:
+        df[result_col] = df[censor_col] + df[numeric_col].astype(str)
     
     return df
 
+#%%% Between censor/numeric components and interval components
+
 def components_to_interval(df,
-                           censor_column = 'CensorComponent',
-                           numeric_column = 'NumericComponent',
                            include_negative_interval = False):
     '''
     A function that utilises the censor and numeric components to convert
     each result into interval notation. Four columns are created to store
     the interval information including left/right bounds and whether the
     endpoints/boundaries are inclusive or exclusive (e.g., <1 vs ≤1)
 
     Parameters
     ----------
     df : DataFrame
         DataFrame containing the censor and numeric columns
-    censor_column : string, optional
-        Column name for the column containing the censor component
-        The default is 'CensorComponent'.
-    numeric_column : string, optional
-        Column name for the column containing the numeric component
-        The default is 'NumericComponent'.
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
         e.g., <0.5 would be converted to [0,5).
         The default is False.
     
@@ -200,66 +132,56 @@
         values for the results
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
-    # Define boundary values as string or integers
-    closed_boundary = 'Closed'
-    open_boundary = 'Open'
-    
     # Define where the left bound is closed
-    df['LeftBoundary'] = np.where(df[censor_column].isin(['','≥']),
-                                  closed_boundary, open_boundary)
+    df[left_boundary_col] = np.where(df[censor_col].isin(['','≥']),
+                                  'Closed', 'Open')
     
     # Define where left bound is unlimited
-    df['LeftBound'] = np.where(df[censor_column].isin(['<','≤']),
-                               -np.inf, df[numeric_column])
+    df[left_bound_col] = np.where(df[censor_col].isin(['<','≤']),
+                               -np.inf, df[numeric_col])
     
     # Define where right bound is unlimited
-    df['RightBound'] = np.where(df[censor_column].isin(['≥','>']),
-                                np.inf, df[numeric_column])
+    df[right_bound_col] = np.where(df[censor_col].isin(['≥','>']),
+                                np.inf, df[numeric_col])
     
     # Define where the right bound is closed
-    df['RightBoundary'] = np.where(df[censor_column].isin(['≤','']),
-                                   closed_boundary, open_boundary)
+    df[right_boundary_col] = np.where(df[censor_col].isin(['≤','']),
+                                   'Closed', 'Open')
     
+    # If left censored are assumed positive
     if not include_negative_interval:
-        if df['LeftBound'].between(-np.inf, 0, inclusive='neither').any():
+        # Check for any negative values (exclude -inf)
+        if df[left_bound_col].between(-np.inf, 0, inclusive='neither').any():
             raise ValueError('Negative values exist in the data. Resolve negative'
                              'values or set include_negative_interval to True')
-        
-        condition = (df['LeftBound'] < 0)
-        df['LeftBoundary'] = np.where(condition, 'Closed', df['LeftBoundary'])
-        df['LeftBound'] = np.where(condition, 0.0, df['LeftBound'])
+        # Set any -inf left bounds to 0 with closed boundary
+        condition = (df[left_bound_col] < 0)
+        df[left_boundary_col] = np.where(condition, 'Closed', df[left_boundary_col])
+        df[left_bound_col] = np.where(condition, 0.0, df[left_bound_col])
     
     return df
 
 
 def interval_to_components(df,
-                           censor_column = 'CensorComponent',
-                           numeric_column = 'NumericComponent',
                            focus_high_potential = True,
                            include_negative_interval = False,
                            precision_tolerance_to_drop_censor = 0.25):
     '''
     A function that determines the censor and numeric components
     from intervals
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains interval information
-    censor_column : string, optional
-        Column name to give the column containing the censor component
-        The default is 'CensorComponent'.
-    numeric_column : string, optional
-        Column name to give the column containing the numeric component
-        The default is 'NumericComponent'.
     focus_high_potential : boolean, optional
         If True, then information on the highest potential result will be
         focused over the lowest potential result.
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
@@ -281,253 +203,239 @@
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
     # Determine the midpoint for the interval if finite interval
-    df['Midpoint'] = np.where((df['LeftBound'] > -np.inf) & (df['RightBound'] < np.inf),
-                              0.5 * (df['LeftBound'] + df['RightBound']),
+    df[midpoint_col] = np.where((df[left_bound_col] > -np.inf) & (df[right_bound_col] < np.inf),
+                              0.5 * (df[left_bound_col] + df[right_bound_col]),
                               np.nan)
     
     
     # Define the conditions for an uncensored result
     conditions = [
         # If the bounds are equal, then the result is uncensored
-        (df['LeftBound'] == df['RightBound']),
+        (df[left_bound_col] == df[right_bound_col]),
         # If the bounds are finite and the interval is within the precision tolerance, avoid the use of censors
-        (df['RightBound'] - df['Midpoint']) <= df['Midpoint'] * precision_tolerance_to_drop_censor
+        (df[right_bound_col] - df[midpoint_col]) <= df[midpoint_col] * precision_tolerance_to_drop_censor
         ]
     
     censor_results = [
         '',
         ''
         ]
     
     numeric_results =[
-        df['Midpoint'],
-        df['Midpoint']
+        df[midpoint_col],
+        df[midpoint_col]
         ]
     
     # If focused on the highest potential result
     if focus_high_potential:
         # Set censor and numeric components for each condition
         conditions += [
             # If there is an infinite right bound, the result is right censored
-            (df['RightBound'] == np.inf) & (df['LeftBound'] > -np.inf) & (df['LeftBoundary'] == 'Open'),
-            (df['RightBound'] == np.inf) & (df['LeftBound'] > -np.inf) & (df['LeftBoundary'] == 'Closed'),
+            (df[right_bound_col] == np.inf) & (df[left_bound_col] > -np.inf) & (df[left_boundary_col] == 'Open'),
+            (df[right_bound_col] == np.inf) & (df[left_bound_col] > -np.inf) & (df[left_boundary_col] == 'Closed'),
             # Otherwise, the result should be left censored
-            (df['RightBound'] < np.inf) & (df['RightBoundary'] == 'Open'),
-            (df['RightBound'] < np.inf) & (df['RightBoundary'] == 'Closed')
+            (df[right_bound_col] < np.inf) & (df[right_boundary_col] == 'Open'),
+            (df[right_bound_col] < np.inf) & (df[right_boundary_col] == 'Closed')
             ]
         
         censor_results += [
             '>',
             '≥',
             '<',
             '≤'
             ]
         
         numeric_results += [
-            df['LeftBound'],
-            df['LeftBound'],
-            df['RightBound'],
-            df['RightBound']
+            df[left_bound_col],
+            df[left_bound_col],
+            df[right_bound_col],
+            df[right_bound_col]
             ]
     # Else focused on the lowest potential result
     else:
         # Determine the lower bound
         if include_negative_interval:
             lower_bound = -np.inf
         else:
             lower_bound = 0.0
         # Set censor and numeric components for each condition
         conditions += [
             # If the left bound is identical to the lowest potential lower bound,
             # then the result is left censored
-            (df['LeftBound'] == lower_bound) & (df['RightBound'] < np.inf) & (df['RightBoundary'] == 'Open'),
-            (df['LeftBound'] == lower_bound) & (df['RightBound'] < np.inf) & (df['RightBoundary'] == 'Closed'),
+            (df[left_bound_col] == lower_bound) & (df[right_bound_col] < np.inf) & (df[right_boundary_col] == 'Open'),
+            (df[left_bound_col] == lower_bound) & (df[right_bound_col] < np.inf) & (df[right_boundary_col] == 'Closed'),
             # Otherwise, the result should be right censored
-            (df['LeftBound'] > lower_bound) & (df['LeftBoundary'] == 'Open'),
-            (df['LeftBound'] > lower_bound) & (df['LeftBoundary'] == 'Closed')
+            (df[left_bound_col] > lower_bound) & (df[left_boundary_col] == 'Open'),
+            (df[left_bound_col] > lower_bound) & (df[left_boundary_col] == 'Closed')
             ]
         
         censor_results += [
             '<',
             '≤',
             '>',
             '≥'
             ]
         
         numeric_results += [
-            df['RightBound'],
-            df['RightBound'],
-            df['LeftBound'],
-            df['LeftBound']
+            df[right_bound_col],
+            df[right_bound_col],
+            df[left_bound_col],
+            df[left_bound_col]
             ]
     
     # Determine the censor and numeric components
     # If no condition is met, default to <> and NaN
-    df[censor_column] = np.select(conditions, censor_results, '<>')
-    df[numeric_column] = np.select(conditions, numeric_results, np.nan)
-    
-    # Only return the censor and numeric columns
-    df = df[['Interval',censor_column,numeric_column]]
-    
-    # Reset index
-    df = df.reset_index()
+    df[censor_col] = np.select(conditions, censor_results, '<>')
+    df[numeric_col] = np.select(conditions, numeric_results, np.nan)
     
     return df
 
+#%%% Interval components to interval string
 
-def components_to_result(df,
-                         censor_column = 'CensorComponent',
-                         numeric_column = 'NumericComponent',
-                         precision_rounding = True):
+def interval_notation(df,
+                      precision_rounding=True):
     '''
-    A function that combines censor and numeric components into a combined
-    string/text result.
+    This function creates a column that combines the interval components
+    into a single text notation for intervals.
 
     Parameters
     ----------
     df : DataFrame
-        DataFrame containing censor and numeric columns that will be combined
-    censor_column : string, optional
-        Column name for the column containing the censor component
-        The default is 'CensorComponent'.
-    numeric_column : string, optional
-        Column name for the column containing the numeric component
-        The default is 'NumericComponent'.
+        DataFrame containing columns for left/right bounds and boundaries
     precision_rounding : boolean, optional
         If True, a rounding method is applied to round results to have no more
         decimals than what can be measured.
         The default is True.
 
     Returns
     -------
     df : DataFrame
-        Input DataFrame that contains a new string/text column that combines
-        the censor and numeric components of a result
+        DataFrame identical to intput with additional column with combined
+        interval notation
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
-    # Combine the censor and numeric components to create a combined result
-    # Apply the appropriate rounding functions if precision_rounding is True
+    # Determine the left boundary symbol
+    df[interval_col] = np.where(df[left_boundary_col] == 'Open', '(', '[')
+    
+    # Incorporate left and right bounds
     if precision_rounding:
-        df['Result'] = df[censor_column] + df[numeric_column].apply(string_precision)
-        df[numeric_column] = df[numeric_column].apply(numeric_precision)
+        df[interval_col] += df[left_bound_col].apply(string_precision) + ', ' + df[right_bound_col].apply(string_precision)
     else:
-        df['Result'] = df[censor_column] + df[numeric_column].astype(str)
+        df[interval_col] += df[left_bound_col].astype(str) + ', ' + df[right_bound_col].astype(str)
+    
+    # Determine the right boundary symbol
+    df[interval_col] += np.where(df[right_boundary_col].isin(['Open']), ')', ']')
     
     return df
 
+
 #%% Maximum Result
 
 def maximum_interval(df,
-                     groupby_columns = None):
+                     groupby_columns):
     '''
     A function that analyses the interval notation form of results returned
     from components_to_interval to generate a new interval for the maximum. Groups
     of results can be defined by including the columns that should be used to
     create groups.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains results in a specific interval notation.
-    groupby_columns : list of strings, optional
+    groupby_columns : list of strings
         List of column names that should be used to create groups.
-        The default is None.
 
     Returns
     -------
     df : DataFrame
         DataFrame that has the interval for the maximum (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy().reset_index()
     
-    # If no groups create empty list
-    if groupby_columns == None:
-        groupby_columns = []
-    
     # Create column that indicates the generated statistic and append to grouping list
-    df['Statistic'] = 'Maximum'
-    groupby_columns.append('Statistic')
+    df[stat_col] = 'Maximum'
+    groupby_columns.append(stat_col)
     
     # Determine left bound and boundary for maximum for each group.
     
     # Consider the maximum bound for each left boundary option to determine
     # whether the bound should be open or closed.
-    left = df.groupby(groupby_columns+['LeftBoundary'])['LeftBound'].max().unstack('LeftBoundary')
+    left = df.groupby(groupby_columns+[left_boundary_col])[left_bound_col].max().unstack(left_boundary_col)
     # Create missing columns
     for item in ['Open','Closed']:
         if item not in left.columns:
             left[item] = np.nan
     # Use the maximum closed boundary if there are no open boundaries or
     # if the closed boundary is larger than the largest open boundary
     condition = (left['Closed'] > left['Open']) | (left['Open'].isna())
-    left['LeftBoundary'] = np.where(condition,'Closed','Open')
-    left['LeftBound'] = np.where(condition,left['Closed'],left['Open'])
-    left = left[['LeftBoundary','LeftBound']]
+    left[left_boundary_col] = np.where(condition,'Closed','Open')
+    left[left_bound_col] = np.where(condition,left['Closed'],left['Open'])
+    left = left[[left_boundary_col,left_bound_col]]
     
     # Determine right bound and boundary for maximum for each group.
     
     # Consider the maximum bound for each right boundary option to determine
     # whether the bound should be open or closed.
-    right = df.groupby(groupby_columns+['RightBoundary'])['RightBound'].max().unstack('RightBoundary')
+    right = df.groupby(groupby_columns+[right_boundary_col])[right_bound_col].max().unstack(right_boundary_col)
     # Create missing columns
     for item in ['Open','Closed']:
         if item not in right.columns:
             right[item] = np.nan
     # Use the maximum closed boundary if there are no open boundaries or
     # if the closed boundary is larger than or equal to the largest open boundary
     condition = (right['Closed'] >= right['Open']) | (right['Open'].isna())
-    right['RightBound'] = np.where(condition,right['Closed'],right['Open'])
-    right['RightBoundary'] = np.where(condition,'Closed','Open')
-    right = right[['RightBound','RightBoundary']]
+    right[right_bound_col] = np.where(condition,right['Closed'],right['Open'])
+    right[right_boundary_col] = np.where(condition,'Closed','Open')
+    right = right[[right_bound_col,right_boundary_col]]
     
     # Merge the two boundaries to create the interval for the maximum
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
+    # Reset index
+    df = df.reset_index()
+    
     return df
 
 def maximum(df,
+            result_col,
             groupby_columns = None,
-            values = ['CensorComponent','NumericComponent'],
             include_negative_interval = False,
             precision_tolerance_to_drop_censor = 0.25,
             precision_rounding = True):
     '''
     A function that combines the relevant maximum and utility functions to
     generate the maxima results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
+    result_col : string
+        The column name for the column that contain the results as text.
+        Only four possible censors should be used (<,≤,≥,>).
     groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. A maximum
         will be found within each group. Multiple lists can be supplied to
         perform sequential maxima before converting intervals to a result.
         The default is None.
-    values : list of strings, optional
-        The column name(s) for the column(s) that contain the results. If a 
-        single column name is given, it is assumed that the column contains
-        combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,,≥,>)
-        and the second should contain only numeric data.
-        The default is ['CensorComponent','NumericComponent'].
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
         e.g., <0.5 would be converted to [0,5).
         This setting only affects results if focus_high_potential is False.
         The default is False.
@@ -548,151 +456,150 @@
         DataFrame that contains a column with the relevant maximum or maxima
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
-    # If single result column provided, then split column
-    if len(values) == 1:
-        censor_column = 'CensorComponent'
-        numeric_column = 'NumericComponent'
-        df = result_to_components(df,values[0])
-    # Else define the names to use for the censor and numeric columns
-    else:
-        censor_column = values[0]
-        numeric_column = values[1]
+    # Split the result into censor and numeric components
+    df = result_to_components(df,result_col)
     
     # Convert the results from censor and numeric components to an interval representation
-    df = components_to_interval(df, censor_column, numeric_column, include_negative_interval)
+    df = components_to_interval(df, include_negative_interval)
+    
+    # Using the intervals, determine the range of possible maxima
     
-    # If multiple groupby lists, then cycle through them in order
-    if isinstance(groupby_columns[0],list):
+    # If there are no groupby-columns, then take max of all results
+    if not groupby_columns:
+        df = maximum_interval(df, groupby_columns=[])
+    # If the groupby_columns is a list of lists, then perform multiple maximums
+    elif isinstance(groupby_columns[0],list):
         for grouping in groupby_columns:
             # Using the intervals, determine the range of possible maxima
             df = maximum_interval(df, grouping)
+    # Else the groupby_columns is a list of column names
     else:
-        # Using the intervals, determine the range of possible maxima
-        df = maximum_interval(df, grouping)
-    
-    # Create interval notation for the maximum
-    df = interval_notation(df, precision_rounding)
+        df = maximum_interval(df, groupby_columns)
     
     # Convert the interval for the maximum into censor and numeric notation
-    df = interval_to_components(df, censor_column, numeric_column,
+    df = interval_to_components(df,
                                 focus_high_potential = True,
                                 include_negative_interval = include_negative_interval,
                                 precision_tolerance_to_drop_censor = precision_tolerance_to_drop_censor)
     
+    # Create interval notation for the maximum
+    df = interval_notation(df, precision_rounding)
+    
     # Combine the censor and numeric components into a result
-    df = components_to_result(df, censor_column, numeric_column, precision_rounding)
+    df = components_to_result(df, precision_rounding)
+    
+    # Drop working columns
+    df = df.drop(df.filter(regex='__').columns, axis=1)
+    
+    # Reorder columns
+    for col in [stat_col,result_col,censor_col,numeric_col,interval_col]:
+        df[col] = df.pop(col)
     
     return df
 
 #%% Minimum Result
 
 def minimum_interval(df,
-                     groupby_columns = None):
+                     groupby_columns):
     '''
     A function that analyses the interval notation form of results returned
     from components_to_interval to generate a new interval for the minimum. Groups
     of results can be defined by including the columns that should be used to
     create groups.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains results in a specific interval notation.
-    groupby_columns : list of strings, optional
+    groupby_columns : list of strings
         List of column names that should be used to create groups.
-        The default is None.
 
     Returns
     -------
     df : DataFrame
         DataFrame that has the interval for the minimum (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy().reset_index()
     
-    # If no groups create empty list
-    if groupby_columns == None:
-        groupby_columns = []
-        
     # Create column that indicates the generated statistic and append to grouping list
-    df['Statistic'] = 'Minimum'
-    groupby_columns.append('Statistic')
+    df[stat_col] = 'Minimum'
+    groupby_columns.append(stat_col)
     
     # Determine left bound and boundary for minimum for each group.
     
     # Consider the minimum bound for each left boundary option to determine
     # whether the bound should be open or closed.
-    left = df.groupby(groupby_columns+['LeftBoundary'])['LeftBound'].min().unstack('LeftBoundary')
+    left = df.groupby(groupby_columns+[left_boundary_col])[left_bound_col].min().unstack(left_boundary_col)
     # Create missing columns
     for item in ['Open','Closed']:
         if item not in left.columns:
             left[item] = np.nan
     # Use the minimum closed boundary if there are no open boundaries or
     # if the closed boundary is less than or equal to the least open boundary
     condition = (left['Closed'] <= left['Open']) | (left['Open'].isna())
-    left['LeftBoundary'] = np.where(condition,'Closed','Open')
-    left['LeftBound'] = np.where(condition,left['Closed'],left['Open'])
-    left = left[['LeftBoundary','LeftBound']]
+    left[left_boundary_col] = np.where(condition,'Closed','Open')
+    left[left_bound_col] = np.where(condition,left['Closed'],left['Open'])
+    left = left[[left_boundary_col,left_bound_col]]
     
     # Determine right bound and boundary for minimum for each group.
     
     # Consider the minimum bound for each right boundary option to determine
     # whether the bound should be open or closed.
-    right = df.groupby(groupby_columns+['RightBoundary'])['RightBound'].min().unstack('RightBoundary')
+    right = df.groupby(groupby_columns+[right_boundary_col])[right_bound_col].min().unstack(right_boundary_col)
     # Create missing columns
     for item in ['Open','Closed']:
         if item not in right.columns:
             right[item] = np.nan
     # Use the minimum closed boundary if there are no open boundaries or
     # if the closed boundary is less than the least open boundary
     condition = (right['Closed'] < right['Open']) | (right['Open'].isna())
-    right['RightBound'] = np.where(condition,right['Closed'],right['Open'])
-    right['RightBoundary'] = np.where(condition,'Closed','Open')
-    right = right[['RightBound','RightBoundary']]
+    right[right_bound_col] = np.where(condition,right['Closed'],right['Open'])
+    right[right_boundary_col] = np.where(condition,'Closed','Open')
+    right = right[[right_bound_col,right_boundary_col]]
     
     # Merge the two boundaries to create the interval for the minimum
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
+    # Reset index
+    df = df.reset_index()
+    
     return df
 
 def minimum(df,
+            result_col,
             groupby_columns = None,
-            values = ['CensorComponent','NumericComponent'],
             include_negative_interval = False,
             precision_tolerance_to_drop_censor = 0.25,
             precision_rounding = True):
     '''
     A function that combines the relevant minimum and utility functions to
     generate the minima results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
+    result_col : string
+        The column name for the column that contain the results as text.
+        Only four possible censors should be used (<,≤,≥,>).
     groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. A minimum
         will be found within each group. Multiple lists can be supplied to
         perform sequential minima before converting intervals to a result.
         The default is None.
-    values : list of strings, optional
-        The column name(s) for the column(s) that contain the results. If a 
-        single column name is given, it is assumed that the column contains
-        combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,,≥,>)
-        and the second should contain only numeric data.
-        The default is ['CensorComponent','NumericComponent'].
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
         e.g., <0.5 would be converted to [0,5).
         This setting only affects results if focus_high_potential is False.
         The default is False.
@@ -713,139 +620,140 @@
         DataFrame that contains a column with the relevant minimum or minima
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
-    # If single result column provided, then split column
-    if len(values) == 1:
-        censor_column = 'CensorComponent'
-        numeric_column = 'NumericComponent'
-        df = result_to_components(df,values[0])
-    # Else define the names to use for the censor and numeric columns
-    else:
-        censor_column = values[0]
-        numeric_column = values[1]
+    # Split the result into censor and numeric components
+    df = result_to_components(df,result_col)
     
     # Convert the results from censor and numeric components to an interval representation
-    df = components_to_interval(df, censor_column, numeric_column, include_negative_interval)
+    df = components_to_interval(df, include_negative_interval)
     
-    # If multiple groupby lists, then cycle through them in order
-    if isinstance(groupby_columns[0],list):
+    # Using the intervals, determine the range of possible minima
+    
+    # If there are no groupby-columns, then take min of all results
+    if not groupby_columns:
+        df = minimum_interval(df, groupby_columns=[])
+    # If the groupby_columns is a list of lists, then perform multiple minimums
+    elif isinstance(groupby_columns[0],list):
         for grouping in groupby_columns:
-            # Using the intervals, determine the range of possible minima
+            # Using the intervals, determine the range of possible maxima
             df = minimum_interval(df, grouping)
+    # Else the groupby_columns is a list of column names
     else:
-        # Using the intervals, determine the range of possible minima
-        df = minimum_interval(df, grouping)
-    
-    # Create interval notation for the minimum
-    df = interval_notation(df, precision_rounding)
+        df = minimum_interval(df, groupby_columns)
     
     # Convert the interval for the minimum into censor and numeric notation
-    df = interval_to_components(df, censor_column, numeric_column,
+    df = interval_to_components(df,
                                 focus_high_potential = False,
                                 include_negative_interval = include_negative_interval,
                                 precision_tolerance_to_drop_censor = precision_tolerance_to_drop_censor)
     
+    # Create interval notation for the minimum
+    df = interval_notation(df, precision_rounding)
+    
     # Combine the censor and numeric components into a result
-    df = components_to_result(df, censor_column, numeric_column, precision_rounding)
+    df = components_to_result(df, censor_col, numeric_col, precision_rounding)
+    
+    # Drop working columns
+    df = df.drop(df.filter(regex='__').columns, axis=1)
+    
+    # Reorder columns
+    for col in [stat_col,result_col,censor_col,numeric_col,interval_col]:
+        df[col] = df.pop(col)
     
     return df
 
 #%% Average Result
 
 def average_interval(df,
-                     groupby_columns = None):
+                     groupby_columns):
     '''
     A function that analyses the interval notation form of results returned
     from components_to_interval to generate a new interval for the average. Groups
     of results can be defined by including the columns that should be used to
     create groups.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains results in a specific interval notation.
-    groupby_columns : list of strings, optional
+    groupby_columns : list of strings
         List of column names that should be used to create groups.
-        The default is None.
 
     Returns
     -------
     df : DataFrame
         DataFrame that has the interval for the average (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy().reset_index()
     
-    # If no groups create empty list
-    if groupby_columns == None:
-        groupby_columns = []
-    
     # Create column that indicates the generated statistic and append to grouping list
-    df['Statistic'] = 'Average'
-    groupby_columns.append('Statistic')
+    df[stat_col] = 'Average'
+    groupby_columns.append(stat_col)
     
     # Change notation of 'Closed' and 'Open' boundaries to 0 and 1, respectively
     # The presence of any open boundaries on one side ensure that the interval for the average is also
     # open on that side
-    df[['LeftBoundary','RightBoundary']] = df[['LeftBoundary','RightBoundary']].replace(['Closed','Open'], [0,1])
+    df[[left_boundary_col,right_boundary_col]] = df[[left_boundary_col,right_boundary_col]].replace(['Closed','Open'], [0,1])
     
     # Get the left/right bounds of the average by averaging bounds within the group
     # Determine whether any Open (now value of 1) boundaries exist. If there are
     # any open boundaries used in the average, then the resulting average will be open
-    df = df.groupby(groupby_columns).agg(LeftBoundary = ('LeftBoundary', 'max'),
-                                         Minimum = ('LeftBound','min'),
-                                         LeftBound = ('LeftBound','mean'),
-                                         RightBound = ('RightBound','mean'),
-                                         Maximum = ('RightBound','max'),
-                                         RightBoundary = ('RightBoundary','max'))
+    df = df.groupby(groupby_columns).agg(**{
+                            left_boundary_col: (left_boundary_col, 'max'),
+                            '__Minimum__': (left_bound_col,'min'),
+                            left_bound_col: (left_bound_col,'mean'),
+                            right_bound_col: (right_bound_col,'mean'),
+                            '__Maximum__': (left_bound_col,'max'),
+                            right_boundary_col: (right_boundary_col,'max')
+                            })
     
     # Replace integers with text for boundaries
-    df[['LeftBoundary','RightBoundary']] = df[['LeftBoundary','RightBoundary']].replace([0,1], ['Closed','Open'])
+    df[[left_boundary_col,right_boundary_col]] = df[[left_boundary_col,right_boundary_col]].replace([0,1], ['Closed','Open'])
     
     # Means with infinite values produce nan values rather than np.inf values
     # Convert nan to inf only if infinite values are included in the mean
-    df['LeftBound'] = np.where(df['Minimum'] == -np.inf, -np.inf, df['LeftBound'])
-    df['RightBound'] = np.where(df['Maximum'] == np.inf, np.inf, df['RightBound'])
+    df[left_bound_col] = np.where(df['__Minimum__'] == -np.inf, -np.inf, df[left_bound_col])
+    df[right_bound_col] = np.where(df['__Maximum__'] == np.inf, np.inf, df[right_bound_col])
+    
+    # Reset index
+    df = df.reset_index()
     
     return df
 
 def average(df,
+            result_col,
             groupby_columns = None,
-            values = ['CensorComponent','NumericComponent'],
             focus_high_potential = True,
             include_negative_interval = False,
             precision_tolerance_to_drop_censor = 0.25,
             precision_rounding = True):
     '''
     A function that combines the relevant average and utility functions to
     generate the average results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
+    result_col : string
+        The column name for the column that contain the results as text.
+        Only four possible censors should be used (<,≤,≥,>).
     groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. An average
         will be found within each group. Multiple lists can be supplied to
         perform sequential averaging before converting intervals to a result.
         The default is None.
-    values : list of strings, optional
-        The column name(s) for the column(s) that contain the results. If a 
-        single column name is given, it is assumed that the column contains
-        combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,,≥,>)
-        and the second should contain only numeric data.
-        The default is ['CensorComponent','NumericComponent'].
     focus_high_potential : boolean, optional
         If True, then information on the highest potential result will be
         focused over the lowest potential result.
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
@@ -869,261 +777,271 @@
         DataFrame that contains calculated averages
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
-    # If single result column provided, then split column
-    if len(values) == 1:
-        censor_column = 'CensorComponent'
-        numeric_column = 'NumericComponent'
-        df = result_to_components(df,values[0])
-    # Else define the names to use for the censor and numeric columns
-    else:
-        censor_column = values[0]
-        numeric_column = values[1]
+    # Split the result into censor and numeric components
+    df = result_to_components(df,result_col)
     
     # Convert the results from censor and numeric components to an interval representation
-    df = components_to_interval(df, censor_column, numeric_column, include_negative_interval)
+    df = components_to_interval(df, include_negative_interval)
     
-    # If multiple groupby lists, then cycle through them in order
-    if isinstance(groupby_columns[0],list):
+    # Using the intervals, determine the range of possible averages
+    
+    # If there are no groupby-columns, then take average of all results
+    if not groupby_columns:
+        df = average_interval(df, groupby_columns=[])
+    # If the groupby_columns is a list of lists, then perform multiple averages
+    elif isinstance(groupby_columns[0],list):
         for grouping in groupby_columns:
-            # Using the intervals, determine the range of possible averages
+            # Using the intervals, determine the range of possible maxima
             df = average_interval(df, grouping)
+    # Else the groupby_columns is a list of column names
     else:
-        # Using the intervals, determine the range of possible averages
-        df = average_interval(df, grouping)
+        df = average_interval(df, groupby_columns)
     
-    # Create interval notation for the minimum
-    df = interval_notation(df, precision_rounding)
-    
-    # Convert the interval for the minimum into censor and numeric notation
-    df = interval_to_components(df, censor_column, numeric_column,
+    # Convert the interval for the average into censor and numeric notation
+    df = interval_to_components(df,
                                 focus_high_potential = focus_high_potential,
                                 include_negative_interval = include_negative_interval,
                                 precision_tolerance_to_drop_censor = precision_tolerance_to_drop_censor)
     
+    # Create interval notation for the average
+    df = interval_notation(df, precision_rounding)
+    
     # Combine the censor and numeric components into a result
-    df = components_to_result(df, censor_column, numeric_column, precision_rounding)
+    df = components_to_result(df, precision_rounding)
+    
+    # Drop working columns
+    df = df.drop(df.filter(regex='__').columns, axis=1)
+    
+    # Reorder columns
+    for col in [stat_col,result_col,censor_col,numeric_col,interval_col]:
+        df[col] = df.pop(col)
     
     return df
 
 #%% Percentile Result
 
 def percentile_interval(df,
+                        groupby_columns,
                         percentile,
-                        method = 'hazen',
-                        groupby_columns = None):
+                        method = 'hazen',):
     '''
     A function that analyses the interval notation form of results returned
     from components_to_interval to generate a new interval for percentiles. Groups
     of results can be defined by including the columns that should be used to
     create groups.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains results in a specific interval notation.
+    groupby_columns : list of strings
+        List of column names that should be used to create groups.
     percentile : float
         The desired percentile. Values should be between 0 and 100.
     method : string
         The percentile method. The options and definitions come from:
             https://environment.govt.nz/assets/Publications/Files/hazen-percentile-calculator-2.xls
             Options include the following, ordered from largest to smallest result.
             - weiball
             - tukey
             - blom
             - hazen
             - excel
         The default is hazen.
-    groupby_columns : list of strings, optional
-        List of column names that should be used to create groups.
-        The default is None.
 
     Returns
     -------
     df : DataFrame
         DataFrame that has the interval for the percentile (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy().reset_index()
     
-    # If no groups create empty list
-    if groupby_columns == None:
-        groupby_columns = []
-    
     # Check the percentile is between 0 and 1
     if percentile < 0 or percentile > 100:
         raise Exception(f'Percentile out of range. Attempted percentile: {percentile}')
     
     # Create column that indicates the generated statistic and append to grouping list
-    df['Statistic'] = f'Percentile-{percentile}'
-    groupby_columns.append('Statistic')
+    df[stat_col] = f'Percentile-{percentile}'
+    groupby_columns.append(stat_col)
     
     # Convert percentile to be between 0 and 1
     percentile = percentile/100
     
     # Determine size of each group
-    df['Size'] = df.groupby(groupby_columns)['SiteID'].transform('size')
+    df['__Size__'] = df.groupby(groupby_columns).transform('size')
     
     # Set values for percentile methods
     method_dict = {'weiball':0.0, 'tukey':1/3, 'blom':3/8, 'hazen':1/2, 'excel':1.0}
     # https://en.wikipedia.org/wiki/Percentile
     C = method_dict[method]
     
     # Calculate minimum data size for percentile method to 
     # ensure rank is at least 1 and no more than len(data)
     minimum_size = round(C + (1-C)*max((1-percentile)/percentile,
                                        percentile/(1-percentile)),10)
     
     # Only consider groups that meet the minimum size requirement
-    df = df[df['Size'] >= minimum_size]
+    df = df[df['__Size__'] >= minimum_size]
     
     # Determine left bound and boundary for each group
     
     # Change notation of 'Closed' and 'Open' boundaries to 0 and 1, respectively
     # Use 0 for closed to ensure that closed boundaries are sorted less than open
     # boundaries when the left bound is tied
-    df['LeftBoundary'] = df['LeftBoundary'].replace(['Closed','Open'], [0,1])
+    df[left_boundary_col] = df[left_boundary_col].replace(['Closed','Open'], [0,1])
     
     # Sort left bound values
-    left = df.copy()[groupby_columns+['Size','LeftBoundary','LeftBound']].sort_values(by=['LeftBound','LeftBoundary'])
+    left = df.copy()[groupby_columns+['__Size__',left_boundary_col,left_bound_col]].sort_values(by=[left_bound_col,left_boundary_col])
     
     # Add index for each group
-    left['Index'] = left.groupby(groupby_columns).cumcount() + 1
+    left['__Index__'] = left.groupby(groupby_columns).cumcount() + 1
     
     # Determine the rank in each group for the percentile
-    left['Rank'] = round(C + percentile*(left['Size'] + 1 - 2*C),8)
+    left['__Rank__'] = round(C + percentile*(left['__Size__'] + 1 - 2*C),8)
     
     # Generate proximity of each result to percentile rank using the index
-    left['Proximity'] = 0
+    left['__Proximity__'] = 0
     
     conditions = [
         # If the percentile rank is a whole number, then use that index result
-        (left['Rank'] == left['Index']),
+        (left['__Rank__'] == left['__Index__']),
         # If the percentile rank is less than 1 above the index value,
         # then assign the appropriate contribution to that index value
-        (left['Rank'] - left['Index']).between(0,1,inclusive='neither'),
+        (left['__Rank__'] - left['__Index__']).between(0,1,inclusive='neither'),
         # If the percentile rank is less than 1 below the index value,
         # then assign the appropriate contribution to that index value
-        (left['Index'] - left['Rank']).between(0,1,inclusive='neither')
+        (left['__Index__'] - left['__Rank__']).between(0,1,inclusive='neither')
         ]
     
     results = [
         1,
-        1 - (left['Rank'] - left['Index']),
-        1 - (left['Index'] - left['Rank']),
+        1 - (left['__Rank__'] - left['__Index__']),
+        1 - (left['__Index__'] - left['__Rank__']),
         ]
     
-    left['Proximity'] = np.select(conditions, results, np.nan)
+    left['__Proximity__'] = np.select(conditions, results, np.nan)
     
     # Drop non-contributing rows
-    left = left[left['Proximity'] > 0]
+    left = left[left['__Proximity__'] > 0]
     
     # Calculate contribution for index values that contribute to the result
-    left['Contribution'] = left['Proximity'] * left['LeftBound']
+    left['__Contribution__'] = left['__Proximity__'] * left[left_bound_col]
     
     # Determine left bound and boundary using the sum of the contributions
     # and an open boundary if any of the contributing values is open
-    left = left.groupby(groupby_columns).agg(LeftBoundary = ('LeftBoundary', 'max'),
-                                             LeftBound = ('Contribution', 'sum'),
-                                             Minimum = ('Contribution', 'min'))
+    left = left.groupby(groupby_columns).agg(**{
+                            left_boundary_col: (left_boundary_col, 'max'),
+                            left_bound_col: ('__Contribution__','sum'),
+                            '__Minimum__': ('__Contribution__','min')
+                            })
     
     # Replace the numeric value for the boundary
-    left['LeftBoundary'] = left['LeftBoundary'].replace([0,1], ['Closed','Open'])
+    left[left_boundary_col] = left[left_boundary_col].replace([0,1], ['Closed','Open'])
     
     # Means with infinite values produce nan values rather than np.inf values
     # Convert nan to inf only if infinite values are included in the mean
-    left['LeftBound'] = np.where(left['Minimum'] == -np.inf, -np.inf, left['LeftBound'])
+    left[left_bound_col] = np.where(left['__Minimum__'] == -np.inf, -np.inf, left[left_bound_col])
     
     # Determine right bound and boundary for each group
     
     # Change notation of 'Closed' and 'Open' boundaries to 1 and 0, respectively
     # Use 1 for closed to ensure that closed boundaries are sorted larger than open
     # boundaries when the right bound is tied
-    df['RightBoundary'] = df['RightBoundary'].replace(['Closed','Open'], [1,0])
+    df[right_boundary_col] = df[right_boundary_col].replace(['Closed','Open'], [1,0])
     
     # Sort right bound values
-    right = df.copy()[groupby_columns+['Size','RightBoundary','RightBound']].sort_values(by=['RightBound','RightBoundary'])
+    right = df.copy()[groupby_columns+['__Size__',right_boundary_col,right_bound_col]].sort_values(by=[right_bound_col,right_boundary_col])
     
     # Add index for each group
-    right['Index'] = right.groupby(groupby_columns).cumcount() + 1
+    right['__Index__'] = right.groupby(groupby_columns).cumcount() + 1
     
     # Determine the rank in each group for the percentile
-    right['Rank'] = round(C + percentile*(right['Size'] + 1 - 2*C),8)
+    right['__Rank__'] = round(C + percentile*(right['__Size__'] + 1 - 2*C),8)
     
     # Generate proximity of each result to percentile rank using the index
-    right['Proximity'] = 0
+    right['__Proximity__'] = 0
     
     conditions = [
         # If the percentile rank is a whole number, then use that index result
-        (right['Rank'] == right['Index']),
+        (right['__Rank__'] == right['__Index__']),
         # If the percentile rank is less than 1 above the index value,
         # then assign the appropriate contribution to that index value
-        (right['Rank'] - right['Index']).between(0,1,inclusive='neither'),
+        (right['__Rank__'] - right['__Index__']).between(0,1,inclusive='neither'),
         # If the percentile rank is less than 1 below the index value,
         # then assign the appropriate contribution to that index value
-        (right['Index'] - right['Rank']).between(0,1,inclusive='neither')
+        (right['__Index__'] - right['__Rank__']).between(0,1,inclusive='neither')
         ]
     
     results = [
         1,
-        1 - (right['Rank'] - right['Index']),
-        1 - (right['Index'] - right['Rank']),
+        1 - (right['__Rank__'] - right['__Index__']),
+        1 - (right['__Index__'] - right['__Rank__']),
         ]
     
-    right['Proximity'] = np.select(conditions, results, np.nan)
+    right['__Proximity__'] = np.select(conditions, results, np.nan)
     
     # Drop non-contributing rows
-    right = right[right['Proximity'] > 0]
+    right = right[right['__Proximity__'] > 0]
     
     # Calculate contribution for index values that contribute to the result
-    right['Contribution'] = right['Proximity'] * right['RightBound']
+    right['__Contribution__'] = right['__Proximity__'] * right[right_bound_col]
     
     # Determine right bound and boundary using the sum of the contributions
     # and an open boundary if any of the contributing values is open
-    right = right.groupby(groupby_columns).agg(RightBound = ('Contribution', 'sum'),
-                                               Maximum = ('Contribution', 'max'),
-                                               RightBoundary = ('RightBoundary', 'min'))
+    right = right.groupby(groupby_columns).agg(**{
+                            right_bound_col: ('__Contribution__','sum'),
+                            right_boundary_col: (right_boundary_col, 'min'),
+                            '__Maximum__': ('__Contribution__','max')
+                            })
     
     # Replace the numeric value for the boundary
-    right['RightBoundary'] = right['RightBoundary'].replace([1,0], ['Closed','Open'])
+    right[right_boundary_col] = right[right_boundary_col].replace([1,0], ['Closed','Open'])
     
     # Means with infinite values produce nan values rather than np.inf values
     # Convert nan to inf only if infinite values are included in the mean
-    right['RightBound'] = np.where(right['Maximum'] == np.inf, np.inf, right['RightBound'])
+    right[right_bound_col] = np.where(right['__Maximum__'] == np.inf, np.inf, right[right_bound_col])
     
     # Merge the two boundaries to create the interval for the percentile
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
+    # Reset index
+    df = df.reset_index()
+    
     return df
 
 def percentile(df,
+               result_col,
                percentile,
                method = 'hazen',
                groupby_columns = None,
-               values = ['CensorComponent','NumericComponent'],
                focus_high_potential = True,
                include_negative_interval = False,
                precision_tolerance_to_drop_censor = 0.25,
                precision_rounding = True):
     '''
     A function that combines the relevant percentile and utility functions to
     generate the percenitle results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
+    result_col : string
+        The column name for the column that contain the results as text.
+        Only four possible censors should be used (<,≤,≥,>).
     percentile : float
         The desired percentile. Values should be between 0 and 100.
     method : string
         The percentile method. The options and definitions come from:
             https://environment.govt.nz/assets/Publications/Files/hazen-percentile-calculator-2.xls
             Options include the following, ordered from largest to smallest result.
             - weiball
@@ -1134,21 +1052,14 @@
         The default is hazen.
     groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. A percentile
         will be found within each group. Multiple lists can be supplied to
         perform sequential median percentiles before calculating a percentile
         over the final grouping.
         The default is None.
-    values : list of strings, optional
-        The column name(s) for the column(s) that contain the results. If a 
-        single column name is given, it is assumed that the column contains
-        combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,,≥,>)
-        and the second should contain only numeric data.
-        The default is ['CensorComponent','NumericComponent'].
     focus_high_potential : boolean, optional
         If True, then information on the highest potential result will be
         focused over the lowest potential result.
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
@@ -1172,83 +1083,86 @@
         DataFrame that contains calculated percentiles
 
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
-    # If single result column provided, then split column
-    if len(values) == 1:
-        censor_column = 'CensorComponent'
-        numeric_column = 'NumericComponent'
-        df = result_to_components(df,values[0])
-    # Else define the names to use for the censor and numeric columns
-    else:
-        censor_column = values[0]
-        numeric_column = values[1]
+    # Split the result into censor and numeric components
+    df = result_to_components(df,result_col)
     
     # Convert the results from censor and numeric components to an interval representation
-    df = components_to_interval(df, censor_column, numeric_column, include_negative_interval)
+    df = components_to_interval(df, include_negative_interval)
+    
+    # Using the intervals, determine the range of possible percentiles
     
-    # If multiple groupby lists, then cycle through them in order
-    if isinstance(groupby_columns[0],list):
+    # If there are no groupby-columns, then take percentile of all results
+    if not groupby_columns:
+        df = percentile_interval(df, groupby_columns=[],
+                                 percentile=percentile,
+                                 method=method)
+    # If the groupby_columns is a list of lists, then perform multiple percentiles
+    elif isinstance(groupby_columns[0],list):
         for grouping in groupby_columns:
             # Only apply percentile to final grouping
             if grouping == groupby_columns[-1]:
                 # Using the intervals, determine the range of possible percentiles
-                df = percentile_interval(df, percentile, method, grouping)
+                df = percentile_interval(df, grouping, percentile, method)
             # Apply median to all prior groupings
             else:
                 # Using the intervals, determine the range of possible medians
-                df = percentile_interval(df, 50, method, grouping)
+                df = percentile_interval(df, grouping, 50, method)
+    # Else the groupby_columns is a list of column names
     else:
-        # Using the intervals, determine the range of possible percentiles
-        df = percentile_interval(df, percentile, method, grouping)
-    
-    # Create interval notation for the average
-    df = interval_notation(df, precision_rounding)
+        df = percentile_interval(df, groupby_columns, percentile, method)
     
     # Convert the interval for the minimum into censor and numeric notation
-    df = interval_to_components(df, censor_column, numeric_column,
+    df = interval_to_components(df,
                                 focus_high_potential = focus_high_potential,
                                 include_negative_interval = include_negative_interval,
                                 precision_tolerance_to_drop_censor = precision_tolerance_to_drop_censor)
     
+    # Create interval notation for the percentile
+    df = interval_notation(df, precision_rounding)
+    
     # Combine the censor and numeric components into a result
-    df = components_to_result(df, censor_column, numeric_column, precision_rounding)
+    df = components_to_result(df, precision_rounding)
+    
+    # Drop working columns
+    df = df.drop(df.filter(regex='__').columns, axis=1)
+    
+    # Reorder columns
+    for col in [stat_col,result_col,censor_col,numeric_col,interval_col]:
+        df[col] = df.pop(col)
     
     return df
 
 def median(df,
+           result_col,
            groupby_columns = None,
-           values = ['CensorComponent','NumericComponent'],
            focus_high_potential = True,
            include_negative_interval = False,
            precision_tolerance_to_drop_censor = 0.25,
            precision_rounding = True):
     '''
     A function that generates median results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
+    result_col : string
+        The column name for the column that contain the results as text.
+        Only four possible censors should be used (<,≤,≥,>).
     groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. A median
         will be found within each group. Multiple lists can be supplied to
         perform sequential median percentiles before calculating a median
         over the final grouping.
         The default is None.
-    values : list of strings, optional
-        The column name(s) for the column(s) that contain the results. If a 
-        single column name is given, it is assumed that the column contains
-        combined censor and numeric components. If two column names are
-        provided, then the first should only contain one of five censors (<,≤,,≥,>)
-        and the second should contain only numeric data.
-        The default is ['CensorComponent','NumericComponent'].
     focus_high_potential : boolean, optional
         If True, then information on the highest potential result will be
         focused over the lowest potential result.
     include_negative_interval : boolean, optional
         If True, then all positive and negative values are considered
         e.g., <0.5 would be converted to (-np.inf,5).
         If False, then only non-negative values are considered
@@ -1274,17 +1188,17 @@
     '''
     
     # Create a copy of the DataFrame
     df = df.copy()
     
     # Call percentile function with percentile = 50
     df = percentile(df,
+                    result_col,
                     50,
                     groupby_columns = groupby_columns,
-                    values = values,
                     focus_high_potential = focus_high_potential,
                     include_negative_interval = include_negative_interval,
                     precision_tolerance_to_drop_censor = precision_tolerance_to_drop_censor,
                     precision_rounding = precision_rounding)
     
     return df
```

### Comparing `censoredsummarystats-1.0.1/LICENSE` & `censoredsummarystats-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-1.0.1/pyproject.toml` & `censoredsummarystats-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "1.0.1"
+version = "1.1.0"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
+license = "Apache-2.0"
 packages = [{include = "censoredsummarystats"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.2"
```

### Comparing `censoredsummarystats-1.0.1/PKG-INFO` & `censoredsummarystats-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
+License: Apache-2.0
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Project-URL: Repository, https://github.com/kurtvanness/CensoredSummaryStats
 Description-Content-Type: text/markdown
```

