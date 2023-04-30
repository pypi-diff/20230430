# Comparing `tmp/landsat9_lc-0.0.5.tar.gz` & `tmp/landsat9_lc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\landsat9_lc-0.0.5.tar", last modified: Sun Apr 23 23:25:51 2023, max compression
+gzip compressed data, was "landsat9_lc-0.0.6.tar", last modified: Sun Apr 30 20:27:24 2023, max compression
```

## Comparing `landsat9_lc-0.0.5.tar` & `landsat9_lc-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 23:25:51.000000 landsat9_lc-0.0.5/
--rw-rw-rw-   0        0        0      176 2023-04-22 16:46:50.000000 landsat9_lc-0.0.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     1094 2023-04-22 16:46:50.000000 landsat9_lc-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      121 2023-04-23 23:17:32.000000 landsat9_lc-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1334 2023-04-23 23:25:51.000000 landsat9_lc-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-04-22 16:46:50.000000 landsat9_lc-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc/
--rw-rw-rw-   0        0        0       52 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/__init__.py
--rw-rw-rw-   0        0        0     3356 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/l9_lc_classifier.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc/pipeline/
--rw-rw-rw-   0        0        0       38 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1782 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/pipeline/model_pipeline.py
--rw-rw-rw-   0        0        0     2366 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/pipeline/spyndex_transformer.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:25:51.000000 landsat9_lc-0.0.5/landsat9_lc/processing/
--rw-rw-rw-   0        0        0       22 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/processing/__init__.py
--rw-rw-rw-   0        0        0     2113 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/processing/data_manager.py
--rw-rw-rw-   0        0        0     9008 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/processing/utils.py
--rw-rw-rw-   0        0        0     1008 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/
--rw-rw-rw-   0        0        0     1334 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      266 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-22 17:23:39.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      266 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      279 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0      482 2023-04-23 23:25:51.000000 landsat9_lc-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2206 2023-04-23 23:25:45.000000 landsat9_lc-0.0.5/setup.py
+drwxrwxrwx   0 rote      (1000) rote      (1000)        0 2023-04-30 20:27:24.866503 landsat9_lc-0.0.6/
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      176 2023-04-22 16:46:50.000000 landsat9_lc-0.0.6/AUTHORS.rst
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     1094 2023-04-22 16:46:50.000000 landsat9_lc-0.0.6/LICENSE
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      121 2023-04-23 23:17:32.000000 landsat9_lc-0.0.6/MANIFEST.in
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     1292 2023-04-30 20:27:24.868515 landsat9_lc-0.0.6/PKG-INFO
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      725 2023-04-22 16:46:50.000000 landsat9_lc-0.0.6/README.md
+drwxrwxrwx   0 rote      (1000) rote      (1000)        0 2023-04-30 20:27:24.493850 landsat9_lc-0.0.6/landsat9_lc/
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      145 2023-04-30 20:04:56.000000 landsat9_lc-0.0.6/landsat9_lc/__init__.py
+drwxrwxrwx   0 rote      (1000) rote      (1000)        0 2023-04-30 20:27:24.684574 landsat9_lc-0.0.6/landsat9_lc/config/
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      146 2023-04-26 19:07:25.000000 landsat9_lc-0.0.6/landsat9_lc/config/__init__.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      403 2023-04-26 19:07:25.000000 landsat9_lc-0.0.6/landsat9_lc/config/data.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     1403 2023-04-30 19:48:34.000000 landsat9_lc-0.0.6/landsat9_lc/config/model.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      173 2023-04-30 04:34:26.000000 landsat9_lc-0.0.6/landsat9_lc/config/package.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      183 2023-04-26 19:07:25.000000 landsat9_lc-0.0.6/landsat9_lc/config/xarray_dims.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     3270 2023-04-26 04:24:55.000000 landsat9_lc-0.0.6/landsat9_lc/l9_lc_classifier.py
+drwxrwxrwx   0 rote      (1000) rote      (1000)        0 2023-04-30 20:27:24.744573 landsat9_lc-0.0.6/landsat9_lc/pipeline/
+-rwxrwxrwx   0 rote      (1000) rote      (1000)       38 2023-04-22 16:46:51.000000 landsat9_lc-0.0.6/landsat9_lc/pipeline/__init__.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     1779 2023-04-26 19:07:25.000000 landsat9_lc-0.0.6/landsat9_lc/pipeline/model_pipeline.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     2366 2023-04-22 16:46:51.000000 landsat9_lc-0.0.6/landsat9_lc/pipeline/spyndex_transformer.py
+drwxrwxrwx   0 rote      (1000) rote      (1000)        0 2023-04-30 20:27:24.782572 landsat9_lc-0.0.6/landsat9_lc/plotting/
+-rwxrwxrwx   0 rote      (1000) rote      (1000)        0 2023-04-30 04:34:27.000000 landsat9_lc-0.0.6/landsat9_lc/plotting/__init__.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     1011 2023-04-30 04:34:27.000000 landsat9_lc-0.0.6/landsat9_lc/plotting/classification_plot.py
+drwxrwxrwx   0 rote      (1000) rote      (1000)        0 2023-04-30 20:27:24.846733 landsat9_lc-0.0.6/landsat9_lc/processing/
+-rwxrwxrwx   0 rote      (1000) rote      (1000)       22 2023-04-22 16:46:51.000000 landsat9_lc-0.0.6/landsat9_lc/processing/__init__.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     3086 2023-04-30 19:48:34.000000 landsat9_lc-0.0.6/landsat9_lc/processing/data_manager.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     9108 2023-04-26 19:07:25.000000 landsat9_lc-0.0.6/landsat9_lc/processing/utils.py
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     1138 2023-04-26 19:07:25.000000 landsat9_lc-0.0.6/landsat9_lc/train_pipeline.py
+drwxrwxrwx   0 rote      (1000) rote      (1000)        0 2023-04-30 20:27:24.585225 landsat9_lc-0.0.6/landsat9_lc.egg-info/
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     1292 2023-04-30 20:27:24.000000 landsat9_lc-0.0.6/landsat9_lc.egg-info/PKG-INFO
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      820 2023-04-30 20:27:24.000000 landsat9_lc-0.0.6/landsat9_lc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      343 2023-04-30 20:27:24.000000 landsat9_lc-0.0.6/landsat9_lc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rote      (1000) rote      (1000)        2 2023-04-22 17:23:39.000000 landsat9_lc-0.0.6/landsat9_lc.egg-info/not-zip-safe
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      342 2023-04-30 20:27:24.000000 landsat9_lc-0.0.6/landsat9_lc.egg-info/requires.txt
+-rwxrwxrwx   0 rote      (1000) rote      (1000)       12 2023-04-30 20:27:24.000000 landsat9_lc-0.0.6/landsat9_lc.egg-info/top_level.txt
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      342 2023-04-30 20:26:37.000000 landsat9_lc-0.0.6/requirements.txt
+-rwxrwxrwx   0 rote      (1000) rote      (1000)      453 2023-04-30 20:27:24.872504 landsat9_lc-0.0.6/setup.cfg
+-rwxrwxrwx   0 rote      (1000) rote      (1000)     1883 2023-04-24 15:22:11.000000 landsat9_lc-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `landsat9_lc-0.0.5/LICENSE` & `landsat9_lc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.5/PKG-INFO` & `landsat9_lc-0.0.6/landsat9_lc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1
-Name: landsat9_lc
-Version: 0.0.5
-Summary: A Short description
-Home-page: https://github.com/hectorpatino/landsat9_lc
-Author: Hector Patino
-Author-email: hectorpatino24@gmail.com
-License: MIT license
-Keywords: landsat9_lc
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-# landsat9_lc
-
-
-[![image](https://img.shields.io/pypi/v/landsat9_lc.svg)](https://pypi.python.org/pypi/landsat9_lc)
-[![image](https://img.shields.io/conda/vn/conda-forge/landsat9_lc.svg)](https://anaconda.org/conda-forge/landsat9_lc)
-
-[![image](https://pyup.io/repos/github/hectorpatino/landsat9_lc/shield.svg)](https://pyup.io/repos/github/hectorpatino/landsat9_lc)
-
-
-**A Short description**
-
-
--   Free software: MIT license
--   Documentation: https://hectorpatino.github.io/landsat9_lc
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: landsat9-lc
+Version: 0.0.6
+Summary: A Short description
+Home-page: https://github.com/hectorpatino/landsat9_lc
+Author: Hector Patino
+Author-email: hectorpatino24@gmail.com
+License: MIT license
+Keywords: landsat9_lc
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# landsat9_lc
+
+
+[![image](https://img.shields.io/pypi/v/landsat9_lc.svg)](https://pypi.python.org/pypi/landsat9_lc)
+[![image](https://img.shields.io/conda/vn/conda-forge/landsat9_lc.svg)](https://anaconda.org/conda-forge/landsat9_lc)
+
+[![image](https://pyup.io/repos/github/hectorpatino/landsat9_lc/shield.svg)](https://pyup.io/repos/github/hectorpatino/landsat9_lc)
+
+
+**A Short description**
+
+
+-   Free software: MIT license
+-   Documentation: https://hectorpatino.github.io/landsat9_lc
+    
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `landsat9_lc-0.0.5/README.md` & `landsat9_lc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.5/landsat9_lc/l9_lc_classifier.py` & `landsat9_lc-0.0.6/landsat9_lc/l9_lc_classifier.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import numpy as np
-import pandas as pd
-import xarray as xr
-
-from landsat9_lc.processing.data_manager import load_pipeline, validate_inputs
-from landsat9_lc.processing.utils import (
-    transforms_xr_to_pandas, convert_numpy_to_xarray, obtain_stac, verify_columns)
-
-
-class Landsat9LCClassifier:
-    """This class provides methods to make predictions of land cover types from Landsat 9 data.
-    It can work with custom pandas dataframes or directly from STAC items.
-    """
-
-    def make_prediction(self, input_data: pd.DataFrame) -> np.ndarray:
-        """
-        Use this method if you have a custom pandas DataFrame that matches the coordinates of the `band` dimension
-        of an xarray object obtained by `pystac` and `stacstack`. If these terms are unfamiliar, we recommend
-        reviewing the `Microsoft Planetary Computer` documentation. Note that this method loads the entire
-        input data into memory, so it is recommended to use smaller portions of the data for larger datasets.
-
-        Parameters
-        ----------
-        input_data :
-            A pandas dataframe with the columns specified in `data_train_config.input_columns`.
-
-        Returns
-        -------
-        np.ndarray:
-            A numpy array with the predictions.
-
-        Raises
-        ------
-        ValueError
-            If the dataframe doesn't have the correct columns.
-        """
-        verify_columns(input_data)
-        pipeline = load_pipeline()
-        if isinstance(input_data, pd.DataFrame):
-            validate_inputs(input_data)
-        # TODO batch predict for memory efficiency
-        prediction = pipeline.predict(input_data)
-        return prediction
-
-    def predict_from_stac(
-            self,
-            scene_id: str,
-            x_min: int,
-            y_max: int,
-            pixels: int = 800,
-    ) -> xr.DataArray:
-        """Use this method if you want to make predictions from a STAC item that is a Landsat9 image.
-        by default the amount of pixels in x and y are 800 and are always square (this behaviour shouldnt
-        be permanent and it should be one of the first things in coming versions). The suggestion is
-        to try to avoid the edges of the image as it can produce not implemented errors and create bad
-        predictions.
-
-        If you are note sure about the identifier of the image you cand read Microsoft Planetary Computer
-        documentation, of check its datasets, if you are a QGIS user you can also use `STAC API Browser Plugin`.
-
-        Parameters
-        ----------
-        scene_id :
-            The identifier of the STAC item.
-        x_min :
-            The x coordinate of the top left corner of the subscene.
-        y_max :
-            The y coordinate of the top left corner of the subscene.
-        pixels :
-            The amount of pixels in x and y, by default 800
-
-        Returns
-        -------
-        xr.DataArray:
-            A xarray DataArray with the predictions.
-
-        """
-        stac = obtain_stac(
-            scene_id=scene_id,
-            x_min=x_min,
-            y_max=y_max,
-            pixels=pixels
-        )
-        stac_df = transforms_xr_to_pandas(stac)
-        predictions = self.make_prediction(stac_df)
-        return convert_numpy_to_xarray(predictions, stac)
+import numpy as np
+import pandas as pd
+import xarray as xr
+
+from landsat9_lc.processing.data_manager import load_pipeline, validate_inputs
+from landsat9_lc.processing.utils import (
+    transforms_xr_to_pandas, convert_numpy_to_xarray, obtain_stac, verify_columns)
+
+
+class Landsat9LCClassifier:
+    """This class provides methods to make predictions of land cover types from Landsat 9 data.
+    It can work with custom pandas dataframes or directly from STAC items.
+    """
+
+    def make_prediction(self, input_data: pd.DataFrame) -> np.ndarray:
+        """
+        Use this method if you have a custom pandas DataFrame that matches the coordinates of the `band` dimension
+        of an xarray object obtained by `pystac` and `stacstack`. If these terms are unfamiliar, we recommend
+        reviewing the `Microsoft Planetary Computer` documentation. Note that this method loads the entire
+        input data into memory, so it is recommended to use smaller portions of the data for larger datasets.
+
+        Parameters
+        ----------
+        input_data :
+            A pandas dataframe with the columns specified in `data_train_config.input_columns`.
+
+        Returns
+        -------
+        np.ndarray:
+            A numpy array with the predictions.
+
+        Raises
+        ------
+        ValueError
+            If the dataframe doesn't have the correct columns.
+        """
+        verify_columns(input_data)
+        pipeline = load_pipeline()
+        if isinstance(input_data, pd.DataFrame):
+            validate_inputs(input_data)
+        # TODO batch predict for memory efficiency
+        prediction = pipeline.predict(input_data)
+        return prediction
+
+    def predict_from_stac(
+            self,
+            scene_id: str,
+            x_min: int,
+            y_max: int,
+            pixels: int = 800,
+    ) -> xr.DataArray:
+        """Use this method if you want to make predictions from a STAC item that is a Landsat9 image.
+        by default the amount of pixels in x and y are 800 and are always square (this behaviour shouldnt
+        be permanent and it should be one of the first things in coming versions). The suggestion is
+        to try to avoid the edges of the image as it can produce not implemented errors and create bad
+        predictions.
+
+        If you are note sure about the identifier of the image you cand read Microsoft Planetary Computer
+        documentation, of check its datasets, if you are a QGIS user you can also use `STAC API Browser Plugin`.
+
+        Parameters
+        ----------
+        scene_id :
+            The identifier of the STAC item.
+        x_min :
+            The x coordinate of the top left corner of the subscene.
+        y_max :
+            The y coordinate of the top left corner of the subscene.
+        pixels :
+            The amount of pixels in x and y, by default 800
+
+        Returns
+        -------
+        xr.DataArray:
+            A xarray DataArray with the predictions.
+
+        """
+        stac = obtain_stac(
+            scene_id=scene_id,
+            x_min=x_min,
+            y_max=y_max,
+            pixels=pixels
+        )
+        stac_df = transforms_xr_to_pandas(stac)
+        predictions = self.make_prediction(stac_df)
+        return convert_numpy_to_xarray(predictions, stac)
```

### Comparing `landsat9_lc-0.0.5/landsat9_lc/pipeline/model_pipeline.py` & `landsat9_lc-0.0.6/landsat9_lc/pipeline/model_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import xgboost as xgb
 
-from sklearn.pipeline import make_pipeline, Pipeline
+from sklearn.pipeline import Pipeline
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import MinMaxScaler, RobustScaler, QuantileTransformer
 from feature_engine.wrappers import SklearnTransformerWrapper
 from feature_engine.imputation import MeanMedianImputer
 from sklearnex import patch_sklearn
 
 from .spyndex_transformer import IndexTransformer
-from config import model_config, data_train_config
+from landsat9_lc.config import model_config, data_train_config
 
 patch_sklearn()
 
 pipeline = Pipeline([
     ('mmi_1', MeanMedianImputer(imputation_method='mean', variables=data_train_config.input_columns)),
     ('it', IndexTransformer(indices=model_config.indexes_columns)),
     ('mmi_2', MeanMedianImputer(
```

### Comparing `landsat9_lc-0.0.5/landsat9_lc/pipeline/spyndex_transformer.py` & `landsat9_lc-0.0.6/landsat9_lc/pipeline/spyndex_transformer.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.5/landsat9_lc/processing/data_manager.py` & `landsat9_lc-0.0.6/landsat9_lc/processing/data_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import joblib
 import json
 import pandas as pd
+import seaborn as sns
+import matplotlib.pyplot as plt
 
 from pathlib import Path
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import LabelEncoder
+from sklearn.metrics import confusion_matrix
 
-from config import data_train_config, model_config
+from landsat9_lc.config import data_train_config, model_config
 
 
 def save_labels(le: LabelEncoder, values) -> None:
     save_path = model_config.path_label_encoder
     encoding_dict = {}
     for value in values:
         encoding_dict[value] = int(le.transform([value])[0])
 
+    # order the dict by value
+    encoding_dict = dict(sorted(encoding_dict.items(), key=lambda item: item[1]))
     encoding_dict = json.dumps(
         encoding_dict,
         ensure_ascii=False,
         indent=4
     )
     with open(save_path, 'w', encoding=model_config.json_encoding) as f:
         f.write(encoding_dict)
@@ -30,16 +35,22 @@
         encoding_dict = json.load(f)
     return encoding_dict
 
 
 def load_dataset(file_name: str) -> pd.DataFrame:
     # TODO esto debería estar en un s3 por que github lo rechaza.
     file_path = Path(__file__).parent.parent / file_name
-    # TODO eliminar el sampling ya que esto es solo en el prototipo.
-    return pd.read_parquet(file_path)[data_train_config.input_columns + [data_train_config.target]].sample(frac=0.01)
+    # TODO esto debería estar con GLFS
+    dataset = pd.read_parquet(file_path)[data_train_config.input_columns + [data_train_config.target]].sample(frac=0.01)
+    dataset = remove_noise(dataset)
+    return dataset
+
+
+def remove_noise(df: pd.DataFrame) -> pd.DataFrame:
+    return df[df[data_train_config.target] != 'Ruido']
 
 
 def save_pipeline(pipeline) -> None:
     """Overwrites any previous pipeline."""
     save_path = Path(f"{model_config.full_path}")
     joblib.dump(pipeline, save_path)
 
@@ -56,7 +67,33 @@
             raise ValueError(f"The column {column} is not numeric")
 
 
 def load_pipeline() -> Pipeline:
     """Loads the latest saved pipeline."""
     save_path = Path(f"{model_config.full_path}")
     return joblib.load(save_path)
+
+
+def save_confusion_matrix(
+    pipeline,
+    x_train,
+    y_true,
+    classes
+):
+    fig, ax = plt.subplots(figsize=(10, 8))
+    y_pred = pipeline.predict(x_train)
+    cm = confusion_matrix(y_true, y_pred)
+    sns.heatmap(
+        cm,
+        annot=True,
+        fmt='d',
+        xticklabels=classes,
+        yticklabels=classes,
+        cmap='Blues',
+    )
+    ax.set_xlabel('Predicted')
+    ax.set_ylabel('Actual')
+    ax.set_title('Confusion Matrix')
+
+    src = str(Path(__file__).parent.parent.parent / 'docs' / 'images' / 'confusion_matrix.png')
+    fig.savefig(src)
+
```

### Comparing `landsat9_lc-0.0.5/landsat9_lc/processing/utils.py` & `landsat9_lc-0.0.6/landsat9_lc/processing/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 import planetary_computer
 import pystac
 import stackstac
 import xarray as xr
 import rioxarray  # Not in use, but needed for xarray to use rasterio
 
-from config import x_array_dims, data_train_config
+from landsat9_lc.config import x_array_dims, data_train_config
 
 
 def transforms_xr_to_pandas(array: xr.DataArray,) -> pd.DataFrame:
     __validate_xarray(array)
     __validate_dimensions(array)
     """Transforms a xr.DataArray to a pandas DataFrame."""
     columns = array.coords[x_array_dims.band].values
@@ -118,14 +118,18 @@
 def obtain_stac(
         scene_id: str,
         x_min: int,
         y_max: int,
         pixels: int = 800,
 ) -> xr.DataArray:
     """Make a prediction using a saved model pipeline."""
+    # TODO scene_id must be a landsat 9 image
+    # TOD scene_id must be a string
+
+
     url = f"https://planetarycomputer.microsoft.com/api/stac/v1/collections/landsat-c2-l2/items/{scene_id}"
     item = pystac.Item.from_file(url)
     signed_item = planetary_computer.sign(item)
     signed_item = stackstac.stack(signed_item)
     __validate_time_values(signed_item, scene_id)
     date_string = np.datetime_as_string(signed_item.time.values[0])
     x_range, y_range = __ranges_by_xmin_ymax(
```

### Comparing `landsat9_lc-0.0.5/landsat9_lc/train_pipeline.py` & `landsat9_lc-0.0.6/landsat9_lc/train_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import numpy as np
 from sklearn.preprocessing import LabelEncoder
-from config import data_train_config
+from landsat9_lc.config import data_train_config
 from landsat9_lc.pipeline import pipeline
-from landsat9_lc.processing.data_manager import load_dataset, save_pipeline, save_labels
+from landsat9_lc.processing.data_manager import load_dataset, save_pipeline, save_labels, save_confusion_matrix
 
 
 def get_labels(y):
     le = LabelEncoder()
     y_trans = le.fit_transform(y)
     save_labels(le, y.unique().tolist())
     return y_trans
@@ -17,12 +18,13 @@
     y_train = data[data_train_config.target]
     y_train = get_labels(y_train)
     for column in x_train.columns:
         if column not in data_train_config.input_columns:
             raise ValueError(f"Input data does not have the correct columns expected columns are "
                              f"{data_train_config.input_columns}")
     pipeline.fit(x_train, y_train)
+    save_confusion_matrix(pipeline, x_train, y_train, np.unique(y_train))
     save_pipeline(pipeline)
 
 
 if __name__ == '__main__':
     run_training()
```

### Comparing `landsat9_lc-0.0.5/landsat9_lc.egg-info/PKG-INFO` & `landsat9_lc-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1
-Name: landsat9-lc
-Version: 0.0.5
-Summary: A Short description
-Home-page: https://github.com/hectorpatino/landsat9_lc
-Author: Hector Patino
-Author-email: hectorpatino24@gmail.com
-License: MIT license
-Keywords: landsat9_lc
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-# landsat9_lc
-
-
-[![image](https://img.shields.io/pypi/v/landsat9_lc.svg)](https://pypi.python.org/pypi/landsat9_lc)
-[![image](https://img.shields.io/conda/vn/conda-forge/landsat9_lc.svg)](https://anaconda.org/conda-forge/landsat9_lc)
-
-[![image](https://pyup.io/repos/github/hectorpatino/landsat9_lc/shield.svg)](https://pyup.io/repos/github/hectorpatino/landsat9_lc)
-
-
-**A Short description**
-
-
--   Free software: MIT license
--   Documentation: https://hectorpatino.github.io/landsat9_lc
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: landsat9_lc
+Version: 0.0.6
+Summary: A Short description
+Home-page: https://github.com/hectorpatino/landsat9_lc
+Author: Hector Patino
+Author-email: hectorpatino24@gmail.com
+License: MIT license
+Keywords: landsat9_lc
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# landsat9_lc
+
+
+[![image](https://img.shields.io/pypi/v/landsat9_lc.svg)](https://pypi.python.org/pypi/landsat9_lc)
+[![image](https://img.shields.io/conda/vn/conda-forge/landsat9_lc.svg)](https://anaconda.org/conda-forge/landsat9_lc)
+
+[![image](https://pyup.io/repos/github/hectorpatino/landsat9_lc/shield.svg)](https://pyup.io/repos/github/hectorpatino/landsat9_lc)
+
+
+**A Short description**
+
+
+-   Free software: MIT license
+-   Documentation: https://hectorpatino.github.io/landsat9_lc
+    
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `landsat9_lc-0.0.5/landsat9_lc.egg-info/SOURCES.txt` & `landsat9_lc-0.0.6/landsat9_lc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,13 +10,20 @@
 landsat9_lc/train_pipeline.py
 landsat9_lc.egg-info/PKG-INFO
 landsat9_lc.egg-info/SOURCES.txt
 landsat9_lc.egg-info/dependency_links.txt
 landsat9_lc.egg-info/not-zip-safe
 landsat9_lc.egg-info/requires.txt
 landsat9_lc.egg-info/top_level.txt
+landsat9_lc/config/__init__.py
+landsat9_lc/config/data.py
+landsat9_lc/config/model.py
+landsat9_lc/config/package.py
+landsat9_lc/config/xarray_dims.py
 landsat9_lc/pipeline/__init__.py
 landsat9_lc/pipeline/model_pipeline.py
 landsat9_lc/pipeline/spyndex_transformer.py
+landsat9_lc/plotting/__init__.py
+landsat9_lc/plotting/classification_plot.py
 landsat9_lc/processing/__init__.py
 landsat9_lc/processing/data_manager.py
 landsat9_lc/processing/utils.py
```

### Comparing `landsat9_lc-0.0.5/setup.py` & `landsat9_lc-0.0.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,59 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = ['pytest-runner', ]
-
-test_requirements = ['pytest>=3', ]
-
-setup(
-    author="Hector Patino",
-    author_email='hectorpatino24@gmail.com',
-    python_requires='>=3.10',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        # 'Programming Language :: Python :: 3',
-        # 'Programming Language :: Python :: 3.7',
-        # 'Programming Language :: Python :: 3.8',
-        # 'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
-    description="A Short description",
-    install_requires=[
-        "pystac==1.6.1",
-        "rioxarray==0.12.1",
-        "planetary_computer==0.4.7",
-        "xarray==2022.6.0",
-        "stackstac==0.4.3",
-        "rasterio==1.3.2",
-        "pandas==1.4.4",
-        "pytest==7.1.3",
-        "pyarrow==9.0.0",
-        "feature_engine==1.6.0",
-        "spyndex==0.4.0",
-        "jupyterlab==3.4.4",
-        "xgboost==1.7.5",
-        "scikit-learn-intelex==2023.1.1",
-        "mkdocs==1.4.2",
-    ],
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='landsat9_lc',
-    name='landsat9_lc',
-    packages=find_packages(include=['landsat9_lc', 'landsat9_lc.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/hectorpatino/landsat9_lc',
-    version='0.0.5',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+from landsat9_lc import __version__
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = ['pytest-runner', ]
+
+test_requirements = ['pytest>=3', ]
+
+setup(
+    author="Hector Patino",
+    author_email='hectorpatino24@gmail.com',
+    python_requires='>=3.10',
+    classifiers=[
+        'Development Status :: 2 - Pre-Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        # 'Programming Language :: Python :: 3',
+        # 'Programming Language :: Python :: 3.7',
+        # 'Programming Language :: Python :: 3.8',
+        # 'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ],
+    description="A Short description",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='landsat9_lc',
+    name='landsat9_lc',
+    packages=find_packages(include=['landsat9_lc', 'landsat9_lc.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/hectorpatino/landsat9_lc',
+    version=__version__,
+    zip_safe=False,
+)
```

