# Comparing `tmp/vents-0.0.4.tar.gz` & `tmp/vents-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.0.4.tar", last modified: Sat Apr 29 18:37:37 2023, max compression
+gzip compressed data, was "vents-0.0.5.tar", last modified: Sun Apr 30 13:24:56 2023, max compression
```

## Comparing `vents-0.0.4.tar` & `vents-0.0.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.965695 vents-0.0.4/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-04-29 18:34:33.000000 vents-0.0.4/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-29 18:37:37.965761 vents-0.0.4/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-04-29 18:37:37.966200 vents-0.0.4/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-04-29 18:34:33.000000 vents-0.0.4/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.961222 vents-0.0.4/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     5330 2023-04-29 18:34:33.000000 vents-0.0.4/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.962510 vents-0.0.4/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      321 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2100 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     2888 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)      438 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/k8s_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-04-29 18:34:33.000000 vents-0.0.4/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.963643 vents-0.0.4/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      233 2023-04-29 18:34:33.000000 vents-0.0.4/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.964002 vents-0.0.4/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.964472 vents-0.0.4/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1520 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/aws/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.965003 vents-0.0.4/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/azure/blob_storage.py
--rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.965578 vents-0.0.4/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)      995 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/gcp/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-29 18:34:33.000000 vents-0.0.4/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.961866 vents-0.0.4/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1209 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       66 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.908438 vents-0.0.5/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-04-30 13:21:50.000000 vents-0.0.5/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-30 13:24:56.908567 vents-0.0.5/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-04-30 13:24:56.909137 vents-0.0.5/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-04-30 13:21:50.000000 vents-0.0.5/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.900783 vents-0.0.5/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     5330 2023-04-30 13:21:50.000000 vents-0.0.5/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.902852 vents-0.0.5/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      321 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2100 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2888 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)      438 2023-04-30 13:21:50.000000 vents-0.0.5/vents/connections/k8s_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-04-30 13:21:50.000000 vents-0.0.5/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.905037 vents-0.0.5/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-04-30 13:21:50.000000 vents-0.0.5/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-04-30 13:21:50.000000 vents-0.0.5/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.905662 vents-0.0.5/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.906509 vents-0.0.5/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.907434 vents-0.0.5/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.908230 vents-0.0.5/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-04-30 13:21:50.000000 vents-0.0.5/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-30 13:21:50.000000 vents-0.0.5/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-30 13:21:50.000000 vents-0.0.5/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-30 13:24:56.901819 vents-0.0.5/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1209 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       66 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-04-30 13:24:56.000000 vents-0.0.5/vents.egg-info/top_level.txt
```

### Comparing `vents-0.0.4/PKG-INFO` & `vents-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.0.4
+Version: 0.0.5
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.0.4/setup.cfg` & `vents-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/setup.py` & `vents-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/config.py` & `vents-0.0.5/vents/config.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/connections/catalog.py` & `vents-0.0.5/vents/connections/catalog.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/connections/connection.py` & `vents-0.0.5/vents/connections/connection.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/connections/connection_schema.py` & `vents-0.0.5/vents/connections/connection_schema.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/notifiers/__init__.py` & `vents-0.0.5/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/notifiers/base.py` & `vents-0.0.5/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/notifiers/discord_webhook.py` & `vents-0.0.5/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/notifiers/hipchat_webhook.py` & `vents-0.0.5/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/notifiers/mattermost_webhook.py` & `vents-0.0.5/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/notifiers/pagerduty_webhook.py` & `vents-0.0.5/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/notifiers/slack_webhook.py` & `vents-0.0.5/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/notifiers/webhook.py` & `vents-0.0.5/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/aws/base.py` & `vents-0.0.5/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/aws/s3.py` & `vents-0.0.5/vents/providers/aws/s3.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,39 +13,40 @@
 
 
 class S3Service(AWSService):
     def _set_session(
         self,
         asynchronous: Optional[bool] = False,
         use_listings_cache: Optional[bool] = False,
-        config_kwargs: Optional[Dict] = None,
-        client_kwargs: Optional[Dict] = None,
         **kwargs
     ):
+        config_kwargs = kwargs.get("config_kwargs", {})
+        if self.region and "region_name" not in config_kwargs:
+            config_kwargs["region_name"] = self.region
+        client_kwargs = kwargs.get("client_kwargs", {})
+        if self.verify_ssl is not None and "verify" not in client_kwargs:
+            client_kwargs["verify"] = self.verify_ssl
         self._session = S3FileSystem(
             key=self.access_key_id,
             secret=self.secret_access_key,
             token=self.session_token,
             use_ssl=self.use_ssl,
+            endpoint_url=self.endpoint_url,
             config_kwargs=config_kwargs,
             client_kwargs=client_kwargs,
             asynchronous=asynchronous,
             use_listings_cache=use_listings_cache,
             **kwargs,
         )
 
     def get_fs(
         self,
         asynchronous: Optional[bool] = False,
         use_listings_cache: Optional[bool] = False,
-        config_kwargs: Optional[Dict] = None,
-        client_kwargs: Optional[Dict] = None,
         **kwargs
     ):
         self._set_session(
             asynchronous=asynchronous,
             use_listings_cache=use_listings_cache,
-            config_kwargs=config_kwargs,
-            client_kwargs=client_kwargs,
             **kwargs,
         )
         return self.session
```

### Comparing `vents-0.0.4/vents/providers/aws/service.py` & `vents-0.0.5/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/azure/base.py` & `vents-0.0.5/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/azure/blob_storage.py` & `vents-0.0.5/vents/providers/azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/azure/service.py` & `vents-0.0.5/vents/providers/azure/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/base.py` & `vents-0.0.5/vents/providers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/gcp/base.py` & `vents-0.0.5/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/gcp/gcs.py` & `vents-0.0.5/vents/providers/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/gcp/service.py` & `vents-0.0.5/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents/providers/kinds.py` & `vents-0.0.5/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.4/vents.egg-info/PKG-INFO` & `vents-0.0.5/vents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.0.4
+Version: 0.0.5
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.0.4/vents.egg-info/SOURCES.txt` & `vents-0.0.5/vents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

