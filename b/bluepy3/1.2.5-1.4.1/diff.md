# Comparing `tmp/bluepy3-1.2.5.tar.gz` & `tmp/bluepy3-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepy3-1.2.5.tar", last modified: Sun Apr 16 14:05:43 2023, max compression
+gzip compressed data, was "bluepy3-1.4.1.tar", last modified: Sun Apr 30 08:41:12 2023, max compression
```

## Comparing `bluepy3-1.2.5.tar` & `bluepy3-1.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:05:43.105247 bluepy3-1.2.5/
--rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-03-04 17:28:46.000000 bluepy3-1.2.5/LICENSE
--rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-16 14:05:43.105334 bluepy3-1.2.5/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)     3454 2023-04-10 10:16:14.000000 bluepy3-1.2.5/README.md
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:05:43.104224 bluepy3-1.2.5/bluepy3/
--rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-09 13:50:23.000000 bluepy3-1.2.5/bluepy3/Makefile
--rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-03-26 10:53:06.000000 bluepy3-1.2.5/bluepy3/__init__.py
--rwxr-xr-x   0 maurice    (501) staff       (20)     4758 2023-04-16 14:01:33.000000 bluepy3-1.2.5/bluepy3/blescan.py
--rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-03-26 11:03:50.000000 bluepy3-1.2.5/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0 maurice    (501) staff       (20)    37227 2023-04-16 14:04:38.000000 bluepy3-1.2.5/bluepy3/btle.py
--rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-03-26 10:58:24.000000 bluepy3-1.2.5/bluepy3/config.5.47.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.5/bluepy3/config.5.50.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.5/bluepy3/config.5.60.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.5/bluepy3/config.5.66.h
--rwxr-xr-x   0 maurice    (501) staff       (20)     9750 2023-04-16 13:52:52.000000 bluepy3-1.2.5/bluepy3/get_services.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-03-26 10:53:06.000000 bluepy3-1.2.5/bluepy3/scan_fuzz.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-03-26 10:53:06.000000 bluepy3-1.2.5/bluepy3/scanner.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-04-16 13:52:52.000000 bluepy3-1.2.5/bluepy3/sensortag.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-04-16 13:52:53.000000 bluepy3-1.2.5/bluepy3/thingy52.py
--rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-03-26 10:53:06.000000 bluepy3-1.2.5/bluepy3/uuids.json
--rw-r--r--   0 maurice    (501) staff       (20)      125 2023-03-08 11:49:00.000000 bluepy3-1.2.5/bluepy3/version.h
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:05:43.105129 bluepy3-1.2.5/bluepy3.egg-info/
--rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)      521 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/SOURCES.txt
--rw-r--r--   0 maurice    (501) staff       (20)        1 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/dependency_links.txt
--rw-r--r--   0 maurice    (501) staff       (20)      117 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/entry_points.txt
--rw-r--r--   0 maurice    (501) staff       (20)        8 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/top_level.txt
--rw-r--r--   0 maurice    (501) staff       (20)       94 2023-04-16 14:05:43.105614 bluepy3-1.2.5/setup.cfg
--rw-r--r--   0 maurice    (501) staff       (20)     3340 2023-04-16 14:05:29.000000 bluepy3-1.2.5/setup.py
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-30 08:41:12.317774 bluepy3-1.4.1/
+-rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.4.1/LICENSE
+-rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-30 08:41:12.317825 bluepy3-1.4.1/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)     3454 2023-04-29 09:30:37.000000 bluepy3-1.4.1/README.md
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-30 08:41:12.317041 bluepy3-1.4.1/bluepy3/
+-rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/Makefile
+-rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/__init__.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-04-29 09:33:24.000000 bluepy3-1.4.1/bluepy3/blescan.py
+-rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0 maurice    (501) staff       (20)    37271 2023-04-30 08:40:15.000000 bluepy3-1.4.1/bluepy3/btle.py
+-rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/config.5.47.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/config.5.50.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/config.5.60.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/config.5.66.h
+-rwxr-xr-x   0 maurice    (501) staff       (20)     9750 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/get_services.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/scan_fuzz.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/scanner.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/sensortag.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/thingy52.py
+-rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/uuids.json
+-rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.4.1/bluepy3/version.h
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-30 08:41:12.317664 bluepy3-1.4.1/bluepy3.egg-info/
+-rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-30 08:41:12.000000 bluepy3-1.4.1/bluepy3.egg-info/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)      521 2023-04-30 08:41:12.000000 bluepy3-1.4.1/bluepy3.egg-info/SOURCES.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        1 2023-04-30 08:41:12.000000 bluepy3-1.4.1/bluepy3.egg-info/dependency_links.txt
+-rw-r--r--   0 maurice    (501) staff       (20)      117 2023-04-30 08:41:12.000000 bluepy3-1.4.1/bluepy3.egg-info/entry_points.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        8 2023-04-30 08:41:12.000000 bluepy3-1.4.1/bluepy3.egg-info/top_level.txt
+-rw-r--r--   0 maurice    (501) staff       (20)       94 2023-04-30 08:41:12.318015 bluepy3-1.4.1/setup.cfg
+-rw-r--r--   0 maurice    (501) staff       (20)     3340 2023-04-30 08:39:51.000000 bluepy3-1.4.1/setup.py
```

### Comparing `bluepy3-1.2.5/LICENSE` & `bluepy3-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/PKG-INFO` & `bluepy3-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.2.5
+Version: 1.4.1
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.2.5/README.md` & `bluepy3-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/Makefile` & `bluepy3-1.4.1/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/blescan.py` & `bluepy3-1.4.1/bluepy3/blescan.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         dev_connectable = "(not connectable)"
         if dev.connectable:
             dev_connectable = ""
         print(
             f"    Device ({status}): {ANSI_WHITE}{dev.addr}{ANSI_OFF} ({dev.addrType}),"
             f" {dev.rssi} dBm {dev_connectable}"
         )
-        for (sdid, desc, val) in dev.getScanData():
+        for sdid, desc, val in dev.getScanData():
             if sdid in [8, 9]:
                 print(f"\t{desc}: '{ANSI_CYAN}{val}{ANSI_OFF}'")
             else:
                 print(f"\t{desc}: <{val}>")
         if not dev.scanData:
             print("\t(no data)")
         print()
@@ -135,18 +135,15 @@
     parser.add_argument(
         "-n",
         "--new",
         action="store_true",
         help="Display only new adv responses, by default show new + updated",
     )
     parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="Increase output verbosity"
+        "-v", "--verbose", action="store_true", help="Increase output verbosity"
     )
     arg = parser.parse_args(sys.argv[1:])
 
     btle.Debugging = arg.verbose
 
     scanner = btle.Scanner(arg.hci).withDelegate(ScanPrint(arg))
```

### Comparing `bluepy3-1.2.5/bluepy3/bluepy3-helper.c` & `bluepy3-1.4.1/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/btle.py` & `bluepy3-1.4.1/bluepy3/btle.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,29 +99,29 @@
     def __init__(self, val, commonName=None):
         """Initialisation
         We accept: 32-digit hex strings, with and without '-' characters,
         4 to 8 digit hex strings, and integers
         """
         if isinstance(val, int):
             if (val < 0) or (val > 0xFFFFFFFF):
-                raise ValueError("*** -btle- Short form UUIDs must be in range 0..0xFFFFFFFF")
+                raise ValueError("(btle.py) Short form UUIDs must be in range 0..0xFFFFFFFF")
             val = f"{val:04X}"
         elif isinstance(val, self.__class__):
             val = str(val)
         else:
             val = str(val)  # Do our best
 
         val = val.replace("-", "")
         if len(val) <= 8:  # Short form
             val = ("0" * (8 - len(val))) + val + "00001000800000805F9B34FB"
 
         self.binVal = binascii.a2b_hex(val.encode("utf-8"))
         if len(self.binVal) != 16:
             raise ValueError(
-                f"*** -btle- UUID must be 16 bytes, got '{val}' (len={len(self.binVal)})"
+                f"(btle.py) UUID must be 16 bytes, got '{val}' (len={len(self.binVal)})"
             )
         self.commonName = commonName
 
     def __str__(self):
         s = binascii.b2a_hex(self.binVal).decode("utf-8")
         return "-".join([s[0:8], s[8:12], s[12:16], s[16:20], s[20:32]])
 
@@ -334,26 +334,26 @@
             self._aiti = None
         if self._stderr is not None:
             self._stderr.close()
             self._stderr = None
 
     def _writeCmd(self, cmd):
         if self._helper is None:
-            raise BTLEInternalError("*** -btle- Helper not started (did you call connect()?)")
+            raise BTLEInternalError("(btle.py) Helper not started (did you call connect()?)")
         DBG(f"    -btle- Sent:   {cmd}")
         self._helper.stdin.write(cmd)
         self._helper.stdin.flush()
 
     def _mgmtCmd(self, cmd):
         self._writeCmd(cmd + "\n")
         rsp = self._waitResp("mgmt")
         if rsp["code"][0] != "success":
             self._stopHelper()
             raise BTLEManagementError(
-                f"*** -btle- Failed to execute management command '{cmd}'", rsp
+                f"(btle.py) Failed to execute management command '{cmd}'", rsp
             )
 
     @staticmethod
     def parseResp(line):
         resp = {}
         for item in line.rstrip().split("\x1e"):
             (tag, tval) = item.split("=")
@@ -364,26 +364,26 @@
                 val = tval[1:]
             elif tval[0] == "h":
                 val = int(tval[1:], 16)
             elif tval[0] == "b":
                 val = binascii.a2b_hex(tval[1:].encode("utf-8"))
             else:
                 raise BTLEInternalError(
-                    f"*** -btle- Cannot understand response value {repr(tval)}"
+                    f"(btle.py) Cannot understand response value {repr(tval)}"
                 )
             if tag not in resp:
                 resp[tag] = [val]
             else:
                 resp[tag].append(val)
         return resp
 
     def _waitResp(self, wantType, timeout=BTLE_TIMEOUT):
         while True:
             if self._helper.poll() is not None:
-                raise BTLEInternalError("*** -btle- Helper exited")
+                raise BTLEInternalError("(btle.py) Helper exited")
 
             try:
                 rv = self._lineq.get(timeout=timeout)
             except Empty:
                 DBG("*** -btle- Select timeout")
                 return None
             dehex_rv = (
@@ -391,22 +391,24 @@
             )
             DBG(f"    -btle- Got:    {dehex_rv}")
             if rv.startswith("#") or rv == "\n" or len(rv) == 0:
                 continue
 
             resp = Bluepy3Helper.parseResp(rv)
             if "rsp" not in resp:
-                raise BTLEInternalError("*** -btle- No response type indicator", resp)
+                raise BTLEInternalError("(btle.py) No response type indicator", resp)
 
             # sometimes devices just keep sending `ntfy`
             if "ntfy" in repr(rv):
                 self._aiti += 1
                 if self._aiti > 3:
                     self._stopHelper()
-                    raise BTLEInternalError("*** -btle- I am not an idiot.", resp)
+                    raise BTLEInternalError(
+                        "(btle.py) Device keeps repeating itself. Giving up.", resp
+                    )
 
             respType = resp["rsp"][0]
 
             # always check for MTU updates
             if "mtu" in resp and len(resp["mtu"]) > 0:
                 new_mtu = int(resp["mtu"][0])
                 if self._mtu != new_mtu:
@@ -414,32 +416,32 @@
                     DBG(f"    -btle- Updated MTU: {str(self._mtu)}")
 
             if respType in wantType:
                 return resp
             elif respType == "stat":
                 if "state" in resp and len(resp["state"]) > 0 and resp["state"][0] == "disc":
                     self._stopHelper()
-                    raise BTLEConnectError("*** -btle- Device disconnected", resp)
+                    raise BTLEConnectError("(btle.py) Device disconnected", resp)
             elif respType == "err":
                 errcode = resp["code"][0]
                 if errcode == "nomgmt":
                     raise BTLEManagementError(
-                        "*** -btle- Management not available (permissions problem?)", resp
+                        "(btle.py) Management not available (permissions problem?)", resp
                     )
                 elif errcode == "atterr":
-                    raise BTLEGattError("*** -btle- Bluetooth command failed", resp)
+                    raise BTLEGattError("(btle.py) Bluetooth command failed", resp)
                 else:
                     raise BTLEException(
-                        f"*** -btle- Error from bluepy3-helper ({errcode})", resp
+                        f"(btle.py) Error from bluepy3-helper ({errcode})", resp
                     )
             elif respType == "scan":
                 # Scan response when we weren't interested. Ignore it
                 continue
             else:
-                raise BTLEInternalError(f"*** -btle- Unexpected response ({respType})", resp)
+                raise BTLEInternalError(f"(btle.py) Unexpected response ({respType})", resp)
 
     def status(self):
         self._writeCmd("stat\n")
         return self._waitResp(["stat"])
 
 
 class Peripheral(Bluepy3Helper):
@@ -482,32 +484,32 @@
             if respType not in wantType:
                 continue
             return resp
 
     def _connect(self, addr, addrType=ADDR_TYPE_PUBLIC, iface=None, timeout=BTLE_TIMEOUT):
         max_retries = 5
         if len(addr.split(":")) != 6:
-            raise ValueError(f"*** -btle- Expected MAC address, got {repr(addr)}")
+            raise ValueError(f"(btle.py) Expected MAC address, got {repr(addr)}")
         if addrType not in (ADDR_TYPE_PUBLIC, ADDR_TYPE_RANDOM):
             raise ValueError(
-                f"*** -btle- Expected address type public or random, got {addrType}"
+                f"(btle.py) Expected address type public or random, got {addrType}"
             )
         self.retries = max_retries
         while self.retries > 0:
             self._startHelper(iface)
             self.addr = addr
             self.addrType = addrType
             self.iface = iface
             if iface is not None:
                 self._writeCmd(f"conn {addr} {addrType} hci{str(iface)}\n")
             else:
                 self._writeCmd(f"conn {addr} {addrType}\n")
             rsp = self._getResp("stat", timeout)
             timeout_exception = BTLEConnectTimeout(
-                f" -btle- Timed out while trying to connect to peripheral {addr}, addr type: {addrType}, interface {iface}, timeout={timeout}",
+                f"(btle.py) Timed out while trying to connect to peripheral {addr}, addr type: {addrType}, interface {iface}, timeout={timeout}",
                 rsp,
             )
             if rsp is None:
                 raise timeout_exception
             while rsp and rsp["state"][0] == "tryconn":
                 rsp = self._getResp("stat", timeout)
             if rsp is not None and rsp["state"][0] == "conn":
@@ -519,15 +521,15 @@
                 if rsp is None:
                     raise timeout_exception
                 else:
                     DBG(f"*** -btle-  Failed to connect. ({self.retries})")
                     time.sleep(0.5 * (max_retries - self.retries))
                     if self.retries <= 1:
                         raise BTLEConnectError(
-                            f"*** -btle- Failed to connect to peripheral {addr}, addr type: {addrType}, interface {iface}, timeout={timeout}",
+                            f"(btle.py) Failed to connect to peripheral {addr}, addr type: {addrType}, interface {iface}, timeout={timeout}",
                             rsp,
                         )
             self.retries -= 1
 
     def connect(self, addr, addrType=ADDR_TYPE_PUBLIC, iface=None, timeout=BTLE_TIMEOUT):
         if isinstance(addr, ScanEntry):
             self._connect(addr.addr, addr.addrType, addr.iface, timeout)
@@ -573,15 +575,15 @@
     def getServiceByUUID(self, uuidVal):
         uuid = UUID(uuidVal)
         if self._serviceMap is not None and uuid in self._serviceMap:
             return self._serviceMap[uuid]
         self._writeCmd(f"svcs {uuid}\n")
         rsp = self._getResp("find")
         if "hstart" not in rsp:
-            raise BTLEGattError(f"*** -btle- Service {uuid.getCommonName()} not found", rsp)
+            raise BTLEGattError(f"(btle.py) Service {uuid.getCommonName()} not found", rsp)
         svc = Service(self, uuid, rsp["hstart"][0], rsp["hend"][0])
 
         if self._serviceMap is None:
             self._serviceMap = {}
         self._serviceMap[uuid] = svc
         return svc
 
@@ -593,15 +595,15 @@
     def getCharacteristics(self, startHnd=1, endHnd=0xFFFF, uuid=None, timeout=BTLE_TIMEOUT):
         cmd = f"char {startHnd:X} {endHnd:X}"
         if uuid:
             cmd += f" {UUID(uuid)}"
         self._writeCmd(cmd + "\n")
         rsp = self._getResp("find", timeout)
         timeout_exception = BTLEConnectTimeout(
-            f" -btle- Timed out while trying to get characteristics from peripheral {self.addr}, addr type: {self.addrType}",
+            f"(btle.py) Timed out while trying to get characteristics from peripheral {self.addr}, addr type: {self.addrType}",
             rsp,
         )
         if rsp is None:
             raise timeout_exception
         nChars = len(rsp["hnd"])
         return [
             Characteristic(self, rsp["uuid"][i], rsp["hnd"][i], rsp["props"][i], rsp["vhnd"][i])
@@ -674,18 +676,18 @@
             cmd += " C_256 " + oob_data["C_256"] + " R_256 " + oob_data["R_256"]
         if iface is not None:
             cmd += " hci" + str(iface)
         self._writeCmd(cmd)
 
     def setRemoteOOB(self, address, address_type, oob_data, iface=None):
         if len(address.split(":")) != 6:
-            raise ValueError(f"*** -btle- Expected MAC address, got {repr(address)}")
+            raise ValueError(f"(btle.py) Expected MAC address, got {repr(address)}")
         if address_type not in (ADDR_TYPE_PUBLIC, ADDR_TYPE_RANDOM):
             raise ValueError(
-                f"*** -btle- Expected address type public or random, got {address_type}"
+                f"(btle.py) Expected address type public or random, got {address_type}"
             )
         if isinstance(address, ScanEntry):
             return self._setRemoteOOB(address.addr, address.addrType, oob_data, address.iface)
         elif address is not None:
             return self._setRemoteOOB(address, address_type, oob_data, iface)
 
     def getLocalOOB(self, iface=None):
@@ -696,45 +698,45 @@
         self._writeCmd("local_oob\n")
         if iface is not None:
             cmd += " hci" + str(iface)
         resp = self._getResp("oob")
         if resp is not None:
             data = resp.get("d", [""])[0]
             if data is None:
-                raise BTLEManagementError("*** -btle- Failed to get local OOB data.")
+                raise BTLEManagementError("(btle.py) Failed to get local OOB data.")
             if (
                 struct.unpack_from("<B", data, 0)[0] != 8
                 or struct.unpack_from("<B", data, 1)[0] != 0x1B
             ):
-                raise BTLEManagementError("*** -btle- Malformed local OOB data (address).")
+                raise BTLEManagementError("(btle.py) Malformed local OOB data (address).")
             address = data[2:8]
             address_type = data[8:9]
             if (
                 struct.unpack_from("<B", data, 9)[0] != 2
                 or struct.unpack_from("<B", data, 10)[0] != 0x1C
             ):
-                raise BTLEManagementError("*** -btle- Malformed local OOB data (role).")
+                raise BTLEManagementError("(btle.py) Malformed local OOB data (role).")
             role = data[11:12]
             if (
                 struct.unpack_from("<B", data, 12)[0] != 17
                 or struct.unpack_from("<B", data, 13)[0] != 0x22
             ):
-                raise BTLEManagementError("*** -btle- Malformed local OOB data (confirm).")
+                raise BTLEManagementError("(btle.py) Malformed local OOB data (confirm).")
             confirm = data[14:30]
             if (
                 struct.unpack_from("<B", data, 30)[0] != 17
                 or struct.unpack_from("<B", data, 31)[0] != 0x23
             ):
-                raise BTLEManagementError("*** -btle- Malformed local OOB data (random).")
+                raise BTLEManagementError("(btle.py) Malformed local OOB data (random).")
             random = data[32:48]
             if (
                 struct.unpack_from("<B", data, 48)[0] != 2
                 or struct.unpack_from("<B", data, 49)[0] != 0x1
             ):
-                raise BTLEManagementError("*** -btle- Malformed local OOB data (flags).")
+                raise BTLEManagementError("(btle.py) Malformed local OOB data (flags).")
             flags = data[50:51]
             return {
                 "Address": "".join(["%02X" % struct.unpack("<B", c)[0] for c in address]),
                 "Type": "".join(["%02X" % struct.unpack("<B", c)[0] for c in address_type]),
                 "Role": "".join(["%02X" % struct.unpack("<B", c)[0] for c in role]),
                 "C_256": "".join(["%02X" % struct.unpack("<B", c)[0] for c in confirm]),
                 "R_256": "".join(["%02X" % struct.unpack("<B", c)[0] for c in random]),
@@ -804,15 +806,15 @@
         self.scanData = {}
         self.updateCount = 0
 
     def _update(self, resp):
         addrType = self.addrTypes.get(resp["type"][0], None)
         if (self.addrType is not None) and (addrType != self.addrType):
             raise BTLEInternalError(
-                f"*** -btle- Address type changed during scan, for address {self.addr}"
+                f"(btle.py) Address type changed during scan, for address {self.addr}"
             )
         self.addrType = addrType
         self.rssi = -resp["rssi"][0]
         self.connectable = (resp["flag"][0] & 0x4) == 0
         data = resp.get("d", [""])[0]
         self.rawData = data
 
@@ -931,15 +933,15 @@
         self._stopHelper()
 
     def clear(self):
         self.scanned = {}
 
     def process(self, timeout=10.0):
         if self._helper is None:
-            raise BTLEInternalError("*** -btle- Helper not started (did you call start()?)")
+            raise BTLEInternalError("(btle.py) Helper not started (did you call start()?)")
         start = time.time()
         while True:
             if timeout:
                 remain = start + timeout - time.time()
                 if remain <= 0.0:
                     break
             else:
@@ -964,15 +966,15 @@
                     dev = ScanEntry(addr, self.iface)
                     self.scanned[addr] = dev
                 isNewData = dev._update(resp)
                 if self.delegate is not None:
                     self.delegate.handleDiscovery(dev, (dev.updateCount <= 1), isNewData)
 
             else:
-                raise BTLEInternalError(f"*** -btle- Unexpected response: {respType}", resp)
+                raise BTLEInternalError(f"(btle.py) Unexpected response: {respType}", resp)
 
     def getDevices(self):
         return list(self.scanned.values())
 
     def scan(self, timeout=10, passive=False):
         self.clear()
         self.start(passive=passive)
@@ -1019,15 +1021,15 @@
 AssignedNumbers = _UUIDNameMap(get_json_uuid())
 
 if __name__ == "__main__":
     if len(sys.argv) < 2:
         sys.exit(f"Usage:\n  {sys.argv[0]} <mac-address> [random]")
 
     if not os.path.isfile(helperExe):
-        raise ImportError(f"*** -btle- Cannot find required executable '{helperExe}'")
+        raise ImportError(f"(btle.py) Cannot find required executable '{helperExe}'")
 
     devAddr = sys.argv[1]
     if len(sys.argv) == 3:
         addrType = sys.argv[2]
     else:
         addrType = ADDR_TYPE_PUBLIC
     print(f"Connecting to: {devAddr}, address type: {addrType}")
```

### Comparing `bluepy3-1.2.5/bluepy3/config.5.47.h` & `bluepy3-1.4.1/bluepy3/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/config.5.50.h` & `bluepy3-1.4.1/bluepy3/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/config.5.60.h` & `bluepy3-1.4.1/bluepy3/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/config.5.66.h` & `bluepy3-1.4.1/bluepy3/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/get_services.py` & `bluepy3-1.4.1/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/scan_fuzz.py` & `bluepy3-1.4.1/bluepy3/scan_fuzz.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/sensortag.py` & `bluepy3-1.4.1/bluepy3/sensortag.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/thingy52.py` & `bluepy3-1.4.1/bluepy3/thingy52.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3/uuids.json` & `bluepy3-1.4.1/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/bluepy3.egg-info/PKG-INFO` & `bluepy3-1.4.1/bluepy3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.2.5
+Version: 1.4.1
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.2.5/bluepy3.egg-info/SOURCES.txt` & `bluepy3-1.4.1/bluepy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.5/setup.py` & `bluepy3-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shlex
 import subprocess
 import sys
 
 from setuptools import setup
 from setuptools.command.build_py import build_py
 
-VERSION = "1.2.5"
+VERSION = "1.4.1"
 MAKEFILE = "bluepy3/Makefile"
 VERSION_FILE = "bluepy3/version.h"
 BLUEZ_VERSION = "(unknown)"
 
 
 def pre_install():
     """Do the custom compiling of the bluepy3-helper executable from the makefile"""
```

