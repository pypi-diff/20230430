# Comparing `tmp/citizenk-0.1.36.tar.gz` & `tmp/citizenk-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.36.tar", max compression
+gzip compressed data, was "citizenk-0.1.37.tar", max compression
```

## Comparing `citizenk-0.1.36.tar` & `citizenk-0.1.37.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.36/citizenk/__init__.py
--rw-r--r--   0        0        0     3885 2023-04-29 16:34:03.427065 citizenk-0.1.36/citizenk/agent.py
--rw-r--r--   0        0        0    19933 2023-04-30 07:00:31.581775 citizenk-0.1.36/citizenk/citizenk.py
--rw-r--r--   0        0        0    20926 2023-04-30 07:13:05.877591 citizenk-0.1.36/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.36/citizenk/murmur2.py
--rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.36/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.36/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-30 07:20:07.476015 citizenk-0.1.36/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-30 07:20:10.053324 citizenk-0.1.36/setup.py
--rw-r--r--   0        0        0     1076 2023-04-30 07:20:10.053601 citizenk-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.37/citizenk/__init__.py
+-rw-r--r--   0        0        0     3885 2023-04-29 16:34:03.427065 citizenk-0.1.37/citizenk/agent.py
+-rw-r--r--   0        0        0    19999 2023-04-30 09:42:47.954845 citizenk-0.1.37/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20926 2023-04-30 07:13:05.877591 citizenk-0.1.37/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.37/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.37/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.37/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-04-30 09:44:31.816027 citizenk-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-30 09:44:34.538723 citizenk-0.1.37/setup.py
+-rw-r--r--   0        0        0     1076 2023-04-30 09:44:34.538985 citizenk-0.1.37/PKG-INFO
```

### Comparing `citizenk-0.1.36/citizenk/agent.py` & `citizenk-0.1.37/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.36/citizenk/citizenk.py` & `citizenk-0.1.37/citizenk/citizenk.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,37 +210,34 @@
             topic.replica_count = len(broker_topics[topic_name].partitions[0].replicas)
 
         # Start consumer
         if len(self.consumer_topics) > 0:
             self.consumer.start_consumer(list(self.consumer_topics))
 
             if self.consumer_in_thred:
-                self.background_loop = asyncio.new_event_loop()
-                loop = self.background_loop
                 self.background_thread = threading.Thread(
-                    target=self.background_consumer_thread,
-                    args=(loop,)
+                    target=self.background_consumer_thread
                 )
             else:
-                loop = self._main_consumer_loop()
-
-            self.main_consumer_loop_task = asyncio.create_task(loop)
+                self.main_consumer_loop_task = asyncio.create_task(self._main_consumer_loop())
             self.monitor_loop_task = asyncio.create_task(self._monitor_loop())
 
     def shutdown(self):
         """CitizenK shutdown Called on FastAPI shutown"""
         logger.debug("CitizenK Shutting down...")
         if self.consumer is not None:
             self.consumer.close()
             self.consumer = None
         if self.producer is not None:
             self.producer.close()
             self.producer = None
         if self.main_consumer_loop_task is not None:
             self.main_consumer_loop_task.cancel()
+        if self.consumer_in_thred:
+            self.background_loop.stop()
 
     def validate_messages(self, msgs: List[ConfluentMessage]) -> List[KafkaEvent]:
         """Validate the incoming Kafka messages"""
         events = []
         for msg in msgs:
             topic_name = msg.topic()
             if topic_name not in self.consumer_topics:
@@ -266,16 +263,19 @@
                     offset=msg.offset(),
                     timestamp=msg.timestamp()[1],
                     headers=msg.headers(),
                 )
             )
         return events
 
-    def background_consumer_thread(self,loop):
+    def background_consumer_thread(self):
+        loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
+        self.background_loop = loop
+        self.main_consumer_loop_task = asyncio.create_task(self._main_consumer_loop())
         try:
             loop.run_forever()
         except asyncio.CancelledError as e:
             logger.error('Background consumer loop cancelled %s',e)
         finally:
             for task in asyncio.all_tasks():
                 logger.info("Stopping %s",task.get_name())
```

### Comparing `citizenk-0.1.36/citizenk/kafka_adapter.py` & `citizenk-0.1.37/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.36/citizenk/murmur2.py` & `citizenk-0.1.37/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.36/citizenk/topic.py` & `citizenk-0.1.37/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.36/pyproject.toml` & `citizenk-0.1.37/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.36"
+version = "0.1.37"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.36/setup.py` & `citizenk-0.1.37/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.36',
+    'version': '0.1.37',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.36/PKG-INFO` & `citizenk-0.1.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.36
+Version: 0.1.37
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

