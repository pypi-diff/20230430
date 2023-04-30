# Comparing `tmp/BlockFrame-0.1.3.tar.gz` & `tmp/BlockFrame-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlockFrame-0.1.3.tar", last modified: Fri Apr 28 14:42:10 2023, max compression
+gzip compressed data, was "BlockFrame-0.1.4.tar", last modified: Sun Apr 30 06:50:31 2023, max compression
```

## Comparing `BlockFrame-0.1.3.tar` & `BlockFrame-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.607876 BlockFrame-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.582413 BlockFrame-0.1.3/BlockFrame/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.3/BlockFrame/__init__.py
--rw-rw-rw-   0        0        0     3747 2023-04-05 06:33:24.000000 BlockFrame-0.1.3/BlockFrame/block_frame.py
-drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.599360 BlockFrame-0.1.3/BlockFrame/chunking_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.3/BlockFrame/chunking_service/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-28 14:30:52.000000 BlockFrame-0.1.3/BlockFrame/chunking_service/chunking.py
--rw-rw-rw-   0        0        0      691 2023-04-28 14:22:04.000000 BlockFrame-0.1.3/BlockFrame/chunking_service/config.py
-drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.605875 BlockFrame-0.1.3/BlockFrame/database_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-0.1.3/BlockFrame/database_service/__init__.py
--rw-rw-rw-   0        0        0      744 2023-04-28 14:05:46.000000 BlockFrame-0.1.3/BlockFrame/database_service/database.py
--rw-rw-rw-   0        0        0     1599 2023-04-28 14:02:33.000000 BlockFrame-0.1.3/BlockFrame/database_service/defaultmodel.py
--rw-rw-rw-   0        0        0      377 2023-04-28 14:26:18.000000 BlockFrame-0.1.3/BlockFrame/database_service/getters.py
--rw-rw-rw-   0        0        0     1372 2023-04-28 14:25:42.000000 BlockFrame-0.1.3/BlockFrame/database_service/initalisation.py
--rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-0.1.3/BlockFrame/database_service/setters.py
-drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.596369 BlockFrame-0.1.3/BlockFrame.egg-info/
--rw-rw-rw-   0        0        0      218 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      218 2023-04-28 14:42:10.607876 BlockFrame-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 14:42:10.607876 BlockFrame-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-04-28 14:42:06.000000 BlockFrame-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.534530 BlockFrame-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.484920 BlockFrame-0.1.4/BlockFrame/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.4/BlockFrame/__init__.py
+-rw-rw-rw-   0        0        0     4424 2023-04-30 06:46:47.000000 BlockFrame-0.1.4/BlockFrame/block_frame.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.526537 BlockFrame-0.1.4/BlockFrame/chunking_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.4/BlockFrame/chunking_service/__init__.py
+-rw-rw-rw-   0        0        0     7285 2023-04-30 06:46:40.000000 BlockFrame-0.1.4/BlockFrame/chunking_service/chunking.py
+-rw-rw-rw-   0        0        0      691 2023-04-28 14:22:04.000000 BlockFrame-0.1.4/BlockFrame/chunking_service/config.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.532538 BlockFrame-0.1.4/BlockFrame/database_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-0.1.4/BlockFrame/database_service/__init__.py
+-rw-rw-rw-   0        0        0      744 2023-04-28 14:05:46.000000 BlockFrame-0.1.4/BlockFrame/database_service/database.py
+-rw-rw-rw-   0        0        0     1599 2023-04-30 05:33:57.000000 BlockFrame-0.1.4/BlockFrame/database_service/defaultmodel.py
+-rw-rw-rw-   0        0        0      377 2023-04-28 14:26:18.000000 BlockFrame-0.1.4/BlockFrame/database_service/getters.py
+-rw-rw-rw-   0        0        0     1345 2023-04-30 04:36:05.000000 BlockFrame-0.1.4/BlockFrame/database_service/initalisation.py
+-rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-0.1.4/BlockFrame/database_service/setters.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.493175 BlockFrame-0.1.4/BlockFrame.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      268 2023-04-30 06:50:31.534530 BlockFrame-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-30 06:50:31.534530 BlockFrame-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      458 2023-04-30 06:50:26.000000 BlockFrame-0.1.4/setup.py
```

### Comparing `BlockFrame-0.1.3/BlockFrame/block_frame.py` & `BlockFrame-0.1.4/BlockFrame/block_frame.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,40 @@
 import hashlib
 import os
-from BlockFrame.chunking_service.config import Config
+import pathlib
+from typing import Literal, Union
+
 from BlockFrame.chunking_service.chunking import ChunkHandler
+from BlockFrame.chunking_service.config import Config
 from BlockFrame.database_service.database import BlockFrameDatabase
 
 
 class BlockFrame:
-    def __init__(self, config: str):
+    def __init__(
+        self,
+        config: str,
+        option: Union[Literal["generic"], Literal["time"], Literal["secure"]],
+    ):
         self.config = Config(config)
+
         self.database = BlockFrameDatabase(db_config=self.config)
-        self.chunker = ChunkHandler(db=self.database.get_db(), config=self.config.config_id)
+        self.chunker = ChunkHandler(
+            db=self.database.get_db(), config=self.config.config_id, option=option
+        )
+
+    def __dir(self):
+        try:
+            return (
+                pathlib.Path(self.config.get("file-storage-path"))
+                if pathlib.Path(self.config.get("file-storage-path"))
+                is pathlib.Path(self.config.get("file-storage-path")).exists
+                else pathlib.Path(self.config.get("file-storage-path")).mkdir()
+            )
+        except FileExistsError:
+            return pathlib.Path(self.config.get("file-storage-path"))
 
 
 class Reconstruct:
     def __init__(self, ccif_file) -> None:
         self.ccif_file = ccif_file
         self.file_name = ""
         self.size = 0
```

### Comparing `BlockFrame-0.1.3/BlockFrame/chunking_service/config.py` & `BlockFrame-0.1.4/BlockFrame/chunking_service/config.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.3/BlockFrame/database_service/database.py` & `BlockFrame-0.1.4/BlockFrame/database_service/database.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.3/BlockFrame/database_service/defaultmodel.py` & `BlockFrame-0.1.4/BlockFrame/database_service/defaultmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, Integer, String, ForeignKey
+from sqlalchemy import Column, ForeignKey, Integer, String
 from sqlalchemy.orm import Relationship
 
 from BlockFrame.database_service.initalisation import DatabaseInterface
 
 
 class DefaultChunkModel(DatabaseInterface().Base):
     __tablename__ = "ChunkModel-default"
```

### Comparing `BlockFrame-0.1.3/BlockFrame/database_service/initalisation.py` & `BlockFrame-0.1.4/BlockFrame/database_service/initalisation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from sqlalchemy.engine import create_engine
-from sqlalchemy.orm import declarative_base
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.orm import declarative_base, sessionmaker
 
 
 class DatabaseInterface:
     Base = declarative_base()
     db_engine = create_engine("sqlite:///block_frame.db")
     sync_session = sessionmaker(autocommit=False, autoflush=False, bind=db_engine)
```

### Comparing `BlockFrame-0.1.3/BlockFrame.egg-info/SOURCES.txt` & `BlockFrame-0.1.4/BlockFrame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

