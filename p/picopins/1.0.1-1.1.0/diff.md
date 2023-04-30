# Comparing `tmp/picopins-1.0.1.tar.gz` & `tmp/picopins-1.1.0.tar.gz`

## Comparing `picopins-1.0.1.tar` & `picopins-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 picopins-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 picopins-1.0.1/Makefile
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 picopins-1.0.1/README.md
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 picopins-1.0.1/check.sh
--rw-r--r--   0        0        0    34361 2020-02-02 00:00:00.000000 picopins-1.0.1/example.png
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 picopins-1.0.1/requirements-dev.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 picopins-1.0.1/requirements.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 picopins-1.0.1/tox.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 picopins-1.0.1/picopins/__init__.py
--rwxr-xr-x   0        0        0     7315 2020-02-02 00:00:00.000000 picopins-1.0.1/picopins/__main__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 picopins-1.0.1/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 picopins-1.0.1/LICENSE
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 picopins-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 picopins-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 picopins-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 picopins-1.1.0/Makefile
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 picopins-1.1.0/README.md
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 picopins-1.1.0/check.sh
+-rw-r--r--   0        0        0    34361 2020-02-02 00:00:00.000000 picopins-1.1.0/example.png
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 picopins-1.1.0/requirements-dev.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 picopins-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 picopins-1.1.0/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 picopins-1.1.0/picopins/__init__.py
+-rwxr-xr-x   0        0        0     9475 2020-02-02 00:00:00.000000 picopins-1.1.0/picopins/__main__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 picopins-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 picopins-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 picopins-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 picopins-1.1.0/PKG-INFO
```

### Comparing `picopins-1.0.1/Makefile` & `picopins-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `picopins-1.0.1/README.md` & `picopins-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -19,8 +19,16 @@
 
 eg:    picopins i2c  - show GPIO and I2C labels
        picopins      - basic GPIO pinout
 ```
 
 # Installing
 
-* Just run `python3 -m pip install picopins`
+* Just run `python3 -m pip install picopins`
+
+# Achknowledgements
+
+This project was inspired by GPIO Zero's command-line pinout - https://github.com/gpiozero/gpiozero
+
+It somehow wasn't inspired by Raspberry Pi Spy's "picopins" which came first and solves this same problem in bash - https://www.raspberrypi-spy.co.uk/2022/12/pi-pico-pinout-display-on-the-command-line/
+
+Like RPi Spy's picopins it started as a GitHub gist, you can find the history here - https://gist.github.com/Gadgetoid/192af85a3eb05d4a6ac1db076c4ef118/revisions
```

### Comparing `picopins-1.0.1/check.sh` & `picopins-1.1.0/check.sh`

 * *Files identical despite different names*

### Comparing `picopins-1.0.1/example.png` & `picopins-1.1.0/example.png`

 * *Files identical despite different names*

### Comparing `picopins-1.0.1/LICENSE` & `picopins-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picopins-1.0.1/pyproject.toml` & `picopins-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `picopins-1.0.1/PKG-INFO` & `picopins-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picopins
-Version: 1.0.1
+Version: 1.1.0
 Summary: A command-line pinout for the Raspberry Pi Pico W
 Project-URL: GitHub, https://www.github.com/pinout-xyz/picopins
 Project-URL: Homepage, https://pico.pinout.xyz
 Author-email: Philip Howard <pinout@gadgetoid.com>
 Maintainer-email: Philip Howard <pinout@gadgetoid.com>
 License: MIT License
         
@@ -68,16 +68,33 @@
 eg:    picopins i2c  - show GPIO and I2C labels
        picopins      - basic GPIO pinout
 ```
 
 # Installing
 
 * Just run `python3 -m pip install picopins`
+
+# Achknowledgements
+
+This project was inspired by GPIO Zero's command-line pinout - https://github.com/gpiozero/gpiozero
+
+It somehow wasn't inspired by Raspberry Pi Spy's "picopins" which came first and solves this same problem in bash - https://www.raspberrypi-spy.co.uk/2022/12/pi-pico-pinout-display-on-the-command-line/
+
+Like RPi Spy's picopins it started as a GitHub gist, you can find the history here - https://gist.github.com/Gadgetoid/192af85a3eb05d4a6ac1db076c4ef118/revisions
 # Changelog
 
+1.1.0
+-----
+
+* Highlight GPIO label if `--find` matches a hidden label
+* Add regex support to `--find`
+* Rewrite render flow to make it less hacky
+* Light mode is back! `--light`
+* Move error text above usage message
+
 1.0.1
 -----
 
 * Tidy up readme
 
 1.0.0
 -----
```

