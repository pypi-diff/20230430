# Comparing `tmp/sigmadsp-3.0.1.tar.gz` & `tmp/sigmadsp-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmadsp-3.0.1.tar", max compression
+gzip compressed data, was "sigmadsp-3.0.2.tar", max compression
```

## Comparing `sigmadsp-3.0.1.tar` & `sigmadsp-3.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/LICENSE
--rw-r--r--   0        0        0     3615 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/README.md
--rw-r--r--   0        0        0     1198 2023-03-06 23:08:33.572149 sigmadsp-3.0.1/pyproject.toml
--rw-r--r--   0        0        0       99 2023-03-06 23:08:33.572149 sigmadsp-3.0.1/sigmadsp/__init__.py
--rw-r--r--   0        0        0    14651 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/sigmadsp/backend.py
--rw-r--r--   0        0        0       92 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/sigmadsp/dsp/__init__.py
--rw-r--r--   0        0        0     3108 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/sigmadsp/dsp/adau14xx.py
--rw-r--r--   0        0        0     3006 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/sigmadsp/dsp/adau1x01.py
--rw-r--r--   0        0        0     9870 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/sigmadsp/dsp/common.py
--rw-r--r--   0        0        0     3297 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/sigmadsp/dsp/factory.py
--rw-r--r--   0        0        0     5268 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/sigmadsp/frontend.py
--rw-r--r--   0        0        0       53 2023-03-06 23:08:11.548360 sigmadsp-3.0.1/sigmadsp/generated/__init__.py
--rw-r--r--   0        0        0      223 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/generated/backend_service/__init__.py
--rw-r--r--   0        0        0     4802 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/generated/backend_service/control_pb2.py
--rw-r--r--   0        0        0     5651 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/generated/backend_service/control_pb2.pyi
--rw-r--r--   0        0        0     4033 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/generated/backend_service/control_pb2_grpc.py
--rw-r--r--   0        0        0       86 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/helper/__init__.py
--rw-r--r--   0        0        0     7352 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/helper/conversion.py
--rw-r--r--   0        0        0     9510 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/helper/parser.py
--rw-r--r--   0        0        0     2226 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/helper/settings.py
--rw-r--r--   0        0        0       78 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/protocols/__init__.py
--rw-r--r--   0        0        0     2981 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/protocols/common.py
--rw-r--r--   0        0        0     1855 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/protocols/i2c.py
--rw-r--r--   0        0        0     4404 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/protocols/spi.py
--rw-r--r--   0        0        0       64 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/sigmastudio/__init__.py
--rw-r--r--   0        0        0     1722 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/sigmastudio/adau14xx.py
--rw-r--r--   0        0        0     1505 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/sigmastudio/adau1x01.py
--rw-r--r--   0        0        0      695 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/sigmastudio/common.py
--rw-r--r--   0        0        0    11449 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/sigmastudio/header.py
--rw-r--r--   0        0        0     8600 2023-03-06 23:08:11.552360 sigmadsp-3.0.1/sigmadsp/sigmastudio/server.py
--rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 sigmadsp-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/LICENSE
+-rw-r--r--   0        0        0     3615 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/README.md
+-rw-r--r--   0        0        0     1198 2023-04-30 06:28:27.613323 sigmadsp-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-04-30 06:28:27.613323 sigmadsp-3.0.2/sigmadsp/__init__.py
+-rw-r--r--   0        0        0    14651 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/backend.py
+-rw-r--r--   0        0        0       92 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/__init__.py
+-rw-r--r--   0        0        0     3108 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/adau14xx.py
+-rw-r--r--   0        0        0     3006 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/adau1x01.py
+-rw-r--r--   0        0        0     9870 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/common.py
+-rw-r--r--   0        0        0     3297 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/factory.py
+-rw-r--r--   0        0        0     5268 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/frontend.py
+-rw-r--r--   0        0        0       53 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/backend_service/__init__.py
+-rw-r--r--   0        0        0     4802 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2.py
+-rw-r--r--   0        0        0     5651 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2.pyi
+-rw-r--r--   0        0        0     4033 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2_grpc.py
+-rw-r--r--   0        0        0       86 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/helper/__init__.py
+-rw-r--r--   0        0        0     7388 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/helper/conversion.py
+-rw-r--r--   0        0        0     9510 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/helper/parser.py
+-rw-r--r--   0        0        0     2262 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/helper/settings.py
+-rw-r--r--   0        0        0       78 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/protocols/__init__.py
+-rw-r--r--   0        0        0     2981 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/protocols/common.py
+-rw-r--r--   0        0        0     1855 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/protocols/i2c.py
+-rw-r--r--   0        0        0     4404 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/protocols/spi.py
+-rw-r--r--   0        0        0       64 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/__init__.py
+-rw-r--r--   0        0        0     1722 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/adau14xx.py
+-rw-r--r--   0        0        0     1505 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/adau1x01.py
+-rw-r--r--   0        0        0      695 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/common.py
+-rw-r--r--   0        0        0    11449 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/header.py
+-rw-r--r--   0        0        0     8600 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/server.py
+-rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 sigmadsp-3.0.2/PKG-INFO
```

### Comparing `sigmadsp-3.0.1/LICENSE` & `sigmadsp-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/README.md` & `sigmadsp-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/pyproject.toml` & `sigmadsp-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sigmadsp"
 license = "GPL-3.0-or-later"
-version = "3.0.1"
+version = "3.0.2"
 description = "A package for controlling Analog Devices Sigma DSP chipsets."
 readme = "README.md"
 authors = ["Adrian Figueroa <elagil@takanome.de>"]
 repository = "https://github.com/elagil/sigmadsp"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -13,15 +13,15 @@
 ]
 
 [tool.poetry.scripts]
 sigmadsp-backend = "sigmadsp.backend:main"
 sigmadsp = "sigmadsp.frontend:sigmadsp"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.9"
 PyYAML = "^6.0"
 spidev = "^3.5"
 retry = "^0.9.2"
 smbus2 = "^0.4.1"
 gpiozero = "^1.6.2"
 protobuf = "^3.20.3"
 click = "^8.1.3"
```

### Comparing `sigmadsp-3.0.1/sigmadsp/backend.py` & `sigmadsp-3.0.2/sigmadsp/backend.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/dsp/adau14xx.py` & `sigmadsp-3.0.2/sigmadsp/dsp/adau14xx.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/dsp/adau1x01.py` & `sigmadsp-3.0.2/sigmadsp/dsp/adau1x01.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/dsp/common.py` & `sigmadsp-3.0.2/sigmadsp/dsp/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/dsp/factory.py` & `sigmadsp-3.0.2/sigmadsp/dsp/factory.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/frontend.py` & `sigmadsp-3.0.2/sigmadsp/frontend.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/generated/backend_service/control_pb2.py` & `sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/generated/backend_service/control_pb2.pyi` & `sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/generated/backend_service/control_pb2_grpc.py` & `sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/helper/conversion.py` & `sigmadsp-3.0.2/sigmadsp/helper/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """This module includes many conversion functions that can be used for different purposes.
 
 - Conversion between linear and dB-scale values
 - Conversion from bytes-like objects of varying length to integers
 - Conversion from integers to bytes-like objects of specified length
 """
+from __future__ import annotations
+
 import math
 from typing import Literal
 from typing import Union
 
 BIT_LENGTH_8_24 = 31
 BIT_LENGTH_5_23 = 27
 SIGMADSP_ENDIANNESS: Literal["big", "little"] = "big"
```

### Comparing `sigmadsp-3.0.1/sigmadsp/helper/parser.py` & `sigmadsp-3.0.2/sigmadsp/helper/parser.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/helper/settings.py` & `sigmadsp-3.0.2/sigmadsp/helper/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """This module contains a class that handles settings for this application."""
+from __future__ import annotations
+
 import logging
 from typing import List
 from typing import Union
 
 import yaml
 
 from sigmadsp.helper.parser import Parser
```

### Comparing `sigmadsp-3.0.1/sigmadsp/protocols/common.py` & `sigmadsp-3.0.2/sigmadsp/protocols/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/protocols/i2c.py` & `sigmadsp-3.0.2/sigmadsp/protocols/i2c.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/protocols/spi.py` & `sigmadsp-3.0.2/sigmadsp/protocols/spi.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/sigmastudio/adau14xx.py` & `sigmadsp-3.0.2/sigmadsp/sigmastudio/adau14xx.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/sigmastudio/adau1x01.py` & `sigmadsp-3.0.2/sigmadsp/sigmastudio/adau1x01.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/sigmastudio/common.py` & `sigmadsp-3.0.2/sigmadsp/sigmastudio/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/sigmastudio/header.py` & `sigmadsp-3.0.2/sigmadsp/sigmastudio/header.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/sigmadsp/sigmastudio/server.py` & `sigmadsp-3.0.2/sigmadsp/sigmastudio/server.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.1/PKG-INFO` & `sigmadsp-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: sigmadsp
-Version: 3.0.1
+Version: 3.0.2
 Summary: A package for controlling Analog Devices Sigma DSP chipsets.
 Home-page: https://github.com/elagil/sigmadsp
 License: GPL-3.0-or-later
 Author: Adrian Figueroa
 Author-email: elagil@takanome.de
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: gpiozero (>=1.6.2,<2.0.0)
```

