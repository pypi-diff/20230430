# Comparing `tmp/pynukibt-0.0.2.tar.gz` & `tmp/pynukibt-0.0.3.tar.gz`

## Comparing `pynukibt-0.0.2.tar` & `pynukibt-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pynukibt-0.0.2/requirements.txt
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pynukibt-0.0.2/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynukibt-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pynukibt-0.0.2/pyNukiBT/__init__.py
--rw-r--r--   0        0        0    38869 2020-02-02 00:00:00.000000 pynukibt-0.0.2/pyNukiBT/const.py
--rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 pynukibt-0.0.2/pyNukiBT/nuki.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pynukibt-0.0.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pynukibt-0.0.2/LICENSE
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pynukibt-0.0.2/README.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pynukibt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 pynukibt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pynukibt-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynukibt-0.0.3/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynukibt-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pynukibt-0.0.3/pyNukiBT/__init__.py
+-rw-r--r--   0        0        0    39005 2020-02-02 00:00:00.000000 pynukibt-0.0.3/pyNukiBT/const.py
+-rw-r--r--   0        0        0    24671 2020-02-02 00:00:00.000000 pynukibt-0.0.3/pyNukiBT/nuki.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pynukibt-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pynukibt-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pynukibt-0.0.3/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pynukibt-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 pynukibt-0.0.3/PKG-INFO
```

### Comparing `pynukibt-0.0.2/setup.py` & `pynukibt-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyNukiBT",
-    version="0.0.1",
+    version="0.0.3",
     author="Ronen Gruengras",
     author_email="ronengr@gmail.com",
     description="Nuki Bluetooth API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ronengr/pyNukiBT",
     packages=find_packages(),
     install_requires=[
         "bleak>=0.20",
-        "fastcrc>=0.2.1",
+        "crccheck>=1.3.0",
         "PyNaCl>=1.3.0",
         "construct>=2.10.68",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `pynukibt-0.0.2/.github/workflows/python-publish.yml` & `pynukibt-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.2/pyNukiBT/const.py` & `pynukibt-0.0.3/pyNukiBT/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import construct
 from construct import Bit, BitStruct, Optional, Padding, Struct, Byte, Enum, Int8ul, Int16ul, Int32ul, Int8sl, Int16sl, Float32l, PaddedString, Bytes, Switch, this
 import functools
-from fastcrc import crc16
+import crccheck
+
+crcCalc = crccheck.crc.Crc(width=16, poly=0x1021, initvalue=0xffff, reflect_input=False, reflect_output=False, xor_output=0x0, check_result=0x31c3, residue=0x0)
 
 class NukiConst:
     ErrorCode = Enum(Int8ul,
         #General error codes
         ERROR_BAD_CRC = 0xFD, #CRC of received command is invalid
         ERROR_BAD_LENGTH = 0xFE, #Length of retrieved command payload does not match expected length
         ERROR_UNKNOWN = 0xFF, #Used if no other error code matche
@@ -547,25 +549,25 @@
     @functools.cached_property
     def NukiMessage(self):
         return Struct(
             "auth_id" / Bytes(4),
             "command" / self.NukiCommand,
             "payload" / Switch(this.command, self.message_types),
             "crc" / NukiChecksum(Int16ul,
-                             lambda data: crc16.xmodem(data, 0xFFFF),
+                             lambda data: crcCalc.calc(data),
                              lambda x: x._io.getvalue()[:x._io.tell()])
         )
 
     @functools.cached_property
     def NukiUnencryptedMessage(self):
         return Struct(
             "command" / self.NukiCommand,
             "payload" / Switch(this.command, self.message_types),
             "crc" / NukiChecksum(Int16ul,
-                             lambda data: crc16.xmodem(data, 0xFFFF),
+                             lambda data: crcCalc.calc(data),
                              lambda x: x._io.getvalue()[:x._io.tell()])
         )
 
     @functools.cached_property
     def NukiMessage2(self):
         return Struct(
             "auth_id" / Bytes(4),
```

### Comparing `pynukibt-0.0.2/pyNukiBT/nuki.py` & `pynukibt-0.0.3/pyNukiBT/nuki.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 from bleak.backends.scanner import AdvertisementData
 from bleak.backends.characteristic import BleakGATTCharacteristic
 
 import async_timeout
 
 # from bleak_retry_connector import BLEAK_RETRY_EXCEPTIONS
 
-from fastcrc import crc16
 import nacl.utils
 import nacl.secret
 from nacl.bindings.crypto_box import crypto_box_beforenm
 from bleak import BleakClient, BleakError
 from bleak.exc import BleakDBusError
 
-from .const import NukiErrorException, NukiLockConst, NukiOpenerConst, NukiConst
+from .const import NukiErrorException, NukiLockConst, NukiOpenerConst, NukiConst, crcCalc
 
 logger = logging.getLogger(__name__)
 
 class NukiDevice:
     def __init__(
         self,
         address,
@@ -158,15 +157,15 @@
 
     def get_config(self):
         return self.config
 
     @staticmethod
     def _prepare_command(cmd: NukiConst.NukiCommand, payload=bytes()):
         message = NukiConst.NukiCommand.build(cmd) + payload
-        crc = crc16.xmodem(message, 0xFFFF).to_bytes(2, "little")
+        crc = crcCalc.calc(message).to_bytes(2, "little")
         message += crc
         return message
 
     async def _send_encrtypted_command(
         self,
         cmd: NukiConst.NukiCommand,
         payload: dict,
```

### Comparing `pynukibt-0.0.2/.gitignore` & `pynukibt-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.2/LICENSE` & `pynukibt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.2/README.md` & `pynukibt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.2/pyproject.toml` & `pynukibt-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyNukiBT"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ronen Gruengras", email="ronengr@gmail.com" },
 ]
 description = "Nuki Bluetooth API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "bleak>=0.20",
-    "fastcrc>=0.2.1",
+    "crccheck>=1.3.0",
     "PyNaCl>=1.3.0",
     "construct>=2.10.68",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ronengr/pyNukiBT"
 "Bug Tracker" = "https://github.com/ronengr/pyNukiBT/issues"
```

### Comparing `pynukibt-0.0.2/PKG-INFO` & `pynukibt-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyNukiBT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Nuki Bluetooth API
 Project-URL: Homepage, https://github.com/ronengr/pyNukiBT
 Project-URL: Bug Tracker, https://github.com/ronengr/pyNukiBT/issues
 Author-email: Ronen Gruengras <ronengr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: bleak>=0.20
 Requires-Dist: construct>=2.10.68
-Requires-Dist: fastcrc>=0.2.1
+Requires-Dist: crccheck>=1.3.0
 Requires-Dist: pynacl>=1.3.0
 Description-Content-Type: text/markdown
 
 # pyNukiBT
 Nuki Bluetooth API
 
 This is only a python API implementation of the Bluetooth communication with Nuki lock.
```

