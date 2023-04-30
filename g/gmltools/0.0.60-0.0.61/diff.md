# Comparing `tmp/gmltools-0.0.60.tar.gz` & `tmp/gmltools-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.60.tar", last modified: Mon Apr 17 07:51:02 2023, max compression
+gzip compressed data, was "gmltools-0.0.61.tar", last modified: Sun Apr 30 15:57:57 2023, max compression
```

## Comparing `gmltools-0.0.60.tar` & `gmltools-0.0.61.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.715516 gmltools-0.0.60/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.60/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.60/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-17 07:51:02.714539 gmltools-0.0.60/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.60/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.558811 gmltools-0.0.60/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.60/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.60/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.60/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-17 07:50:11.000000 gmltools-0.0.60/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 07:51:02.715516 gmltools-0.0.60/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-17 07:49:54.000000 gmltools-0.0.60/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.501195 gmltools-0.0.60/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.574332 gmltools-0.0.60/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.60/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.60/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.612204 gmltools-0.0.60/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.60/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.60/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.656108 gmltools-0.0.60/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.60/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.60/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.60/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.60/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   119078 2023-04-14 10:28:24.000000 gmltools-0.0.60/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.60/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    12799 2023-04-14 10:43:53.000000 gmltools-0.0.60/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.677594 gmltools-0.0.60/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.60/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.60/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.60/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.712541 gmltools-0.0.60/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.60/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.60/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.60/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.60/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:51:02.608283 gmltools-0.0.60/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 07:51:02.000000 gmltools-0.0.60/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.920664 gmltools-0.0.61/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.61/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.61/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-30 15:57:57.919658 gmltools-0.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.61/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.633862 gmltools-0.0.61/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.61/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.61/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.61/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-30 15:56:07.000000 gmltools-0.0.61/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 15:57:57.920664 gmltools-0.0.61/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-30 15:55:59.000000 gmltools-0.0.61/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.563552 gmltools-0.0.61/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.659415 gmltools-0.0.61/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.61/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.61/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.727767 gmltools-0.0.61/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.61/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.61/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.828422 gmltools-0.0.61/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.61/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.61/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.61/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.61/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   119074 2023-04-30 15:55:22.000000 gmltools-0.0.61/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.61/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    12799 2023-04-14 10:43:53.000000 gmltools-0.0.61/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.866742 gmltools-0.0.61/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.61/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.61/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.61/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.916638 gmltools-0.0.61/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.61/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.61/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.61/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.61/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.706203 gmltools-0.0.61/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-30 15:57:56.000000 gmltools-0.0.61/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-04-30 15:57:57.000000 gmltools-0.0.61/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 15:57:56.000000 gmltools-0.0.61/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-30 15:57:56.000000 gmltools-0.0.61/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 15:57:56.000000 gmltools-0.0.61/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.60/LICENSE` & `gmltools-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/Models.ipynb` & `gmltools-0.0.61/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/PKG-INFO` & `gmltools-0.0.61/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.60
+Version: 0.0.61
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.60/README.md` & `gmltools-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.61/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/gmltools.yml` & `gmltools-0.0.61/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/mltools.yml` & `gmltools-0.0.61/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/pyproject.toml` & `gmltools-0.0.61/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.60"
+version = "0.0.61"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.60/setup.py` & `gmltools-0.0.61/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.60',
+    'version': '0.0.61',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.60/src/gmltools/To_Do.txt` & `gmltools-0.0.61/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/eda/eda.py` & `gmltools-0.0.61/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/models/bayes.py` & `gmltools-0.0.61/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.61/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/models/dummy_model.py` & `gmltools-0.0.61/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/models/model.py` & `gmltools-0.0.61/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,18 +362,18 @@
         self.model = None
         self.model_name = model_name
         self.X_train = X_train
         self.y_train = y_train
         self.cv = cv
     def RandomForest_Classifier(self, ordinal_cat_cols:List[str]=None,
                                 scoring='accuracy', class_weight=None,
-                                grid_params:dict={'RFC__n_estimators': [100, 200],
-                                            'RFC__max_depth': [None, 10, 20],
-                                            'RFC__min_samples_split': [2, 5],
-                                            'RFC__max_features': ['sqrt', None]},
+                                grid_params:dict={'RF__n_estimators': [100, 200],
+                                            'RF__max_depth': [None, 10, 20],
+                                            'RF__min_samples_split': [2, 5],
+                                            'RF__max_features': ['sqrt', None]},
                                 random_params:dict=None,
                                 random_n_iter:int=10,
                                 bayes_pbounds:dict=None,
                                 bayes_int_params:List[str]=None, 
                                 bayes_n_iter:int=30,
                                 criterion='gini',
                                 sample_weight=None,
```

### Comparing `gmltools-0.0.60/src/gmltools/models/models_info.py` & `gmltools-0.0.61/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.61/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.61/src/gmltools/models_analysis/classification_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1044,16 +1044,14 @@
         Returns
         -------
         None.
             Plot is generated.
         """
         sns.set()
         #assertions
-        if save:
-            assert os.path.exists(f'./models/{self.model_name})'), f'./models/{self.model_name} does not exist. Please create the directory and try again.'
         assert train_or_test_or_val.lower() in ['train', 'test','val'], "train_or_test must be either 'train' or 'test'"
         assert isinstance(figsize, tuple) and len(figsize) == 2, "figsize must be a tuple and figsize must be a tuple of length 2"
         assert isinstance(bins, int) and bins > 0, "bins must be an integer greater than 0"
         assert isinstance(smooth_order, int) and smooth_order > 0, "smooth_order must be an integer greater than 0"
         # Create the residuals
         assert train_or_test_or_val.lower() in ['train','test','val'], "train_or_test must be 'train', 'test' or 'val'"
         assert remove_vars is None or isinstance(remove_vars, list), "remove_vars must be a list"
@@ -1119,14 +1117,16 @@
                 input_num += 1
             else:
                 ax.axis('off')
         plt.suptitle(self.model_name + train_or_test_or_val.capitalize() + ' Residual Analysis', fontsize=18)
         plt.show()
         self.fig_residual_analysis = fig
         if save:
+            if not os.path.exists(f'./models/{self.model_name}'):
+                os.makedirs(f'./models/{self.model_name}')
             fig.savefig(f'./models/{self.model_name}/residual_analysis_{train_or_test_or_val.lower()}.png')
 
 
 
     def summaryLinReg(self, use_old:bool= True):
         """
         Summary of scikit 'LinearRegression' models.
@@ -1294,16 +1294,14 @@
             Size of the figure. The default is (12, 4).
 
         Returns
         -------
         None.
             Plot is generated.
         """
-        if save:
-            assert os.path.exists(f'./models/{self.model_name})'), f'./models/{self.model_name} does not exist. Please create the directory and try again.'
         assert not isinstance(self.model, list), 'model must be a single model, not a list. Comparison of models is only supported for plot_roc_curve(), plot_calibration_curve() and plot_accuracy_across_thresholds()'
         assert n_repeats > 0, "n_repeats must be greater than 0 for permutation importance"
         assert random_state is None or isinstance(random_state, int), "random_state must be an integer or None"
         assert isinstance(figsize, tuple) and len(figsize) == 2, "figsize must be a tuple and figsize must be a tuple of length 2"
         importances = permutation_importance(self.model, 
                                     self.X_train, self.y_train,
                                     n_repeats=n_repeats,
@@ -1315,14 +1313,17 @@
         plt.ylabel('Permutation Importance')
         plt.title(self.model_name + " " + title)
         plt.xticks(rotation=rotation)
         plt.grid()
         plt.show()
         self.fig_permutation_importance = fig
         if save:
+            if not os.path.exists(f'./models/{self.model_name}'):
+                os.makedirs(f'./models/{self.model_name}')
+
             fig.savefig(f'./models/{self.model_name}/permutation_importance.png')
 
 
     def get_metrics_summary(self, sample_weight:str=None, multioutput='uniform_average', save:bool = True)-> pd.DataFrame:
         """
         Prints a summary of the metrics of a model for a given threshold
         and returns them in a DataFrame
@@ -1438,23 +1439,23 @@
         summary=pd.DataFrame(metrics_dict,index=[0])
 
         self.metrics_summary = summary
         if save:
             if not os.path.exists('./models'):
                 os.makedirs('./models')
 
-            if not os.path.isfile('./models/summary_models.xlsx'):
+            if not os.path.isfile('./models/summary_models_analysis.xlsx'):
                 df=pd.DataFrame(columns=summary.columns)
                 #save the summary data to the excel
-                df.to_excel('./models/summary_models.xlsx',index=False,sheet_name='Sheet1')
+                df.to_excel('./models/summary_models_analysis.xlsx',index=False,sheet_name='Sheet1')
             else:
-                df=pd.read_excel('./models/summary_models.xlsx',sheet_name='Sheet1')
+                df=pd.read_excel('./models/summary_models_analysis.xlsx',sheet_name='Sheet1')
                 #concat the summary data to the excel
                 df=pd.concat([df,summary],axis=0,ignore_index=True)
-                df.to_excel('./models/summary_models.xlsx',index=False,sheet_name='Sheet1')
+                df.to_excel('./models/summary_models_analysis.xlsx',index=False,sheet_name='Sheet1')
     
         return  self.metrics_summary
```

### Comparing `gmltools-0.0.60/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.61/src/gmltools/models_analysis/xai.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         assert isinstance(y_train, pd.Series) or isinstance(y_train,pd.DataFrame), "y_train must be a pandas Series or DataFrame"
         assert isinstance(figsize, tuple), "figsize must be a tuple"
         assert isinstance(max_display, int), "max_display must be an integer"
         assert isinstance(kernel_nsamples, int), "nsamples must be an integer" 
 
         model_name=[step for step in model.best_estimator_.named_steps.keys()][-1]
 
-        if model_name in ["XGB","RFC","DT","LGBM"]: #For tree based models
+        if model_name in ["XGB","RF","DT","LGBM"]: #For tree based models
             explainer = shap.TreeExplainer(model.best_estimator_[model_name])
             shap_values = explainer.shap_values(X_train)
         else: #For not tree based models
             explainer = shap.KernelExplainer(model.best_estimator_.predict_proba, X_train)
             shap_values = explainer.shap_values(X_train, nsamples=kernel_nsamples)
         
         if y_train.value_counts().size > 2 and y_train.value_counts().size < 8: #For multiclass classification
```

### Comparing `gmltools-0.0.60/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.61/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.61/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.61/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.60/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.61/src/gmltools.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.60
+Version: 0.0.61
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.60/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.61/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

