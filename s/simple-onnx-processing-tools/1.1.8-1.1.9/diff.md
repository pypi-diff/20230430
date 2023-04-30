# Comparing `tmp/simple_onnx_processing_tools-1.1.8.tar.gz` & `tmp/simple_onnx_processing_tools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_onnx_processing_tools-1.1.8.tar", last modified: Mon Jan  2 05:52:56 2023, max compression
+gzip compressed data, was "simple_onnx_processing_tools-1.1.9.tar", last modified: Mon Jan  2 06:15:25 2023, max compression
```

## Comparing `simple_onnx_processing_tools-1.1.8.tar` & `simple_onnx_processing_tools-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 05:52:56.582058 simple_onnx_processing_tools-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-02 05:52:50.000000 simple_onnx_processing_tools-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20321 2023-01-02 05:52:56.578058 simple_onnx_processing_tools-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-01-02 05:52:50.000000 simple_onnx_processing_tools-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-02 05:52:56.582058 simple_onnx_processing_tools-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-01-02 05:52:50.000000 simple_onnx_processing_tools-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 05:52:56.578058 simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-02 05:52:50.000000 simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 05:52:56.578058 simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20321 2023-01-02 05:52:56.000000 simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-02 05:52:56.000000 simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 05:52:56.000000 simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-02 05:52:56.000000 simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-02 05:52:56.000000 simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 06:15:25.275070 simple_onnx_processing_tools-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-02 06:15:15.000000 simple_onnx_processing_tools-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20321 2023-01-02 06:15:25.275070 simple_onnx_processing_tools-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-01-02 06:15:15.000000 simple_onnx_processing_tools-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-02 06:15:25.275070 simple_onnx_processing_tools-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-01-02 06:15:15.000000 simple_onnx_processing_tools-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 06:15:25.275070 simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-02 06:15:15.000000 simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 06:15:25.275070 simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20321 2023-01-02 06:15:25.000000 simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-02 06:15:25.000000 simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 06:15:25.000000 simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-02 06:15:25.000000 simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-02 06:15:25.000000 simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools.egg-info/top_level.txt
```

### Comparing `simple_onnx_processing_tools-1.1.8/LICENSE` & `simple_onnx_processing_tools-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_onnx_processing_tools-1.1.8/PKG-INFO` & `simple_onnx_processing_tools-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_onnx_processing_tools
-Version: 1.1.8
+Version: 1.1.9
 Summary: A set of simple tools for splitting, merging, OP deletion, size compression, rewriting attributes and constants, OP generation, change opset, change to the specified input order, addition of OP, RGB to BGR conversion, change batch size, batch rename of OP, and JSON convertion for ONNX models.
 Home-page: https://github.com/PINTO0309/simple-onnx-processing-tools
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -38,15 +38,15 @@
 && python3 -m pip install -U onnx_graphsurgeon --index-url https://pypi.ngc.nvidia.com
 ```
 ### Docker
 ```bash
 $ docker run --rm -it \
 -v `pwd`:/workdir \
 -w /workdir \
-ghcr.io/pinto0309/simple-onnx-processing-tools:1.1.8
+ghcr.io/pinto0309/simple-onnx-processing-tools:1.1.9
 ```
 
 |No.|Tool Name|Tags|Summary|
 |:-:|:-:|:-:|:-|
 |1|**[snc4onnx](https://github.com/PINTO0309/snc4onnx)**<br>![snc](https://user-images.githubusercontent.com/33194443/170050379-72e2819a-8cc4-40c2-9cc9-d4ca50b83866.png)|[![PyPI](https://img.shields.io/pypi/v/snc4onnx?color=2BAF2B)](https://pypi.org/project/snc4onnx/)[![snc](https://img.shields.io/github/stars/PINTO0309/snc4onnx.svg?style=social)](https://github.com/PINTO0309/snc4onnx)|Simple tool to combine(merge) onnx models. **S**imple **N**etwork **C**ombine Tool for **ONNX**.|
 |2|**[sne4onnx](https://github.com/PINTO0309/sne4onnx)**<br>![image](https://user-images.githubusercontent.com/33194443/170036340-dd098dd2-4955-48b6-a0dd-6b59c3598018.png)|[![PyPI](https://img.shields.io/pypi/v/sne4onnx?color=2BAF2B)](https://pypi.org/project/sne4onnx/)[![sne](https://img.shields.io/github/stars/PINTO0309/sne4onnx.svg?style=social)](https://github.com/PINTO0309/sne4onnx)|A very simple tool for situations where optimization with onnx-simplifier would exceed the Protocol Buffers upper file size limit of 2GB, or simply to separate onnx files to any size you want. **S**imple **N**etwork **E**xtraction for **ONNX**.|
 |3|**[snd4onnx](https://github.com/PINTO0309/snd4onnx)**<br>![snd](https://user-images.githubusercontent.com/33194443/170049884-63abc243-0493-400a-9d95-612a800fbfce.png)|[![PyPI](https://img.shields.io/pypi/v/snd4onnx?color=2BAF2B)](https://pypi.org/project/snd4onnx/)[![snd](https://img.shields.io/github/stars/PINTO0309/snd4onnx.svg?style=social)](https://github.com/PINTO0309/snd4onnx)|Simple node deletion tool for onnx. **S**imple **N**ode **D**eletion for **ONNX**.|
```

### Comparing `simple_onnx_processing_tools-1.1.8/README.md` & `simple_onnx_processing_tools-1.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 && python3 -m pip install -U onnx_graphsurgeon --index-url https://pypi.ngc.nvidia.com
 ```
 ### Docker
 ```bash
 $ docker run --rm -it \
 -v `pwd`:/workdir \
 -w /workdir \
-ghcr.io/pinto0309/simple-onnx-processing-tools:1.1.8
+ghcr.io/pinto0309/simple-onnx-processing-tools:1.1.9
 ```
 
 |No.|Tool Name|Tags|Summary|
 |:-:|:-:|:-:|:-|
 |1|**[snc4onnx](https://github.com/PINTO0309/snc4onnx)**<br>![snc](https://user-images.githubusercontent.com/33194443/170050379-72e2819a-8cc4-40c2-9cc9-d4ca50b83866.png)|[![PyPI](https://img.shields.io/pypi/v/snc4onnx?color=2BAF2B)](https://pypi.org/project/snc4onnx/)[![snc](https://img.shields.io/github/stars/PINTO0309/snc4onnx.svg?style=social)](https://github.com/PINTO0309/snc4onnx)|Simple tool to combine(merge) onnx models. **S**imple **N**etwork **C**ombine Tool for **ONNX**.|
 |2|**[sne4onnx](https://github.com/PINTO0309/sne4onnx)**<br>![image](https://user-images.githubusercontent.com/33194443/170036340-dd098dd2-4955-48b6-a0dd-6b59c3598018.png)|[![PyPI](https://img.shields.io/pypi/v/sne4onnx?color=2BAF2B)](https://pypi.org/project/sne4onnx/)[![sne](https://img.shields.io/github/stars/PINTO0309/sne4onnx.svg?style=social)](https://github.com/PINTO0309/sne4onnx)|A very simple tool for situations where optimization with onnx-simplifier would exceed the Protocol Buffers upper file size limit of 2GB, or simply to separate onnx files to any size you want. **S**imple **N**etwork **E**xtraction for **ONNX**.|
 |3|**[snd4onnx](https://github.com/PINTO0309/snd4onnx)**<br>![snd](https://user-images.githubusercontent.com/33194443/170049884-63abc243-0493-400a-9d95-612a800fbfce.png)|[![PyPI](https://img.shields.io/pypi/v/snd4onnx?color=2BAF2B)](https://pypi.org/project/snd4onnx/)[![snd](https://img.shields.io/github/stars/PINTO0309/snd4onnx.svg?style=social)](https://github.com/PINTO0309/snd4onnx)|Simple node deletion tool for onnx. **S**imple **N**ode **D**eletion for **ONNX**.|
```

### Comparing `simple_onnx_processing_tools-1.1.8/setup.py` & `simple_onnx_processing_tools-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     author_email="rmsdh122@yahoo.co.jp",
     url="https://github.com/PINTO0309/simple-onnx-processing-tools",
     license="MIT License",
     packages=find_packages(),
     platforms=["linux", "unix"],
     python_requires=">=3.6",
     install_requires = [
-        'snc4onnx >= 1.0.10',
+        'snc4onnx >= 1.0.11',
         'sne4onnx >= 1.0.10',
         'snd4onnx >= 1.1.6',
         'scs4onnx >= 1.0.18',
         'sog4onnx >= 1.0.15',
         'sam4onnx >= 1.0.11',
         'soc4onnx >= 1.0.2',
         'scc4onnx >= 1.0.5',
```

### Comparing `simple_onnx_processing_tools-1.1.8/simple_onnx_processing_tools.egg-info/PKG-INFO` & `simple_onnx_processing_tools-1.1.9/simple_onnx_processing_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-onnx-processing-tools
-Version: 1.1.8
+Version: 1.1.9
 Summary: A set of simple tools for splitting, merging, OP deletion, size compression, rewriting attributes and constants, OP generation, change opset, change to the specified input order, addition of OP, RGB to BGR conversion, change batch size, batch rename of OP, and JSON convertion for ONNX models.
 Home-page: https://github.com/PINTO0309/simple-onnx-processing-tools
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -38,15 +38,15 @@
 && python3 -m pip install -U onnx_graphsurgeon --index-url https://pypi.ngc.nvidia.com
 ```
 ### Docker
 ```bash
 $ docker run --rm -it \
 -v `pwd`:/workdir \
 -w /workdir \
-ghcr.io/pinto0309/simple-onnx-processing-tools:1.1.8
+ghcr.io/pinto0309/simple-onnx-processing-tools:1.1.9
 ```
 
 |No.|Tool Name|Tags|Summary|
 |:-:|:-:|:-:|:-|
 |1|**[snc4onnx](https://github.com/PINTO0309/snc4onnx)**<br>![snc](https://user-images.githubusercontent.com/33194443/170050379-72e2819a-8cc4-40c2-9cc9-d4ca50b83866.png)|[![PyPI](https://img.shields.io/pypi/v/snc4onnx?color=2BAF2B)](https://pypi.org/project/snc4onnx/)[![snc](https://img.shields.io/github/stars/PINTO0309/snc4onnx.svg?style=social)](https://github.com/PINTO0309/snc4onnx)|Simple tool to combine(merge) onnx models. **S**imple **N**etwork **C**ombine Tool for **ONNX**.|
 |2|**[sne4onnx](https://github.com/PINTO0309/sne4onnx)**<br>![image](https://user-images.githubusercontent.com/33194443/170036340-dd098dd2-4955-48b6-a0dd-6b59c3598018.png)|[![PyPI](https://img.shields.io/pypi/v/sne4onnx?color=2BAF2B)](https://pypi.org/project/sne4onnx/)[![sne](https://img.shields.io/github/stars/PINTO0309/sne4onnx.svg?style=social)](https://github.com/PINTO0309/sne4onnx)|A very simple tool for situations where optimization with onnx-simplifier would exceed the Protocol Buffers upper file size limit of 2GB, or simply to separate onnx files to any size you want. **S**imple **N**etwork **E**xtraction for **ONNX**.|
 |3|**[snd4onnx](https://github.com/PINTO0309/snd4onnx)**<br>![snd](https://user-images.githubusercontent.com/33194443/170049884-63abc243-0493-400a-9d95-612a800fbfce.png)|[![PyPI](https://img.shields.io/pypi/v/snd4onnx?color=2BAF2B)](https://pypi.org/project/snd4onnx/)[![snd](https://img.shields.io/github/stars/PINTO0309/snd4onnx.svg?style=social)](https://github.com/PINTO0309/snd4onnx)|Simple node deletion tool for onnx. **S**imple **N**ode **D**eletion for **ONNX**.|
```

