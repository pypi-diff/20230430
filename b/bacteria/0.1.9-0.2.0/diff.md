# Comparing `tmp/bacteria-0.1.9.tar.gz` & `tmp/bacteria-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.1.9.tar", last modified: Thu Apr 27 17:39:27 2023, max compression
+gzip compressed data, was "bacteria-0.2.0.tar", last modified: Sun Apr 30 12:57:51 2023, max compression
```

## Comparing `bacteria-0.1.9.tar` & `bacteria-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:39:27.887000 bacteria-0.1.9/
--rw-rw-rw-   0        0        0      593 2023-04-27 17:39:27.758000 bacteria-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2023-04-27 16:19:57.000000 bacteria-0.1.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-27 17:39:27.303000 bacteria-0.1.9/bacteria/
--rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-0.1.9/bacteria/__init__.py
--rw-rw-rw-   0        0        0   142656 2023-04-27 17:31:20.000000 bacteria-0.1.9/bacteria/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:39:27.686000 bacteria-0.1.9/bacteria.egg-info/
--rw-rw-rw-   0        0        0      593 2023-04-27 17:39:26.000000 bacteria-0.1.9/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-27 17:39:26.000000 bacteria-0.1.9/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:39:26.000000 bacteria-0.1.9/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-27 17:39:26.000000 bacteria-0.1.9/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 17:39:26.000000 bacteria-0.1.9/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 17:39:27.852000 bacteria-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-04-27 17:39:23.000000 bacteria-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:57:51.621000 bacteria-0.2.0/
+-rw-rw-rw-   0        0        0      593 2023-04-30 12:57:51.465000 bacteria-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2023-04-27 16:19:57.000000 bacteria-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 12:57:50.629000 bacteria-0.2.0/bacteria/
+-rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-0.2.0/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   143037 2023-04-30 12:57:03.000000 bacteria-0.2.0/bacteria/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:57:51.414000 bacteria-0.2.0/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 12:57:48.000000 bacteria-0.2.0/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 12:57:51.581000 bacteria-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1097 2023-04-30 12:57:39.000000 bacteria-0.2.0/setup.py
```

### Comparing `bacteria-0.1.9/PKG-INFO` & `bacteria-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.9
+Version: 0.2.0
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.9/README.rst` & `bacteria-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.9/bacteria/functions.py` & `bacteria-0.2.0/bacteria/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2772,18 +2772,23 @@
         if lineage_plot_size != 1:
             ax[count].set_xlabel('Time (min)',fontsize = 15)
         else:
             ax.set_xlabel('Time (min)', fontsize = 15)
         fig.suptitle('Lineage of Cell {}'.format(mother_cell),fontsize = 17)
         plt.show()
 
-def plot_distance_minima_lineage(df_3d,df_2d,lineages_list,column='Fluor1 sum',derivative_column='Derivative',order=9,ax = None):
+def plot_distance_minima_lineage(df_3d,df_2d,lineages_list,column='Fluor1 sum',derivative_column='Derivative',order=5,ax = None):
     """
     Function to plot the distance between the minimas for
-    an specifics lineages.
+    an specifics lineages. Here we are calculating the 
+    minima inside the lineage, so it might be better to 
+    just use the diff_minima() function. Change the
+    diff_minima() function to return the minimum along 
+    with the Cells ID and use that data here. This may 
+    be better for the smooth (TODO) tuning issue
 
     Parameters
     --------------
     df_3d : DataFrame
         DataFrame of 3D data
     df_2d : DataFrame
         DataFrame of 2D data
@@ -3085,16 +3090,14 @@
             ax[0][1].set_ylim(0,5)
             ax[0][1].set_xlim(.5,5.5)
             ax[0][1].legend()
 
             ax[1][1].hist(vol_dict['pre']['diff'],color = color_pre)
             ax[1][1].set_title('Pre {} Histogram'.format(vol_dict['order']['pre']),fontsize = 17)
             ax[1][1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-            y_min.append(ax[1][1].get_ylim()[0])
-            y_max.append(ax[1][1].get_ylim()[1])
 
             model = LinearRegression()
             model.fit(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1),
                     np.asarray(vol_dict['pos']['diff']).reshape(len(vol_dict['pos']['diff'])))
 
             ax[0][2].plot(vol_dict['pos']['min'],vol_dict['pos']['diff'],'.',color = color_pos)
             ax[0][2].plot(vol_dict['pos']['min'],model.predict(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1)),
@@ -3104,16 +3107,14 @@
             ax[0][2].set_ylim(0,5)
             ax[0][2].set_xlim(.5,5.5)
             ax[0][2].legend()
 
             ax[1][2].hist(vol_dict['pos']['diff'],color = color_pos)
             ax[1][2].set_title('Pos {} Histogram'.format(vol_dict['order']['pos']),fontsize = 17)
             ax[1][2].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-            y_min.append(ax[1][2].get_ylim()[0])
-            y_max.append(ax[1][2].get_ylim()[1])
 
             model = LinearRegression()
             model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
                     np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
 
             ax[0][0].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.',color = color)
             ax[0][0].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
@@ -3124,23 +3125,28 @@
             ax[0][0].set_ylim(0,5)
             ax[0][0].set_xlim(.5,5.5)
             ax[0][0].legend()
 
             ax[1][0].hist(vol_dict['all']['diff'],color = color)
             ax[1][0].set_title('All the time Histogram',fontsize = 17)
             ax[1][0].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-            y_min.append(ax[1][0].get_ylim()[0])
-            y_max.append(ax[1][0].get_ylim()[1])
 
-            ax[1][0].set_ylim(min(y_min),max(y_max)+100)
-            ax[1][1].set_ylim(min(y_min),max(y_max)+100)
-            ax[1][2].set_ylim(min(y_min),max(y_max)+100)
-            ax[1][0].set_xlim(0,5.5)
-            ax[1][1].set_xlim(0,5.5)
-            ax[1][2].set_xlim(0,5.5)
+            if key is None:
+                y_min.append(ax[1][1].get_ylim()[0])
+                y_max.append(ax[1][1].get_ylim()[1])
+                y_min.append(ax[1][0].get_ylim()[0])
+                y_max.append(ax[1][0].get_ylim()[1])
+                y_min.append(ax[1][2].get_ylim()[0])
+                y_max.append(ax[1][2].get_ylim()[1])
+                ax[1][0].set_ylim(min(y_min),max(y_max)+100)
+                ax[1][1].set_ylim(min(y_min),max(y_max)+100)
+                ax[1][2].set_ylim(min(y_min),max(y_max)+100)
+                ax[1][0].set_xlim(0,5.5)
+                ax[1][1].set_xlim(0,5.5)
+                ax[1][2].set_xlim(0,5.5)
 
             plt.tight_layout()
 
 def plot_distance_minima(vol_dict,key,color = None,ax=None):
     """
     Function to plot the distance between the minimas.
     The function will plot the volume minima by the
```

### Comparing `bacteria-0.1.9/bacteria.egg-info/PKG-INFO` & `bacteria-0.2.0/bacteria.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.9
+Version: 0.2.0
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.9/setup.py` & `bacteria-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.rst", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.1.9',      
+    version = '0.2.0',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[           
@@ -19,15 +19,14 @@
             'pandas',
             'graphviz',
             'scikit-learn',
             'seaborn',
             'natsort',
             'anytree',
             'tqdm',
-            # 'matlabengine',
             'scipy'
         ],
     classifiers=[
       'Development Status :: 4 - Beta',      
       'Intended Audience :: Developers',      
       'Topic :: Software Development :: Build Tools',
       'License :: OSI Approved :: MIT License',
```

