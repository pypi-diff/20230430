# Comparing `tmp/iothealth-0.0.4.tar.gz` & `tmp/iothealth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iothealth-0.0.4.tar", last modified: Sat May 15 06:35:38 2021, max compression
+gzip compressed data, was "iothealth-0.0.5.tar", last modified: Sun Apr 30 06:18:23 2023, max compression
```

## Comparing `iothealth-0.0.4.tar` & `iothealth-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2021-05-15 06:35:38.000000 iothealth-0.0.4/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     3507 2021-05-15 06:35:38.000000 iothealth-0.0.4/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2345 2021-05-15 05:53:24.000000 iothealth-0.0.4/README.rst
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2020-12-14 07:17:46.000000 iothealth-0.0.4/iothealth/__init__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      162 2020-12-14 07:17:46.000000 iothealth-0.0.4/iothealth/__main__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1950 2021-05-15 05:30:55.000000 iothealth-0.0.4/iothealth/_base_health.py
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth/bin/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2020-12-14 07:17:46.000000 iothealth-0.0.4/iothealth/bin/__init__.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1706 2020-12-14 07:17:46.000000 iothealth-0.0.4/iothealth/bin/cli.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2551 2021-05-15 05:30:55.000000 iothealth-0.0.4/iothealth/device_health.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     5145 2021-05-15 05:30:55.000000 iothealth-0.0.4/iothealth/linux.py
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1722 2021-05-15 05:30:55.000000 iothealth-0.0.4/iothealth/raspberry_pi.py
-drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth.egg-info/
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     3507 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth.egg-info/PKG-INFO
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      408 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth.egg-info/SOURCES.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth.egg-info/dependency_links.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       59 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth.egg-info/entry_points.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       13 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth.egg-info/requires.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       10 2021-05-15 06:35:38.000000 iothealth-0.0.4/iothealth.egg-info/top_level.txt
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2021-05-15 06:35:38.000000 iothealth-0.0.4/setup.cfg
--rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1053 2021-05-15 06:09:30.000000 iothealth-0.0.4/setup.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1070 2023-01-03 00:32:11.000000 iothealth-0.0.5/LICENSE
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2752 2023-04-30 06:18:23.071322 iothealth-0.0.5/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2345 2023-01-03 00:32:11.000000 iothealth-0.0.5/README.rst
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.061322 iothealth-0.0.5/docs/
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/docs/source/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1990 2023-01-03 00:32:11.000000 iothealth-0.0.5/docs/source/conf.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/iothealth/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/__init__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      162 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/__main__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1925 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/_base_health.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/iothealth/bin/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/bin/__init__.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1706 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/bin/cli.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2545 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/device_health.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     5120 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/linux.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     1697 2023-01-03 00:32:11.000000 iothealth-0.0.5/iothealth/raspberry_pi.py
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/iothealth.egg-info/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)     2752 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/PKG-INFO
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      490 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)        1 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       58 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/entry_points.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       13 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/requires.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       26 2023-04-30 06:18:23.000000 iothealth-0.0.5/iothealth.egg-info/top_level.txt
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      633 2023-04-30 06:17:46.000000 iothealth-0.0.5/pyproject.toml
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)       38 2023-04-30 06:18:23.071322 iothealth-0.0.5/setup.cfg
+drwxr-xr-x   0 shunsvineyard  (1000) shunsvineyard  (1000)        0 2023-04-30 06:18:23.071322 iothealth-0.0.5/tests/
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      162 2023-01-03 00:32:11.000000 iothealth-0.0.5/tests/test_device_health.py
+-rw-r--r--   0 shunsvineyard  (1000) shunsvineyard  (1000)      131 2023-01-03 00:32:11.000000 iothealth-0.0.5/tests/test_linux.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `iothealth-0.0.4/README.rst` & `iothealth-0.0.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     :target: https://github.com/psf/black
 
 IoT Health is a library which provides the health information for supported IoT devices.
 
 
 Requirements
 ------------
-``Python 3.7`` or newer is required.
+``Python 3.9`` or newer is required.
 
 
 Installation
 ------------
 There are a few ways to install ``IoT Health``. 
 
 - Install the latest release from PyPI
```

### Comparing `iothealth-0.0.4/iothealth/_base_health.py` & `iothealth-0.0.5/iothealth/_base_health.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # Copyright © 2020 by IoT Spectator. All rights reserved.
 
 """Interface definition."""
 
 import abc
 
-from typing import Dict
-
 
 class BaseHealth(abc.ABC):
     """Definition for common health information."""
 
     @classmethod
-    def summary(cls) -> Dict:
+    def summary(cls) -> dict:
         """Provide the device health summary."""
         return {
             "platform": cls.device_platform(),
             "cpu_arch": cls.processor_architecture(),
             "os": cls.operating_system(),
             "processors": cls.processors(),
             "memory": cls.memory(),
@@ -40,34 +38,34 @@
     @abc.abstractmethod
     def operating_system(cls) -> str:
         """Provide the device OS info."""
         raise NotImplementedError()
 
     @classmethod
     @abc.abstractmethod
-    def processors(cls) -> Dict:
+    def processors(cls) -> dict:
         """Provice the device processors info."""
         raise NotImplementedError()
 
     @classmethod
     @abc.abstractmethod
-    def memory(cls) -> Dict:
+    def memory(cls) -> dict:
         """Provide the device memory info."""
         raise NotImplementedError()
 
     @classmethod
     @abc.abstractmethod
-    def capacity(cls) -> Dict:
+    def capacity(cls) -> dict:
         """Provide the device disk usage info."""
         raise NotImplementedError()
 
     @classmethod
     @abc.abstractmethod
-    def temperature(cls) -> Dict:
+    def temperature(cls) -> dict:
         """Provide the device temperature."""
         raise NotImplementedError()
 
     @classmethod
     @abc.abstractmethod
-    def cameras(cls) -> Dict:
+    def cameras(cls) -> dict:
         """Provide the cameras info."""
         raise NotImplementedError()
```

### Comparing `iothealth-0.0.4/iothealth/bin/cli.py` & `iothealth-0.0.5/iothealth/bin/cli.py`

 * *Files identical despite different names*

### Comparing `iothealth-0.0.4/iothealth/device_health.py` & `iothealth-0.0.5/iothealth/device_health.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright © 2020 by IoT Spectator. All rights reserved.
 
 """IoT Health."""
 
-from typing import Dict, Optional
+from typing import Optional
 
 from iothealth import _base_health
 from iothealth import linux
 from iothealth import raspberry_pi
 
 
 class DeviceHealth(_base_health.BaseHealth):
     """Generic class for a device health info."""
 
     _current_device_cache: Optional[_base_health.BaseHealth] = None
 
     # Override
     @classmethod
-    def summary(cls) -> Dict:
+    def summary(cls) -> dict:
         """Provide the health information for the current device.
 
         Returns
         -------
         `dict`
             All the available health information as a key-value dictionary.
         """
@@ -42,39 +42,39 @@
     @classmethod
     def operating_system(cls) -> str:
         """Provide the device OS info."""
         return DeviceHealth._current_device().operating_system()
 
     # Override
     @classmethod
-    def processors(cls) -> Dict:
+    def processors(cls) -> dict:
         """Provice the device processors info."""
         return DeviceHealth._current_device().processors()
 
     # Override
     @classmethod
-    def memory(cls) -> Dict:
+    def memory(cls) -> dict:
         """Provide the device memory info."""
         return DeviceHealth._current_device().memory()
 
     # Override
     @classmethod
-    def capacity(cls) -> Dict:
+    def capacity(cls) -> dict:
         """Provide the device disk usage info."""
         return DeviceHealth._current_device().capacity()
 
     # Override
     @classmethod
-    def temperature(cls) -> Dict:
+    def temperature(cls) -> dict:
         """Provide the device temperature."""
         return DeviceHealth._current_device().temperature()
 
     # Override
     @classmethod
-    def cameras(cls) -> Dict:
+    def cameras(cls) -> dict:
         """Provide the cameras info."""
         return DeviceHealth._current_device().cameras()
 
     @classmethod
     def _current_device(cls) -> _base_health.BaseHealth:
         if cls._current_device_cache is None:
             if "Raspberry Pi" in raspberry_pi.RaspberryPi().device_platform():
```

### Comparing `iothealth-0.0.4/iothealth/linux.py` & `iothealth-0.0.5/iothealth/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 import platform
 import shutil
 import subprocess
 
 import psutil
 
-from typing import Dict
-
 from iothealth import _base_health
 
 
 class Linux(_base_health.BaseHealth):
     """Health information for general Linux devices."""
 
     # Override
@@ -58,15 +56,15 @@
             An empty string is returned if the OS is unknown.
             Otherwise, return the processor type, e.g., `Linux`.
         """
         return platform.system()
 
     # Override
     @classmethod
-    def processors(cls) -> Dict:
+    def processors(cls) -> dict:
         """Get the detail processor information as JSON format.
 
         Returns
         -------
         `dict`
             The detail information is as the following format:
         .. code-block:: JSON
@@ -112,15 +110,15 @@
             "usage_per_core": usages,
             "total_usage": psutil.cpu_percent(),
         }
         return result
 
     # Override
     @classmethod
-    def memory(cls) -> Dict:
+    def memory(cls) -> dict:
         """Get virtual memory usage in bytes.
 
         Returns
         -------
         `dict`
             Usages returned as a `dictionary` with keys `total`, `available`,
             and `used`.
@@ -130,29 +128,29 @@
             "total": result.total,
             "available": result.available,
             "used": result.used,
         }
 
     # Override
     @classmethod
-    def capacity(cls) -> Dict:
+    def capacity(cls) -> dict:
         """Get the current disk capacity usage in bytes.
 
         Returns
         -------
         `dict`
             Usages returned as a `dictionary` with keys `total`, `available`,
             and `used`.
         """
         result = shutil.disk_usage("/")
         return {"total": result.total, "available": result.free, "used": result.used}
 
     # Override
     @classmethod
-    def temperature(cls) -> Dict:
+    def temperature(cls) -> dict:
         """Provide the device temperature."""
         thermal_zone_path = "/sys/devices/virtual/thermal/thermal_zone"
         zone_temps = {}
         for zone_number in range(0, 6):
             zone_dir = thermal_zone_path + str(zone_number)
             zname = subprocess.run(
                 ["cat", zone_dir + "/type"],
@@ -171,10 +169,10 @@
             zone_temps[zname.stdout.decode("utf-8").strip()] = ztemp.stdout.decode(
                 "utf-8"
             ).strip()
         return zone_temps
 
     # Override
     @classmethod
-    def cameras(cls) -> Dict:
+    def cameras(cls) -> dict:
         """Provide cameras information."""
         return {}
```

### Comparing `iothealth-0.0.4/iothealth/raspberry_pi.py` & `iothealth-0.0.5/iothealth/raspberry_pi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Copyright © 2020 by IoT Spectator. All rights reserved.
 
 """Raspberry Pi health information."""
 
 import re
 import subprocess
 
-from typing import Dict
-
 from iothealth import linux
 
 
 class RaspberryPi(linux.Linux):
     """Check Raspberry Pi health and status."""
 
     # Override
@@ -32,15 +30,15 @@
         )
         if result.stderr:
             return str()
         return result.stdout.decode("utf-8").strip()
 
     # Override
     @classmethod
-    def temperature(cls) -> Dict:
+    def temperature(cls) -> dict:
         """Get the device's temperature.
 
         Returns
         -------
         float
             The device temperature, e.g., 54.8.
             The temperature unit is Celsius.
@@ -60,10 +58,10 @@
             if temp:
                 return {"chip": temp.group(0)}
 
         return {}
 
     # Override
     @classmethod
-    def cameras(cls) -> Dict:
+    def cameras(cls) -> dict:
         """Provide the cameras info."""
         return {}
```

