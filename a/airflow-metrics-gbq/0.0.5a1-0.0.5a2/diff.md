# Comparing `tmp/airflow_metrics_gbq-0.0.5a1.tar.gz` & `tmp/airflow_metrics_gbq-0.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_metrics_gbq-0.0.5a1.tar", max compression
+gzip compressed data, was "airflow_metrics_gbq-0.0.5a2.tar", max compression
```

## Comparing `airflow_metrics_gbq-0.0.5a1.tar` & `airflow_metrics_gbq-0.0.5a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1296 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/LICENSE
--rw-r--r--   0        0        0     2487 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/__init__.py
--rw-r--r--   0        0        0       94 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/exceptions.py
--rw-r--r--   0        0        0    10738 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/metrics.py
--rw-r--r--   0        0        0      700 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/utils/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/utils/gbq_connector.py
--rw-r--r--   0        0        0     1320 2023-04-27 22:54:10.903660 airflow_metrics_gbq-0.0.5a1/pyproject.toml
--rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.5a1/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-04-30 16:15:24.710732 airflow_metrics_gbq-0.0.5a2/LICENSE
+-rw-r--r--   0        0        0     2487 2023-04-30 16:15:24.710732 airflow_metrics_gbq-0.0.5a2/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 16:15:24.710732 airflow_metrics_gbq-0.0.5a2/airflow_metrics_gbq/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-30 16:15:24.710732 airflow_metrics_gbq-0.0.5a2/airflow_metrics_gbq/exceptions.py
+-rw-r--r--   0        0        0    10739 2023-04-30 16:15:24.710732 airflow_metrics_gbq-0.0.5a2/airflow_metrics_gbq/metrics.py
+-rw-r--r--   0        0        0      700 2023-04-30 16:15:24.710732 airflow_metrics_gbq-0.0.5a2/airflow_metrics_gbq/utils/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-30 16:15:24.710732 airflow_metrics_gbq-0.0.5a2/airflow_metrics_gbq/utils/gbq_connector.py
+-rw-r--r--   0        0        0     1320 2023-04-30 16:15:24.710732 airflow_metrics_gbq-0.0.5a2/pyproject.toml
+-rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 airflow_metrics_gbq-0.0.5a2/PKG-INFO
```

### Comparing `airflow_metrics_gbq-0.0.5a1/LICENSE` & `airflow_metrics_gbq-0.0.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.5a1/README.md` & `airflow_metrics_gbq-0.0.5a2/README.md`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/metrics.py` & `airflow_metrics_gbq-0.0.5a2/airflow_metrics_gbq/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from enum import Enum, unique
 from collections import defaultdict
 from dataclasses import dataclass
 import pandas as pd
 from tenacity import (
     retry,
     retry_if_exception_type,
-    wait_fixed,
-    wait_random,
+    wait_exponential,
     stop_after_attempt,
 )
 
 from airflow_metrics_gbq.utils import GoogleBigQueryConnector, setup_gcloud_logging
 from airflow_metrics_gbq.exceptions import NoMetricFoundException
 
 
@@ -190,16 +189,16 @@
         if metrics:
             self.logger.debug(f"Flushing out {len(metrics)} metrics to BigQuery")
             self.send_metrics(metrics)
             self._last_flush = time.time()
 
     @retry(
         retry=(retry_if_exception_type(queue.Full) | retry_if_exception_type(NoMetricFoundException)),
-        wait=wait_fixed(2) + wait_random(0, 2),
-        stop=stop_after_attempt(10),
+        wait=wait_exponential(multiplier=1, min=4, max=10),
+        stop=stop_after_attempt(20),
         reraise=True,
     )
     def _fetch(self):
         """Fetch metrics from Airflow"""
         while True:
             measure: str = self._sock.recv(1024).decode("utf-8")
```

### Comparing `airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/utils/__init__.py` & `airflow_metrics_gbq-0.0.5a2/airflow_metrics_gbq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.5a1/airflow_metrics_gbq/utils/gbq_connector.py` & `airflow_metrics_gbq-0.0.5a2/airflow_metrics_gbq/utils/gbq_connector.py`

 * *Files identical despite different names*

### Comparing `airflow_metrics_gbq-0.0.5a1/pyproject.toml` & `airflow_metrics_gbq-0.0.5a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-metrics-gbq"
-version = "0.0.5a1"
+version = "0.0.5a2"
 description = "Airflow metrics to Google BigQuery"
 authors = ["Shaurya Rawat <rawatshaurya1994@gmail.com>"]
 license = "BSD2"
 readme = "README.md"
 homepage="https://github.com/abyssnlp/airflow-metrics-gbq"
 repository="https://github.com/abyssnlp/airflow-metrics-gbq"
 include=[
```

### Comparing `airflow_metrics_gbq-0.0.5a1/PKG-INFO` & `airflow_metrics_gbq-0.0.5a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metrics-gbq
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: Airflow metrics to Google BigQuery
 Home-page: https://github.com/abyssnlp/airflow-metrics-gbq
 License: BSD2
 Author: Shaurya Rawat
 Author-email: rawatshaurya1994@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

