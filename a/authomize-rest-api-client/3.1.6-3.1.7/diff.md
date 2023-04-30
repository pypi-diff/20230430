# Comparing `tmp/authomize-rest-api-client-3.1.6.tar.gz` & `tmp/authomize-rest-api-client-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-3.1.6.tar", last modified: Wed Apr 19 21:40:02 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-3.1.7.tar", last modified: Sun Apr 30 12:19:10 2023, max compression
```

## Comparing `authomize-rest-api-client-3.1.6.tar` & `authomize-rest-api-client-3.1.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2120 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73155 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23487 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185133 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63873 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-19 21:39:42.000000 authomize-rest-api-client-3.1.6/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-19 21:40:02.000000 authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-04-19 21:40:02.665993 authomize-rest-api-client-3.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-04-19 21:39:45.000000 authomize-rest-api-client-3.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.090364 authomize-rest-api-client-3.1.7/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73614 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24331 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185721 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64787 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-04-30 12:18:54.000000 authomize-rest-api-client-3.1.7/setup.py
```

### Comparing `authomize-rest-api-client-3.1.6/LICENSE.txt` & `authomize-rest-api-client-3.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.6/README.md` & `authomize-rest-api-client-3.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 
 for connectors-rest-api:
 ```
 curl --socks5-hostname 127.0.0.1:1337 http://connectors-rest-api.application.svc:8080/openapi-extended.json | jq --indent 2 . > authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
 ```
 ```
 pip install -e .[codegen]
-datamodel-codegen --input authomize/rest_api_client/openapi/connectors_rest_api/openapi.json --output authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+datamodel-codegen --use-default-kwarg --input authomize/rest_api_client/openapi/connectors_rest_api/openapi.json --output authomize/rest_api_client/generated/connectors_rest_api/schemas.py
 ```
 
 for external-rest-api:
 ```
 curl https://apidev.authomize.com/openapi-platform.json | jq --indent 2 . > authomize/rest_api_client/openapi/external_rest_api/openapi.json
 ```
 ```
-datamodel-codegen --input authomize/rest_api_client/openapi/external_rest_api/openapi.json --output authomize/rest_api_client/generated/external_rest_api/schemas.py
+datamodel-codegen --use-default-kwarg --input authomize/rest_api_client/openapi/external_rest_api/openapi.json --output authomize/rest_api_client/generated/external_rest_api/schemas.py
 ```
```

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-04-19T21:29:38+00:00
+#   timestamp: 2023-04-30T09:35:02+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -454,14 +454,17 @@
         default=None,
         description='The uniqueId of the user who is the "owner" (or manager) of the group.\n',
         title='Owner',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags on the access grouping.\n', title='Tags'
     )
+    alternativeName: Optional[constr(max_length=256)] = Field(
+        default=None, description='Alias of the grouping.', title='Alternativename'
+    )
 
 
 class NewGroupingResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
         default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
@@ -936,14 +939,17 @@
         default=None,
         description='The uniqueId of the user who is the "owner" (or manager) of the group.\n',
         title='Owner',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags on the access grouping.\n', title='Tags'
     )
+    alternativeName: Optional[constr(max_length=256)] = Field(
+        default=None, description='Alias of the grouping.', title='Alternativename'
+    )
 
 
 class UpdateGroupingsResponseSchema(BaseModel):
     acceptedTimestamp: Optional[datetime] = Field(
         default=None,
         description='**The accepted time of the request**',
         title='Acceptedtimestamp',
@@ -1121,14 +1127,17 @@
         default=None,
         description='The uniqueId of the user who is the "owner" (or manager) of the group.\n',
         title='Owner',
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags on the access grouping.\n', title='Tags'
     )
+    alternativeName: Optional[constr(max_length=256)] = Field(
+        default=None, description='Alias of the grouping.', title='Alternativename'
+    )
 
 
 class HTTPValidationError(BaseModel):
     detail: Optional[List[ValidationError]] = Field(default=None, title='Detail')
 
 
 class IdentityDescription(BaseModel):
```

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-04-19T21:34:40+00:00
+#   timestamp: 2023-04-30T11:50:50+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -70,67 +70,37 @@
     Impact = 'Impact'
     Initial_Access = 'Initial Access'
     Lateral_Movement = 'Lateral Movement'
     Persistence = 'Persistence'
     Privilege_Escalation = 'Privilege Escalation'
 
 
-class BaseBooleanFilter(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    field_eq: Optional[bool] = Field(
-        default=None, alias='$eq', description='Equals To', title='$Eq'
-    )
-
-
-class BaseDateFilter(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    field_gt: Optional[datetime] = Field(
-        default=None, alias='$gt', description='Greater Than', title='$Gt'
-    )
-    field_gte: Optional[datetime] = Field(
-        default=None,
-        alias='$gte',
-        description='Greater Than Or Equals To',
-        title='$Gte',
-    )
-    field_lt: Optional[datetime] = Field(
-        default=None, alias='$lt', description='Less Than', title='$Lt'
-    )
-    field_lte: Optional[datetime] = Field(
-        default=None, alias='$lte', description='Less Than Or Equals To', title='$Lte'
-    )
-
-
-class BaseSingleValuedStringFilter(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    field_eq: Optional[str] = Field(
-        default=None, alias='$eq', description='Equals To', title='$Eq'
-    )
-
-
 class CampaignExpansion(Enum):
     owner = 'owner'
 
 
 class CampaignStatus(Enum):
     draft = 'draft'
     initializing = 'initializing'
     running = 'running'
     completed = 'completed'
     failed = 'failed'
     empty = 'empty'
     overdue = 'overdue'
 
 
+class CampaignStatusFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[CampaignStatus]] = Field(
+        default=None, alias='$in', description='In'
+    )
+
+
 class Ccm301Standard(Enum):
     AIS_04 = 'AIS-04'
     IAM_01 = 'IAM-01'
     IAM_02 = 'IAM-02'
     IAM_03 = 'IAM-03'
     IAM_04 = 'IAM-04'
     IAM_05 = 'IAM-05'
@@ -206,14 +176,21 @@
 
     id: str = Field(..., description='Unique ID of comment.', title='Id')
     content: constr(max_length=1025) = Field(
         ..., description='Content of comment.', title='Content'
     )
 
 
+class EventStatusType(Enum):
+    Open = 'Open'
+    InProgress = 'InProgress'
+    WaitingForInput = 'WaitingForInput'
+    Closed = 'Closed'
+
+
 class FieldName(Enum):
     name = 'name'
     status = 'status'
     startDate = 'startDate'
     endDate = 'endDate'
     createdAt = 'createdAt'
     reviewerType = 'reviewerType'
@@ -221,26 +198,90 @@
 
 
 class IncidentExpansion(Enum):
     policy = 'policy'
     assignee = 'assignee'
 
 
-class IncidentSeverity(Enum):
-    Low = 'Low'
-    Medium = 'Medium'
-    High = 'High'
-    Critical = 'Critical'
+class IncidentsCreatedAtFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_lte: Optional[datetime] = Field(
+        default=None, alias='$lte', description='Less Than Or Equals To', title='$Lte'
+    )
+    field_gte: Optional[datetime] = Field(
+        default=None,
+        alias='$gte',
+        description='Greater Than Or Equals To',
+        title='$Gte',
+    )
+    field_lt: Optional[datetime] = Field(
+        default=None, alias='$lt', description='Less Than', title='$Lt'
+    )
+    field_gt: Optional[datetime] = Field(
+        default=None, alias='$gt', description='Greater Than', title='$Gt'
+    )
 
 
-class IncidentStatus(Enum):
-    Open = 'Open'
-    InProgress = 'InProgress'
-    WaitingForInput = 'WaitingForInput'
-    Closed = 'Closed'
+class IncidentsIsResolvedFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_eq: Optional[bool] = Field(
+        default=None, alias='$eq', description='Equals To', title='$Eq'
+    )
+
+
+class IncidentsPolicyIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_eq: Optional[str] = Field(
+        default=None, alias='$eq', description='Equals To', title='$Eq'
+    )
+
+
+class IncidentsPolicyTempalteIdFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_eq: Optional[str] = Field(
+        default=None, alias='$eq', description='Equals To', title='$Eq'
+    )
+
+
+class IncidentsStatusFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[EventStatusType]] = Field(
+        default=None, alias='$in', description='In'
+    )
+
+
+class IncidentsUpdatedAtFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_lte: Optional[datetime] = Field(
+        default=None, alias='$lte', description='Less Than Or Equals To', title='$Lte'
+    )
+    field_gte: Optional[datetime] = Field(
+        default=None,
+        alias='$gte',
+        description='Greater Than Or Equals To',
+        title='$Gte',
+    )
+    field_lt: Optional[datetime] = Field(
+        default=None, alias='$lt', description='Less Than', title='$Lt'
+    )
+    field_gt: Optional[datetime] = Field(
+        default=None, alias='$gt', description='Greater Than', title='$Gt'
+    )
 
 
 class InventoryObjects(Enum):
     identity = 'identity'
     account = 'account'
     asset = 'asset'
     privilege = 'privilege'
@@ -271,15 +312,15 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='3.1.5', description='**version**', title='Version'
+        default='3.1.6', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
@@ -340,14 +381,21 @@
 
 class Selection(Enum):
     keep = 'keep'
     revoke = 'revoke'
     null = 'null'
 
 
+class SeverityType(Enum):
+    Low = 'Low'
+    Medium = 'Medium'
+    High = 'High'
+    Critical = 'Critical'
+
+
 class SortOrder(Enum):
     ASC = 'ASC'
     DESC = 'DESC'
 
 
 class SortSchemaFieldName(BaseModel):
     class Config:
@@ -383,19 +431,19 @@
         extra = Extra.forbid
 
     assigneeId: Optional[str] = Field(
         default=None,
         description='ID of the entity assigned to this incident.',
         title='Assigneeid',
     )
-    status: Optional[IncidentStatus] = Field(
+    status: Optional[EventStatusType] = Field(
         default=None,
         description='The status of the incident (Open, InProgress, WaitingForInput, or Closed).',
     )
-    severity: Optional[IncidentSeverity] = Field(
+    severity: Optional[SeverityType] = Field(
         default=None,
         description='The severity of the incident (Low, Medium, High or Critical).',
     )
 
 
 class UserSchema(BaseModel):
     userId: str = Field(..., description='Unique ID', title='Userid')
@@ -416,55 +464,28 @@
         default='aicpaTsc2017', description='UniqueID', title='Id'
     )
     name: Optional[str] = Field(
         default='SOC 2 (TSC 2017)', description='Name', title='Name'
     )
 
 
-class BasicEnumFilterCampaignStatus(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    field_in: Optional[List[CampaignStatus]] = Field(
-        default=None, alias='$in', description='In'
-    )
-
-
-class BasicEnumFilterIncidentSeverity(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    field_in: Optional[List[IncidentSeverity]] = Field(
-        default=None, alias='$in', description='In'
-    )
-
-
-class BasicEnumFilterIncidentStatus(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    field_in: Optional[List[IncidentStatus]] = Field(
-        default=None, alias='$in', description='In'
-    )
-
-
-class BasicEnumFilterSelection(BaseModel):
+class CampaignPermissionDecisionFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[Selection]] = Field(
         default=None, alias='$in', description='In'
     )
 
 
 class CampaignPermissionsSearchFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    decision: Optional[BasicEnumFilterSelection] = Field(
+    decision: Optional[CampaignPermissionDecisionFilter] = Field(
         default=None,
         description='Reviewer decisions (keep, revoke or null).\n',
         title='Decision',
     )
 
 
 class CampaignSchema(BaseModel):
@@ -488,15 +509,15 @@
     )
 
 
 class CampaignSearchFilterBody(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    status: Optional[BasicEnumFilterCampaignStatus] = Field(
+    status: Optional[CampaignStatusFilter] = Field(
         default=None,
         description='Enum: "draft" "initializing" "running" "completed" "failed" "empty" "overdue"\n',
         title='Status',
     )
 
 
 class Ccm301(BaseModel):
@@ -532,14 +553,23 @@
         default=None, description='Origin ID', title='Originid'
     )
     originType: Optional[str] = Field(
         default=None, description='Origin Type', title='Origintype'
     )
 
 
+class IncidentsSeverityFilter(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    field_in: Optional[List[SeverityType]] = Field(
+        default=None, alias='$in', description='In'
+    )
+
+
 class IsoIec27001(BaseModel):
     values: List[IsoIec27001Standard] = Field(..., description='Values')
     id: Optional[str] = Field(default='isoIec27001', description='UniqueID', title='Id')
     name: Optional[str] = Field(
         default='ISO/IEC 27001', description='Name', title='Name'
     )
 
@@ -614,33 +644,33 @@
     )
 
 
 class SearchIncidentsFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    createdAt: Optional[BaseDateFilter] = Field(
+    createdAt: Optional[IncidentsCreatedAtFilter] = Field(
         default=None, description='Created At date', title='Createdat'
     )
-    updatedAt: Optional[BaseDateFilter] = Field(
+    updatedAt: Optional[IncidentsUpdatedAtFilter] = Field(
         default=None, description='Updated At date', title='Updatedat'
     )
-    severity: Optional[BasicEnumFilterIncidentSeverity] = Field(
+    severity: Optional[IncidentsSeverityFilter] = Field(
         default=None, description='Severity', title='Severity'
     )
-    status: Optional[BasicEnumFilterIncidentStatus] = Field(
+    status: Optional[IncidentsStatusFilter] = Field(
         default=None, description='Status', title='Status'
     )
-    policyId: Optional[BaseSingleValuedStringFilter] = Field(
+    policyId: Optional[IncidentsPolicyIdFilter] = Field(
         default=None, description='Policy Id ', title='Policyid'
     )
-    policyTemplateId: Optional[BaseSingleValuedStringFilter] = Field(
+    policyTemplateId: Optional[IncidentsPolicyTempalteIdFilter] = Field(
         default=None, description='Policy Template ID', title='Policytemplateid'
     )
-    isResolved: Optional[BaseBooleanFilter] = Field(
+    isResolved: Optional[IncidentsIsResolvedFilter] = Field(
         default=None, description='Is resolved?', title='Isresolved'
     )
 
 
 class SearchIncidentsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -722,19 +752,19 @@
     tactics: Optional[List[AttackTacticType]] = Field(default=[], description='Tactics')
     compliance: Optional[
         List[Union[IsoIec27001, AicpaTsc2017, Ccm402, Ccm301, Cisv8]]
     ] = Field(default=[], description='Compliance', title='Compliance')
     techniques: Optional[List[str]] = Field(
         default=[], description='Techniques', title='Techniques'
     )
-    status: Optional[IncidentStatus] = Field(
+    status: Optional[EventStatusType] = Field(
         default=None,
         description='The status of the incident (Open, In Progress, Waiting for Input, or Closed)',
     )
-    severity: IncidentSeverity = Field(
+    severity: SeverityType = Field(
         ..., description='The severity of the incident (Low, Medium, High or Critical).'
     )
     policyId: str = Field(..., description='Unique id of policy.', title='Policyid')
     policy: Optional[PolicySchema] = Field(
         default=None, description='Policy', title='Policy'
     )
     assigneeId: Optional[str] = Field(
```

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874931498015874%*

 * *Differences: {"'components'": "{'schemas': {'GroupingSchema': {'properties': {'alternativeName': "*

 * *                 "OrderedDict([('title', 'Alternativename'), ('maxLength', 256), ('type', "*

 * *                 "'string'), ('description', 'Alias of the grouping.')])}}, "*

 * *                 "'NewGroupingRequestSchema': {'properties': {'alternativeName': "*

 * *                 "OrderedDict([('title', 'Alternativename'), ('maxLength', 256), ('type', "*

 * *                 "'string'), ('description', 'Alias of the grouping.')])}}, "*

 * *    […]*

```diff
@@ -422,14 +422,20 @@
                 ],
                 "title": "ExportResponse",
                 "type": "object"
             },
             "GroupingSchema": {
                 "description": "Grouping schema",
                 "properties": {
+                    "alternativeName": {
+                        "description": "Alias of the grouping.",
+                        "maxLength": 256,
+                        "title": "Alternativename",
+                        "type": "string"
+                    },
                     "anyoneCanJoinOrLeave": {
                         "default": false,
                         "description": "Must be either `ture` or `false`.\nWhen set to `true` users can give themselves membership in this grouping without the grouping's managers' or owners' permission. \nExamples include public groups (M365), Google Groups with specific flags, ...\nValid only when `groupingType = Group`\n",
                         "title": "Anyonecanjoinorleave",
                         "type": "boolean"
                     },
                     "isRole": {
@@ -1409,14 +1415,20 @@
                 ],
                 "title": "NewAssetsResponseSchema",
                 "type": "object"
             },
             "NewGroupingRequestSchema": {
                 "description": "New group request schema",
                 "properties": {
+                    "alternativeName": {
+                        "description": "Alias of the grouping.",
+                        "maxLength": 256,
+                        "title": "Alternativename",
+                        "type": "string"
+                    },
                     "anyoneCanJoinOrLeave": {
                         "default": false,
                         "description": "Must be either `ture` or `false`.\nWhen set to `true` users can give themselves membership in this grouping without the grouping's managers' or owners' permission. \nExamples include public groups (M365), Google Groups with specific flags, ...\nValid only when `groupingType = Group`\n",
                         "title": "Anyonecanjoinorleave",
                         "type": "boolean"
                     },
                     "isRole": {
@@ -3180,14 +3192,20 @@
                 ],
                 "title": "UpdateGroupingsListRequestSchema",
                 "type": "object"
             },
             "UpdateGroupingsRequestSchema": {
                 "description": "New group request schema",
                 "properties": {
+                    "alternativeName": {
+                        "description": "Alias of the grouping.",
+                        "maxLength": 256,
+                        "title": "Alternativename",
+                        "type": "string"
+                    },
                     "anyoneCanJoinOrLeave": {
                         "default": false,
                         "description": "Must be either `ture` or `false`.\nWhen set to `true` users can give themselves membership in this grouping without the grouping's managers' or owners' permission. \nExamples include public groups (M365), Google Groups with specific flags, ...\nValid only when `groupingType = Group`\n",
                         "title": "Anyonecanjoinorleave",
                         "type": "boolean"
                     },
                     "isRole": {
@@ -3701,15 +3719,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "3.1.5",
+        "version": "3.1.6",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -5450,15 +5468,15 @@
                         "schema": {
                             "title": "Appid",
                             "type": "string"
                         }
                     },
                     {
                         "description": "Delete all the app data lastly updated before the given date.",
-                        "example": "2023-04-19T21:27:04.123723+00:00",
+                        "example": "2023-04-30T09:34:20.489062+00:00",
                         "in": "query",
                         "name": "modifiedBefore",
                         "required": false,
                         "schema": {
                             "description": "Delete all the app data lastly updated before the given date.",
                             "format": "date-time",
                             "title": "Modifiedbefore",
```

### Comparing `authomize-rest-api-client-3.1.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9810032316230919%*

 * *Differences: {"'components'": "{'schemas': {'CampaignPermissionsSearchFilterBody': {'properties': {'decision': "*

 * *                 "{'allOf': {0: {'$ref': "*

 * *                 "'#/components/schemas/CampaignPermissionDecisionFilter'}}}}}, "*

 * *                 "'CampaignSearchFilterBody': {'properties': {'status': {'allOf': {0: {'$ref': "*

 * *                 "'#/components/schemas/CampaignStatusFilter'}}}}}, 'IncidentSchema': "*

 * *                 "{'properties': {'status': {'allOf': {0: {'$ref': "*

 * *                 "'#/components/s […]*

```diff
@@ -113,144 +113,44 @@
                     "Initial Access",
                     "Lateral Movement",
                     "Persistence",
                     "Privilege Escalation"
                 ],
                 "title": "AttackTacticType"
             },
-            "BaseBooleanFilter": {
-                "additionalProperties": false,
-                "description": "Base schema for all incoming API requests.",
-                "properties": {
-                    "$eq": {
-                        "description": "Equals To",
-                        "title": "$Eq",
-                        "type": "boolean"
-                    }
-                },
-                "title": "BaseBooleanFilter",
-                "type": "object"
-            },
-            "BaseDateFilter": {
-                "additionalProperties": false,
-                "description": "Base schema for all incoming API requests.",
-                "properties": {
-                    "$gt": {
-                        "description": "Greater Than",
-                        "format": "date-time",
-                        "title": "$Gt",
-                        "type": "string"
-                    },
-                    "$gte": {
-                        "description": "Greater Than Or Equals To",
-                        "format": "date-time",
-                        "title": "$Gte",
-                        "type": "string"
-                    },
-                    "$lt": {
-                        "description": "Less Than",
-                        "format": "date-time",
-                        "title": "$Lt",
-                        "type": "string"
-                    },
-                    "$lte": {
-                        "description": "Less Than Or Equals To",
-                        "format": "date-time",
-                        "title": "$Lte",
-                        "type": "string"
-                    }
-                },
-                "title": "BaseDateFilter",
-                "type": "object"
-            },
-            "BaseSingleValuedStringFilter": {
-                "additionalProperties": false,
-                "description": "Base schema for all incoming API requests.",
-                "properties": {
-                    "$eq": {
-                        "description": "Equals To",
-                        "title": "$Eq",
-                        "type": "string"
-                    }
-                },
-                "title": "BaseSingleValuedStringFilter",
-                "type": "object"
-            },
-            "BasicEnumFilter_CampaignStatus_": {
-                "additionalProperties": false,
-                "properties": {
-                    "$in": {
-                        "description": "In",
-                        "items": {
-                            "$ref": "#/components/schemas/CampaignStatus"
-                        },
-                        "type": "array"
-                    }
-                },
-                "title": "BasicEnumFilter[CampaignStatus]",
-                "type": "object"
-            },
-            "BasicEnumFilter_IncidentSeverity_": {
-                "additionalProperties": false,
-                "properties": {
-                    "$in": {
-                        "description": "In",
-                        "items": {
-                            "$ref": "#/components/schemas/IncidentSeverity"
-                        },
-                        "type": "array"
-                    }
-                },
-                "title": "BasicEnumFilter[IncidentSeverity]",
-                "type": "object"
-            },
-            "BasicEnumFilter_IncidentStatus_": {
-                "additionalProperties": false,
-                "properties": {
-                    "$in": {
-                        "description": "In",
-                        "items": {
-                            "$ref": "#/components/schemas/IncidentStatus"
-                        },
-                        "type": "array"
-                    }
-                },
-                "title": "BasicEnumFilter[IncidentStatus]",
-                "type": "object"
+            "CampaignExpansion": {
+                "description": "An enumeration.",
+                "enum": [
+                    "owner"
+                ],
+                "title": "CampaignExpansion",
+                "type": "string"
             },
-            "BasicEnumFilter_Selection_": {
+            "CampaignPermissionDecisionFilter": {
                 "additionalProperties": false,
                 "properties": {
                     "$in": {
                         "description": "In",
                         "items": {
                             "$ref": "#/components/schemas/Selection"
                         },
                         "type": "array"
                     }
                 },
-                "title": "BasicEnumFilter[Selection]",
+                "title": "CampaignPermissionDecisionFilter",
                 "type": "object"
             },
-            "CampaignExpansion": {
-                "description": "An enumeration.",
-                "enum": [
-                    "owner"
-                ],
-                "title": "CampaignExpansion",
-                "type": "string"
-            },
             "CampaignPermissionsSearchFilterBody": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "decision": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BasicEnumFilter_Selection_"
+                                "$ref": "#/components/schemas/CampaignPermissionDecisionFilter"
                             }
                         ],
                         "description": "Reviewer decisions (keep, revoke or null).\n",
                         "title": "Decision"
                     }
                 },
                 "title": "CampaignPermissionsSearchFilterBody",
@@ -325,15 +225,15 @@
             "CampaignSearchFilterBody": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "status": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BasicEnumFilter_CampaignStatus_"
+                                "$ref": "#/components/schemas/CampaignStatusFilter"
                             }
                         ],
                         "description": "Enum: \"draft\" \"initializing\" \"running\" \"completed\" \"failed\" \"empty\" \"overdue\"\n",
                         "title": "Status"
                     }
                 },
                 "title": "CampaignSearchFilterBody",
@@ -348,14 +248,28 @@
                     "completed",
                     "failed",
                     "empty",
                     "overdue"
                 ],
                 "title": "CampaignStatus"
             },
+            "CampaignStatusFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "description": "In",
+                        "items": {
+                            "$ref": "#/components/schemas/CampaignStatus"
+                        },
+                        "type": "array"
+                    }
+                },
+                "title": "CampaignStatusFilter",
+                "type": "object"
+            },
             "CampaignsPermissionSchema": {
                 "properties": {
                     "accessById": {
                         "description": "Access by ID (Account or Grouping ID) that their access was reviewed. \n",
                         "title": "Accessbyid",
                         "type": "string"
                     },
@@ -614,14 +528,24 @@
                 "required": [
                     "id",
                     "content"
                 ],
                 "title": "CommentSchema",
                 "type": "object"
             },
+            "EventStatusType": {
+                "description": "An enumeration.",
+                "enum": [
+                    "Open",
+                    "InProgress",
+                    "WaitingForInput",
+                    "Closed"
+                ],
+                "title": "EventStatusType"
+            },
             "FieldName": {
                 "description": "An enumeration.",
                 "enum": [
                     "name",
                     "status",
                     "startDate",
                     "endDate",
@@ -806,23 +730,23 @@
                         "description": "Recommendation",
                         "title": "Recommendation",
                         "type": "string"
                     },
                     "severity": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/IncidentSeverity"
+                                "$ref": "#/components/schemas/SeverityType"
                             }
                         ],
                         "description": "The severity of the incident (Low, Medium, High or Critical)."
                     },
                     "status": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/IncidentStatus"
+                                "$ref": "#/components/schemas/EventStatusType"
                             }
                         ],
                         "description": "The status of the incident (Open, In Progress, Waiting for Input, or Closed)"
                     },
                     "tactics": {
                         "default": [],
                         "description": "Tactics",
@@ -858,35 +782,139 @@
                     "policyId",
                     "isResolved",
                     "url"
                 ],
                 "title": "IncidentSchema",
                 "type": "object"
             },
-            "IncidentSeverity": {
-                "description": "An enumeration.",
-                "enum": [
-                    "Low",
-                    "Medium",
-                    "High",
-                    "Critical"
-                ],
-                "title": "IncidentSeverity",
-                "type": "string"
+            "IncidentsCreatedAtFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$gt": {
+                        "description": "Greater Than",
+                        "format": "date-time",
+                        "title": "$Gt",
+                        "type": "string"
+                    },
+                    "$gte": {
+                        "description": "Greater Than Or Equals To",
+                        "format": "date-time",
+                        "title": "$Gte",
+                        "type": "string"
+                    },
+                    "$lt": {
+                        "description": "Less Than",
+                        "format": "date-time",
+                        "title": "$Lt",
+                        "type": "string"
+                    },
+                    "$lte": {
+                        "description": "Less Than Or Equals To",
+                        "format": "date-time",
+                        "title": "$Lte",
+                        "type": "string"
+                    }
+                },
+                "title": "IncidentsCreatedAtFilter",
+                "type": "object"
             },
-            "IncidentStatus": {
-                "description": "An enumeration.",
-                "enum": [
-                    "Open",
-                    "InProgress",
-                    "WaitingForInput",
-                    "Closed"
-                ],
-                "title": "IncidentStatus",
-                "type": "string"
+            "IncidentsIsResolvedFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$eq": {
+                        "description": "Equals To",
+                        "title": "$Eq",
+                        "type": "boolean"
+                    }
+                },
+                "title": "IncidentsIsResolvedFilter",
+                "type": "object"
+            },
+            "IncidentsPolicyIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$eq": {
+                        "description": "Equals To",
+                        "title": "$Eq",
+                        "type": "string"
+                    }
+                },
+                "title": "IncidentsPolicyIdFilter",
+                "type": "object"
+            },
+            "IncidentsPolicyTempalteIdFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$eq": {
+                        "description": "Equals To",
+                        "title": "$Eq",
+                        "type": "string"
+                    }
+                },
+                "title": "IncidentsPolicyTempalteIdFilter",
+                "type": "object"
+            },
+            "IncidentsSeverityFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "description": "In",
+                        "items": {
+                            "$ref": "#/components/schemas/SeverityType"
+                        },
+                        "type": "array"
+                    }
+                },
+                "title": "IncidentsSeverityFilter",
+                "type": "object"
+            },
+            "IncidentsStatusFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$in": {
+                        "description": "In",
+                        "items": {
+                            "$ref": "#/components/schemas/EventStatusType"
+                        },
+                        "type": "array"
+                    }
+                },
+                "title": "IncidentsStatusFilter",
+                "type": "object"
+            },
+            "IncidentsUpdatedAtFilter": {
+                "additionalProperties": false,
+                "properties": {
+                    "$gt": {
+                        "description": "Greater Than",
+                        "format": "date-time",
+                        "title": "$Gt",
+                        "type": "string"
+                    },
+                    "$gte": {
+                        "description": "Greater Than Or Equals To",
+                        "format": "date-time",
+                        "title": "$Gte",
+                        "type": "string"
+                    },
+                    "$lt": {
+                        "description": "Less Than",
+                        "format": "date-time",
+                        "title": "$Lt",
+                        "type": "string"
+                    },
+                    "$lte": {
+                        "description": "Less Than Or Equals To",
+                        "format": "date-time",
+                        "title": "$Lte",
+                        "type": "string"
+                    }
+                },
+                "title": "IncidentsUpdatedAtFilter",
+                "type": "object"
             },
             "InventoryObjects": {
                 "description": "An enumeration.",
                 "enum": [
                     "identity",
                     "account",
                     "asset",
@@ -972,15 +1000,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "3.1.5",
+                        "default": "3.1.6",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1379,69 +1407,69 @@
             "SearchIncidentsFilter": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "createdAt": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BaseDateFilter"
+                                "$ref": "#/components/schemas/IncidentsCreatedAtFilter"
                             }
                         ],
                         "description": "Created At date",
                         "title": "Createdat"
                     },
                     "isResolved": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BaseBooleanFilter"
+                                "$ref": "#/components/schemas/IncidentsIsResolvedFilter"
                             }
                         ],
                         "description": "Is resolved?",
                         "title": "Isresolved"
                     },
                     "policyId": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BaseSingleValuedStringFilter"
+                                "$ref": "#/components/schemas/IncidentsPolicyIdFilter"
                             }
                         ],
                         "description": "Policy Id ",
                         "title": "Policyid"
                     },
                     "policyTemplateId": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BaseSingleValuedStringFilter"
+                                "$ref": "#/components/schemas/IncidentsPolicyTempalteIdFilter"
                             }
                         ],
                         "description": "Policy Template ID",
                         "title": "Policytemplateid"
                     },
                     "severity": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BasicEnumFilter_IncidentSeverity_"
+                                "$ref": "#/components/schemas/IncidentsSeverityFilter"
                             }
                         ],
                         "description": "Severity",
                         "title": "Severity"
                     },
                     "status": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BasicEnumFilter_IncidentStatus_"
+                                "$ref": "#/components/schemas/IncidentsStatusFilter"
                             }
                         ],
                         "description": "Status",
                         "title": "Status"
                     },
                     "updatedAt": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/BaseDateFilter"
+                                "$ref": "#/components/schemas/IncidentsUpdatedAtFilter"
                             }
                         ],
                         "description": "Updated At date",
                         "title": "Updatedat"
                     }
                 },
                 "title": "SearchIncidentsFilter",
@@ -1505,14 +1533,24 @@
                 "enum": [
                     "keep",
                     "revoke",
                     "null"
                 ],
                 "title": "Selection"
             },
+            "SeverityType": {
+                "description": "An enumeration.",
+                "enum": [
+                    "Low",
+                    "Medium",
+                    "High",
+                    "Critical"
+                ],
+                "title": "SeverityType"
+            },
             "SortOrder": {
                 "description": "An enumeration.",
                 "enum": [
                     "ASC",
                     "DESC"
                 ],
                 "title": "SortOrder",
@@ -1604,23 +1642,23 @@
                         "description": "ID of the entity assigned to this incident.",
                         "title": "Assigneeid",
                         "type": "string"
                     },
                     "severity": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/IncidentSeverity"
+                                "$ref": "#/components/schemas/SeverityType"
                             }
                         ],
                         "description": "The severity of the incident (Low, Medium, High or Critical)."
                     },
                     "status": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/IncidentStatus"
+                                "$ref": "#/components/schemas/EventStatusType"
                             }
                         ],
                         "description": "The status of the incident (Open, InProgress, WaitingForInput, or Closed)."
                     }
                 },
                 "title": "UpdateIncidentRequestSchema",
                 "type": "object"
@@ -1691,15 +1729,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "3.1.5",
+        "version": "3.1.6",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
```

### Comparing `authomize-rest-api-client-3.1.6/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.6/setup.py` & `authomize-rest-api-client-3.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='3.1.6',
+        version='3.1.7',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

