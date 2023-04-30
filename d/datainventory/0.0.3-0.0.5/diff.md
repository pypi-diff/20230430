# Comparing `tmp/datainventory-0.0.3.tar.gz` & `tmp/datainventory-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datainventory-0.0.3.tar", last modified: Sun Oct  3 04:57:51 2021, max compression
+gzip compressed data, was "datainventory-0.0.5.tar", last modified: Sun Apr 30 06:09:42 2023, max compression
```

## Comparing `datainventory-0.0.3.tar` & `datainventory-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2021-10-03 04:57:51.000000 datainventory-0.0.3/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2093 2021-10-03 04:57:51.000000 datainventory-0.0.3/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1211 2021-09-20 00:18:53.000000 datainventory-0.0.3/README.rst
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2021-10-03 04:57:51.000000 datainventory-0.0.3/datainventory/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2021-08-29 05:10:07.000000 datainventory-0.0.3/datainventory/__init__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      485 2021-09-20 00:18:53.000000 datainventory-0.0.3/datainventory/_internal_store.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      992 2021-09-20 00:18:53.000000 datainventory-0.0.3/datainventory/common.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     3218 2021-09-20 00:18:53.000000 datainventory-0.0.3/datainventory/inventory.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     3598 2021-09-20 00:18:53.000000 datainventory-0.0.3/datainventory/media_store.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1000 2021-09-20 00:18:53.000000 datainventory-0.0.3/datainventory/model_store.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2470 2021-09-20 00:18:53.000000 datainventory-0.0.3/datainventory/table_store.py
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2021-10-03 04:57:51.000000 datainventory-0.0.3/datainventory.egg-info/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2093 2021-10-03 04:57:51.000000 datainventory-0.0.3/datainventory.egg-info/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      400 2021-10-03 04:57:51.000000 datainventory-0.0.3/datainventory.egg-info/SOURCES.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2021-10-03 04:57:51.000000 datainventory-0.0.3/datainventory.egg-info/dependency_links.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       18 2021-10-03 04:57:51.000000 datainventory-0.0.3/datainventory.egg-info/requires.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       14 2021-10-03 04:57:51.000000 datainventory-0.0.3/datainventory.egg-info/top_level.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2021-10-03 04:57:51.000000 datainventory-0.0.3/setup.cfg
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1024 2021-10-03 04:56:54.000000 datainventory-0.0.3/setup.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:09:42.301315 datainventory-0.0.5/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1070 2023-01-03 00:32:35.000000 datainventory-0.0.5/LICENSE
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1619 2023-04-30 06:09:42.301315 datainventory-0.0.5/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1211 2023-01-03 00:32:35.000000 datainventory-0.0.5/README.rst
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:09:42.291315 datainventory-0.0.5/datainventory/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-01-03 00:32:35.000000 datainventory-0.0.5/datainventory/__init__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      485 2023-01-03 00:32:35.000000 datainventory-0.0.5/datainventory/_internal_store.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:09:42.301315 datainventory-0.0.5/datainventory/bin/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-02-11 03:11:09.000000 datainventory-0.0.5/datainventory/bin/__init__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1337 2023-02-11 03:11:09.000000 datainventory-0.0.5/datainventory/bin/app.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      992 2023-01-03 00:32:35.000000 datainventory-0.0.5/datainventory/common.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     3486 2023-02-11 03:11:09.000000 datainventory-0.0.5/datainventory/inventory.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     3614 2023-02-11 03:11:09.000000 datainventory-0.0.5/datainventory/media_store.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1000 2023-01-03 00:32:35.000000 datainventory-0.0.5/datainventory/model_store.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2638 2023-02-11 03:11:09.000000 datainventory-0.0.5/datainventory/table_store.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:09:42.301315 datainventory-0.0.5/datainventory.egg-info/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1619 2023-04-30 06:09:42.000000 datainventory-0.0.5/datainventory.egg-info/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      585 2023-04-30 06:09:42.000000 datainventory-0.0.5/datainventory.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2023-04-30 06:09:42.000000 datainventory-0.0.5/datainventory.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       61 2023-04-30 06:09:42.000000 datainventory-0.0.5/datainventory.egg-info/entry_points.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       24 2023-04-30 06:09:42.000000 datainventory-0.0.5/datainventory.egg-info/requires.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       27 2023-04-30 06:09:42.000000 datainventory-0.0.5/datainventory.egg-info/top_level.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      650 2023-04-30 06:09:15.000000 datainventory-0.0.5/pyproject.toml
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2023-04-30 06:09:42.301315 datainventory-0.0.5/setup.cfg
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:09:42.301315 datainventory-0.0.5/tests/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      716 2023-01-03 00:32:35.000000 datainventory-0.0.5/tests/test_inventory.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1781 2023-01-03 00:32:35.000000 datainventory-0.0.5/tests/test_media_store.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1165 2023-02-11 03:11:09.000000 datainventory-0.0.5/tests/test_table_store.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datainventory-0.0.3/PKG-INFO` & `datainventory-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 Metadata-Version: 2.1
 Name: datainventory
-Version: 0.0.3
+Version: 0.0.5
 Summary: Data Inventory
-Home-page: https://github.com/iot-spectator/datainventory
 Author: IoT Spectator
-License: MIT
-Description: Data Inventory
-        ==============
-        
-        .. image:: https://github.com/iot-spectator/datainventory/actions/workflows/testing.yml/badge.svg
-            :target: https://github.com/iot-spectator/datainventory/actions/workflows/testing.yml
-        
-        .. image:: https://github.com/iot-spectator/datainventory/actions/workflows/linting.yml/badge.svg
-            :target: https://github.com/iot-spectator/datainventory/actions/workflows/linting.yml
-            
-        .. image:: https://codecov.io/gh/iot-spectator/datainventory/branch/main/graph/badge.svg?token=3XR09X8NYZ
-            :target: https://codecov.io/gh/iot-spectator/datainventory
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/psf/black
-        
-        Data Inventory is a database designed for managing machine learning models. It is also suitable for storing images and videos.
-        
-        
-        Requirements
-        ------------
-        ``Python 3.7`` or newer is required.
-        
-        
-        Installation
-        ------------
-        There are a few ways to install ``Data Inventory``.
-        
-        - Install the latest release from PyPI
-        
-        .. code-block:: bash
-        
-            pip install datainventory
-        
-        - Install from source
-        
-        .. code-block:: bash
-        
-            git clone https://github.com/iot-spectator/datainventory.git
-            cd datainventory
-            pip install .
-        
+License: MIT License
+Project-URL: repository, https://github.com/iot-spectator/datainventory
 Keywords: image and video database
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Data Inventory
+==============
+
+.. image:: https://github.com/iot-spectator/datainventory/actions/workflows/testing.yml/badge.svg
+    :target: https://github.com/iot-spectator/datainventory/actions/workflows/testing.yml
+
+.. image:: https://github.com/iot-spectator/datainventory/actions/workflows/linting.yml/badge.svg
+    :target: https://github.com/iot-spectator/datainventory/actions/workflows/linting.yml
+    
+.. image:: https://codecov.io/gh/iot-spectator/datainventory/branch/main/graph/badge.svg?token=3XR09X8NYZ
+    :target: https://codecov.io/gh/iot-spectator/datainventory
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+Data Inventory is a database designed for managing machine learning models. It is also suitable for storing images and videos.
+
+
+Requirements
+------------
+``Python 3.7`` or newer is required.
+
+
+Installation
+------------
+There are a few ways to install ``Data Inventory``.
+
+- Install the latest release from PyPI
+
+.. code-block:: bash
+
+    pip install datainventory
+
+- Install from source
+
+.. code-block:: bash
+
+    git clone https://github.com/iot-spectator/datainventory.git
+    cd datainventory
+    pip install .
```

### Comparing `datainventory-0.0.3/README.rst` & `datainventory-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `datainventory-0.0.3/datainventory/common.py` & `datainventory-0.0.5/datainventory/common.py`

 * *Files identical despite different names*

### Comparing `datainventory-0.0.3/datainventory/inventory.py` & `datainventory-0.0.5/datainventory/inventory.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         self._data_inventory = self._inventory / pathlib.Path("data")
         self._database_name = f"{self._inventory.name}.db"
         self._database = self._inventory / self._database_name
 
         if not self._inventory.exists():
             self._inventory.mkdir()
         self._engine = sqlalchemy.create_engine(f"sqlite:///{self._database}")
-        self._metadata = sqlalchemy.MetaData(bind=self._engine)
+        self._metadata = sqlalchemy.MetaData()
+        self._metadata.create_all(bind=self._engine)
 
     def get_media_store(self) -> media_store.MediaStore:
         """Return an instance of the media store."""
         Session = sessionmaker(bind=self._engine)
         return media_store.MediaStore(
             create_key=_internal_store.CREATE_KEY,
             device_id=self._device_id,
@@ -56,14 +57,15 @@
         """Return an instance of the table store."""
         Session = sessionmaker(bind=self._engine)
         return table_store.TableStore(
             create_key=_internal_store.CREATE_KEY,
             device_id=self._device_id,
             metadata=self._metadata,
             session=Session(),
+            connection=self._engine.connect(),
         )
 
     def export(self, dest_filename: pathlib.Path) -> pathlib.Path:
         """Export the entire data inventory."""
         self._metadata.reflect(self._engine)
         session = sessionmaker(bind=self._engine)()
         tables = list()
@@ -83,7 +85,11 @@
                 table_csv_file.unlink()
         return pathlib.Path(archive_path)
 
     def destroy(self) -> None:
         """Destory the entire data inventory."""
         if self._inventory:
             shutil.rmtree(self._inventory)
+
+    def import_data(self, source_data: pathlib.Path) -> None:
+        """Import data into the data inventory."""
+        raise NotImplementedError("This function is not implemented.")
```

### Comparing `datainventory-0.0.3/datainventory/media_store.py` & `datainventory-0.0.5/datainventory/media_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,8 +103,8 @@
     ) -> List:
         """Retrieve the media data."""
         if query_statement:
             result = self._session.execute(query_statement)
         else:
             query_statement = sqlalchemy.select(Media)
             result = self._session.execute(query_statement)
-        return result.all()
+        return result.all()  # type: ignore
```

### Comparing `datainventory-0.0.3/datainventory/model_store.py` & `datainventory-0.0.5/datainventory/model_store.py`

 * *Files identical despite different names*

### Comparing `datainventory-0.0.3/datainventory/table_store.py` & `datainventory-0.0.5/datainventory/table_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,20 +20,23 @@
 
     def __init__(
         self,
         create_key,
         device_id: str,
         metadata: sqlalchemy.MetaData,
         session: Session,
+        connection: sqlalchemy.engine.Connection,
     ) -> None:
         _internal_store.InternalStore.__init__(
             self, create_key=create_key, device_id=device_id
         )
         self._session = session
         self._metadata = metadata
+        self._connection = connection
+        self._metadata.create_all(bind=self._connection)
 
     def create_table(
         self, table_name: str, columns: Dict[str, common.ColumnType]
     ) -> None:
         """Create a table."""
         columns["device_id"] = common.ColumnType.String
         columns["timestamp"] = common.ColumnType.DateTime
@@ -42,15 +45,15 @@
             table_name,
             self._metadata,
             *(
                 sqlalchemy.Column(column_name, column_type.value)
                 for column_name, column_type in columns.items()
             ),
         )
-        table.create(checkfirst=True)
+        table.create(bind=self._connection, checkfirst=True)
 
     def insert(self, table_name: str, values: List[Dict]) -> None:
         """Insert data."""
         for item in values:
             item["device_id"] = self._device_id
             item["timestamp"] = datetime.datetime.utcnow()
```

### Comparing `datainventory-0.0.3/datainventory.egg-info/PKG-INFO` & `datainventory-0.0.5/datainventory.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 Metadata-Version: 2.1
 Name: datainventory
-Version: 0.0.3
+Version: 0.0.5
 Summary: Data Inventory
-Home-page: https://github.com/iot-spectator/datainventory
 Author: IoT Spectator
-License: MIT
-Description: Data Inventory
-        ==============
-        
-        .. image:: https://github.com/iot-spectator/datainventory/actions/workflows/testing.yml/badge.svg
-            :target: https://github.com/iot-spectator/datainventory/actions/workflows/testing.yml
-        
-        .. image:: https://github.com/iot-spectator/datainventory/actions/workflows/linting.yml/badge.svg
-            :target: https://github.com/iot-spectator/datainventory/actions/workflows/linting.yml
-            
-        .. image:: https://codecov.io/gh/iot-spectator/datainventory/branch/main/graph/badge.svg?token=3XR09X8NYZ
-            :target: https://codecov.io/gh/iot-spectator/datainventory
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/psf/black
-        
-        Data Inventory is a database designed for managing machine learning models. It is also suitable for storing images and videos.
-        
-        
-        Requirements
-        ------------
-        ``Python 3.7`` or newer is required.
-        
-        
-        Installation
-        ------------
-        There are a few ways to install ``Data Inventory``.
-        
-        - Install the latest release from PyPI
-        
-        .. code-block:: bash
-        
-            pip install datainventory
-        
-        - Install from source
-        
-        .. code-block:: bash
-        
-            git clone https://github.com/iot-spectator/datainventory.git
-            cd datainventory
-            pip install .
-        
+License: MIT License
+Project-URL: repository, https://github.com/iot-spectator/datainventory
 Keywords: image and video database
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Data Inventory
+==============
+
+.. image:: https://github.com/iot-spectator/datainventory/actions/workflows/testing.yml/badge.svg
+    :target: https://github.com/iot-spectator/datainventory/actions/workflows/testing.yml
+
+.. image:: https://github.com/iot-spectator/datainventory/actions/workflows/linting.yml/badge.svg
+    :target: https://github.com/iot-spectator/datainventory/actions/workflows/linting.yml
+    
+.. image:: https://codecov.io/gh/iot-spectator/datainventory/branch/main/graph/badge.svg?token=3XR09X8NYZ
+    :target: https://codecov.io/gh/iot-spectator/datainventory
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+Data Inventory is a database designed for managing machine learning models. It is also suitable for storing images and videos.
+
+
+Requirements
+------------
+``Python 3.7`` or newer is required.
+
+
+Installation
+------------
+There are a few ways to install ``Data Inventory``.
+
+- Install the latest release from PyPI
+
+.. code-block:: bash
+
+    pip install datainventory
+
+- Install from source
+
+.. code-block:: bash
+
+    git clone https://github.com/iot-spectator/datainventory.git
+    cd datainventory
+    pip install .
```

