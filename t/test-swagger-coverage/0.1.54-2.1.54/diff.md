# Comparing `tmp/test_swagger_coverage-0.1.54.tar.gz` & `tmp/test_swagger_coverage-2.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_swagger_coverage-0.1.54.tar", max compression
+gzip compressed data, was "test_swagger_coverage-2.1.54.tar", max compression
```

## Comparing `test_swagger_coverage-0.1.54.tar` & `test_swagger_coverage-2.1.54.tar`

### file list

```diff
@@ -1,18 +1,45 @@
--rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-0.1.54/LICENSE
--rw-r--r--   0        0        0     5845 2023-04-10 11:50:18.637247 test_swagger_coverage-0.1.54/README.md
--rw-r--r--   0        0        0      685 2023-04-10 12:01:19.306316 test_swagger_coverage-0.1.54/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 11:50:18.637989 test_swagger_coverage-0.1.54/swagger_coverage/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 11:50:18.638133 test_swagger_coverage-0.1.54/swagger_coverage/scripts/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-10 11:50:18.638296 test_swagger_coverage-0.1.54/swagger_coverage/scripts/swagger_report.py
--rw-r--r--   0        0        0     1300 2023-04-10 11:50:18.638469 test_swagger_coverage-0.1.54/swagger_coverage/src/check_data.py
--rw-r--r--   0        0        0     6302 2023-04-10 11:50:18.638626 test_swagger_coverage-0.1.54/swagger_coverage/src/coverage.py
--rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-0.1.54/swagger_coverage/src/deco.py
--rw-r--r--   0        0        0     1297 2023-04-10 11:50:18.638879 test_swagger_coverage-0.1.54/swagger_coverage/src/files.py
--rw-r--r--   0        0        0      849 2023-04-10 11:50:18.639190 test_swagger_coverage-0.1.54/swagger_coverage/src/logger.py
--rw-r--r--   0        0        0      907 2023-04-10 11:50:18.639306 test_swagger_coverage-0.1.54/swagger_coverage/src/models.py
--rw-r--r--   0        0        0     1884 2023-04-10 11:50:18.639434 test_swagger_coverage-0.1.54/swagger_coverage/src/prepare_data.py
--rw-r--r--   0        0        0    16694 2023-04-10 11:50:18.639647 test_swagger_coverage-0.1.54/swagger_coverage/src/report.py
--rw-r--r--   0        0        0      326 2023-04-10 11:50:18.639786 test_swagger_coverage-0.1.54/swagger_coverage/src/singltone_like.py
--rw-r--r--   0        0        0     2008 2023-04-10 11:50:18.639926 test_swagger_coverage-0.1.54/swagger_coverage/src/swagger_diff.py
--rw-r--r--   0        0        0     3992 2023-04-10 11:50:18.640099 test_swagger_coverage-0.1.54/swagger_coverage/src/utils.py
--rw-r--r--   0        0        0     6571 1970-01-01 00:00:00.000000 test_swagger_coverage-0.1.54/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-2.1.54/LICENSE
+-rw-r--r--   0        0        0     5845 2023-04-10 11:50:18.637247 test_swagger_coverage-2.1.54/README.md
+-rw-r--r--   0        0        0      668 2023-04-27 16:02:15.877854 test_swagger_coverage-2.1.54/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 08:08:13.320535 test_swagger_coverage-2.1.54/swagger_coverage/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-14 08:15:46.280403 test_swagger_coverage-2.1.54/swagger_coverage/scripts/swagger_report.py
+-rw-r--r--   0        0        0        0 2023-04-14 08:08:31.328063 test_swagger_coverage-2.1.54/swagger_coverage/src/__init__.py
+-rw-r--r--   0        0        0     1354 2023-04-14 13:05:24.138537 test_swagger_coverage-2.1.54/swagger_coverage/src/check_data.py
+-rw-r--r--   0        0        0     3229 2023-04-27 16:02:33.057677 test_swagger_coverage-2.1.54/swagger_coverage/src/coverage.py
+-rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-2.1.54/swagger_coverage/src/deco.py
+-rw-r--r--   0        0        0     2056 2023-04-27 16:02:40.028529 test_swagger_coverage-2.1.54/swagger_coverage/src/files.py
+-rw-r--r--   0        0        0      849 2023-04-14 08:16:42.485998 test_swagger_coverage-2.1.54/swagger_coverage/src/logger.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:31:54.617585 test_swagger_coverage-2.1.54/swagger_coverage/src/models/__init__.py
+-rw-r--r--   0        0        0     1175 2023-04-27 16:01:57.068459 test_swagger_coverage-2.1.54/swagger_coverage/src/models/stats.py
+-rw-r--r--   0        0        0      461 2023-04-27 14:54:00.916774 test_swagger_coverage-2.1.54/swagger_coverage/src/models/swagger_data.py
+-rw-r--r--   0        0        0     2060 2023-04-27 16:24:53.724437 test_swagger_coverage-2.1.54/swagger_coverage/src/prepare_data.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:29:27.954717 test_swagger_coverage-2.1.54/swagger_coverage/src/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:29:45.222122 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/__init__.py
+-rw-r--r--   0        0        0     6123 2023-04-27 16:03:56.022244 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/accordion.py
+-rw-r--r--   0        0        0      883 2023-04-27 16:03:26.744052 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/body.py
+-rw-r--r--   0        0        0      766 2023-04-27 16:03:55.974209 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/btn_group.py
+-rw-r--r--   0        0        0      196 2023-04-27 16:01:57.073937 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/colors.py
+-rw-r--r--   0        0        0      165 2023-04-27 16:01:57.076766 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/constants.py
+-rw-r--r--   0        0        0      235 2023-04-27 16:01:57.084743 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/h2.py
+-rw-r--r--   0        0        0      710 2023-04-27 16:03:55.971852 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/head.py
+-rw-r--r--   0        0        0      180 2023-04-27 16:01:57.092106 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/href.py
+-rw-r--r--   0        0        0     4706 2023-04-30 07:05:11.452022 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/html_report.py
+-rw-r--r--   0        0        0      883 2023-04-27 16:01:57.123593 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/models.py
+-rw-r--r--   0        0        0      670 2023-04-27 16:03:54.865325 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/navbar.py
+-rw-r--r--   0        0        0      132 2023-04-27 16:01:57.095766 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/p.py
+-rw-r--r--   0        0        0      446 2023-04-27 16:01:57.121785 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/prepare_data.py
+-rw-r--r--   0        0        0      829 2023-04-27 16:06:14.093094 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/progress.py
+-rw-r--r--   0        0        0     2911 2023-04-27 16:01:57.330789 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/scripts.py
+-rw-r--r--   0        0        0     2017 2023-04-27 16:01:57.143069 test_swagger_coverage-2.1.54/swagger_coverage/src/report/html/table.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:29:38.904729 test_swagger_coverage-2.1.54/swagger_coverage/src/report/plain/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-27 16:01:57.115041 test_swagger_coverage-2.1.54/swagger_coverage/src/report/plain/plain_report.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:29:33.654900 test_swagger_coverage-2.1.54/swagger_coverage/src/report/report.py
+-rw-r--r--   0        0        0      915 2023-04-27 16:04:59.724175 test_swagger_coverage-2.1.54/swagger_coverage/src/requests.py
+-rw-r--r--   0        0        0        0 2023-04-17 15:15:04.775886 test_swagger_coverage-2.1.54/swagger_coverage/src/results/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-27 16:19:19.207957 test_swagger_coverage-2.1.54/swagger_coverage/src/results/load_results.py
+-rw-r--r--   0        0        0      550 2023-04-27 16:01:57.133390 test_swagger_coverage-2.1.54/swagger_coverage/src/results/swagger_diff.py
+-rw-r--r--   0        0        0     1470 2023-04-27 16:05:14.499393 test_swagger_coverage-2.1.54/swagger_coverage/src/results/swagger_results.py
+-rw-r--r--   0        0        0     2907 2023-04-27 16:05:09.299861 test_swagger_coverage-2.1.54/swagger_coverage/src/results/swagger_summary.py
+-rw-r--r--   0        0        0      326 2023-04-14 12:08:09.802242 test_swagger_coverage-2.1.54/swagger_coverage/src/singltone_like.py
+-rw-r--r--   0        0        0      384 2023-04-27 16:01:57.142956 test_swagger_coverage-2.1.54/swagger_coverage/src/utils.py
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 test_swagger_coverage-2.1.54/PKG-INFO
```

### Comparing `test_swagger_coverage-0.1.54/LICENSE` & `test_swagger_coverage-2.1.54/LICENSE`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-0.1.54/README.md` & `test_swagger_coverage-2.1.54/README.md`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-0.1.54/pyproject.toml` & `test_swagger_coverage-2.1.54/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "test-swagger-coverage"
-version = "0.1.54"
+version = "2.1.54"
 description = "Swagger coverage for API tests"
 authors = ["alexanderlozovoy <berpress@gmail.com>"]
 packages = [{ include = "swagger_coverage" }]
 readme = "README.md"
 repository = "https://github.com/berpress/swagger-coverage"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-requests = "^2.27.1"
-PyYAML = "^6.0"
-Jinja2 = "^3.1.2"
+python = "^3.10"
+requests = "^2.28.2"
+pyyaml = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 coverage = "^6.3.2"
 pre-commit = "^2.18.1"
```

### Comparing `test_swagger_coverage-0.1.54/swagger_coverage/scripts/swagger_report.py` & `test_swagger_coverage-2.1.54/swagger_coverage/scripts/swagger_report.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-0.1.54/swagger_coverage/src/check_data.py` & `test_swagger_coverage-2.1.54/swagger_coverage/src/check_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 from requests import Response
 
 from swagger_coverage.src.coverage import SwaggerCoverage
 
 
 class SwaggerChecker:
     def __init__(self):
-        self.data = SwaggerCoverage().data
+        self.swagger_data: dict = SwaggerCoverage().data.swagger_data
 
     def swagger_check(self, key: str, res: Response, time_execution: float) -> None:
         """
         Try to check response status code and swagger data
         """
-        dict_data = copy.deepcopy(self.data)
-        SwaggerCoverage().data = self._set_check_result(
+        dict_data = copy.deepcopy(self.swagger_data)
+        SwaggerCoverage().data.swagger_data = self._set_check_result(
             key, res.status_code, dict_data, time_execution
         )
+        pass
 
     @staticmethod
     def _set_check_result(
-        key: str, status_code: int, data, time_execution: float
+        key: str, status_code: int, data: dict, time_execution: float
     ) -> dict:
         """
         Set check result
         """
-        endpoint = data.swagger_data.get(key)
+        endpoint = data.get(key)
         if endpoint:
             if endpoint.get("time_executions") is None:
                 endpoint["time_executions"] = [time_execution]
             else:
                 t_exc = endpoint.get("time_executions")
                 t_exc.append(time_execution)
             statuses = endpoint.get("statuses")
```

### Comparing `test_swagger_coverage-0.1.54/swagger_coverage/src/deco.py` & `test_swagger_coverage-2.1.54/swagger_coverage/src/deco.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-0.1.54/swagger_coverage/src/logger.py` & `test_swagger_coverage-2.1.54/swagger_coverage/src/logger.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-0.1.54/swagger_coverage/src/prepare_data.py` & `test_swagger_coverage-2.1.54/swagger_coverage/src/prepare_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from typing import Dict
-
-import requests
-
 import logging
 
-import yaml
+from swagger_coverage.src.models.swagger_data import SwaggerResponse
 
 logger = logging.getLogger("swagger")
 
 
+def _prepare_swagger(data, status_codes):
+    res_dict = {}
+    for key, value in data.items():
+        list_values = list(value.values())
+        for values in list_values:
+            res_dict[values.get("operationId")] = []
+        for method, description in value.items():
+            res_dict[description.get("operationId")] = {
+                "method": method.upper(),
+                "description": description.get("description"),
+                "path": key,
+                "statuses": status_codes,
+                "tag": description.get("tags")[0],
+            }
+    return res_dict
+
+
+def _prepare_openapi(data, status_codes):
+    res_dict = {}
+    uuid = 1
+    for key, value in data.items():
+        for method, description in value.items():
+            res_dict[uuid] = {
+                "method": method.upper(),
+                "description": description.get("summary"),
+                "path": key,
+                "statuses": status_codes,
+                "tag": description.get("tags")[0],
+            }
+            uuid = uuid + 1
+    return res_dict
 class PrepareData:
-    @staticmethod
-    def load_swagger(url: str) -> Dict:
-        """
-        Load and get swagger data
-        """
-        logger.info(f"Start load swagger {url}")
-        res = requests.get(url)
-        if res.status_code == 200:
-            try:
-                data = yaml.safe_load(res.text)
-                return data.get("paths")
-            except Exception:
-                raise ValueError("Couldn't load yaml")
-        else:
-            logger.error(f"Couldn't get the file, status code is {res.status_code}")
-
-    @staticmethod
-    def prepare_swagger_data(data, status_codes: list) -> dict:
+    def prepare_swagger_data(self, data: SwaggerResponse, status_codes: list) -> dict:
         """
         Preparing data for tests
         :param status_codes:
         :param data:
         :return: swagger dict
         """
-        res_dict = {}
-        for key, value in data.items():
-            list_values = list(value.values())
-            for values in list_values:
-                res_dict[values.get("operationId")] = []
-            for k, v in value.items():
-                res_dict[v.get("operationId")] = {
-                    "method": k.upper(),
-                    "description": v.get("description"),
-                    "path": key,
-                    "statuses": status_codes,
-                    "tag": v.get("tags")[0],
-                    "time": [],
-                }
-        return res_dict
+        type_swagger = data.swagger_type
+        return self._map_prepare.get(type_swagger)(data.paths, status_codes)
 
     @staticmethod
     def prepare_check_file_data(data: dict) -> dict:
         """
         Prepare data for check
         """
         for k, value in data.items():
             statuses = value.get("statuses")
             if statuses:
                 new_statuses = []
                 for s in statuses:
                     new_statuses.append({s: 0})
                 value["statuses"] = new_statuses
         return data
+
+    _map_prepare = {"swagger": _prepare_swagger, "openapi": _prepare_openapi}
+
```

### Comparing `test_swagger_coverage-0.1.54/PKG-INFO` & `test_swagger_coverage-2.1.54/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: test-swagger-coverage
-Version: 0.1.54
+Version: 2.1.54
 Summary: Swagger coverage for API tests
 Home-page: https://github.com/berpress/swagger-coverage
 Author: alexanderlozovoy
 Author-email: berpress@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/berpress/swagger-coverage
 Description-Content-Type: text/markdown
 
 # swagger-coverage
 [![Tests](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml/badge.svg)](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml)
 ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/maintainability)](https://codeclimate.com/github/berpress/swagger-coverage/maintainability)
```

