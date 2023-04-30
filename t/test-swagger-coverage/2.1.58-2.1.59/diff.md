# Comparing `tmp/test_swagger_coverage-2.1.58.tar.gz` & `tmp/test_swagger_coverage-2.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_swagger_coverage-2.1.58.tar", max compression
+gzip compressed data, was "test_swagger_coverage-2.1.59.tar", max compression
```

## Comparing `test_swagger_coverage-2.1.58.tar` & `test_swagger_coverage-2.1.59.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-2.1.58/LICENSE
--rw-r--r--   0        0        0     5845 2023-04-10 11:50:18.637247 test_swagger_coverage-2.1.58/README.md
--rw-r--r--   0        0        0      667 2023-04-30 09:14:08.444908 test_swagger_coverage-2.1.58/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 08:08:13.320535 test_swagger_coverage-2.1.58/swagger_coverage/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-14 08:15:46.280403 test_swagger_coverage-2.1.58/swagger_coverage/scripts/swagger_report.py
--rw-r--r--   0        0        0        0 2023-04-14 08:08:31.328063 test_swagger_coverage-2.1.58/swagger_coverage/src/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-14 13:05:24.138537 test_swagger_coverage-2.1.58/swagger_coverage/src/check_data.py
--rw-r--r--   0        0        0     3195 2023-04-30 08:04:55.295455 test_swagger_coverage-2.1.58/swagger_coverage/src/coverage.py
--rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-2.1.58/swagger_coverage/src/deco.py
--rw-r--r--   0        0        0     2056 2023-04-27 16:02:40.028529 test_swagger_coverage-2.1.58/swagger_coverage/src/files.py
--rw-r--r--   0        0        0      849 2023-04-14 08:16:42.485998 test_swagger_coverage-2.1.58/swagger_coverage/src/logger.py
--rw-r--r--   0        0        0        0 2023-04-14 11:31:54.617585 test_swagger_coverage-2.1.58/swagger_coverage/src/models/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-27 16:01:57.068459 test_swagger_coverage-2.1.58/swagger_coverage/src/models/stats.py
--rw-r--r--   0        0        0      461 2023-04-27 14:54:00.916774 test_swagger_coverage-2.1.58/swagger_coverage/src/models/swagger_data.py
--rw-r--r--   0        0        0     2060 2023-04-27 16:24:53.724437 test_swagger_coverage-2.1.58/swagger_coverage/src/prepare_data.py
--rw-r--r--   0        0        0        0 2023-04-19 15:29:27.954717 test_swagger_coverage-2.1.58/swagger_coverage/src/report/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 15:29:45.222122 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/__init__.py
--rw-r--r--   0        0        0     6123 2023-04-27 16:03:56.022244 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/accordion.py
--rw-r--r--   0        0        0      883 2023-04-27 16:03:26.744052 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/body.py
--rw-r--r--   0        0        0      766 2023-04-27 16:03:55.974209 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/btn_group.py
--rw-r--r--   0        0        0      196 2023-04-27 16:01:57.073937 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/colors.py
--rw-r--r--   0        0        0      165 2023-04-27 16:01:57.076766 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/constants.py
--rw-r--r--   0        0        0      235 2023-04-27 16:01:57.084743 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/h2.py
--rw-r--r--   0        0        0      710 2023-04-27 16:03:55.971852 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/head.py
--rw-r--r--   0        0        0      180 2023-04-27 16:01:57.092106 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/href.py
--rw-r--r--   0        0        0     4706 2023-04-30 07:05:11.452022 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/html_report.py
--rw-r--r--   0        0        0      883 2023-04-27 16:01:57.123593 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/models.py
--rw-r--r--   0        0        0      670 2023-04-27 16:03:54.865325 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/navbar.py
--rw-r--r--   0        0        0      132 2023-04-27 16:01:57.095766 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/p.py
--rw-r--r--   0        0        0      446 2023-04-27 16:01:57.121785 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/prepare_data.py
--rw-r--r--   0        0        0      829 2023-04-27 16:06:14.093094 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/progress.py
--rw-r--r--   0        0        0     2911 2023-04-27 16:01:57.330789 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/scripts.py
--rw-r--r--   0        0        0     2027 2023-04-30 09:13:46.596899 test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/table.py
--rw-r--r--   0        0        0        0 2023-04-19 15:29:38.904729 test_swagger_coverage-2.1.58/swagger_coverage/src/report/plain/__init__.py
--rw-r--r--   0        0        0       64 2023-04-27 16:01:57.115041 test_swagger_coverage-2.1.58/swagger_coverage/src/report/plain/plain_report.py
--rw-r--r--   0        0        0        0 2023-04-19 15:29:33.654900 test_swagger_coverage-2.1.58/swagger_coverage/src/report/report.py
--rw-r--r--   0        0        0      710 2023-04-30 08:39:24.664235 test_swagger_coverage-2.1.58/swagger_coverage/src/requests.py
--rw-r--r--   0        0        0        0 2023-04-17 15:15:04.775886 test_swagger_coverage-2.1.58/swagger_coverage/src/results/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-27 16:19:19.207957 test_swagger_coverage-2.1.58/swagger_coverage/src/results/load_results.py
--rw-r--r--   0        0        0      550 2023-04-27 16:01:57.133390 test_swagger_coverage-2.1.58/swagger_coverage/src/results/swagger_diff.py
--rw-r--r--   0        0        0     1470 2023-04-27 16:05:14.499393 test_swagger_coverage-2.1.58/swagger_coverage/src/results/swagger_results.py
--rw-r--r--   0        0        0     2907 2023-04-27 16:05:09.299861 test_swagger_coverage-2.1.58/swagger_coverage/src/results/swagger_summary.py
--rw-r--r--   0        0        0      326 2023-04-14 12:08:09.802242 test_swagger_coverage-2.1.58/swagger_coverage/src/singltone_like.py
--rw-r--r--   0        0        0      384 2023-04-27 16:01:57.142956 test_swagger_coverage-2.1.58/swagger_coverage/src/utils.py
--rw-r--r--   0        0        0     6532 1970-01-01 00:00:00.000000 test_swagger_coverage-2.1.58/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 11:50:18.636935 test_swagger_coverage-2.1.59/LICENSE
+-rw-r--r--   0        0        0     5418 2023-04-30 10:05:22.859355 test_swagger_coverage-2.1.59/README.md
+-rw-r--r--   0        0        0      667 2023-04-30 10:55:24.027848 test_swagger_coverage-2.1.59/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 08:08:13.320535 test_swagger_coverage-2.1.59/swagger_coverage/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-14 08:15:46.280403 test_swagger_coverage-2.1.59/swagger_coverage/scripts/swagger_report.py
+-rw-r--r--   0        0        0        0 2023-04-14 08:08:31.328063 test_swagger_coverage-2.1.59/swagger_coverage/src/__init__.py
+-rw-r--r--   0        0        0     1354 2023-04-14 13:05:24.138537 test_swagger_coverage-2.1.59/swagger_coverage/src/check_data.py
+-rw-r--r--   0        0        0     3225 2023-04-30 10:51:59.096355 test_swagger_coverage-2.1.59/swagger_coverage/src/coverage.py
+-rw-r--r--   0        0        0      576 2023-04-10 11:50:18.638741 test_swagger_coverage-2.1.59/swagger_coverage/src/deco.py
+-rw-r--r--   0        0        0     2056 2023-04-27 16:02:40.028529 test_swagger_coverage-2.1.59/swagger_coverage/src/files.py
+-rw-r--r--   0        0        0      849 2023-04-14 08:16:42.485998 test_swagger_coverage-2.1.59/swagger_coverage/src/logger.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:31:54.617585 test_swagger_coverage-2.1.59/swagger_coverage/src/models/__init__.py
+-rw-r--r--   0        0        0     1175 2023-04-27 16:01:57.068459 test_swagger_coverage-2.1.59/swagger_coverage/src/models/stats.py
+-rw-r--r--   0        0        0      461 2023-04-27 14:54:00.916774 test_swagger_coverage-2.1.59/swagger_coverage/src/models/swagger_data.py
+-rw-r--r--   0        0        0     2060 2023-04-27 16:24:53.724437 test_swagger_coverage-2.1.59/swagger_coverage/src/prepare_data.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:29:27.954717 test_swagger_coverage-2.1.59/swagger_coverage/src/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:29:45.222122 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/__init__.py
+-rw-r--r--   0        0        0     6123 2023-04-27 16:03:56.022244 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/accordion.py
+-rw-r--r--   0        0        0      883 2023-04-27 16:03:26.744052 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/body.py
+-rw-r--r--   0        0        0      766 2023-04-27 16:03:55.974209 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/btn_group.py
+-rw-r--r--   0        0        0      196 2023-04-27 16:01:57.073937 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/colors.py
+-rw-r--r--   0        0        0      165 2023-04-27 16:01:57.076766 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/constants.py
+-rw-r--r--   0        0        0      235 2023-04-27 16:01:57.084743 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/h2.py
+-rw-r--r--   0        0        0      710 2023-04-27 16:03:55.971852 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/head.py
+-rw-r--r--   0        0        0      180 2023-04-27 16:01:57.092106 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/href.py
+-rw-r--r--   0        0        0     4706 2023-04-30 07:05:11.452022 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/html_report.py
+-rw-r--r--   0        0        0      883 2023-04-27 16:01:57.123593 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/models.py
+-rw-r--r--   0        0        0      670 2023-04-27 16:03:54.865325 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/navbar.py
+-rw-r--r--   0        0        0      132 2023-04-27 16:01:57.095766 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/p.py
+-rw-r--r--   0        0        0      446 2023-04-27 16:01:57.121785 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/prepare_data.py
+-rw-r--r--   0        0        0      829 2023-04-27 16:06:14.093094 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/progress.py
+-rw-r--r--   0        0        0     2911 2023-04-27 16:01:57.330789 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/scripts.py
+-rw-r--r--   0        0        0     2027 2023-04-30 09:13:46.596899 test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/table.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:29:38.904729 test_swagger_coverage-2.1.59/swagger_coverage/src/report/plain/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-27 16:01:57.115041 test_swagger_coverage-2.1.59/swagger_coverage/src/report/plain/plain_report.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:29:33.654900 test_swagger_coverage-2.1.59/swagger_coverage/src/report/report.py
+-rw-r--r--   0        0        0      710 2023-04-30 08:39:24.664235 test_swagger_coverage-2.1.59/swagger_coverage/src/requests.py
+-rw-r--r--   0        0        0        0 2023-04-17 15:15:04.775886 test_swagger_coverage-2.1.59/swagger_coverage/src/results/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-27 16:19:19.207957 test_swagger_coverage-2.1.59/swagger_coverage/src/results/load_results.py
+-rw-r--r--   0        0        0      550 2023-04-27 16:01:57.133390 test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_diff.py
+-rw-r--r--   0        0        0     1470 2023-04-27 16:05:14.499393 test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_results.py
+-rw-r--r--   0        0        0     2907 2023-04-27 16:05:09.299861 test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_summary.py
+-rw-r--r--   0        0        0      326 2023-04-14 12:08:09.802242 test_swagger_coverage-2.1.59/swagger_coverage/src/singltone_like.py
+-rw-r--r--   0        0        0      384 2023-04-27 16:01:57.142956 test_swagger_coverage-2.1.59/swagger_coverage/src/utils.py
+-rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 test_swagger_coverage-2.1.59/PKG-INFO
```

### Comparing `test_swagger_coverage-2.1.58/LICENSE` & `test_swagger_coverage-2.1.59/LICENSE`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/README.md` & `test_swagger_coverage-2.1.59/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # swagger-coverage
 [![Tests](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml/badge.svg)](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml)
 ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/maintainability)](https://codeclimate.com/github/berpress/swagger-coverage/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/test_coverage)](https://codeclimate.com/github/berpress/swagger-coverage/test_coverage)
 [![PyPI version](https://badge.fury.io/py/test-swagger-coverage.svg)](https://badge.fury.io/py/test-swagger-coverage)
 [![Downloads](https://pepy.tech/badge/test-swagger-coverage)](https://pepy.tech/project/test-swagger-coverage)
 
 About
 ------------
 
 Swagger coverage report helps the QA automation and developer to get a simple API coverage report for endpoints tests
@@ -32,48 +31,45 @@
 We will check which endpoints were called and what statuses we checked.
 
 We can't always trust our swagger, so you can manually set the status of the codes yourself, which need to be checked.
 
 Examples
 ------------
 
-First, we need a link to your swagger. For example,  let's take this  https://app.swaggerhub.com/apis-docs/berpress/flask-rest-api/1.0.0 (see more about this api https://github.com/berpress/flask-restful-api),
-and take url to yaml/yml/json swagger file - https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+First, we need a link to your swagger. For example,  let's take this  https://petstore.swagger.io/
 
 Next, in our project, we need to create a file describing our endpoints, which our tests will use to generate a coverage report.
 
-We can do it automatically via the command line
+We can do it automatically via the command line, get json swagger file
 
-    $ swagger_coverage https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+    $ swagger_coverage https://petstore.swagger.io/v2/swagger.json
 
 Result
 
-    $ 2022-04-15 11:22:37 INFO Start load swagger https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+    $ 2022-04-15 11:22:37 INFO Start load swagger swagger_coverage https://petstore.swagger.io/v2/swagger.json
     $ 2022-04-15 11:22:38 INFO The swagger report was successfully saved to the folder: /Users/user/Documents/git/python-api-tests/swagger_report
 
 
 
 The **swagger_report** directory will be created
 and a **data_swagger.yaml** file will appear inside, which will be the settings for building a test coverage report
 
 The **data_swagger.yaml** file looks something like this
 
 
  ```
  ...
-regUser:
-  description: null
+addPet:
+  description: 'Add new pet'
   method: POST
-  path: /register
+  path: /pet
   statuses:
-  - 201  <---- change from 200 to 201
-  - 400
-  - 401
-  - 403
-  tag: register
+  - 200
+  - 404
+  tag: pet
   ...
  ```
 
 where **regUser** is the unique id of our endpoint
 
 **statuses** is a list of statuses that we will check (that they were called).
 You can customize this list yourself.
```

### Comparing `test_swagger_coverage-2.1.58/pyproject.toml` & `test_swagger_coverage-2.1.59/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test-swagger-coverage"
-version = "2.1.58"
+version = "2.1.59"
 description = "Swagger coverage for API tests"
 authors = ["alexanderlozovoy <berpress@gmail.com>"]
 packages = [{ include = "swagger_coverage" }]
 readme = "README.md"
 repository = "https://github.com/berpress/swagger-coverage"
 
 [tool.poetry.dependencies]
```

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/scripts/swagger_report.py` & `test_swagger_coverage-2.1.59/swagger_coverage/scripts/swagger_report.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/check_data.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/check_data.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/coverage.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         results = SwaggerResults(self)
         return results.save_results(self.path)
 
     def create_report(self, path=_SWAGGER_REPORT_DIR, report_type="html"):
         # merge results
         result_path = f"{path}/json_results"
         if not is_file_exist(result_path):
-            self.save_results()
+            create_dir(self.path)
+        self.save_results()
         result_paths = get_json_result_path(path=result_path)
         load_results = LoadSwaggerResults()
         merge_result = load_results.merge_results(result_paths)
         # create report
         report = HtmlReport(merge_result)
         report.create(path)
```

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/deco.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/deco.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/files.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/files.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/logger.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/logger.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/models/stats.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/models/stats.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/prepare_data.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/prepare_data.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/accordion.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/accordion.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/body.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/body.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/btn_group.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/btn_group.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/head.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/head.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/html_report.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/html_report.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/models.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/models.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/navbar.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/navbar.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/progress.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/progress.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/scripts.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/scripts.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/report/html/table.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/report/html/table.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/requests.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/requests.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/results/load_results.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/results/load_results.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/results/swagger_diff.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_diff.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/results/swagger_results.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_results.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/swagger_coverage/src/results/swagger_summary.py` & `test_swagger_coverage-2.1.59/swagger_coverage/src/results/swagger_summary.py`

 * *Files identical despite different names*

### Comparing `test_swagger_coverage-2.1.58/PKG-INFO` & `test_swagger_coverage-2.1.59/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-swagger-coverage
-Version: 2.1.58
+Version: 2.1.59
 Summary: Swagger coverage for API tests
 Home-page: https://github.com/berpress/swagger-coverage
 Author: alexanderlozovoy
 Author-email: berpress@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,14 @@
 Project-URL: Repository, https://github.com/berpress/swagger-coverage
 Description-Content-Type: text/markdown
 
 # swagger-coverage
 [![Tests](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml/badge.svg)](https://github.com/berpress/swagger-coverage/actions/workflows/python-app.yml)
 ![versions](https://img.shields.io/pypi/pyversions/pybadges.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/maintainability)](https://codeclimate.com/github/berpress/swagger-coverage/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/45afb8b947b1c7e9cec8/test_coverage)](https://codeclimate.com/github/berpress/swagger-coverage/test_coverage)
 [![PyPI version](https://badge.fury.io/py/test-swagger-coverage.svg)](https://badge.fury.io/py/test-swagger-coverage)
 [![Downloads](https://pepy.tech/badge/test-swagger-coverage)](https://pepy.tech/project/test-swagger-coverage)
 
 About
 ------------
 
 Swagger coverage report helps the QA automation and developer to get a simple API coverage report for endpoints tests
@@ -50,48 +49,45 @@
 We will check which endpoints were called and what statuses we checked.
 
 We can't always trust our swagger, so you can manually set the status of the codes yourself, which need to be checked.
 
 Examples
 ------------
 
-First, we need a link to your swagger. For example,  let's take this  https://app.swaggerhub.com/apis-docs/berpress/flask-rest-api/1.0.0 (see more about this api https://github.com/berpress/flask-restful-api),
-and take url to yaml/yml/json swagger file - https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+First, we need a link to your swagger. For example,  let's take this  https://petstore.swagger.io/
 
 Next, in our project, we need to create a file describing our endpoints, which our tests will use to generate a coverage report.
 
-We can do it automatically via the command line
+We can do it automatically via the command line, get json swagger file
 
-    $ swagger_coverage https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+    $ swagger_coverage https://petstore.swagger.io/v2/swagger.json
 
 Result
 
-    $ 2022-04-15 11:22:37 INFO Start load swagger https://api.swaggerhub.com/apis/berpress/flask-rest-api/1.0.0
+    $ 2022-04-15 11:22:37 INFO Start load swagger swagger_coverage https://petstore.swagger.io/v2/swagger.json
     $ 2022-04-15 11:22:38 INFO The swagger report was successfully saved to the folder: /Users/user/Documents/git/python-api-tests/swagger_report
 
 
 
 The **swagger_report** directory will be created
 and a **data_swagger.yaml** file will appear inside, which will be the settings for building a test coverage report
 
 The **data_swagger.yaml** file looks something like this
 
 
  ```
  ...
-regUser:
-  description: null
+addPet:
+  description: 'Add new pet'
   method: POST
-  path: /register
+  path: /pet
   statuses:
-  - 201  <---- change from 200 to 201
-  - 400
-  - 401
-  - 403
-  tag: register
+  - 200
+  - 404
+  tag: pet
   ...
  ```
 
 where **regUser** is the unique id of our endpoint
 
 **statuses** is a list of statuses that we will check (that they were called).
 You can customize this list yourself.
```

