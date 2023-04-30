# Comparing `tmp/repid-1.1.0.tar.gz` & `tmp/repid-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repid-1.1.0.tar", last modified: Sun Apr 30 00:36:25 2023, max compression
+gzip compressed data, was "repid-1.1.1.tar", last modified: Sun Apr 30 00:36:49 2023, max compression
```

## Comparing `repid-1.1.0.tar` & `repid-1.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1069 2023-04-30 00:35:58.893529 repid-1.1.0/LICENSE
--rw-r--r--   0        0        0     2589 2023-04-30 00:35:58.893529 repid-1.1.0/README.md
--rw-r--r--   0        0        0     3194 2023-04-30 00:36:25.261788 repid-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      588 2023-04-30 00:35:58.897529 repid-1.1.0/repid/__init__.py
--rw-r--r--   0        0        0     1393 2023-04-30 00:35:58.897529 repid-1.1.0/repid/_asyncify.py
--rw-r--r--   0        0        0     5073 2023-04-30 00:35:58.897529 repid-1.1.0/repid/_processor.py
--rw-r--r--   0        0        0     4061 2023-04-30 00:35:58.897529 repid-1.1.0/repid/_runner.py
--rw-r--r--   0        0        0      509 2023-04-30 00:35:58.897529 repid-1.1.0/repid/actor.py
--rw-r--r--   0        0        0     2316 2023-04-30 00:35:58.897529 repid-1.1.0/repid/config.py
--rw-r--r--   0        0        0     3313 2023-04-30 00:35:58.897529 repid-1.1.0/repid/connection.py
--rw-r--r--   0        0        0      698 2023-04-30 00:35:58.897529 repid-1.1.0/repid/connections/__init__.py
--rw-r--r--   0        0        0     6594 2023-04-30 00:35:58.897529 repid-1.1.0/repid/connections/abc.py
--rw-r--r--   0        0        0      158 2023-04-30 00:35:58.897529 repid-1.1.0/repid/connections/dummy/__init__.py
--rw-r--r--   0        0        0     1472 2023-04-30 00:35:58.897529 repid-1.1.0/repid/connections/dummy/bucket_broker.py
--rw-r--r--   0        0        0     2748 2023-04-30 00:35:58.897529 repid-1.1.0/repid/connections/dummy/consumer.py
--rw-r--r--   0        0        0     3792 2023-04-30 00:35:58.897529 repid-1.1.0/repid/connections/dummy/message_broker.py
--rw-r--r--   0        0        0      860 2023-04-30 00:35:58.897529 repid-1.1.0/repid/connections/dummy/utils.py
--rw-r--r--   0        0        0       90 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/rabbitmq/__init__.py
--rw-r--r--   0        0        0     6161 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/rabbitmq/consumer.py
--rw-r--r--   0        0        0     7091 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/rabbitmq/message_broker.py
--rw-r--r--   0        0        0      362 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/rabbitmq/protocols.py
--rw-r--r--   0        0        0      910 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/rabbitmq/utils.py
--rw-r--r--   0        0        0      158 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/redis/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/redis/bucket_broker.py
--rw-r--r--   0        0        0     7593 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/redis/consumer.py
--rw-r--r--   0        0        0     7609 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/redis/message_broker.py
--rw-r--r--   0        0        0     3818 2023-04-30 00:35:58.901528 repid-1.1.0/repid/connections/redis/utils.py
--rw-r--r--   0        0        0     1944 2023-04-30 00:35:58.901528 repid-1.1.0/repid/converter.py
--rw-r--r--   0        0        0      355 2023-04-30 00:35:58.901528 repid-1.1.0/repid/data/__init__.py
--rw-r--r--   0        0        0     2275 2023-04-30 00:35:58.901528 repid-1.1.0/repid/data/_buckets.py
--rw-r--r--   0        0        0      819 2023-04-30 00:35:58.901528 repid-1.1.0/repid/data/_key.py
--rw-r--r--   0        0        0     5545 2023-04-30 00:35:58.901528 repid-1.1.0/repid/data/_parameters.py
--rw-r--r--   0        0        0       95 2023-04-30 00:35:58.901528 repid-1.1.0/repid/data/priorities.py
--rw-r--r--   0        0        0     3873 2023-04-30 00:35:58.901528 repid-1.1.0/repid/data/protocols.py
--rw-r--r--   0        0        0     7465 2023-04-30 00:35:58.901528 repid-1.1.0/repid/job.py
--rw-r--r--   0        0        0      546 2023-04-30 00:35:58.901528 repid-1.1.0/repid/logger.py
--rw-r--r--   0        0        0     1655 2023-04-30 00:35:58.901528 repid-1.1.0/repid/main.py
--rw-r--r--   0        0        0      257 2023-04-30 00:35:58.901528 repid-1.1.0/repid/middlewares/__init__.py
--rw-r--r--   0        0        0      347 2023-04-30 00:35:58.901528 repid-1.1.0/repid/middlewares/consts.py
--rw-r--r--   0        0        0     3680 2023-04-30 00:35:58.901528 repid-1.1.0/repid/middlewares/middleware.py
--rw-r--r--   0        0        0     3647 2023-04-30 00:35:58.901528 repid-1.1.0/repid/middlewares/wrapper.py
--rw-r--r--   0        0        0        0 2023-04-30 00:35:58.901528 repid-1.1.0/repid/py.typed
--rw-r--r--   0        0        0     1064 2023-04-30 00:35:58.901528 repid-1.1.0/repid/queue.py
--rw-r--r--   0        0        0     1319 2023-04-30 00:35:58.901528 repid-1.1.0/repid/retry_policy.py
--rw-r--r--   0        0        0     5021 2023-04-30 00:35:58.901528 repid-1.1.0/repid/router.py
--rw-r--r--   0        0        0      604 2023-04-30 00:35:58.901528 repid-1.1.0/repid/serializer.py
--rw-r--r--   0        0        0      917 2023-04-30 00:35:58.901528 repid-1.1.0/repid/utils.py
--rw-r--r--   0        0        0     3971 2023-04-30 00:35:58.901528 repid-1.1.0/repid/worker.py
--rw-r--r--   0        0        0        0 2023-04-30 00:35:58.901528 repid-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      743 2023-04-30 00:35:58.901528 repid-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-30 00:35:58.901528 repid-1.1.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     3241 2023-04-30 00:35:58.901528 repid-1.1.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     1337 2023-04-30 00:35:58.901528 repid-1.1.0/tests/integration/test_buckets.py
--rw-r--r--   0        0        0     4335 2023-04-30 00:35:58.901528 repid-1.1.0/tests/integration/test_consumer.py
--rw-r--r--   0        0        0     4003 2023-04-30 00:35:58.901528 repid-1.1.0/tests/integration/test_default_flow.py
--rw-r--r--   0        0        0     1904 2023-04-30 00:35:58.901528 repid-1.1.0/tests/integration/test_no_messages_lost.py
--rw-r--r--   0        0        0      431 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_actor.py
--rw-r--r--   0        0        0     3110 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_config.py
--rw-r--r--   0        0        0     1962 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_connection.py
--rw-r--r--   0        0        0     3818 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_consumer.py
--rw-r--r--   0        0        0     2835 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_consumer_abc.py
--rw-r--r--   0        0        0    10233 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_default_data_models.py
--rw-r--r--   0        0        0     3003 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_hypothesis.py
--rw-r--r--   0        0        0     3591 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_job.py
--rw-r--r--   0        0        0      849 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_main.py
--rw-r--r--   0        0        0     7842 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_middleware.py
--rw-r--r--   0        0        0     1097 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     1484 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_pydantic.py
--rw-r--r--   0        0        0      414 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_queue.py
--rw-r--r--   0        0        0     3194 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_router.py
--rw-r--r--   0        0        0      764 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_serializer.py
--rw-r--r--   0        0        0      685 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_utils_wait_until.py
--rw-r--r--   0        0        0     6887 2023-04-30 00:35:58.901528 repid-1.1.0/tests/test_worker.py
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 repid-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-30 00:36:20.722967 repid-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2589 2023-04-30 00:36:20.722967 repid-1.1.1/README.md
+-rw-r--r--   0        0        0     3194 2023-04-30 00:36:49.898706 repid-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-04-30 00:36:20.726967 repid-1.1.1/repid/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-30 00:36:20.726967 repid-1.1.1/repid/_asyncify.py
+-rw-r--r--   0        0        0     5073 2023-04-30 00:36:20.726967 repid-1.1.1/repid/_processor.py
+-rw-r--r--   0        0        0     4061 2023-04-30 00:36:20.730967 repid-1.1.1/repid/_runner.py
+-rw-r--r--   0        0        0      509 2023-04-30 00:36:20.730967 repid-1.1.1/repid/actor.py
+-rw-r--r--   0        0        0     2316 2023-04-30 00:36:20.730967 repid-1.1.1/repid/config.py
+-rw-r--r--   0        0        0     3313 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connection.py
+-rw-r--r--   0        0        0      698 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/__init__.py
+-rw-r--r--   0        0        0     6594 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/abc.py
+-rw-r--r--   0        0        0      158 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/__init__.py
+-rw-r--r--   0        0        0     1472 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/bucket_broker.py
+-rw-r--r--   0        0        0     2748 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/consumer.py
+-rw-r--r--   0        0        0     3792 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/message_broker.py
+-rw-r--r--   0        0        0      860 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/dummy/utils.py
+-rw-r--r--   0        0        0       90 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     6161 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/consumer.py
+-rw-r--r--   0        0        0     7091 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/message_broker.py
+-rw-r--r--   0        0        0      362 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/protocols.py
+-rw-r--r--   0        0        0      910 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/rabbitmq/utils.py
+-rw-r--r--   0        0        0      158 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/__init__.py
+-rw-r--r--   0        0        0     1513 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/bucket_broker.py
+-rw-r--r--   0        0        0     7593 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/consumer.py
+-rw-r--r--   0        0        0     7609 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/message_broker.py
+-rw-r--r--   0        0        0     3818 2023-04-30 00:36:20.730967 repid-1.1.1/repid/connections/redis/utils.py
+-rw-r--r--   0        0        0     1944 2023-04-30 00:36:20.730967 repid-1.1.1/repid/converter.py
+-rw-r--r--   0        0        0      355 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/__init__.py
+-rw-r--r--   0        0        0     2275 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/_buckets.py
+-rw-r--r--   0        0        0      819 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/_key.py
+-rw-r--r--   0        0        0     5545 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/_parameters.py
+-rw-r--r--   0        0        0       95 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/priorities.py
+-rw-r--r--   0        0        0     3873 2023-04-30 00:36:20.730967 repid-1.1.1/repid/data/protocols.py
+-rw-r--r--   0        0        0     7465 2023-04-30 00:36:20.730967 repid-1.1.1/repid/job.py
+-rw-r--r--   0        0        0      546 2023-04-30 00:36:20.730967 repid-1.1.1/repid/logger.py
+-rw-r--r--   0        0        0     1655 2023-04-30 00:36:20.730967 repid-1.1.1/repid/main.py
+-rw-r--r--   0        0        0      257 2023-04-30 00:36:20.730967 repid-1.1.1/repid/middlewares/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-30 00:36:20.730967 repid-1.1.1/repid/middlewares/consts.py
+-rw-r--r--   0        0        0     3680 2023-04-30 00:36:20.730967 repid-1.1.1/repid/middlewares/middleware.py
+-rw-r--r--   0        0        0     3647 2023-04-30 00:36:20.730967 repid-1.1.1/repid/middlewares/wrapper.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:36:20.730967 repid-1.1.1/repid/py.typed
+-rw-r--r--   0        0        0     1064 2023-04-30 00:36:20.730967 repid-1.1.1/repid/queue.py
+-rw-r--r--   0        0        0     1319 2023-04-30 00:36:20.730967 repid-1.1.1/repid/retry_policy.py
+-rw-r--r--   0        0        0     5021 2023-04-30 00:36:20.730967 repid-1.1.1/repid/router.py
+-rw-r--r--   0        0        0      604 2023-04-30 00:36:20.730967 repid-1.1.1/repid/serializer.py
+-rw-r--r--   0        0        0      917 2023-04-30 00:36:20.730967 repid-1.1.1/repid/utils.py
+-rw-r--r--   0        0        0     3971 2023-04-30 00:36:20.730967 repid-1.1.1/repid/worker.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:36:20.730967 repid-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-30 00:36:20.730967 repid-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3241 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1337 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/test_buckets.py
+-rw-r--r--   0        0        0     4335 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/test_consumer.py
+-rw-r--r--   0        0        0     4003 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/test_default_flow.py
+-rw-r--r--   0        0        0     1904 2023-04-30 00:36:20.730967 repid-1.1.1/tests/integration/test_no_messages_lost.py
+-rw-r--r--   0        0        0      431 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_actor.py
+-rw-r--r--   0        0        0     3110 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_config.py
+-rw-r--r--   0        0        0     1962 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_connection.py
+-rw-r--r--   0        0        0     3818 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_consumer.py
+-rw-r--r--   0        0        0     2835 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_consumer_abc.py
+-rw-r--r--   0        0        0    10233 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_default_data_models.py
+-rw-r--r--   0        0        0     3003 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_hypothesis.py
+-rw-r--r--   0        0        0     3591 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_job.py
+-rw-r--r--   0        0        0      849 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_main.py
+-rw-r--r--   0        0        0     7842 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_middleware.py
+-rw-r--r--   0        0        0     1097 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     1484 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_pydantic.py
+-rw-r--r--   0        0        0      414 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_queue.py
+-rw-r--r--   0        0        0     3194 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_router.py
+-rw-r--r--   0        0        0      764 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_serializer.py
+-rw-r--r--   0        0        0      685 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_utils_wait_until.py
+-rw-r--r--   0        0        0     6887 2023-04-30 00:36:20.730967 repid-1.1.1/tests/test_worker.py
+-rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 repid-1.1.1/PKG-INFO
```

### Comparing `repid-1.1.0/LICENSE` & `repid-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/README.md` & `repid-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/pyproject.toml` & `repid-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "typing-extensions>=4.3.0,<5.0.0; python_version < \"3.10\"",
 ]
 description = "Repid framework: simple to use, fast to run and extensible to adopt job scheduler"
 dynamic = []
 name = "repid"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.1.0"
+version = "1.1.1"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 amqp = [
     "aiormq<7.0.0,>=6.4.0",
```

### Comparing `repid-1.1.0/repid/__init__.py` & `repid-1.1.1/repid/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/_asyncify.py` & `repid-1.1.1/repid/_asyncify.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations
 
 import asyncio
 import sys
-from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 from functools import partial, wraps
 from typing import Any, Callable, Coroutine, TypeVar, overload
 
 if sys.version_info >= (3, 10):  # pragma: no cover
     from typing import ParamSpec
 else:  # pragma: no cover
     from typing_extensions import ParamSpec
 
+if sys.platform != "emscripten":  # pragma: no cover
+    from concurrent.futures import ProcessPoolExecutor
+else:  # pragma: no cover
+    ProcessPoolExecutor = ThreadPoolExecutor
+
 FnP = ParamSpec("FnP")
 FnR = TypeVar("FnR")
 
 
 @overload
 def asyncify(
     fn: Callable[FnP, Coroutine[Any, Any, FnR]],
```

### Comparing `repid-1.1.0/repid/_processor.py` & `repid-1.1.1/repid/_processor.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/_runner.py` & `repid-1.1.1/repid/_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/config.py` & `repid-1.1.1/repid/config.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connection.py` & `repid-1.1.1/repid/connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/__init__.py` & `repid-1.1.1/repid/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/abc.py` & `repid-1.1.1/repid/connections/abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/dummy/bucket_broker.py` & `repid-1.1.1/repid/connections/dummy/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/dummy/consumer.py` & `repid-1.1.1/repid/connections/dummy/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/dummy/message_broker.py` & `repid-1.1.1/repid/connections/dummy/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/dummy/utils.py` & `repid-1.1.1/repid/connections/dummy/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/rabbitmq/consumer.py` & `repid-1.1.1/repid/connections/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/rabbitmq/message_broker.py` & `repid-1.1.1/repid/connections/rabbitmq/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/rabbitmq/utils.py` & `repid-1.1.1/repid/connections/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/redis/bucket_broker.py` & `repid-1.1.1/repid/connections/redis/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/redis/consumer.py` & `repid-1.1.1/repid/connections/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/redis/message_broker.py` & `repid-1.1.1/repid/connections/redis/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/connections/redis/utils.py` & `repid-1.1.1/repid/connections/redis/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/converter.py` & `repid-1.1.1/repid/converter.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/data/_buckets.py` & `repid-1.1.1/repid/data/_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/data/_key.py` & `repid-1.1.1/repid/data/_key.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/data/_parameters.py` & `repid-1.1.1/repid/data/_parameters.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/data/protocols.py` & `repid-1.1.1/repid/data/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/job.py` & `repid-1.1.1/repid/job.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/logger.py` & `repid-1.1.1/repid/logger.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/main.py` & `repid-1.1.1/repid/main.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/middlewares/middleware.py` & `repid-1.1.1/repid/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/middlewares/wrapper.py` & `repid-1.1.1/repid/middlewares/wrapper.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/queue.py` & `repid-1.1.1/repid/queue.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/retry_policy.py` & `repid-1.1.1/repid/retry_policy.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/router.py` & `repid-1.1.1/repid/router.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/serializer.py` & `repid-1.1.1/repid/serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/utils.py` & `repid-1.1.1/repid/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/repid/worker.py` & `repid-1.1.1/repid/worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/conftest.py` & `repid-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/integration/conftest.py` & `repid-1.1.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/integration/test_buckets.py` & `repid-1.1.1/tests/integration/test_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/integration/test_consumer.py` & `repid-1.1.1/tests/integration/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/integration/test_default_flow.py` & `repid-1.1.1/tests/integration/test_default_flow.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/integration/test_no_messages_lost.py` & `repid-1.1.1/tests/integration/test_no_messages_lost.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_config.py` & `repid-1.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_connection.py` & `repid-1.1.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_consumer.py` & `repid-1.1.1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_consumer_abc.py` & `repid-1.1.1/tests/test_consumer_abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_default_data_models.py` & `repid-1.1.1/tests/test_default_data_models.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_hypothesis.py` & `repid-1.1.1/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_job.py` & `repid-1.1.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_main.py` & `repid-1.1.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_middleware.py` & `repid-1.1.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_multiprocessing.py` & `repid-1.1.1/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_pydantic.py` & `repid-1.1.1/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_router.py` & `repid-1.1.1/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_serializer.py` & `repid-1.1.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_utils_wait_until.py` & `repid-1.1.1/tests/test_utils_wait_until.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/tests/test_worker.py` & `repid-1.1.1/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.1.0/PKG-INFO` & `repid-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repid
-Version: 1.1.0
+Version: 1.1.1
 Summary: Repid framework: simple to use, fast to run and extensible to adopt job scheduler
 Author-Email: aleksul <me@aleksul.space>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repid Version: 1.1.0 Summary: Repid framework:
+Metadata-Version: 2.1 Name: repid Version: 1.1.1 Summary: Repid framework:
 simple to use, fast to run and extensible to adopt job scheduler Author-Email:
 aleksul
 aleksul.space> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

