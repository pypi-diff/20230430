# Comparing `tmp/longalpha_utils-0.41.tar.gz` & `tmp/longalpha_utils-0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.41.tar", last modified: Sun Apr 23 15:45:38 2023, max compression
+gzip compressed data, was "longalpha_utils-0.42.tar", last modified: Sun Apr 30 16:06:39 2023, max compression
```

## Comparing `longalpha_utils-0.41.tar` & `longalpha_utils-0.42.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:45:38.880103 longalpha_utils-0.41/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 15:45:38.880103 longalpha_utils-0.41/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:45:38.880103 longalpha_utils-0.41/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-23 15:45:25.000000 longalpha_utils-0.41/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:45:38.880103 longalpha_utils-0.41/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 15:45:38.000000 longalpha_utils-0.41/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:45:38.880103 longalpha_utils-0.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-23 15:45:25.000000 longalpha_utils-0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:39.361355 longalpha_utils-0.42/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-30 16:06:39.361355 longalpha_utils-0.42/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:39.357355 longalpha_utils-0.42/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:39.361355 longalpha_utils-0.42/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:06:39.361355 longalpha_utils-0.42/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-30 16:06:25.000000 longalpha_utils-0.42/setup.py
```

### Comparing `longalpha_utils-0.41/longalpha_utils/messenger.py` & `longalpha_utils-0.42/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.41/longalpha_utils/transfers.py` & `longalpha_utils-0.42/longalpha_utils/transfers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
             endpoint=minio_url,
             access_key=minio_access_key,
             secret_key=minio_secret_key,
             secure=False,
         )
 
     def fput(
-            self,
-            file_path,
-            bucket_name: str,
-            object_name: str,
+        self,
+        file_path,
+        bucket_name: str,
+        object_name: str,
     ):
         """
         put a file to s3
         Args:
             file_path: path to the file
             bucket_name: Minio bucket_name
             object_name: object name in the minio bucket
@@ -64,18 +64,18 @@
                 raise ValueError("Incorrect file format")
             self.fput(file_path=path, bucket_name=bucket_name, object_name=object_name)
 
     def fget(self, file_path: str, bucket_name: str, object_name: str):
         self.minio_client.fget_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
     def get(
-            self,
-            bucket_name: str,
-            object_name: str,
-            file_format: str,
+        self,
+        bucket_name: str,
+        object_name: str,
+        file_format: str,
     ) -> pd.DataFrame:
         """
         get a parquet from s3 and read it into pandas dataframe
         Args:
             bucket_name: Minio bucket_name
             object_name: path + file_name
             file_format: parquet or pickle
@@ -111,20 +111,19 @@
         return self.get(bucket_name=bucket_name, object_name=latest_obj.object_name, file_format=file_format)
 
     def list(self, bucket_name: str) -> List[str]:
         return [i.object_name for i in self.minio_client.list_objects(bucket_name)]
 
 
 def init_spark(
-        spark_executor_memory: str = "30g",
-        spark_driver_memory: str = "90g",
-        connect_psql: bool = False,
-        minio_endpoint: Optional[str] = None,
-        minio_access_key: Optional[str] = None,
-        minio_secret_key: Optional[str] = None,
+    spark_executor_memory: str = "30g",
+    spark_driver_memory: str = "90g",
+    minio_endpoint: Optional[str] = None,
+    minio_access_key: Optional[str] = None,
+    minio_secret_key: Optional[str] = None,
 ) -> SparkSession:
     """
     get a spark instance.
 
     if connect_psql is True, then we will connect to psql.
     if minio_endpoint is not None, then we will connect to minio.
     if both are None, then we will connect to local spark.
@@ -137,50 +136,45 @@
         minio_secret_key:  minio_secret_key
         spark_executor_memory: size of spark_executor_memory
         spark_driver_memory: size of spark_driver_memory
         connect_psql: whether to connect to psql
     Returns:
 
     """
-    jars = []
-    if connect_psql:
-        jars+=["org.postgresql:postgresql:42.5.2"]
-    if minio_endpoint is not None:
-        jars += ["org.apache.hadoop:hadoop-aws:3.3.2", "com.amazonaws:aws-java-sdk-bundle:1.12.405"]
+    jars = [
+        "org.postgresql:postgresql:42.5.2",
+        "org.apache.hadoop:hadoop-aws:3.3.2",
+        "com.amazonaws:aws-java-sdk-bundle:1.12.405",
+    ]
 
     spark_conf = (
         SparkConf()
         .set("spark.executor.memory", spark_executor_memory)
         .set("spark.driver.memory", spark_driver_memory)
         .set("spark.sql.execution.arrow.pyspark.enabled", "true")
         .set("spark.ui.port", "4043")
         .set(
-            "spark.jars.packages",
-            ",".join(jars)
+            "spark.jars.packages", ",".join(jars)
         )  # if you set park.jars.packages more than once, only the last one will be used.
         .set("spark.hadoop.fs.s3a.impl", "org.apache.hadoop.fs.s3a.S3AFileSystem")
         .set("spark.hadoop.fs.s3a.path.style.access ", "true")
-
-    )
-    spark = (
-        SparkSession.builder.config(conf=spark_conf).getOrCreate()
-
     )
+    spark = SparkSession.builder.config(conf=spark_conf).getOrCreate()
 
     if minio_endpoint is not None:
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.endpoint", minio_endpoint)
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.access.key", minio_access_key)
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.secret.key", minio_secret_key)
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.connection.ssl.enabled", "false")
 
     return spark
 
 
 def spark_read_psql(
-        spark: SparkSession, psql_url: str, psql_db: str, psql_table: str, psql_usr: str, psql_pwd: str
+    spark: SparkSession, psql_url: str, psql_db: str, psql_table: str, psql_usr: str, psql_pwd: str
 ) -> DataFrame:
     """
     use spark to read psql
     Args:
         spark: spark instance. Must be created with support for psql.
         psql_url: url of psql
         psql_db: database name
@@ -199,25 +193,25 @@
         .option("password", psql_pwd)
         .option("driver", "org.postgresql.Driver")
         .load()
     )
 
 
 def df_to_psql(
-        df: pd.DataFrame,
-        table_name: str,
-        index=False,
-        dtype: Optional[Dict[str, Any]] = None,
-        if_exists: str = "append",
-        engine: Optional[Engine] = None,
-        user_name: Optional[str] = None,
-        password: Optional[str] = None,
-        host_with_port: Optional[str] = None,
-        db_name: Optional[str] = None,
-        **kwargs: Any,
+    df: pd.DataFrame,
+    table_name: str,
+    index=False,
+    dtype: Optional[Dict[str, Any]] = None,
+    if_exists: str = "append",
+    engine: Optional[Engine] = None,
+    user_name: Optional[str] = None,
+    password: Optional[str] = None,
+    host_with_port: Optional[str] = None,
+    db_name: Optional[str] = None,
+    **kwargs: Any,
 ) -> None:
     """
     write a pandas dataframe to psql
     Args:
         df: pandas dataframe
         table_name: table name to write to psql
         index: whether to write index to psql
@@ -238,25 +232,25 @@
     """
     if engine is not None and user_name is not None:
         raise ValueError("engine and user_name cannot be both not None")
     if engine is None and user_name is None:
         raise ValueError("engine and user_name cannot be both None")
     if engine is None:
         engine = create_engine(f"postgresql://{user_name}:{password}@{host_with_port}/{db_name}")
-    df.to_sql(table_name, con=engine, index=index, if_exists = if_exists, dtype = dtype, **kwargs)
+    df.to_sql(table_name, con=engine, index=index, if_exists=if_exists, dtype=dtype, **kwargs)
 
 
 def df_from_psql(
-        sql: str,
-        engine: Optional[Engine] = None,
-        user_name: Optional[str] = None,
-        password: Optional[str] = None,
-        host_with_port: Optional[str] = None,
-        db_name: Optional[str] = None,
-        **kwargs: Any,
+    sql: str,
+    engine: Optional[Engine] = None,
+    user_name: Optional[str] = None,
+    password: Optional[str] = None,
+    host_with_port: Optional[str] = None,
+    db_name: Optional[str] = None,
+    **kwargs: Any,
 ) -> pd.DataFrame:
     """
     read a pandas dataframe from psql
     Args:
         sql: sql query
         engine: sqlalchemy engine. If not None, then we will use this engine to write to psql.
         user_name:  username of psql
@@ -271,8 +265,8 @@
     if engine is not None and user_name is not None:
         raise ValueError("engine and user_name cannot be both not None")
     if engine is None and user_name is None:
         raise ValueError("engine and user_name cannot be both None")
     if engine is None:
         engine = create_engine(f"postgresql://{user_name}:{password}@{host_with_port}/{db_name}")
     query = text(sql)
-    return pd.read_sql(sql=query, con=engine.connect(), **kwargs)
+    return pd.read_sql(sql=query, con=engine.connect(), **kwargs)
```

### Comparing `longalpha_utils-0.41/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.42/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.41/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.42/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.41/setup.py` & `longalpha_utils-0.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.41",
+    version="0.42",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

