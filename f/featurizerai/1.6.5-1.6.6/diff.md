# Comparing `tmp/featurizerai-1.6.5.tar.gz` & `tmp/featurizerai-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.6.5.tar", last modified: Sat Apr 29 16:05:19 2023, max compression
+gzip compressed data, was "featurizerai-1.6.6.tar", last modified: Sun Apr 30 01:34:33 2023, max compression
```

## Comparing `featurizerai-1.6.5.tar` & `featurizerai-1.6.6.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.911069 featurizerai-1.6.5/
--rw-rw-rw-   0        0        0     1100 2023-04-29 00:34:12.000000 featurizerai-1.6.5/LICENSE
--rw-rw-rw-   0        0        0       89 2023-04-29 00:34:12.000000 featurizerai-1.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0      879 2023-04-29 16:05:19.911069 featurizerai-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-29 00:34:12.000000 featurizerai-1.6.5/pyproject.toml
--rw-rw-rw-   0        0        0      123 2023-04-29 16:05:19.911069 featurizerai-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1378 2023-04-29 16:03:47.000000 featurizerai-1.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.864246 featurizerai-1.6.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.879801 featurizerai-1.6.5/src/features/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/__init__.py
--rw-rw-rw-   0        0        0      704 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/authenticate.py
--rw-rw-rw-   0        0        0     4329 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/create_stream.py
--rw-rw-rw-   0        0        0      870 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/custom_schema.py
--rw-rw-rw-   0        0        0     4865 2023-04-29 16:03:39.000000 featurizerai-1.6.5/src/features/materialize.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.895520 featurizerai-1.6.5/src/features/tests/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/tests/__init__.py
--rw-rw-rw-   0        0        0     2817 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/tests/test_materialize.py
--rw-rw-rw-   0        0        0     1563 2023-04-29 00:34:12.000000 featurizerai-1.6.5/src/features/tests/test_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-29 16:05:19.911069 featurizerai-1.6.5/src/featurizerai.egg-info/
--rw-rw-rw-   0        0        0      879 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 16:05:19.000000 featurizerai-1.6.5/src/featurizerai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 01:34:33.027009 featurizerai-1.6.6/
+-rw-rw-rw-   0        0        0     1100 2023-04-29 00:34:12.000000 featurizerai-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0       89 2023-04-29 00:34:12.000000 featurizerai-1.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      879 2023-04-30 01:34:33.027009 featurizerai-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-29 00:34:12.000000 featurizerai-1.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0      123 2023-04-30 01:34:33.035597 featurizerai-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1378 2023-04-30 01:33:44.000000 featurizerai-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:34:32.972860 featurizerai-1.6.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 01:34:33.011252 featurizerai-1.6.6/src/features/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:34:12.000000 featurizerai-1.6.6/src/features/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-04-29 00:34:12.000000 featurizerai-1.6.6/src/features/authenticate.py
+-rw-rw-rw-   0        0        0     4329 2023-04-29 00:34:12.000000 featurizerai-1.6.6/src/features/create_stream.py
+-rw-rw-rw-   0        0        0      979 2023-04-30 01:32:51.000000 featurizerai-1.6.6/src/features/custom_schema.py
+-rw-rw-rw-   0        0        0     4984 2023-04-30 01:32:51.000000 featurizerai-1.6.6/src/features/materialize.py
+-rw-rw-rw-   0        0        0     6710 2023-04-30 01:32:51.000000 featurizerai-1.6.6/src/features/test.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:34:33.027009 featurizerai-1.6.6/src/featurizerai.egg-info/
+-rw-rw-rw-   0        0        0      879 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 01:34:32.000000 featurizerai-1.6.6/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.6.5/LICENSE` & `featurizerai-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.5/PKG-INFO` & `featurizerai-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.6.5
+Version: 1.6.6
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.6.5/setup.py` & `featurizerai-1.6.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.6.5',
+    version='1.6.6',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.6.5/src/features/authenticate.py` & `featurizerai-1.6.6/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.5/src/features/create_stream.py` & `featurizerai-1.6.6/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.6.5/src/features/custom_schema.py` & `featurizerai-1.6.6/src/features/custom_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,16 @@
             "string": StringType
         }
 
         for field in schema_fields:
             field_name = field.get("name")
             field_type = field.get("type")
             field_nullable = field.get("nullable", True)
+            field_aggregation = field.get("aggregation", None)
 
             if field_name and field_type in type_mapping:
                 struct_field = StructField(
-                    field_name, type_mapping[field_type](), field_nullable
+                    field_name, type_mapping[field_type](), field_nullable, metadata={"aggregation": field_aggregation}
                 )
                 struct_fields.append(struct_field)
 
         return StructType(struct_fields)
```

### Comparing `featurizerai-1.6.5/src/features/materialize.py` & `featurizerai-1.6.6/src/features/materialize.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import json
-import logging
-from datetime import datetime, timedelta
-import jwt
-from pymongo import MongoClient
-from pyspark.sql import SparkSession
-from pyspark.sql.functions import col, count
-from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
-from pyspark.sql import functions as F
-import certifi
-from pymongo.server_api import ServerApi
-from pyspark.sql.functions import col
-
-
-class materialize:
-    def __init__(self, mongo_connection, aggregation_date, groupby_attr, groupby_value, token, schema, sparksql, partition_column=None):
-        self.mongo_connection = mongo_connection
-        self.aggregation_date = datetime.strptime(aggregation_date, "%Y-%m-%d %H:%M:%S")
-        self.groupby = groupby_value
-        self.groupby_attr = groupby_attr
-        self.token = token
-        self.schema = schema
-        self.sparksql = sparksql
-        self.partition_column = partition_column
-
-        self.spark = SparkSession.builder \
-            .appName("Aggregation") \
-            .master("local[*]") \
-            .getOrCreate()
-        self.spark.sparkContext.setLogLevel("ERROR")
-
-    def read_data_and_aggregate(self):
-
-
-        # authenticate token
-        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
-        mongo_db = mongo_client[self.mongo_connection['database']]
-        mongo_db_featurizer = mongo_client['featurizer']
-        users_collection = mongo_db_featurizer["users"]
-        SECRET_KEY = "features"  # Change this to your desired secret key
-        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
-
-        try:
-            payload = jwt.decode(self.token, SECRET_KEY, algorithms=["HS256"])
-            user_id: str = payload.get("user_id")
-            if user_id is None:
-                print("User not found")
-                return ("Invalid token")
-            print("Authenticated user: " + user_id)
-            user = users_collection.find_one({"userid": user_id})
-            if user is None:
-                print("User not found")
-                return ("Invalid token")
-        except Exception as e:
-            print(e)
-            return ("Invalid token")
-
-        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
-        aggregated_data_collection = mongo_db[self.mongo_connection['collection']]
-
-        raw_data = raw_data_collection.find()
-        raw_data_list = [doc for doc in raw_data]
-        df = self.spark.createDataFrame(raw_data_list, self.schema)
-
-        # Apply partitioning if the partition_column is specified
-        if self.partition_column:
-            print("Partitioning the DataFrame based on the column: " + self.partition_column)
-            # raw_data_collection.create_index(self.partition_column)
-            # raw_data_collection.create_index(self.groupby_attr)
-            df = df.repartition(col(self.partition_column))
-
-        # Filter the DataFrame based on the given device_id
-        df = df.filter(col(self.groupby_attr) == self.groupby)
-        start_time = self.aggregation_date
-        df = df.filter((col(self.groupby_attr) == self.groupby) & (col("timestamp") < start_time.timestamp()))
-        df = df.withColumn("timestamp_unix", F.col("timestamp").cast("bigint"))
-        df.createOrReplaceTempView("temp_table")
-
-        # Define empty schema for DataFrame
-        schema = StructType([
-            StructField(self.groupby_attr, StringType(), True)
-        ])
-        # Create empty DataFrame
-        result_df = self.spark.createDataFrame([], schema)
-
-        # Execute the dynamic Spark SQL
-        for sql in self.sparksql:
-            sql_base = sql.replace("{"+ self.groupby_attr + "}", str(self.groupby))
-            hour = int(sql.split("_")[3])
-            sql_with_timestamp = sql_base.replace("{timestamp}", str(int((start_time - timedelta(hours=hour)).timestamp())))
-            sql_with_timestamp_base = sql_with_timestamp.replace("{timestamp_base}", str(int((start_time).timestamp())))
-            c_count = self.spark.sql(sql_with_timestamp_base)
-            result_df = result_df.join(c_count, self.groupby_attr, "full") \
-                .select(result_df.columns + [col for col in c_count.columns if col not in result_df.columns])
-
-        if result_df.isEmpty():
-            json_aggregated_data = "{'error': 'No data found'}"
-        else:
-            json_aggregated_data = result_df.toJSON().collect()[0]
-
-        if json_aggregated_data is not None:
-            aggregated_data_collection.update_one(
-                {"date": start_time, "aggregated_key": self.groupby},
-                {"$set": {"aggregated_data": json_aggregated_data}},
-                upsert=True
-            )
-        else:
-            logging.error("Serialized aggregated data is None, skipping update")
-
-        return json_aggregated_data
-
-
+import json
+import logging
+from datetime import datetime, timedelta
+import jwt
+from pymongo import MongoClient
+from pyspark.sql import SparkSession
+from pyspark.sql.functions import col, count
+from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
+from pyspark.sql import functions as F
+import certifi
+from pymongo.server_api import ServerApi
+from pyspark.sql.functions import col
+
+
+class materialize:
+    def __init__(self, mongo_connection, aggregation_date, groupby_attr, groupby_value, token, schema, sparksql, partition_column=None):
+        self.mongo_connection = mongo_connection
+        self.aggregation_date = datetime.strptime(aggregation_date, "%Y-%m-%d %H:%M:%S")
+        self.groupby = groupby_value
+        self.groupby_attr = groupby_attr
+        self.token = token
+        self.schema = schema
+        self.sparksql = sparksql
+        self.partition_column = partition_column
+
+        self.spark = SparkSession.builder \
+            .appName("IncrementalAggregation") \
+            .master("local[*]") \
+            .getOrCreate()
+        self.spark.sparkContext.setLogLevel("ERROR")
+
+    def read_data_and_aggregate(self):
+
+
+        # authenticate token
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        mongo_db_featurizer = mongo_client['featurizer']
+        users_collection = mongo_db_featurizer["users"]
+        SECRET_KEY = "features"  # Change this to your desired secret key
+        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
+
+        try:
+            payload = jwt.decode(self.token, SECRET_KEY, algorithms=["HS256"])
+            user_id: str = payload.get("user_id")
+            if user_id is None:
+                print("User not found")
+                return ("Invalid token")
+            print("Authenticated user: " + user_id)
+            user = users_collection.find_one({"userid": user_id})
+            if user is None:
+                print("User not found")
+                return ("Invalid token")
+        except Exception as e:
+            print(e)
+            return ("Invalid token")
+
+        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
+        aggregated_data_collection = mongo_db[self.mongo_connection['collection']]
+
+        raw_data = raw_data_collection.find()
+        raw_data_list = [doc for doc in raw_data]
+        df = self.spark.createDataFrame(raw_data_list, self.schema)
+
+        # Apply partitioning if the partition_column is specified
+        if self.partition_column:
+            print("Partitioning the DataFrame based on the column: " + self.partition_column)
+            raw_data_collection.create_index(self.partition_column)
+            raw_data_collection.create_index(self.groupby_attr)
+            df = df.repartition(col(self.partition_column))
+
+        # Filter the DataFrame based on the given device_id
+        df = df.filter(col(self.groupby_attr) == self.groupby)
+        start_time = self.aggregation_date
+        df = df.filter((col(self.groupby_attr) == self.groupby) & (col("timestamp") < start_time.timestamp()))
+        df = df.withColumn("timestamp_unix", F.col("timestamp").cast("bigint"))
+        df.createOrReplaceTempView("temp_table")
+
+        # Define empty schema for DataFrame
+        schema = StructType([
+            StructField(self.groupby_attr, StringType(), True)
+        ])
+        # Create empty DataFrame
+        result_df = self.spark.createDataFrame([], schema)
+
+        # Execute the dynamic Spark SQL
+        for sql in self.sparksql:
+            sql_base = sql.replace("{"+ self.groupby_attr + "}", str(self.groupby))
+            hour = int(sql.split("_")[2])
+            sql_with_timestamp = sql_base.replace("{timestamp}", str(int((start_time - timedelta(hours=hour)).timestamp())))
+            sql_with_timestamp_base = sql_with_timestamp.replace("{timestamp_base}", str(int((start_time).timestamp())))
+            c_count = self.spark.sql(sql_with_timestamp_base)
+            result_df = result_df.join(c_count, self.groupby_attr, "full") \
+                .select(result_df.columns + [col for col in c_count.columns if col not in result_df.columns])
+
+        if result_df.isEmpty():
+            json_aggregated_data = "{'error': 'No data found'}"
+        else:
+            json_aggregated_data = result_df.toJSON().collect()[0]
+
+        if json_aggregated_data is not None:
+            aggregated_data_collection.update_one(
+                {"date": start_time, "aggregated_key": self.groupby},
+                {"$set": {"aggregated_data": json_aggregated_data}},
+                upsert=True
+            )
+        else:
+            logging.error("Serialized aggregated data is None, skipping update")
+
+        return json_aggregated_data
+
+
```

### Comparing `featurizerai-1.6.5/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.6.6/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.6.5
+Version: 1.6.6
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

