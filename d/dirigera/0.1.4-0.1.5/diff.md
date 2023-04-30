# Comparing `tmp/dirigera-0.1.4.tar.gz` & `tmp/dirigera-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-0.1.4.tar", last modified: Wed Apr 26 20:27:27 2023, max compression
+gzip compressed data, was "dirigera-0.1.5.tar", last modified: Sun Apr 30 09:20:18 2023, max compression
```

## Comparing `dirigera-0.1.4.tar` & `dirigera-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-26 20:27:18.000000 dirigera-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-26 20:27:27.418074 dirigera-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-26 20:27:18.000000 dirigera-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-26 20:27:18.000000 dirigera-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:27:27.418074 dirigera-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:27:18.000000 dirigera-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/devices/light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-26 20:27:18.000000 dirigera-0.1.4/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-26 20:27:18.000000 dirigera-0.1.4/tests/test_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.025783 dirigera-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-30 09:20:09.000000 dirigera-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-30 09:20:18.025783 dirigera-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-30 09:20:09.000000 dirigera-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-30 09:20:09.000000 dirigera-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 09:20:18.025783 dirigera-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 09:20:09.000000 dirigera-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.021783 dirigera-0.1.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.021783 dirigera-0.1.5/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.025783 dirigera-0.1.5/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/devices/light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.025783 dirigera-0.1.5/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-30 09:20:09.000000 dirigera-0.1.5/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.021783 dirigera-0.1.5/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 09:20:18.000000 dirigera-0.1.5/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 09:20:18.025783 dirigera-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-30 09:20:09.000000 dirigera-0.1.5/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-30 09:20:09.000000 dirigera-0.1.5/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-30 09:20:09.000000 dirigera-0.1.5/tests/test_light.py
```

### Comparing `dirigera-0.1.4/LICENSE` & `dirigera-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.4/PKG-INFO` & `dirigera-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.4
+Version: 0.1.5
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,44 +40,52 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Dirigera Python Client
 ![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
 ![Pypi](https://img.shields.io/pypi/v/dirigera)
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
-
+![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
+ - [blinds control](#controlling-blinds)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
 ```bash
 pip install dirigera
 ```
 
 ## Quickstart
 
 1. Find out the ip-address of your Dirigera (check your router)
-2. Run the generate-token script:
+2. Once you installed `dirigera` with pip you can run the included generate-token script. Here you can directly set the ip-address of you dirigera as parameter.
    ```bash
    generate-token <Dirigera ip-address>
    ```
-   When prompted, you must push the action button on Dirigera. After that hit ENTER and your `token` will be printed to the console.  
+3. The script starts the auth process. When prompted, you must push the action button on the bottom of your Dirigera. 
+4. After that hit ENTER and your `token` will be printed to the console.  
    Example:
-   ```
+    ```
     Press the action button on Dirigera then hit ENTER ...
     Your Token:
     mgwB.aXqwpzV89N0aUwBhZMJjD8a.UBPyzy2InGtqgwo2MO5.xX4ug7.uBcVJquwYzLnAijF7SdYKvNxTo0uzQKahV10A-3ZQOz-UAubGP6sHWt1CJx3QmWZyE7ZcMZKgODXjSzWL1lumKgGz5dUIwFi3rhNxgK-IsBGeGVhNXPt8vGrYEcZePwPvNAIg8RqmlH27L-JZPnkAtP2wHoOdW72Djot3yJsohtEsb0p9mJvoZFSavTlTr4LDuf584vuH5fha5xoR9QhhIvvgbAP-s4EHFqENNi6vrYLHKR.sdqnv4sYw6UH-l6oiPnnRLxinoqBPOlWhlcL9doFviXQE.tZ9X8WVqyBrd0NYHlo9iorEvUbnZuD02BEJrg4NLwgh3rZtyF0Mi46HenynzBohbPn4RnuSYYCiHt5EZnWedxBtDqc7mSTm1ZtyD
-   ```
-6. Done
+    ```
+5. Done. Use this token in the hub setup.
+     ```
+    dirigera.Hub(
+        token="mgwB.aXqwpzV89N0aUwBhZMJjD8a...",
+        ip_address="192.1..."
+    )
+    ```
 
 ## [Dirigera Hub](./src/dirigera/hub/hub.py)
 
 Setting up the client works by providing the token and ip address.
 
 ```python
 import dirigera
@@ -127,14 +135,45 @@
 light.set_color_temperature(color_temp=3000)
 
 light.set_light_color(hue=128, saturation=0.5)
 
 light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Blinds](./src/dirigera/devices/blinds.py)
+
+To get information about the available blinds, you can use the `get_blinds()` method:
+
+```python
+blinds = dirigera_hub.get_blinds()
+```
+
+The blind object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+target_level: int
+current_level: int
+state: str
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName", "blindsCurrentLevel", "blindsTargetLevel", "blindsState"]
+```
+
+Available methods for blinds are:
+
+```python
+blind.set_name(name="kitchen blind 1")
+
+blind.set_target_level(target_level=90)
+```
+
+
 ## [Environment Sensor](./src/dirigera/devices/environment_sensor.py)
 Currently only tested with the VINDSTYRKA sensor. If you have other sensors please send me the json and I will add support or create a PR.
 
 
 To get the environment sensors use:
 ```python
 sensors = dirigera_hub.get_environment_sensors()
```

### Comparing `dirigera-0.1.4/README.md` & `dirigera-0.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 # Dirigera Python Client
 ![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
 ![Pypi](https://img.shields.io/pypi/v/dirigera)
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
-
+![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
+ - [blinds control](#controlling-blinds)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
 ```bash
 pip install dirigera
 ```
 
 ## Quickstart
 
 1. Find out the ip-address of your Dirigera (check your router)
-2. Run the generate-token script:
+2. Once you installed `dirigera` with pip you can run the included generate-token script. Here you can directly set the ip-address of you dirigera as parameter.
    ```bash
    generate-token <Dirigera ip-address>
    ```
-   When prompted, you must push the action button on Dirigera. After that hit ENTER and your `token` will be printed to the console.  
+3. The script starts the auth process. When prompted, you must push the action button on the bottom of your Dirigera. 
+4. After that hit ENTER and your `token` will be printed to the console.  
    Example:
-   ```
+    ```
     Press the action button on Dirigera then hit ENTER ...
     Your Token:
     mgwB.aXqwpzV89N0aUwBhZMJjD8a.UBPyzy2InGtqgwo2MO5.xX4ug7.uBcVJquwYzLnAijF7SdYKvNxTo0uzQKahV10A-3ZQOz-UAubGP6sHWt1CJx3QmWZyE7ZcMZKgODXjSzWL1lumKgGz5dUIwFi3rhNxgK-IsBGeGVhNXPt8vGrYEcZePwPvNAIg8RqmlH27L-JZPnkAtP2wHoOdW72Djot3yJsohtEsb0p9mJvoZFSavTlTr4LDuf584vuH5fha5xoR9QhhIvvgbAP-s4EHFqENNi6vrYLHKR.sdqnv4sYw6UH-l6oiPnnRLxinoqBPOlWhlcL9doFviXQE.tZ9X8WVqyBrd0NYHlo9iorEvUbnZuD02BEJrg4NLwgh3rZtyF0Mi46HenynzBohbPn4RnuSYYCiHt5EZnWedxBtDqc7mSTm1ZtyD
-   ```
-6. Done
+    ```
+5. Done. Use this token in the hub setup.
+     ```
+    dirigera.Hub(
+        token="mgwB.aXqwpzV89N0aUwBhZMJjD8a...",
+        ip_address="192.1..."
+    )
+    ```
 
 ## [Dirigera Hub](./src/dirigera/hub/hub.py)
 
 Setting up the client works by providing the token and ip address.
 
 ```python
 import dirigera
@@ -85,14 +93,45 @@
 light.set_color_temperature(color_temp=3000)
 
 light.set_light_color(hue=128, saturation=0.5)
 
 light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Blinds](./src/dirigera/devices/blinds.py)
+
+To get information about the available blinds, you can use the `get_blinds()` method:
+
+```python
+blinds = dirigera_hub.get_blinds()
+```
+
+The blind object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+target_level: int
+current_level: int
+state: str
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName", "blindsCurrentLevel", "blindsTargetLevel", "blindsState"]
+```
+
+Available methods for blinds are:
+
+```python
+blind.set_name(name="kitchen blind 1")
+
+blind.set_target_level(target_level=90)
+```
+
+
 ## [Environment Sensor](./src/dirigera/devices/environment_sensor.py)
 Currently only tested with the VINDSTYRKA sensor. If you have other sensors please send me the json and I will add support or create a PR.
 
 
 To get the environment sensors use:
 ```python
 sensors = dirigera_hub.get_environment_sensors()
```

### Comparing `dirigera-0.1.4/pyproject.toml` & `dirigera-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
    "setuptools",
    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "0.1.4"
+version = "0.1.5"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["python", "iot", "smarthome", "hub", "lighting", "ikea", "tradfri", "dirigera"]
 dependencies = [
     "requests >= 2.22.0",
```

### Comparing `dirigera-0.1.4/src/dirigera/devices/environment_sensor.py` & `dirigera-0.1.5/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.4/src/dirigera/devices/light.py` & `dirigera-0.1.5/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.4/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-0.1.5/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.4/src/dirigera/hub/auth.py` & `dirigera-0.1.5/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.4/src/dirigera.egg-info/PKG-INFO` & `dirigera-0.1.5/src/dirigera.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.4
+Version: 0.1.5
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,44 +40,52 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Dirigera Python Client
 ![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
 ![Pypi](https://img.shields.io/pypi/v/dirigera)
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
-
+![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
+ - [blinds control](#controlling-blinds)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
 ```bash
 pip install dirigera
 ```
 
 ## Quickstart
 
 1. Find out the ip-address of your Dirigera (check your router)
-2. Run the generate-token script:
+2. Once you installed `dirigera` with pip you can run the included generate-token script. Here you can directly set the ip-address of you dirigera as parameter.
    ```bash
    generate-token <Dirigera ip-address>
    ```
-   When prompted, you must push the action button on Dirigera. After that hit ENTER and your `token` will be printed to the console.  
+3. The script starts the auth process. When prompted, you must push the action button on the bottom of your Dirigera. 
+4. After that hit ENTER and your `token` will be printed to the console.  
    Example:
-   ```
+    ```
     Press the action button on Dirigera then hit ENTER ...
     Your Token:
     mgwB.aXqwpzV89N0aUwBhZMJjD8a.UBPyzy2InGtqgwo2MO5.xX4ug7.uBcVJquwYzLnAijF7SdYKvNxTo0uzQKahV10A-3ZQOz-UAubGP6sHWt1CJx3QmWZyE7ZcMZKgODXjSzWL1lumKgGz5dUIwFi3rhNxgK-IsBGeGVhNXPt8vGrYEcZePwPvNAIg8RqmlH27L-JZPnkAtP2wHoOdW72Djot3yJsohtEsb0p9mJvoZFSavTlTr4LDuf584vuH5fha5xoR9QhhIvvgbAP-s4EHFqENNi6vrYLHKR.sdqnv4sYw6UH-l6oiPnnRLxinoqBPOlWhlcL9doFviXQE.tZ9X8WVqyBrd0NYHlo9iorEvUbnZuD02BEJrg4NLwgh3rZtyF0Mi46HenynzBohbPn4RnuSYYCiHt5EZnWedxBtDqc7mSTm1ZtyD
-   ```
-6. Done
+    ```
+5. Done. Use this token in the hub setup.
+     ```
+    dirigera.Hub(
+        token="mgwB.aXqwpzV89N0aUwBhZMJjD8a...",
+        ip_address="192.1..."
+    )
+    ```
 
 ## [Dirigera Hub](./src/dirigera/hub/hub.py)
 
 Setting up the client works by providing the token and ip address.
 
 ```python
 import dirigera
@@ -127,14 +135,45 @@
 light.set_color_temperature(color_temp=3000)
 
 light.set_light_color(hue=128, saturation=0.5)
 
 light.set_startup_behaviour(behaviour=StartupEnum.START_OFF)
 ```
 
+## [Controlling Blinds](./src/dirigera/devices/blinds.py)
+
+To get information about the available blinds, you can use the `get_blinds()` method:
+
+```python
+blinds = dirigera_hub.get_blinds()
+```
+
+The blind object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+target_level: int
+current_level: int
+state: str
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName", "blindsCurrentLevel", "blindsTargetLevel", "blindsState"]
+```
+
+Available methods for blinds are:
+
+```python
+blind.set_name(name="kitchen blind 1")
+
+blind.set_target_level(target_level=90)
+```
+
+
 ## [Environment Sensor](./src/dirigera/devices/environment_sensor.py)
 Currently only tested with the VINDSTYRKA sensor. If you have other sensors please send me the json and I will add support or create a PR.
 
 
 To get the environment sensors use:
 ```python
 sensors = dirigera_hub.get_environment_sensors()
```

### Comparing `dirigera-0.1.4/src/dirigera.egg-info/SOURCES.txt` & `dirigera-0.1.5/src/dirigera.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 src/dirigera.egg-info/PKG-INFO
 src/dirigera.egg-info/SOURCES.txt
 src/dirigera.egg-info/dependency_links.txt
 src/dirigera.egg-info/entry_points.txt
 src/dirigera.egg-info/requires.txt
 src/dirigera.egg-info/top_level.txt
 src/dirigera/devices/__init__.py
+src/dirigera/devices/blinds.py
 src/dirigera/devices/device.py
 src/dirigera/devices/environment_sensor.py
 src/dirigera/devices/light.py
 src/dirigera/hub/__init__.py
 src/dirigera/hub/abstract_smart_home_hub.py
 src/dirigera/hub/auth.py
 src/dirigera/hub/hub.py
+tests/test_blinds.py
 tests/test_environment_sensor.py
 tests/test_light.py
```

### Comparing `dirigera-0.1.4/tests/test_environment_sensor.py` & `dirigera-0.1.5/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.4/tests/test_light.py` & `dirigera-0.1.5/tests/test_light.py`

 * *Files identical despite different names*

