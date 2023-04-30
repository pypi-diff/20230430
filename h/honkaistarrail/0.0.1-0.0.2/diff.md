# Comparing `tmp/honkaistarrail-0.0.1.tar.gz` & `tmp/honkaistarrail-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honkaistarrail-0.0.1.tar", max compression
+gzip compressed data, was "honkaistarrail-0.0.2.tar", max compression
```

## Comparing `honkaistarrail-0.0.1.tar` & `honkaistarrail-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.1/honkaistarrail/calculator.py
--rw-r--r--   0        0        0     1246 2023-04-30 01:48:24.518000 honkaistarrail-0.0.1/honkaistarrail/modal.py
--rw-r--r--   0        0        0     4612 2023-04-30 02:10:08.645612 honkaistarrail-0.0.1/honkaistarrail/starrail.py
--rw-r--r--   0        0        0      480 2023-04-30 02:50:08.383217 honkaistarrail-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-04-30 02:44:15.431196 honkaistarrail-0.0.1/README.md
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 honkaistarrail-0.0.1/setup.py
--rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 honkaistarrail-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.2/honkaistarrail/calculator.py
+-rw-r--r--   0        0        0     1246 2023-04-30 01:48:24.518000 honkaistarrail-0.0.2/honkaistarrail/modal.py
+-rw-r--r--   0        0        0     4612 2023-04-30 02:10:08.645612 honkaistarrail-0.0.2/honkaistarrail/starrail.py
+-rw-r--r--   0        0        0      480 2023-04-30 02:50:31.766312 honkaistarrail-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1080 2023-04-30 02:50:22.110995 honkaistarrail-0.0.2/README.md
+-rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 honkaistarrail-0.0.2/setup.py
+-rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 honkaistarrail-0.0.2/PKG-INFO
```

### Comparing `honkaistarrail-0.0.1/honkaistarrail/calculator.py` & `honkaistarrail-0.0.2/honkaistarrail/calculator.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.1/honkaistarrail/modal.py` & `honkaistarrail-0.0.2/honkaistarrail/modal.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.1/honkaistarrail/starrail.py` & `honkaistarrail-0.0.2/honkaistarrail/starrail.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.1/README.md` & `honkaistarrail-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# StarRail.py
+# HonkaiStarRail.py
 
 # Asynchronous module for working with API Honkai: Star Rail
 
 At the moment it only supports counting guarantors and getting a jumps 
 
 ### Installation: 
 ```
-pip install starrail
+pip install honkaistarrail
 ```
 
 ### Launc:
 
 ```py
 # Copyright 2023 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
@@ -18,15 +18,15 @@
 '''
 This method returns the full history of jumps for the 
 last 3 months, does not return the results of jumps 
 and how much is left before the guarantor.
 '''
 
 import asyncio
-from starrail import starrail
+from honkaistarrail import starrail
 
 async def get_jump_history():
     link = ""
     async with starrail.Jump(link,3,"en") as hist:
         async for key in hist.get_history():
             for info in key:
                 print(f'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}')
```

### Comparing `honkaistarrail-0.0.1/setup.py` & `honkaistarrail-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['honkaistarrail']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'honkaistarrail',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Asynchronous module for working with API Honkai: Star Rail',
-    'long_description': '# StarRail.py\n\n# Asynchronous module for working with API Honkai: Star Rail\n\nAt the moment it only supports counting guarantors and getting a jumps \n\n### Installation: \n```\npip install starrail\n```\n\n### Launc:\n\n```py\n# Copyright 2023 DEViantUa <t.me/deviant_ua>\n# All rights reserved.\n\n\'\'\'\nThis method returns the full history of jumps for the \nlast 3 months, does not return the results of jumps \nand how much is left before the guarantor.\n\'\'\'\n\nimport asyncio\nfrom starrail import starrail\n\nasync def get_jump_history():\n    link = ""\n    async with starrail.Jump(link,3,"en") as hist:\n        async for key in hist.get_history():\n            for info in key:\n                print(f\'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}\')\n\n\nasyncio.run(get_jump_history())\n```\n\nYou can also see other usage examples here: [OPEN](https://github.com/DEViantUA/starrail.py/tree/main/Examples)\n\nInstructions for getting a link to the history of jumps: [OPEN](https://github.com/DEViantUA/starrail.py/blob/main/Instruction.md)\n\n',
+    'long_description': '# HonkaiStarRail.py\n\n# Asynchronous module for working with API Honkai: Star Rail\n\nAt the moment it only supports counting guarantors and getting a jumps \n\n### Installation: \n```\npip install honkaistarrail\n```\n\n### Launc:\n\n```py\n# Copyright 2023 DEViantUa <t.me/deviant_ua>\n# All rights reserved.\n\n\'\'\'\nThis method returns the full history of jumps for the \nlast 3 months, does not return the results of jumps \nand how much is left before the guarantor.\n\'\'\'\n\nimport asyncio\nfrom honkaistarrail import starrail\n\nasync def get_jump_history():\n    link = ""\n    async with starrail.Jump(link,3,"en") as hist:\n        async for key in hist.get_history():\n            for info in key:\n                print(f\'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}\')\n\n\nasyncio.run(get_jump_history())\n```\n\nYou can also see other usage examples here: [OPEN](https://github.com/DEViantUA/starrail.py/tree/main/Examples)\n\nInstructions for getting a link to the history of jumps: [OPEN](https://github.com/DEViantUA/starrail.py/blob/main/Instruction.md)\n\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/HonkaiStarRail.py',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `honkaistarrail-0.0.1/PKG-INFO` & `honkaistarrail-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: honkaistarrail
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous module for working with API Honkai: Star Rail
 Home-page: https://github.com/DEViantUA/HonkaiStarRail.py
 Author: None
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/DEViantUA/HonkaiStarRail.py
 Description-Content-Type: text/markdown
 
-# StarRail.py
+# HonkaiStarRail.py
 
 # Asynchronous module for working with API Honkai: Star Rail
 
 At the moment it only supports counting guarantors and getting a jumps 
 
 ### Installation: 
 ```
-pip install starrail
+pip install honkaistarrail
 ```
 
 ### Launc:
 
 ```py
 # Copyright 2023 DEViantUa <t.me/deviant_ua>
 # All rights reserved.
@@ -34,15 +34,15 @@
 '''
 This method returns the full history of jumps for the 
 last 3 months, does not return the results of jumps 
 and how much is left before the guarantor.
 '''
 
 import asyncio
-from starrail import starrail
+from honkaistarrail import starrail
 
 async def get_jump_history():
     link = ""
     async with starrail.Jump(link,3,"en") as hist:
         async for key in hist.get_history():
             for info in key:
                 print(f'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}')
```

