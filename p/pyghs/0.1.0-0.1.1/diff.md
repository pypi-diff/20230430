# Comparing `tmp/pyghs-0.1.0.tar.gz` & `tmp/pyghs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghs-0.1.0.tar", last modified: Sat Apr 29 07:28:29 2023, max compression
+gzip compressed data, was "pyghs-0.1.1.tar", last modified: Sun Apr 30 04:07:09 2023, max compression
```

## Comparing `pyghs-0.1.0.tar` & `pyghs-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-29 07:28:29.049757 pyghs-0.1.0/
--rw-r--r--   0 chaoying   (501) staff       (20)      182 2023-04-29 07:28:29.049630 pyghs-0.1.0/PKG-INFO
--rw-r--r--   0 chaoying   (501) staff       (20)      561 2023-04-29 07:24:47.000000 pyghs-0.1.0/README.md
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-29 07:28:29.048308 pyghs-0.1.0/ghs/
--rw-r--r--   0 chaoying   (501) staff       (20)       46 2023-04-29 07:13:49.000000 pyghs-0.1.0/ghs/__init__.py
--rw-r--r--   0 chaoying   (501) staff       (20)     4113 2023-04-29 07:22:21.000000 pyghs-0.1.0/ghs/storage.py
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-29 07:28:29.049193 pyghs-0.1.0/pyghs.egg-info/
--rw-r--r--   0 chaoying   (501) staff       (20)      182 2023-04-29 07:28:29.000000 pyghs-0.1.0/pyghs.egg-info/PKG-INFO
--rw-r--r--   0 chaoying   (501) staff       (20)      221 2023-04-29 07:28:29.000000 pyghs-0.1.0/pyghs.egg-info/SOURCES.txt
--rw-r--r--   0 chaoying   (501) staff       (20)        1 2023-04-29 07:28:29.000000 pyghs-0.1.0/pyghs.egg-info/dependency_links.txt
--rw-r--r--   0 chaoying   (501) staff       (20)       29 2023-04-29 07:28:29.000000 pyghs-0.1.0/pyghs.egg-info/requires.txt
--rw-r--r--   0 chaoying   (501) staff       (20)        4 2023-04-29 07:28:29.000000 pyghs-0.1.0/pyghs.egg-info/top_level.txt
--rw-r--r--   0 chaoying   (501) staff       (20)      501 2023-04-29 07:28:21.000000 pyghs-0.1.0/pyproject.toml
--rw-r--r--   0 chaoying   (501) staff       (20)       38 2023-04-29 07:28:29.049794 pyghs-0.1.0/setup.cfg
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-29 07:28:29.049351 pyghs-0.1.0/tests/
--rw-r--r--   0 chaoying   (501) staff       (20)      830 2023-04-29 07:21:05.000000 pyghs-0.1.0/tests/test_storage.py
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-30 04:07:09.994519 pyghs-0.1.1/
+-rw-r--r--   0 chaoying   (501) staff       (20)      182 2023-04-30 04:07:09.994391 pyghs-0.1.1/PKG-INFO
+-rw-r--r--   0 chaoying   (501) staff       (20)      564 2023-04-29 07:30:53.000000 pyghs-0.1.1/README.md
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-30 04:07:09.993350 pyghs-0.1.1/ghs/
+-rw-r--r--   0 chaoying   (501) staff       (20)       46 2023-04-29 07:13:49.000000 pyghs-0.1.1/ghs/__init__.py
+-rw-r--r--   0 chaoying   (501) staff       (20)     4055 2023-04-30 04:06:28.000000 pyghs-0.1.1/ghs/storage.py
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-30 04:07:09.994040 pyghs-0.1.1/pyghs.egg-info/
+-rw-r--r--   0 chaoying   (501) staff       (20)      182 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/PKG-INFO
+-rw-r--r--   0 chaoying   (501) staff       (20)      221 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/SOURCES.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)        1 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/dependency_links.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)       29 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/requires.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)        4 2023-04-30 04:07:09.000000 pyghs-0.1.1/pyghs.egg-info/top_level.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)      501 2023-04-30 04:00:33.000000 pyghs-0.1.1/pyproject.toml
+-rw-r--r--   0 chaoying   (501) staff       (20)       38 2023-04-30 04:07:09.994557 pyghs-0.1.1/setup.cfg
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-04-30 04:07:09.994154 pyghs-0.1.1/tests/
+-rw-r--r--   0 chaoying   (501) staff       (20)      830 2023-04-30 03:59:02.000000 pyghs-0.1.1/tests/test_storage.py
```

### Comparing `pyghs-0.1.0/README.md` & `pyghs-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GHS
 
 Storage csv file in github repository.
 
 ## Installation
 
 ```bash
-pip install ghs
+pip install pyghs
 ```
 
 ## Usage
 
 ```python
 from ghs import GHS
 import pandas as pd
@@ -32,8 +32,8 @@
 This prints:
 
 ```bash
    a  b
 0  1  4
 1  2  5
 2  3  6
-```
+```
```

### Comparing `pyghs-0.1.0/ghs/storage.py` & `pyghs-0.1.1/ghs/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,17 @@
         access_token: str,
         repository: str,
     ) -> None:
         self.repository = repository
         self._session = self._get_session(access_token)
 
     async def create(self, path: str, df: pd.DataFrame) -> None:
-        csv = df.to_csv(index=False)
         payload = {
             "message": "Create",
-            "content": base64.b64encode(csv.encode()).decode(),
+            "content": base64.b64encode(df.to_csv().encode()).decode(),
         }
         async with self._session.put(
             f"/repos/{self.repository}/contents/{path}", data=json.dumps(payload)
         ) as r:
             try:
                 r.raise_for_status()
             except aiohttp.ClientResponseError as e:
@@ -44,19 +43,18 @@
         try:
             sha = await self.get_sha(path)
         except FileNotFoundError:
             if upsert:
                 await self.create(path, df)
                 return
             raise
-        csv = df.to_csv(index=False)
         payload = {
             "message": "Update",
             "sha": sha,
-            "content": base64.b64encode(csv.encode()).decode(),
+            "content": base64.b64encode(df.to_csv().encode()).decode(),
         }
         async with self._session.put(
             f"/repos/{self.repository}/contents/{path}", data=json.dumps(payload)
         ) as r:
             try:
                 r.raise_for_status()
             except aiohttp.ClientResponseError as e:
```

### Comparing `pyghs-0.1.0/tests/test_storage.py` & `pyghs-0.1.1/tests/test_storage.py`

 * *Files identical despite different names*

