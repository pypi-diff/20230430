# Comparing `tmp/unisci-1.4.0.tar.gz` & `tmp/unisci-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.4.0.tar", last modified: Sun Apr 30 05:16:48 2023, max compression
+gzip compressed data, was "unisci-1.4.1.tar", last modified: Sun Apr 30 05:45:22 2023, max compression
```

## Comparing `unisci-1.4.0.tar` & `unisci-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:16:48.975935 unisci-1.4.0/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.0/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.0/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-30 05:16:48.975617 unisci-1.4.0/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.0/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-30 05:16:48.976022 unisci-1.4.0/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-04-30 05:15:00.000000 unisci-1.4.0/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:16:48.969041 unisci-1.4.0/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-30 05:15:09.000000 unisci-1.4.0/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.0/unisci/constants.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1508 2023-04-26 14:57:12.000000 unisci-1.4.0/unisci/conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.0/unisci/error.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:16:48.971941 unisci-1.4.0/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.0/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)    16653 2023-04-30 05:13:24.000000 unisci-1.4.0/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1840 2023-04-26 16:06:26.000000 unisci-1.4.0/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:16:48.975218 unisci-1.4.0/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.0/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.4.0/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.0/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    38863 2023-04-28 04:22:19.000000 unisci-1.4.0/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:16:48.971432 unisci-1.4.0/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-30 05:16:48.000000 unisci-1.4.0/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      492 2023-04-30 05:16:48.000000 unisci-1.4.0/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-30 05:16:48.000000 unisci-1.4.0/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-04-30 05:16:48.000000 unisci-1.4.0/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-30 05:16:48.000000 unisci-1.4.0/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:45:22.234675 unisci-1.4.1/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.1/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.1/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-30 05:45:22.234325 unisci-1.4.1/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.1/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-30 05:45:22.234785 unisci-1.4.1/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-04-30 05:44:14.000000 unisci-1.4.1/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:45:22.229196 unisci-1.4.1/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-30 05:44:09.000000 unisci-1.4.1/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.1/unisci/constants.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1508 2023-04-26 14:57:12.000000 unisci-1.4.1/unisci/conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.1/unisci/error.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:45:22.232350 unisci-1.4.1/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.1/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2263 2023-04-30 05:43:17.000000 unisci-1.4.1/unisci/formulas/_validation.py
+-rw-r--r--   0 vivaan     (501) staff       (20)    14487 2023-04-30 05:43:08.000000 unisci-1.4.1/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1840 2023-04-26 16:06:26.000000 unisci-1.4.1/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:45:22.233929 unisci-1.4.1/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.1/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.4.1/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.1/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    38863 2023-04-28 04:22:19.000000 unisci-1.4.1/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-30 05:45:22.231513 unisci-1.4.1/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-30 05:45:22.000000 unisci-1.4.1/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      523 2023-04-30 05:45:22.000000 unisci-1.4.1/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-30 05:45:22.000000 unisci-1.4.1/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-04-30 05:45:22.000000 unisci-1.4.1/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-30 05:45:22.000000 unisci-1.4.1/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.4.0/LICENSE` & `unisci-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/PKG-INFO` & `unisci-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.0
+Version: 1.4.1
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.0/README.md` & `unisci-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/setup.py` & `unisci-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.4.0',
+    version='1.4.1',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.4.0/unisci/conversion_factors.py` & `unisci-1.4.1/unisci/conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/unisci/error.py` & `unisci-1.4.1/unisci/error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/unisci/formulas/chemistry.py` & `unisci-1.4.1/unisci/formulas/chemistry.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,75 +4,19 @@
 from sympy import Eq, symbols, solve, log
 from typing import Union
 from unisci.types import *
 from unisci.types import numeric
 from unisci.error import *
 from unisci.constants import *
 from unisci.conversion_factors import *
+from unisci.formulas._validation import _get_args, UNKNOWN
 
-UNKNOWN = 'x'
 PAREN_OPEN = 'j'
 PAREN_CLOSE = 'q'
 
-# generate type alias
-expression = type(2*symbols('X'))
-
-def _get_number(value: Union[Quantity, numeric], intended_types: dict, name: str) -> numeric:
-    
-    # return a symbol if none - represents a variable
-    if value is None:
-        return symbols(UNKNOWN)
-    
-    if isinstance(value, (Temperature, Quantity)):
-
-        # standarizes to quantity
-        if isinstance(value, Temperature):
-            value = Quantity(value.kelvin, {'K': 1})
-
-        # eliminate all special types from intended
-        quan_intended_types = Quantity(1, intended_types.copy())
-        quan_intended_types = quan_intended_types.to_base_units()
-        value = value.converted(list(intended_types.keys())).to_base_units()
-
-        # fully match value with intended types - turn off auto format for this
-        old_format = Quantity.auto_format
-        Quantity.set_auto_format(False)
-        value = value.converted(list(quan_intended_types.unit_type.keys()))
-        Quantity.set_auto_format(old_format)
-        
-        if value.units != quan_intended_types.units:
-            raise CompatabilityError(f"The units of '{name}' are not compatible with the equation.")
-        
-        # returns the converted value number
-        return value.value
-    
-    # normal number passes check
-    elif isinstance(value, (float, int)):
-        return value
-    
-    else:
-        raise UnsupportedError(f"Unsupported datatype given for '{name}'.")
-    
-def _get_args(types: dict[str, dict[str, int]], arguments: dict[str, Union[Quantity, numeric]]) -> dict[str, numeric]:
-    """
-    Arguments: two dictionaries, one of types of each of the arguments in the other. Keys should match.
-
-    Raises: ArgumentError for if the arguments dictionary is not missing one value
-
-    Returns: a new dictionary with numerical values
-    """
-
-    # checks arguments were rights
-    if list(arguments.values()).count(None) != 1:
-        raise ArgumentError("You must have exactly one missing argument.")
-    
-    # asserts types are valid and converts to numbers
-    args = {name: _get_number(value=var, intended_types=types[name], name=name) for name, var in arguments.items()}
-    return args
-
 def nernst_equation(reduction_potential: Union[numeric, Quantity] = None,
                     standard_potential: Union[numeric, Quantity] = None,
                     temperature: Union[numeric, Temperature, Quantity] = None,
                     reaction_quotient: numeric = None,
                     electron_count: numeric = None) -> Quantity:
     """
     Arguments: Four out of the following five: 
@@ -372,16 +316,14 @@
 
     solution = solve(equations, symbs, dict=True)[0]
 
     # format coefficients to be whole numbers
     multiplication_factor = 1
     for expression in solution.values():
         div_by = expression.as_numer_denom()[1]
-        if div_by == 1:
-            continue
         multiplication_factor = math.lcm(multiplication_factor, div_by)
 
     # return output
     output = { __show_parens(str(base_symbol)) : multiplication_factor }
     for symbol, expression in solution.items():
         output[__show_parens(str(symbol))] = round(float(expression.coeff(base_symbol, 1)) * multiplication_factor)
     return output
```

### Comparing `unisci-1.4.0/unisci/metric.py` & `unisci-1.4.1/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/unisci/periodic/periodic-table-lookup.json` & `unisci-1.4.1/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/unisci/periodic/periodic-table-numbers.json` & `unisci-1.4.1/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/unisci/periodic/periodic-table-symbols.json` & `unisci-1.4.1/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/unisci/types.py` & `unisci-1.4.1/unisci/types.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.0/unisci.egg-info/PKG-INFO` & `unisci-1.4.1/unisci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.0
+Version: 1.4.1
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

