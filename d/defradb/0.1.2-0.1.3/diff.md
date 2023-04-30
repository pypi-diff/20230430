# Comparing `tmp/defradb-0.1.2.tar.gz` & `tmp/defradb-0.1.3.tar.gz`

## Comparing `defradb-0.1.2.tar` & `defradb-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 defradb-0.1.2/Makefile
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 defradb-0.1.2/requirements-dev.lock
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 defradb-0.1.2/requirements.lock
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 defradb-0.1.2/src/example.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 defradb-0.1.2/src/defradb/__init__.py
--rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 defradb-0.1.2/src/defradb/defradb.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 defradb-0.1.2/src/defradb/rpc/api_pb2.py
--rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 defradb-0.1.2/src/defradb/rpc/api_pb2_grpc.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 defradb-0.1.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 defradb-0.1.2/LICENSE
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 defradb-0.1.2/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 defradb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 defradb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 defradb-0.1.3/Makefile
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 defradb-0.1.3/example.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 defradb-0.1.3/requirements-dev.lock
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 defradb-0.1.3/requirements.lock
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 defradb-0.1.3/src/defradb/__init__.py
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 defradb-0.1.3/src/defradb/defradb.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 defradb-0.1.3/src/defradb/rpc/api_pb2.py
+-rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 defradb-0.1.3/src/defradb/rpc/api_pb2_grpc.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 defradb-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 defradb-0.1.3/LICENSE
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 defradb-0.1.3/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 defradb-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 defradb-0.1.3/PKG-INFO
```

### Comparing `defradb-0.1.2/Makefile` & `defradb-0.1.3/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -12,7 +12,12 @@
 	python -m grpc_tools.protoc -I $(REPO_NAME)/$(PROTO_DIR) --python_out=$(PYTHON_OUT) --grpc_python_out=$(PYTHON_OUT) $(PROTO_FILE) 
 
 clone:
 	if [ ! -d $(REPO) ]; then \
 		git clone $(REPO) $(REPO_NAME) || true; \
 	fi
 	cd $(REPO_NAME) && git pull origin master && cd -
+
+publish:
+	rm -rf ./dist
+	rye build
+	twine upload dist/*
```

### Comparing `defradb-0.1.2/requirements-dev.lock` & `defradb-0.1.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `defradb-0.1.2/requirements.lock` & `defradb-0.1.3/requirements.lock`

 * *Files identical despite different names*

### Comparing `defradb-0.1.2/src/example.py` & `defradb-0.1.3/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # A minimal example of how to use DefraClient.
 
 import uuid
 
 from gql import gql
 
-from defradb import (
+from src.defradb import (
     DefraClient,
     DefraConfig,
     dict_to_create_query,
 )
 
 # Configuring the client.
 endpoint = "localhost:9181/api/v0/"
```

### Comparing `defradb-0.1.2/src/defradb/defradb.py` & `defradb-0.1.3/src/defradb/defradb.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 @dataclass
 class DefraConfig:
     """
     Configuration for DefraDB client.
     """
 
-    api_url: str = "localhost:9181/api/v0"
+    api_url: str = "localhost:9181/api/v0/"
     tcp_multiaddr: str = "localhost:9161"
     scheme = "http://"
 
 
 class DefraClient:
     """
     Client for DefraDB, providing methods for interacting with the DefraDB node.
```

### Comparing `defradb-0.1.2/src/defradb/rpc/api_pb2.py` & `defradb-0.1.3/src/defradb/rpc/api_pb2.py`

 * *Files identical despite different names*

### Comparing `defradb-0.1.2/src/defradb/rpc/api_pb2_grpc.py` & `defradb-0.1.3/src/defradb/rpc/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `defradb-0.1.2/.gitignore` & `defradb-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `defradb-0.1.2/LICENSE` & `defradb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `defradb-0.1.2/pyproject.toml` & `defradb-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "defradb"
-version = "0.1.2"
+version = "0.1.3"
 description = "DefraDB Python client"
 authors = [
     { name = "Orpheus Lummis", email = "o@orpheuslummis.info" }
 ]
 dependencies = ["grpcio~=1.54.0", "requests~=2.29.0", "grpcio-tools~=1.54.0", "multiaddr~=0.0.9", "gql~=3.5.0b3", "aiohttp~=3.8", "requests_toolbelt~=0.10.1"]
 readme = "README.md"
 requires-python = ">= 3.10"
```

### Comparing `defradb-0.1.2/PKG-INFO` & `defradb-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defradb
-Version: 0.1.2
+Version: 0.1.3
 Summary: DefraDB Python client
 Project-URL: Homepage, https://github.com/sourcenetwork/defradb-client-py
 Project-URL: Bug Tracker, https://github.com/sourcenetwork/defradb-client-py/issues
 Author-email: Orpheus Lummis <o@orpheuslummis.info>
 License: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

