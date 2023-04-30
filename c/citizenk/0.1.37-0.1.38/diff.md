# Comparing `tmp/citizenk-0.1.37.tar.gz` & `tmp/citizenk-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.37.tar", max compression
+gzip compressed data, was "citizenk-0.1.38.tar", max compression
```

## Comparing `citizenk-0.1.37.tar` & `citizenk-0.1.38.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.37/citizenk/__init__.py
--rw-r--r--   0        0        0     3885 2023-04-29 16:34:03.427065 citizenk-0.1.37/citizenk/agent.py
--rw-r--r--   0        0        0    19999 2023-04-30 09:42:47.954845 citizenk-0.1.37/citizenk/citizenk.py
--rw-r--r--   0        0        0    20926 2023-04-30 07:13:05.877591 citizenk-0.1.37/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.37/citizenk/murmur2.py
--rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.37/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.37/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-04-30 09:44:31.816027 citizenk-0.1.37/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-30 09:44:34.538723 citizenk-0.1.37/setup.py
--rw-r--r--   0        0        0     1076 2023-04-30 09:44:34.538985 citizenk-0.1.37/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.38/citizenk/__init__.py
+-rw-r--r--   0        0        0     3885 2023-04-29 16:34:03.427065 citizenk-0.1.38/citizenk/agent.py
+-rw-r--r--   0        0        0    20673 2023-04-30 10:20:37.732046 citizenk-0.1.38/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20926 2023-04-30 07:13:05.877591 citizenk-0.1.38/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.38/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.38/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.38/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-04-30 10:21:24.440462 citizenk-0.1.38/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-30 10:21:26.805660 citizenk-0.1.38/setup.py
+-rw-r--r--   0        0        0     1076 2023-04-30 10:21:26.805921 citizenk-0.1.38/PKG-INFO
```

### Comparing `citizenk-0.1.37/citizenk/agent.py` & `citizenk-0.1.38/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.37/citizenk/citizenk.py` & `citizenk-0.1.38/citizenk/citizenk.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,33 +210,40 @@
             topic.replica_count = len(broker_topics[topic_name].partitions[0].replicas)
 
         # Start consumer
         if len(self.consumer_topics) > 0:
             self.consumer.start_consumer(list(self.consumer_topics))
 
             if self.consumer_in_thred:
+                # Start in thread
+                self.background_loop = asyncio.new_event_loop()
                 self.background_thread = threading.Thread(
-                    target=self.background_consumer_thread
-                )
+                    target=self.background_consumer_thread,
+                    args=(self.background_loop,))
+                self.background_thread.start()
+                self.main_consumer_loop_task = asyncio.run_coroutine_threadsafe(
+                    self._main_consumer_loop(),
+                    self.background_loop)
             else:
+                # Start in task
                 self.main_consumer_loop_task = asyncio.create_task(self._main_consumer_loop())
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
-        if self.consumer_in_thred:
+        if self.background_loop is not None:
             self.background_loop.stop()
 
     def validate_messages(self, msgs: List[ConfluentMessage]) -> List[KafkaEvent]:
         """Validate the incoming Kafka messages"""
         events = []
         for msg in msgs:
             topic_name = msg.topic()
@@ -263,19 +270,16 @@
                     offset=msg.offset(),
                     timestamp=msg.timestamp()[1],
                     headers=msg.headers(),
                 )
             )
         return events
 
-    def background_consumer_thread(self):
-        loop = asyncio.new_event_loop()
+    def background_consumer_thread(self, loop:asyncio.BaseEventLoop):
         asyncio.set_event_loop(loop)
-        self.background_loop = loop
-        self.main_consumer_loop_task = asyncio.create_task(self._main_consumer_loop())
         try:
             loop.run_forever()
         except asyncio.CancelledError as e:
             logger.error('Background consumer loop cancelled %s',e)
         finally:
             for task in asyncio.all_tasks():
                 logger.info("Stopping %s",task.get_name())
@@ -285,15 +289,26 @@
             loop.close()
 
     async def _monitor_loop(self):
         """Periodic task that checks Kafka status, and kills the process"""
         logger.debug("CitizenK Main monitor loop started...")
         while True:
             await asyncio.sleep(10)
-            if not self.status():
+            alive = True
+            done = True
+            # Check background thread status
+            if self.background_consumer_thread is not None:
+                alive = self.background_thread.is_alive()
+
+            # Check consumer task status
+            if self.main_consumer_loop_task is not None:
+                done = self.main_consumer_loop_task.done()
+
+            # Check kafka
+            if not self.status() or not alive or done:
                 self.shutdown()
                 os.kill(os.getpid(), signal.SIGINT)
                 await asyncio.sleep(60)
                 os.kill(os.getpid(), signal.SIGKILL)
 
     async def _main_consumer_loop(self):
         """Main Kafka consumer loop which invokes the process agents"""
```

### Comparing `citizenk-0.1.37/citizenk/kafka_adapter.py` & `citizenk-0.1.38/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.37/citizenk/murmur2.py` & `citizenk-0.1.38/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.37/citizenk/topic.py` & `citizenk-0.1.38/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.37/pyproject.toml` & `citizenk-0.1.38/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.37"
+version = "0.1.38"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.37/setup.py` & `citizenk-0.1.38/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.37',
+    'version': '0.1.38',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.37/PKG-INFO` & `citizenk-0.1.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.37
+Version: 0.1.38
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

