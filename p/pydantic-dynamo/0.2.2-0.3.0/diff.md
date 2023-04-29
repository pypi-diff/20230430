# Comparing `tmp/pydantic_dynamo-0.2.2.tar.gz` & `tmp/pydantic_dynamo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_dynamo-0.2.2.tar", max compression
+gzip compressed data, was "pydantic_dynamo-0.3.0.tar", max compression
```

## Comparing `pydantic_dynamo-0.2.2.tar` & `pydantic_dynamo-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.2.2/pydantic_dynamo/__init__.py
--rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.2.2/pydantic_dynamo/constants.py
--rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.2.2/pydantic_dynamo/exceptions.py
--rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.2/pydantic_dynamo/models.py
--rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.2.2/pydantic_dynamo/repository.py
--rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.2.2/pydantic_dynamo/utils.py
--rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.2.2/pydantic_dynamo/v2/__init__.py
--rw-r--r--   0        0        0     4403 2023-04-29 12:58:54.202235 pydantic_dynamo-0.2.2/pydantic_dynamo/v2/models.py
--rw-r--r--   0        0        0    17272 2023-04-29 12:59:41.536221 pydantic_dynamo-0.2.2/pydantic_dynamo/v2/repository.py
--rw-r--r--   0        0        0     3805 2023-04-29 13:00:04.168642 pydantic_dynamo-0.2.2/pydantic_dynamo/v2/sync_repository.py
--rw-r--r--   0        0        0     1260 2023-04-29 12:57:04.660325 pydantic_dynamo-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    16867 2023-04-29 12:57:04.658325 pydantic_dynamo-0.2.2/README.md
--rw-r--r--   0        0        0    17035 1970-01-01 00:00:00.000000 pydantic_dynamo-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-03-07 03:45:50.202681 pydantic_dynamo-0.3.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-07 03:36:36.814175 pydantic_dynamo-0.3.0/pydantic_dynamo/__init__.py
+-rw-r--r--   0        0        0      243 2023-04-04 19:40:26.272160 pydantic_dynamo-0.3.0/pydantic_dynamo/constants.py
+-rw-r--r--   0        0        0       53 2023-03-07 03:09:09.986643 pydantic_dynamo-0.3.0/pydantic_dynamo/exceptions.py
+-rw-r--r--   0        0        0     3294 2023-04-19 02:51:16.873917 pydantic_dynamo-0.3.0/pydantic_dynamo/models.py
+-rw-r--r--   0        0        0    14586 2023-04-13 17:24:33.661892 pydantic_dynamo-0.3.0/pydantic_dynamo/repository.py
+-rw-r--r--   0        0        0    10579 2023-04-19 02:51:16.873917 pydantic_dynamo-0.3.0/pydantic_dynamo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:23:43.683503 pydantic_dynamo-0.3.0/pydantic_dynamo/v2/__init__.py
+-rw-r--r--   0        0        0     4403 2023-04-29 12:58:54.202235 pydantic_dynamo-0.3.0/pydantic_dynamo/v2/models.py
+-rw-r--r--   0        0        0    17272 2023-04-29 20:42:00.023856 pydantic_dynamo-0.3.0/pydantic_dynamo/v2/repository.py
+-rw-r--r--   0        0        0     3805 2023-04-29 13:00:04.168642 pydantic_dynamo-0.3.0/pydantic_dynamo/v2/sync_repository.py
+-rw-r--r--   0        0        0     2372 2023-04-29 22:36:31.894682 pydantic_dynamo-0.3.0/pydantic_dynamo/v2/write_once.py
+-rw-r--r--   0        0        0     1260 2023-04-29 22:53:52.876922 pydantic_dynamo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    18573 2023-04-29 23:01:49.944457 pydantic_dynamo-0.3.0/README.md
+-rw-r--r--   0        0        0    18706 1970-01-01 00:00:00.000000 pydantic_dynamo-0.3.0/PKG-INFO
```

### Comparing `pydantic_dynamo-0.2.2/LICENSE` & `pydantic_dynamo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.2/pydantic_dynamo/models.py` & `pydantic_dynamo-0.3.0/pydantic_dynamo/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.2/pydantic_dynamo/repository.py` & `pydantic_dynamo-0.3.0/pydantic_dynamo/repository.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.2/pydantic_dynamo/utils.py` & `pydantic_dynamo-0.3.0/pydantic_dynamo/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.2/pydantic_dynamo/v2/models.py` & `pydantic_dynamo-0.3.0/pydantic_dynamo/v2/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.2/pydantic_dynamo/v2/repository.py` & `pydantic_dynamo-0.3.0/pydantic_dynamo/v2/repository.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.2/pydantic_dynamo/v2/sync_repository.py` & `pydantic_dynamo-0.3.0/pydantic_dynamo/v2/sync_repository.py`

 * *Files identical despite different names*

### Comparing `pydantic_dynamo-0.2.2/pyproject.toml` & `pydantic_dynamo-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-dynamo"
-version = "0.2.2"
+version = "0.3.0"
 description = ""
 authors = ["David Jetter <davidajetter@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pydantic_dynamo"}]
 homepage = "https://github.com/david-a-jetter/pydantic-dynamo"
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_dynamo-0.2.2/README.md` & `pydantic_dynamo-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -452,7 +452,42 @@
         sort_ascending=True,
         limit=None,
         filters=None
     )
     for content in response.contents
 ]
 ```
+
+### Write Once Repository
+This utility grew out of a need to minimize duplicate data being saved to the database, because new
+was going to be broadcast to data warehouse for wider analysis. 
+This wrapper around the v2 `DynamoRepository` will return a `List[PartitionedContent[ObjT]]` 
+for all records actually written to the database. The database will be queried, and each item
+will be compared to an existing record, if one exists, using Python equivalency.
+
+Assuming the underlying repository is using strongly consistent reads, this should minimize the
+number of duplicate writes, although there is no statistical evaluation to prove its efficacy.
+
+**A note on costs:**
+
+Cost optimization is not the goal of this feature, but rather achieving a reasonable likelihood of
+saving any given record only once.
+This actually queries the database to compare input data to the existing data. This may cost more
+than just blindly putting the content. However, since write units cost significantly more than read units
+(maybe 4x? the pricing is confusing), if you have a high likelihood of duplicate data being saved, this
+*may* actually be able to save you some money. As with all things MIT licensed... no guarantees :)
+
+```python
+from pydantic_dynamo.v2.write_once import WriteOnceRepository
+
+write_once = WriteOnceRepository[Example](async_repo=repo)
+
+count = 10000
+data = [PartitionedContent(...) for _ in range(count)]
+
+actually_written: List[PartitionedContent[ObjT]] = await write_once.write(data)
+assert len(actually_written) == count
+
+actually_written_again: List[PartitionedContent[ObjT]] = await write_once.write(data)
+assert len(actually_written_again) == 0
+
+```
```

### Comparing `pydantic_dynamo-0.2.2/PKG-INFO` & `pydantic_dynamo-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-dynamo
-Version: 0.2.2
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/david-a-jetter/pydantic-dynamo
 Author: David Jetter
 Author-email: davidajetter@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -471,7 +471,42 @@
         limit=None,
         filters=None
     )
     for content in response.contents
 ]
 ```
 
+### Write Once Repository
+This utility grew out of a need to minimize duplicate data being saved to the database, because new
+was going to be broadcast to data warehouse for wider analysis. 
+This wrapper around the v2 `DynamoRepository` will return a `List[PartitionedContent[ObjT]]` 
+for all records actually written to the database. The database will be queried, and each item
+will be compared to an existing record, if one exists, using Python equivalency.
+
+Assuming the underlying repository is using strongly consistent reads, this should minimize the
+number of duplicate writes, although there is no statistical evaluation to prove its efficacy.
+
+**A note on costs:**
+
+Cost optimization is not the goal of this feature, but rather achieving a reasonable likelihood of
+saving any given record only once.
+This actually queries the database to compare input data to the existing data. This may cost more
+than just blindly putting the content. However, since write units cost significantly more than read units
+(maybe 4x? the pricing is confusing), if you have a high likelihood of duplicate data being saved, this
+*may* actually be able to save you some money. As with all things MIT licensed... no guarantees :)
+
+```python
+from pydantic_dynamo.v2.write_once import WriteOnceRepository
+
+write_once = WriteOnceRepository[Example](async_repo=repo)
+
+count = 10000
+data = [PartitionedContent(...) for _ in range(count)]
+
+actually_written: List[PartitionedContent[ObjT]] = await write_once.write(data)
+assert len(actually_written) == count
+
+actually_written_again: List[PartitionedContent[ObjT]] = await write_once.write(data)
+assert len(actually_written_again) == 0
+
+```
+
```

