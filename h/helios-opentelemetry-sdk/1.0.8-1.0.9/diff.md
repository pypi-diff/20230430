# Comparing `tmp/helios-opentelemetry-sdk-1.0.8.tar.gz` & `tmp/helios-opentelemetry-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-opentelemetry-sdk-1.0.8.tar", last modified: Mon Jul 18 13:04:03 2022, max compression
+gzip compressed data, was "helios-opentelemetry-sdk-1.0.9.tar", last modified: Wed Jul 20 15:11:28 2022, max compression
```

## Comparing `helios-opentelemetry-sdk-1.0.8.tar` & `helios-opentelemetry-sdk-1.0.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.336413 helios-opentelemetry-sdk-1.0.8/helios/
--rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.336413 helios-opentelemetry-sdk-1.0.8/helios/aiosmtplib_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/aiosmtplib_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.336413 helios-opentelemetry-sdk-1.0.8/helios/aiosmtplib_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/aiosmtplib_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.336413 helios-opentelemetry-sdk-1.0.8/helios/aiosmtplib_instrumentation/src/aiosmtplib/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.336413 helios-opentelemetry-sdk-1.0.8/helios/base/
--rw-r--r--   0 runner    (1001) docker     (121)    14478 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8421 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/data_obfuscator.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.336413 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.336413 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/conditional_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/fork_process_otlp_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/hooked_batch_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/base/tracing/suppress_tracing.py
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     7594 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/helios.py
--rw-r--r--   0 runner    (1001) docker     (121)     5191 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/helios_test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/aiosmtplib.py
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/base_http_instrumentor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/
--rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/ses.py
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/sns.py
--rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/sqs.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/sqs_message_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5970 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/django.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8605 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/helios_asgi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/httpx.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/kafka.py
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/pika.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/raven.py
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/sentry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/starlette.py
--rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/tornado.py
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/urllib.py
--rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/instrumentation/urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/src/kafka/
--rw-r--r--   0 runner    (1001) docker     (121)     9882 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/src/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/src/kafka/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.340413 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/src/pyspark/
--rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/src/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/src/pyspark/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7585 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/tests/test_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/raven/
--rw-r--r--   0 runner    (1001) docker     (121)     2170 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/raven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/raven/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/sentry/
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/sentry/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/helios/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-18 13:04:03.000000 helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-07-18 13:04:03.000000 helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 13:04:03.000000 helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-07-18 13:04:03.000000 helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-07-18 13:04:03.000000 helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-18 13:04:03.000000 helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/hstest/
--rw-r--r--   0 runner    (1001) docker     (121)     9810 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/hstest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/hstest/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-18 13:04:03.344413 helios-opentelemetry-sdk-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-07-18 13:03:36.000000 helios-opentelemetry-sdk-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/
+-rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/aiosmtplib/
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/base/
+-rw-r--r--   0 runner    (1001) docker     (121)    14478 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8873 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/data_obfuscator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/conditional_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/fork_process_otlp_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/hooked_batch_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/suppress_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7594 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/helios.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5191 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/helios_test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/aiosmtplib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/base_http_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/
+-rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/ses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sqs_message_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5970 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/django.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8605 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/helios_asgi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pika.py
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/raven.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/redis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/kafka/
+-rw-r--r--   0 runner    (1001) docker     (121)     9882 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/kafka/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/pyspark/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7585 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/tests/test_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/raven/
+-rw-r--r--   0 runner    (1001) docker     (121)     2170 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/raven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/raven/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/sentry/
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/sentry/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/hstest/
+-rw-r--r--   0 runner    (1001) docker     (121)     9810 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/hstest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/hstest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/setup.py
```

### Comparing `helios-opentelemetry-sdk-1.0.8/LICENSE` & `helios-opentelemetry-sdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/PKG-INFO` & `helios-opentelemetry-sdk-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Helios OpenTelemetry SDK
 Home-page: https://github.com/helios/python-sdk
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Platform: UNKNOWN
```

### Comparing `helios-opentelemetry-sdk-1.0.8/README.md` & `helios-opentelemetry-sdk-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/base/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/base/data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/data_obfuscator.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 DATA_TO_DROP = [SpanAttributes.HTTP_RESPONSE_BODY]
 DATA_TO_OBFUSCATE = [
     SpanAttributes.DB_QUERY_RESULT,
     SpanAttributes.DB_STATEMENT,
     SpanAttributes.HTTP_REQUEST_BODY,
     SpanAttributes.MESSAGING_PAYLOAD,
 ]
+IS_DATA_OBFUSCATED_KEY = 'hs_data_obfuscated'
+
 ExpectedValueType = Optional[Union[str, float, int, bool]]
 Mode = Optional[str]
 Rules = Optional[List[Union[Tuple[str, ExpectedValueType], str]]]
 
 
 @dataclass
 class DataObfuscatorConfiguration:
@@ -59,14 +61,16 @@
     def obfuscate_data(self, span: ReadableSpan) -> None:
         # noinspection PyProtectedMember
         attributes = span._attributes
 
         if attributes is None:
             return
 
+        self._inject_data_obfuscation_flag(span)
+
         for datum_to_drop in DATA_TO_DROP:
             if datum_to_drop in attributes:
                 # noinspection PyUnresolvedReferences
                 del attributes[datum_to_drop]
 
         for datum_to_obfuscate in DATA_TO_OBFUSCATE:
             if datum_to_obfuscate in attributes:
@@ -114,14 +118,22 @@
             try:
                 parsed_local_rules.append(parse(path_expression))
             except Exception as exception:
                 _LOG.debug(f'Ignoring invalid path expression {path_expression}.', exception)
 
         return parsed_local_rules
 
+    @staticmethod
+    def _inject_data_obfuscation_flag(span: ReadableSpan) -> None:
+        try:
+            # noinspection PyProtectedMember, PyUnresolvedReferences
+            span.resource.attributes._dict[IS_DATA_OBFUSCATED_KEY] = True
+        except Exception as exception:
+            _LOG.debug('Cannot inject data obfuscation flag.', exception)
+
     def _obfuscate_datum(self, value: AttributeValue) -> AttributeValue:
         if isinstance(value, str):
             dict_or_list: Optional[Union[dict, list]]
 
             try:
                 dict_or_list = loads(value)
             except JSONDecodeError:
```

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/conditional_span_processor.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/conditional_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/fork_process_otlp_span_exporter.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/fork_process_otlp_span_exporter.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/base/tracing/export/hooked_batch_span_processor.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/hooked_batch_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/helios.py` & `helios-opentelemetry-sdk-1.0.9/helios/helios.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/helios_test_trace.py` & `helios-opentelemetry-sdk-1.0.9/helios/helios_test_trace.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/aiohttp.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/aiohttp.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/aiosmtplib.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/aiosmtplib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/base.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/base.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/base_http_instrumentor.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/base_http_instrumentor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/consts.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/consts.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/dynamodb.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/dynamodb.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/s3.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/s3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/ses.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/ses.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/sns.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sns.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/sqs.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sqs.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/sqs_message_context.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sqs_message_context.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/botocore/utils.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/django.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/django.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/elasticsearch.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/fastapi.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/flask.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/grpc.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/grpc.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/helios_asgi_middleware.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/helios_asgi_middleware.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/httpx.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/httpx.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/kafka.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/logging.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/pika.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/psycopg2.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/psycopg2.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/pymongo.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pymongo.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/pyspark.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/raven.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/raven.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/redis.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/redis.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/requests.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/requests.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/sentry.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/sentry.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/starlette.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/starlette.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/tornado.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/tornado.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/urllib.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/urllib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/instrumentation/urllib3.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/urllib3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/src/kafka/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/kafka_instrumentation/tests/test_kafka.py` & `helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/src/pyspark/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/pyspark_instrumentation/tests/test_pyspark.py` & `helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/sampler.py` & `helios-opentelemetry-sdk-1.0.9/helios/sampler.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/raven/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/raven/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios/sentry_instrumentation/src/sentry/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/PKG-INFO` & `helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Helios OpenTelemetry SDK
 Home-page: https://github.com/helios/python-sdk
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Platform: UNKNOWN
```

### Comparing `helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/SOURCES.txt` & `helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/helios_opentelemetry_sdk.egg-info/requires.txt` & `helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/hstest/__init__.py` & `helios-opentelemetry-sdk-1.0.9/hstest/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.8/setup.py` & `helios-opentelemetry-sdk-1.0.9/setup.py`

 * *Files identical despite different names*

