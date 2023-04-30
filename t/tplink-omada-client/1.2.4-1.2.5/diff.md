# Comparing `tmp/tplink_omada_client-1.2.4.tar.gz` & `tmp/tplink_omada_client-1.2.5.tar.gz`

## Comparing `tplink_omada_client-1.2.4.tar` & `tplink_omada_client-1.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.pylintrc
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/Dockerfile.dev
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/requirements.txt
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/requirements_test.txt
--rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/sample_client.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.vscode/launch.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/__init__.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/definitions.py
--rw-r--r--   0        0        0    18473 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/devices.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/exceptions.py
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/omadaapiconnection.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/omadaclient.py
--rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/omadasiteclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/py.typed
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/__main__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_default.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_devices.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_gateway.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_switch.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_switches.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_target.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_targets.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/config.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/src/tplink_omada_client/cli/util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/README.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.pylintrc
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/Dockerfile.dev
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/requirements.txt
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/requirements_test.txt
+-rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/sample_client.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.vscode/launch.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/__init__.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/definitions.py
+-rw-r--r--   0        0        0    19064 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/devices.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/exceptions.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/omadaapiconnection.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/omadaclient.py
+-rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/omadasiteclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/py.typed
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/__main__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_default.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_devices.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_gateway.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_switch.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_switches.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_target.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_targets.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/config.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/src/tplink_omada_client/cli/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/tests/conftest.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.5/PKG-INFO
```

### Comparing `tplink_omada_client-1.2.4/Dockerfile.dev` & `tplink_omada_client-1.2.5/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/sample_client.py` & `tplink_omada_client-1.2.5/sample_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/.devcontainer/devcontainer.json` & `tplink_omada_client-1.2.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/.github/workflows/python-package.yml` & `tplink_omada_client-1.2.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/.github/workflows/python-publish.yml` & `tplink_omada_client-1.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/.vscode/launch.json` & `tplink_omada_client-1.2.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/definitions.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,16 @@
     DISABLED = -1
     WAN = 0
     LAN = 1
 
 class LinkStatus(IntEnum):
     """Known link statuses."""
 
-    LINK_UP = 0
-    LINK_DOWN = 2
+    LINK_DOWN = 0
+    LINK_UP = 1
 
 
 class LinkSpeed(IntEnum):
     """Known link speeds."""
 
     SPEED_AUTO = 0
     SPEED_10_MBPS = 1
```

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/devices.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,49 +67,67 @@
 
     @property
     def ip_address(self) -> str:
         """IP address of the device."""
         return self._data["ip"]
 
     @property
-    def display_uptime(self) -> str:
+    def display_uptime(self) -> Optional[str]:
         """Uptime of the device, as a display string"""
-        return self._data["uptime"]
+        if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
+            return self._data["uptime"]
+        else:
+            return None
 
     @property
     def cpu_usage(self) -> int:
-        return self._data["cpuUtil"]
+        if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
+            return self._data["cpuUtil"]
+        else:
+            return 0
         
     @property
     def mem_usage(self) -> int:
-        return self._data["memUtil"]
+        if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
+            return self._data["memUtil"]
+        else:
+            return 0
 
     @property
     def uptime(self) -> int:
         """Uptime of the device, as a display string"""
-        return self._data["uptimeLong"]
+        if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
+            return self._data["uptimeLong"]
+        else:
+            return 0
 
     @property
     def firmware_version(self) -> str:
         """Firmware version of the device"""
         return self._data["firmwareVersion"]
 
 
 class OmadaListDevice(OmadaDevice):
     """An Omada Device (router, switch, eap) as represented in the device list"""
 
     @property
     def need_upgrade(self) -> bool:
         """True, if a firmware upgrade is available for the device."""
-        return self._data["needUpgrade"]
+        if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
+            return self._data["needUpgrade"]
+        else:
+            return False
 
     @property
     def fw_download(self) -> bool:
         """True, if a firmware upgrade is being downloaded."""
-        return self._data["fwDownload"]
+        if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
+            return self._data["fwDownload"]
+        else:
+            return False
 
 
 class OmadaLink(OmadaApiData):
     """Up/Downlink connection from a switch/ap device."""
 
     @property
     def mac(self) -> str:
@@ -557,16 +575,15 @@
     def mode(self) -> GatewayPortMode:
         """Whether the port is operating in WAN or LAN mode"""
         return GatewayPortMode(self._data["mode"])
 
     @property
     def link_status(self) -> LinkStatus:
         """Low level connectivity status of the link."""
-        # Defined differently to switches, so mangle the values to match
-        return LinkStatus.LINK_UP if self._data["status"] == 1 else LinkStatus.LINK_DOWN
+        return LinkStatus(self._data["status"])
 
     @property
     def wan_connected(self) -> bool:
         """True if the port is connected to the internet/WAN"""
         return self._data.get("internetState", 0) != 0
 
     @property
```

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/exceptions.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/omadaapiconnection.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/omadaapiconnection.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/omadaclient.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/omadaclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/omadasiteclient.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/omadasiteclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/__init__.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_default.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_default.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_devices.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_devices.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_gateway.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_gateway.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_switch.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_switch.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_switches.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_switches.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_target.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_target.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/command_targets.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/command_targets.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/config.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/src/tplink_omada_client/cli/util.py` & `tplink_omada_client-1.2.5/src/tplink_omada_client/cli/util.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/LICENSE` & `tplink_omada_client-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/README.md` & `tplink_omada_client-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.4/pyproject.toml` & `tplink_omada_client-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tplink_omada_client"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
   { name="Mark Godwin", email="author@example.com" },
 ]
 description = "Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `tplink_omada_client-1.2.4/PKG-INFO` & `tplink_omada_client-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplink_omada_client
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)
 Project-URL: Homepage, https://github.com/MarkGodwin/tplink-omada-api
 Project-URL: Bug Tracker, https://github.com/MarkGodwin/tplink-omada-api/issues
 Author-email: Mark Godwin <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

