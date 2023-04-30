# Comparing `tmp/jiggybase-0.0.17.tar.gz` & `tmp/jiggybase-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.17.tar", last modified: Sat Apr 29 04:16:05 2023, max compression
+gzip compressed data, was "jiggybase-0.0.18.tar", last modified: Sun Apr 30 01:07:28 2023, max compression
```

## Comparing `jiggybase-0.0.17.tar` & `jiggybase-0.0.18.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.818916 jiggybase-0.0.17/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.17/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)      533 2023-04-29 04:16:05.818577 jiggybase-0.0.17/PKG-INFO
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.812430 jiggybase-0.0.17/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.17/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1769 2023-04-28 15:29:35.000000 jiggybase-0.0.17/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     8278 2023-04-29 04:07:23.000000 jiggybase-0.0.17/jiggybase/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 jiggybase-0.0.17/jiggybase/config.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.17/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.17/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.817708 jiggybase-0.0.17/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.17/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.17/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.17/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.17/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.17/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.17/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.17/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.17/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.17/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.17/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.17/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.17/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.17/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.17/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4315 2023-04-24 00:03:45.000000 jiggybase-0.0.17/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.813788 jiggybase-0.0.17/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)      533 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      744 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-04-29 04:16:05.000000 jiggybase-0.0.17/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      669 2023-04-29 04:14:16.000000 jiggybase-0.0.17/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-29 04:16:05.819006 jiggybase-0.0.17/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-29 04:16:05.818062 jiggybase-0.0.17/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.17/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.806875 jiggybase-0.0.18/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.18/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)      533 2023-04-30 01:07:28.806461 jiggybase-0.0.18/PKG-INFO
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.800026 jiggybase-0.0.18/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.18/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1769 2023-04-28 15:29:35.000000 jiggybase-0.0.18/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.18/jiggybase/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 jiggybase-0.0.18/jiggybase/config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.18/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.18/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.805604 jiggybase-0.0.18/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.18/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.18/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.18/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.18/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.18/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.18/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.18/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.18/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.18/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.18/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.18/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.18/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.18/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.18/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.18/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.801386 jiggybase-0.0.18/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)      533 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      744 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-04-30 01:07:28.000000 jiggybase-0.0.18/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      669 2023-04-30 01:06:52.000000 jiggybase-0.0.18/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-30 01:07:28.806991 jiggybase-0.0.18/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-30 01:07:28.805947 jiggybase-0.0.18/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.18/test/test.py
```

### Comparing `jiggybase-0.0.17/LICENSE` & `jiggybase-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/PKG-INFO` & `jiggybase-0.0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.17
+Version: 0.0.18
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.17/jiggybase/client.py` & `jiggybase-0.0.18/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/collection.py` & `jiggybase-0.0.18/jiggybase/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,21 @@
             queries = [Query(query=queries, top_k=top_k)]
         elif isinstance(queries, Query):
             queries = [Query(query=q, top_k=top_k) for q in queries]
         qr = QueryRequest(queries=queries)
         rsp = self.plugin_session.post("/query", model=qr)
         return  QueryResponse.parse_obj(rsp.json())
 
+    def get_doc(self, id: str) -> list[DocumentChunk]:
+        """
+        Get a document by id
+        """
+        rsp = self.plugin_session.get(f"/docs/{id}")
+        return [DocumentChunk.parse_obj(c) for c in rsp.json()]
+    
     def get_chunks(self, 
                    start: int = 0, 
                    limit: int = 10, 
                    reverse: bool = True) -> List[DocumentChunk]:
         """
         low level interface for iterating through the chunks in a collection
         start - Offset of the first result to return
```

### Comparing `jiggybase-0.0.17/jiggybase/config.py` & `jiggybase-0.0.18/jiggybase/config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/jiggybase_session.py` & `jiggybase-0.0.18/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/login.py` & `jiggybase-0.0.18/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/auth.py` & `jiggybase-0.0.18/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/chat.py` & `jiggybase-0.0.18/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/chunk.py` & `jiggybase-0.0.18/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/collection.py` & `jiggybase-0.0.18/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/metadata.py` & `jiggybase-0.0.18/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/org.py` & `jiggybase-0.0.18/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/plugin.py` & `jiggybase-0.0.18/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/plugin_config.py` & `jiggybase-0.0.18/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/prompt.py` & `jiggybase-0.0.18/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/providers.py` & `jiggybase-0.0.18/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/models/user.py` & `jiggybase-0.0.18/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/jiggybase/org.py` & `jiggybase-0.0.18/jiggybase/org.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,20 @@
                           description: Optional[str] = None) -> Collection:
         rsp = self.session.post(f"/orgs/{self.id}/collections", model=CollectionPostRequest(**locals()))
         return Collection(self.session, **rsp.json())
 
     def collections(self) -> list[Collection]:
         rsp = self.session.get(f"/orgs/{self.id}/collections")
         return [Collection(self.session, **c) for c in rsp.json()]
+
+    def collection(self, name: str) -> Collection:
+        collections = [c for c in self.collections() if c.name == name or c.display_name.lower() == name.lower()]
+        if not collections:
+            raise ValueError(f"Collection {name} not found")
+        return collections[0]
     
     def members(self) -> List[OrgMember]:
         return [OrgMember(**tm) for tm in self.session.get(f'/orgs/{self.id}/members').json()]
     
     def add_member(self, email : EmailStr, role : OrgRole) -> OrgMember:
         """
         Invite the specified email to this org with the corresponding OrgRole.
```

### Comparing `jiggybase-0.0.17/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.18/jiggybase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.17
+Version: 0.0.18
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.17/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.18/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.17/pyproject.toml` & `jiggybase-0.0.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.17"
+version = "0.0.18"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pedantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.17/test/test.py` & `jiggybase-0.0.18/test/test.py`

 * *Files identical despite different names*

