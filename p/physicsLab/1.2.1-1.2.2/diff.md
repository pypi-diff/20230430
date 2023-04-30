# Comparing `tmp/physicsLab-1.2.1.tar.gz` & `tmp/physicsLab-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\physicsLab-1.2.1.tar", last modified: Fri Apr 21 15:10:13 2023, max compression
+gzip compressed data, was "dist\physicsLab-1.2.2.tar", last modified: Sun Apr 30 08:38:11 2023, max compression
```

## Comparing `physicsLab-1.2.1.tar` & `physicsLab-1.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/
--rw-rw-rw-   0        0        0     1094 2023-04-05 15:16:06.000000 physicsLab-1.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4440 2023-04-21 15:10:13.000000 physicsLab-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3880 2023-04-19 15:49:15.000000 physicsLab-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/
--rw-rw-rw-   0        0        0      391 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/__init__.py
--rw-rw-rw-   0        0        0      966 2023-04-14 14:26:12.000000 physicsLab-1.2.1/physicsLab/_colorUtils.py
--rw-rw-rw-   0        0        0     3384 2023-04-21 14:57:54.000000 physicsLab-1.2.1/physicsLab/_fileGlobals.py
--rw-rw-rw-   0        0        0      715 2023-04-21 13:17:54.000000 physicsLab-1.2.1/physicsLab/_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/astrophysics/
--rw-rw-rw-   0        0        0       13 2023-04-21 15:04:35.000000 physicsLab-1.2.1/physicsLab/astrophysics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/electricity/
--rw-rw-rw-   0        0        0      335 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/electricity/__init__.py
--rw-rw-rw-   0        0        0     4319 2023-04-21 14:37:03.000000 physicsLab-1.2.1/physicsLab/electricity/element.py
--rw-rw-rw-   0        0        0      478 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/electricity/elementPin.py
--rw-rw-rw-   0        0        0     2435 2023-04-21 14:03:16.000000 physicsLab-1.2.1/physicsLab/electricity/elementXYZ.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/
--rw-rw-rw-   0        0        0      342 2023-04-21 15:04:35.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/__init__.py
--rw-rw-rw-   0        0        0     4936 2023-04-21 14:31:05.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/_elementClassHead.py
--rw-rw-rw-   0        0        0     9181 2023-04-21 13:46:31.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/artificialCircuit.py
--rw-rw-rw-   0        0        0     8656 2023-04-21 12:38:58.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/basicCircuit.py
--rw-rw-rw-   0        0        0    17020 2023-04-21 13:47:04.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/logicCircuit.py
--rw-rw-rw-   0        0        0     4590 2023-04-21 12:38:59.000000 physicsLab-1.2.1/physicsLab/electricity/elementsClass/otherCircuit.py
--rw-rw-rw-   0        0        0     3043 2023-04-21 14:31:05.000000 physicsLab-1.2.1/physicsLab/electricity/wire.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/electromagnetism/
--rw-rw-rw-   0        0        0       13 2023-04-21 15:04:35.000000 physicsLab-1.2.1/physicsLab/electromagnetism/__init__.py
--rw-rw-rw-   0        0        0      319 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/errors.py
--rw-rw-rw-   0        0        0    11450 2023-04-21 14:31:05.000000 physicsLab-1.2.1/physicsLab/experiment.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab/unionElements/
--rw-rw-rw-   0        0        0      166 2023-04-21 15:04:35.000000 physicsLab-1.2.1/physicsLab/unionElements/__init__.py
--rw-rw-rw-   0        0        0       13 2023-04-21 12:39:34.000000 physicsLab-1.2.1/physicsLab/unionElements/_unionClassHead.py
--rw-rw-rw-   0        0        0     6835 2023-04-21 12:32:51.000000 physicsLab-1.2.1/physicsLab/unionElements/unionLogic.py
--rw-rw-rw-   0        0        0       69 2023-04-21 12:39:18.000000 physicsLab-1.2.1/physicsLab/unionElements/unionPin.py
--rw-rw-rw-   0        0        0     1369 2023-04-21 12:38:49.000000 physicsLab-1.2.1/physicsLab/unionElements/union_music.py
--rw-rw-rw-   0        0        0        0 2023-04-08 12:26:18.000000 physicsLab-1.2.1/physicsLab/userlog.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/
--rw-rw-rw-   0        0        0     4440 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1117 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-21 15:10:13.000000 physicsLab-1.2.1/physicsLab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      581 2023-03-16 14:16:49.000000 physicsLab-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 15:10:13.000000 physicsLab-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1151 2023-04-21 15:10:05.000000 physicsLab-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-05 15:16:06.000000 physicsLab-1.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4440 2023-04-30 08:38:11.000000 physicsLab-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3880 2023-04-19 15:49:15.000000 physicsLab-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/
+-rw-rw-rw-   0        0        0      379 2023-04-30 06:47:35.000000 physicsLab-1.2.2/physicsLab/__init__.py
+-rw-rw-rw-   0        0        0      966 2023-04-14 14:26:12.000000 physicsLab-1.2.2/physicsLab/_colorUtils.py
+-rw-rw-rw-   0        0        0     3471 2023-04-30 06:47:19.000000 physicsLab-1.2.2/physicsLab/_fileGlobals.py
+-rw-rw-rw-   0        0        0      715 2023-04-21 15:10:17.000000 physicsLab-1.2.2/physicsLab/_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/astrophysics/
+-rw-rw-rw-   0        0        0       13 2023-04-21 15:10:17.000000 physicsLab-1.2.2/physicsLab/astrophysics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/electricity/
+-rw-rw-rw-   0        0        0      619 2023-04-28 12:19:38.000000 physicsLab-1.2.2/physicsLab/electricity/__init__.py
+-rw-rw-rw-   0        0        0     4424 2023-04-28 12:17:30.000000 physicsLab-1.2.2/physicsLab/electricity/element.py
+-rw-rw-rw-   0        0        0      688 2023-04-30 07:33:03.000000 physicsLab-1.2.2/physicsLab/electricity/elementPin.py
+-rw-rw-rw-   0        0        0     2887 2023-04-30 06:49:55.000000 physicsLab-1.2.2/physicsLab/electricity/elementXYZ.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/
+-rw-rw-rw-   0        0        0      483 2023-04-28 12:01:14.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/__init__.py
+-rw-rw-rw-   0        0        0     4942 2023-04-28 09:39:05.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/_elementClassHead.py
+-rw-rw-rw-   0        0        0     9761 2023-04-28 12:34:35.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/artificialCircuit.py
+-rw-rw-rw-   0        0        0     9101 2023-04-28 12:34:35.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/basicCircuit.py
+-rw-rw-rw-   0        0        0    18300 2023-04-28 12:30:37.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/logicCircuit.py
+-rw-rw-rw-   0        0        0     4640 2023-04-28 12:34:35.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/otherCircuit.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/
+-rw-rw-rw-   0        0        0      297 2023-04-30 07:25:33.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/__init__.py
+-rw-rw-rw-   0        0        0     1641 2023-04-30 06:47:19.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/_unionClassHead.py
+-rw-rw-rw-   0        0        0    15760 2023-04-30 07:51:24.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/unionLogic.py
+-rw-rw-rw-   0        0        0     1376 2023-04-28 12:35:26.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/unionMusic.py
+-rw-rw-rw-   0        0        0      605 2023-04-30 08:22:07.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/unionPin.py
+-rw-rw-rw-   0        0        0     1883 2023-04-30 08:29:02.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/wires.py
+-rw-rw-rw-   0        0        0     3433 2023-04-30 08:03:53.000000 physicsLab-1.2.2/physicsLab/electricity/wire.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/electromagnetism/
+-rw-rw-rw-   0        0        0       13 2023-04-21 15:10:17.000000 physicsLab-1.2.2/physicsLab/electromagnetism/__init__.py
+-rw-rw-rw-   0        0        0      436 2023-04-30 08:01:14.000000 physicsLab-1.2.2/physicsLab/errors.py
+-rw-rw-rw-   0        0        0    11653 2023-04-28 12:47:59.000000 physicsLab-1.2.2/physicsLab/experiment.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/
+-rw-rw-rw-   0        0        0     4440 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1200 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      581 2023-03-16 14:16:49.000000 physicsLab-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 08:38:11.000000 physicsLab-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2023-04-30 08:37:00.000000 physicsLab-1.2.2/setup.py
```

### Comparing `physicsLab-1.2.1/LICENSE.txt` & `physicsLab-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `physicsLab-1.2.1/PKG-INFO` & `physicsLab-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.2.1
+Version: 1.2.2
 Summary: Doing experiments in the physics lab AR by python
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `physicsLab-1.2.1/README.md` & `physicsLab-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `physicsLab-1.2.1/physicsLab/_colorUtils.py` & `physicsLab-1.2.2/physicsLab/_colorUtils.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.2.1/physicsLab/_fileGlobals.py` & `physicsLab-1.2.2/physicsLab/_fileGlobals.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,8 +99,13 @@
         "Interfaces": {
             "Play-Expanded": False,
             "Chart-Expanded": False
         }
     }
 
     elements_Position = {}
-    elements_Index = []
+    elements_Index = []
+
+# 获取sav
+def get_Sav() -> dict:
+    import copy
+    return copy.deepcopy(sav)
```

### Comparing `physicsLab-1.2.1/physicsLab/_tools.py` & `physicsLab-1.2.2/physicsLab/_tools.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.2.1/physicsLab/electricity/element.py` & `physicsLab-1.2.2/physicsLab/electricity/element.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #coding=utf-8
 import physicsLab._tools as _tools
 import physicsLab._fileGlobals as _fileGlobals
-from physicsLab.electricity.elementsClass import *
 import physicsLab.electricity.elementXYZ as _elementXYZ
+import physicsLab.electricity.elementsClass as _elementsClass
 
 # 创建原件，本质上仍然是实例化
 def crt_Element(
         name: str,
         x: _tools.numType = 0,
         y: _tools.numType = 0,
         z: _tools.numType = 0,
@@ -18,31 +18,31 @@
             and isinstance(z, (int, float))
     ):
         raise RuntimeError("Wrong parameter type")
     name = name.strip()
     if name == '':
         raise RuntimeError('Name cannot be an empty string')
         # 元件坐标系
-    if elementXYZ == True or (_elementXYZ.elementXYZ == True and elementXYZ is None):
+    if elementXYZ == True or (_elementXYZ.is_elementXYZ() == True and elementXYZ is None):
         x, y, z = _elementXYZ.xyzTranslate(x, y, z)
     x, y, z = _tools.roundData(x, y, z)
     if (name == '555 Timer'):
-        return NE555(x, y, z)
+        return _elementsClass.NE555(x, y, z)
     elif (name == '8bit Input'):
-        return eight_bit_Input(x, y, z)
+        return _elementsClass.eight_bit_Input(x, y, z)
     elif (name == '8bit Display'):
-        return eight_bit_Display(x, y, z)
+        return _elementsClass.eight_bit_Display(x, y, z)
     else:
         try:
-            return eval(name.replace(' ', '_').replace('-', '_') + f'({x},{y},{z})')
+            return eval(f"_elementsClass.{name.replace(' ', '_').replace('-', '_')}({x},{y},{z})")
         except SyntaxError:
             raise RuntimeError(f"{name} original that does not exist")
 
 # 获取对应坐标的self
-def get_Element(*args, **kwargs):
+def get_Element(*args, **kwargs) -> _elementsClass.elementBase:
     # 通过坐标索引元件
     def position_Element(x: _tools.numType, y: _tools.numType, z: _tools.numType):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise TypeError('illegal argument')
         x, y, z = _tools.roundData(x), _tools.roundData(y), _tools.roundData(z)
         if (x, y, z) not in _fileGlobals.elements_Position.keys():
             raise RuntimeError("Error coordinates that do not exist")
```

### Comparing `physicsLab-1.2.1/physicsLab/electricity/elementXYZ.py` & `physicsLab-1.2.2/physicsLab/electricity/elementXYZ.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,22 +12,26 @@
 
 # _elementClassHead里的element_Init_HEAD有部分处理元件坐标系的代码，并调用了该文件
 
 import physicsLab._tools as _tools
 
 ### define ###
 
-# 是否将全局设置为元件坐标系
-elementXYZ: bool = False
+_elementXYZ: bool = False
 
+# 是否将全局设置为元件坐标系
 def set_elementXYZ(boolen: bool) -> None:
     if not isinstance(boolen, bool):
         raise TypeError
-    global elementXYZ
-    elementXYZ = boolen
+    global _elementXYZ
+    _elementXYZ = boolen
+
+# 获取是否为元件坐标系
+def is_elementXYZ() -> bool:
+    return _elementXYZ
 
 # 物实坐标系x, y, z单位1
 _xUnit: _tools.numType = 0.16
 _yUnit: _tools.numType = 0.08
 _zUnit: _tools.numType = 0.1
 # big_element坐标修正
 _yAmend = 0.045
@@ -78,8 +82,22 @@
         y: _tools.numType, 
         z: _tools.numType
     ):
     return x, y + _yAmend, z
 
 # 获取坐标原点
 def get_OriginPosition():
-    return _xOrigin, _yOrigin, _zOrigin
+    return _xOrigin, _yOrigin, _zOrigin
+
+# 输入"x" 返回_xUnit
+# 输入"y", "z" 返回_yUnit, _zUnit
+def get_xyzUnit(*args):
+    if any(i not in ("x", "y", "z") for i in args):
+        raise TypeError
+    index = {
+        "x": _xUnit,
+        "y": _yUnit,
+        "z": _zUnit
+    }
+    if len(args) == 1:
+        return index[args[0]]
+    return (index[string] for string in args)
```

### Comparing `physicsLab-1.2.1/physicsLab/electricity/elementsClass/_elementClassHead.py` & `physicsLab-1.2.2/physicsLab/electricity/elementsClass/_elementClassHead.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementXYZ as _elementXYZ
 
 # 是否为big_Element
 is_big_Element: bool = False
 
 # 所有元件的父类
-class elementObject:
+class elementBase:
     # 设置原件的角度
     def set_Rotation(self, xRotation: _tools.numType = 0, yRotation: _tools.numType = 0,
                      zRotation: _tools.numType = 180):
         if not (isinstance(xRotation, (int, float)) and isinstance(yRotation, (int, float)) and isinstance(zRotation, (
         int, float))):
             raise RuntimeError('illegal argument')
         self._arguments[
@@ -81,15 +81,15 @@
         # 初始化全局变量
         global is_big_Element
         is_big_Element = False
 
         x, y, z = _tools.roundData(x, y, z)
         self._position = (x, y, z)
         # 元件坐标系
-        if elementXYZ == True or (_elementXYZ.elementXYZ == True and elementXYZ is None):
+        if elementXYZ == True or (_elementXYZ.is_elementXYZ() == True and elementXYZ is None):
             x, y, z = _elementXYZ.xyzTranslate(x, y, z)
         func(self, x, y, z)
         # 若是big_Element，则修正坐标
         if is_big_Element:
             x, y, z = _elementXYZ.amend_big_Element(x, y, z)
 
         self._arguments["Identifier"] = _tools.randString(32)
@@ -99,15 +99,15 @@
 
         # 该坐标是否已存在，则存入列表
         if self._position in _fileGlobals.elements_Position.keys():
             _fileGlobals.elements_Position[self._position]['self'].append(self)
         else:
             elementDict: dict = {
                 'self': [self],
-                'elementXYZ': _elementXYZ.elementXYZ,  # 是否为元件坐标系
+                'elementXYZ': _elementXYZ.is_elementXYZ,  # 是否为元件坐标系
                 'originPosition': tuple(_elementXYZ.get_OriginPosition())  # 坐标原点
             }
             _fileGlobals.elements_Position[self._position] = elementDict
         self.set_Rotation()
         # 通过元件生成顺序来索引元件
         global _index
         self._index = _index
```

### Comparing `physicsLab-1.2.1/physicsLab/electricity/elementsClass/artificialCircuit.py` & `physicsLab-1.2.2/physicsLab/electricity/elementsClass/artificialCircuit.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,179 +2,179 @@
 import physicsLab._tools as _tools
 from ..elementXYZ import amend_big_Element
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
 
 
 # 555定时器
-class NE555(_elementClassHead.elementObject):
+class NE555(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '555 Timer', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0},
                            'Statistics': {'供电': 10, '放电': 0.0, '阈值': 4,
                                           '控制': 6.6666666666666666, '触发': 4,
                                           '输出': 0, '重设': 10, '接地': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
         _elementClassHead.is_big_Element = True
 
     @property
-    def VCC(self):
+    def VCC(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def Dis(self):
+    def Dis(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def Thr(self):
+    def Thr(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def Ctrl(self):
+    def Ctrl(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def Trig(self):
+    def Trig(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def Out(self):
+    def Out(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def Reset(self):
+    def Reset(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 6)
 
     @property
-    def Ground(self):
+    def Ground(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 7)
 
 # 电容
 @_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Basic_Capacitor(_elementClassHead.elementObject):
+class Basic_Capacitor(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Basic Capacitor', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False, 'Properties': {'耐压': 16.0, '电容': 1e-06, '内阻': 5.0, '锁定': 1.0},
                            'Statistics': {}, 'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
 # 接地
-class Ground_Component(_elementClassHead.elementObject):
+class Ground_Component(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Ground Component', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False, 'Properties': {'锁定': 1.0},
                            'Statistics': {'电流': 0}, 'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i(self):
+    def i(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
 # 运算放大器
-class Operational_Amplifier(_elementClassHead.elementObject):
+class Operational_Amplifier(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Operational Amplifier', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False,
                            'Properties': {'增益系数': 100_0000.0, '最大电压': 15.0, '最小电压': -15.0, '锁定': 1.0},
                            'Statistics': {'电压-': 0, '电压+': 0, '输出电压': 0,
                                           '输出电流': 0, '输出功率': 0},
                            'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def o(self):
+    def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
 # 继电器
-class Relay_Component(_elementClassHead.elementObject):
+class Relay_Component(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Relay Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
                            'Properties': {'开关': 0.0, '线圈电感': 0.2, '线圈电阻': 20.0,
                                           '接通电流': 0.02, '额定电流': 1.0, '锁定': 1.0}, 'Statistics': {},
                            'Position': '', 'Rotation': '',
                            'DiagramCached': False, 'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
                            'DiagramRotation': 0}
 
     @property
-    def l_up(self):
+    def l_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def l_low(self):
+    def l_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def mid(self):
+    def mid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def r_up(self):
+    def r_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def r_low(self):
+    def r_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
 # n mos
-class N_MOSFET(_elementClassHead.elementObject):
+class N_MOSFET(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'N-MOSFET', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False, 'Properties': {'PNP': 1.0, '放大系数': 0.027, '阈值电压': 1.5, '最大功率': 100.0, '锁定': 1.0},
                            'Statistics': {'电压GS': 0.0, '电压': 0.0, '电流': 0.0, '功率': 0.0, '状态': 0.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def D(self):
+    def D(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def S(self):
+    def S(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def G(self):
+    def G(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
 # 波形发生器基类
-class _source_element(_elementClassHead.elementObject):
+class _source_element(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False,
                            'Properties': {'电压': 3.0, '内阻': 0.5, '频率': 20000.0, '偏移': 0.0, '占空比': 0.5, '锁定': 1.0},
                            'Statistics': {'电流': 0.0, '功率': 0.0, '电压': -3.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l(self):
+    def l(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
     i = l
 
     @property
-    def r(self):
+    def r(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
     o = r
 
 # 正弦波发生器
 class Sinewave_Source(_source_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Sinewave_Source, self).__init__(x, y, z, elementXYZ)
```

### Comparing `physicsLab-1.2.1/physicsLab/electricity/elementsClass/basicCircuit.py` & `physicsLab-1.2.2/physicsLab/electricity/elementsClass/basicCircuit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #coding=utf-8
 import physicsLab._tools as _tools
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
 
 # 开关基类
 
-class _switch_Element(_elementClassHead.elementObject):
+class _switch_Element(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {"ModelID": "", "Identifier": "", "IsBroken": False,
                           "IsLocked": False, "Properties": {"开关": 0, "锁定": 1.0},
                           "Statistics": {}, "Position": "",
                           "Rotation": '', "DiagramCached": False,
                           "DiagramPosition": {"X": 0, "Y": 0, "Z": 0, "Magnitude": 0}, "DiagramRotation": 0}
@@ -24,81 +24,81 @@
 # 单刀双掷开关
 class SPDT_Switch(_switch_Element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(SPDT_Switch, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'SPDT Switch'
 
     @property
-    def l(self):
+    def l(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def mid(self):
+    def mid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def r(self):
+    def r(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
 # 双刀双掷开关
 class DPDT_Switch(_switch_Element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(DPDT_Switch, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'DPDT Switch'
 
     @property
-    def l_up(self):
+    def l_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def mid_up(self):
+    def mid_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def r_up(self):
+    def r_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def l_low(self):
+    def l_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def mid_low(self):
+    def mid_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def r_low(self):
+    def r_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
 # 按钮开关
 @_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Push_Switch(_elementClassHead.elementObject):
+class Push_Switch(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {
             'ModelID': 'Push Switch', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
             'Properties': {'开关': 0.0, '默认开关': 0.0, '锁定': 1.0}, 'Statistics': {'电流': 0.0}, 'Position': '',
             'Rotation': '', 'DiagramCached': False, 'DiagramPosition': {
                 'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
 
 # 一节电池
 @_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Battery_Source(_elementClassHead.elementObject):
+class Battery_Source(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Battery Source', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False, 'Properties': {'最大功率': 16.2, '电压': 3.0, '内阻': 0.5},
                            'Statistics': {'电流': 0, '功率': 0, '电压': 0},
                            'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
 # 学生电源
-class Student_Source(_elementClassHead.elementObject):
+class Student_Source(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Student Source', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
                            'Properties': {'交流电压': 3.0, '直流电压': 3.0, '开关': 0.0, '频率': 50.0},
                            'Statistics': {'瞬间功率': 0.0, '瞬间电压': 0.0, '瞬间电流': 0.0,
                                           '瞬间电阻': 0.0, '功率': 0.0, '电阻': 0.0, '电流': 0.0,
                                           '瞬间功率1': 0.0, '瞬间电压1': 0.0, '瞬间电流1': 0.0,
@@ -106,73 +106,73 @@
                                           '功率1': 0.0, '电阻1': 0.0, '电流1': 0.0},
                            'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
                            'DiagramRotation': 0}
 
     @property
-    def l(self):
+    def l(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def l_mid(self):
+    def l_mid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def r_mid(self):
+    def r_mid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def r(self):
+    def r(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
 # 电阻
 @_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Resistor(_elementClassHead.elementObject):
+class Resistor(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Resistor', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False,
                            'Properties': {'最大电阻': 1000_0000.0, '最小电阻': 0.1, '电阻': 10, '锁定': 1.0},
                            'Statistics': {'瞬间功率': 0, '瞬间电流': 0,
                                           '瞬间电压': 0, '功率': 0,
                                           '电压': 0, '电流': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
 # 保险丝
 @_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Fuse_Component(_elementClassHead.elementObject):
+class Fuse_Component(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Fuse Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
                            'Properties': {'开关': 1.0, '额定电流': 0.30000001192092896, '熔断电流': 0.5, '锁定': 1.0},
                            'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
 # 滑动变阻器
-class Slide_Rheostat(_elementClassHead.elementObject):
+class Slide_Rheostat(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Slide Rheostat', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
                            'Properties': {'额定电阻': 10.0, '滑块位置': 0.0, '电阻1': 10, '电阻2': 10.0, '锁定': 1.0},
                            'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0,
                                           '瞬间功率1': 0.0, '瞬间电流1': 0.0, '瞬间电压1': 0.0, '功率1': 0.0, '电压1': 0.0, '电流1': 0.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l_low(self):
+    def l_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def r_low(self):
+    def r_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def l_up(self):
+    def l_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def r_up(self):
+    def r_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
```

### Comparing `physicsLab-1.2.1/physicsLab/electricity/elementsClass/logicCircuit.py` & `physicsLab-1.2.2/physicsLab/electricity/elementsClass/logicCircuit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,77 @@
 #coding=utf-8
 import physicsLab._tools as _tools
-from ..elementXYZ import amend_big_Element
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
 
-# 逻辑电路类装饰器
-def logic_Circuit_Method(cls):
+class _logicBase(_elementClassHead.elementBase):
     # 设置高电平的值
     def set_HighLeaveValue(self, num: _tools.numType) -> None:
         if not isinstance(num, (int, float)):
             raise RuntimeError('illegal argument')
         self._arguments['Properties']['高电平'] = num
-    cls.set_HighLeaveValue = set_HighLeaveValue
 
     # 设置低电平的值
-    def set_LowLeaveValue(self, num : _tools.numType) -> None:
+    def set_LowLeaveValue(self, num: _tools.numType) -> None:
         if not isinstance(num, (int, float)):
             raise RuntimeError('illegal argument')
         self._arguments['Properties']['低电平'] = num
-    cls.set_LowLeaveValue = set_LowLeaveValue
 
-    return cls
 
 # _arguments是参数的意思
 
 # 逻辑输入
-@logic_Circuit_Method
-class Logic_Input(_elementClassHead.elementObject):
+class Logic_Input(_logicBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {"ModelID": "Logic Input", "Identifier": "",
                           "IsBroken": False, "IsLocked": False, "Properties": {"高电平": 3.0, "低电平": 0.0, "锁定": 1.0, "开关": 0},
                           "Statistics": {"电流": 0.0, "电压": 0.0, "功率": 0.0},
                           "Position": "",
                           "Rotation": "", "DiagramCached": False,
                           "DiagramPosition": {"X": 0, "Y": 0, "Magnitude": 0.0},
                           "DiagramRotation": 0}
 
     def set_highLevel(self) -> None:
         self._arguments['Properties']['开关'] = 1.0
 
     @property
-    def o(self):
+    def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
 # 逻辑输出
-@logic_Circuit_Method
-class Logic_Output(_elementClassHead.elementObject):
+class Logic_Output(_logicBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Logic Output', 'Identifier': "",
                           'IsBroken': False, 'IsLocked': False,
                           'Properties': {'状态': 0.0, '高电平': 3.0, '低电平': 0.0, '锁定': 1.0}, 'Statistics': {},
                           'Position': "",
                           'Rotation': '0,180,0', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i(self):
+    def i(self) -> _elementPin.element_Pin:
             return _elementPin.element_Pin(self, 0)
 
 # 2引脚门电路
-@logic_Circuit_Method
-class _2_pin_Gate(_elementClassHead.elementObject):
+class _2_pin_Gate(_logicBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': "", 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '最大电流': 0.1, '锁定': 1.0},
                           'Statistics': {}, 'Position': "", 'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i(self):
+    def i(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o(self):
+    def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # 是门
 class Yes_Gate(_2_pin_Gate):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Yes_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Yes Gate'
@@ -87,33 +79,32 @@
 # 非门
 class No_Gate(_2_pin_Gate):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(No_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'No Gate'
 
 # 3引脚门电路
-@logic_Circuit_Method
-class _3_pin_Gate(_elementClassHead.elementObject):
+class _3_pin_Gate(_logicBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '', 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '最大电流': 0.1, '锁定': 1.0},
                           'Statistics': {}, 'Position': "", 'Rotation': "", 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def o(self):
+    def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
 # 或门
 class Or_Gate(_3_pin_Gate):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Or_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Or Gate'
@@ -157,16 +148,15 @@
 # 蕴含非门
 class Nimp_Gate(_3_pin_Gate):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Nimp_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Nimp Gate'
 
 # 2体积元件父类
-@logic_Circuit_Method
-class _big_element(_elementClassHead.elementObject):
+class _big_element(_logicBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '', 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0}, 'Statistics': {},
                           'Position': '', 'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
         _elementClassHead.is_big_Element = True
@@ -174,308 +164,306 @@
 # 半加器
 class Half_Adder(_big_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Half_Adder, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Half Adder'
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # 全加器
 class Full_Adder(_big_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Full_Adder, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Full Adder'
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def i_mid(self):
+    def i_mid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # 二位乘法器
 class Multiplier(_big_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Multiplier, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Multiplier'
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def i_upmid(self):
+    def i_upmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def i_lowmid(self):
+    def i_lowmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 6)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 7)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o_upmid(self):
+    def o_upmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def o_lowmid(self):
+    def o_lowmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
 # D触发器
 class D_Flipflop(_big_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(D_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'D Flipflop'
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # T触发器
 class T_Flipflop(_big_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(T_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'T Flipflop'
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # JK触发器
 class JK_Flipflop(_big_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(JK_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'JK Flipflop'
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def i_mid(self):
+    def i_mid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # 计数器
 class Counter(_big_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Counter, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Counter'
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o_upmid(self):
+    def o_upmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def o_lowmid(self):
+    def o_lowmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
 # 随机数发生器
 class Random_Generator(_big_element):
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         super(Random_Generator, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Random Generator'
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o_upmid(self):
+    def o_upmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def o_lowmid(self):
+    def o_lowmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
 # 8位输入器
-@logic_Circuit_Method
-class eight_bit_Input(_elementClassHead.elementObject):
+class eight_bit_Input(_logicBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '8bit Input', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '十进制': 0.0, '锁定': 1.0},
                            'Statistics': {}, 'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     def set_num(self, num : int):
         if 0 <= num <= 255:
             self._arguments['Properties']['十进制'] = num
         else:
             raise RuntimeError('The number range entered is incorrect')
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def i_upmid(self):
+    def i_upmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def i_lowmid(self):
+    def i_lowmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def o_upmid(self):
+    def o_upmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def o_lowmid(self):
+    def o_lowmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 6)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 7)
 
 # 8位显示器
-@logic_Circuit_Method
-class eight_bit_Display(_elementClassHead.elementObject):
+class eight_bit_Display(_logicBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '8bit Display', 'Identifier': '',
                           'IsBroken': False, 'IsLocked': False,
                           'Properties': {'高电平': 3.0, '低电平': 0.0, '状态': 0.0, '锁定': 1.0},
                           'Statistics': {'7': 0.0, '6': 0.0, '5': 0.0, '4': 0.0, '3': 0.0, '2': 0.0, '1': 0.0, '0': 0.0,
                                          '十进制': 0.0}, 'Position': '',
                           'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i_up(self):
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def i_upmid(self):
+    def i_upmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def i_lowmid(self):
+    def i_lowmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
     @property
-    def i_low(self):
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def o_up(self):
+    def o_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def o_upmid(self):
+    def o_upmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def o_lowmid(self):
+    def o_lowmid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 6)
 
     @property
-    def o_low(self):
+    def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 7)
```

### Comparing `physicsLab-1.2.1/physicsLab/electricity/elementsClass/otherCircuit.py` & `physicsLab-1.2.2/physicsLab/electricity/elementsClass/otherCircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 import physicsLab._tools as _tools
 from string import digits as _digits
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
 
 # 小电扇
 @_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Electric_Fan(_elementClassHead.elementObject):
+class Electric_Fan(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Electric Fan', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False,
                            'Properties': {'额定电阻': 1.0, '马达常数': 0.1, '转动惯量': 0.01, '电感': 5e-05, '负荷扭矩': 0.01,
                                           '反电动势系数': 0.001, '粘性摩擦系数': 0.01, '角速度': 0, '锁定': 1.0},
                            'Statistics': {'瞬间功率': 0, '瞬间电流': 0, '瞬间电压': 0, '功率': 0,
                                           '电压': 0, '电流': 0, '摩擦扭矩': 0, '角速度': 0,
                                           '反电动势': 0, '转速': 0, '输入功率': 0, '输出功率': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
 # 简单乐器（更多功能的源代码在union_music）
-class Simple_Instrument(_elementClassHead.elementObject):
+class Simple_Instrument(_elementClassHead.elementBase):
     @_elementClassHead.element_Init_HEAD
     def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Simple Instrument', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
                            'Properties': {'额定电压': 3.0, '额定功率': 0.3, '音量': 1.0, '音高': 60.0, '节拍': 70.0, '锁定': 1.0,
                                           '乐器': 1.0},
                            'Statistics': {'瞬间功率': 0, '瞬间电流': 0, '瞬间电压': 0, '功率': 0, '电压': 0, '电流': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i(self):
+    def i(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def o(self):
+    def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     # 设置音高
     '''
     输入格式：
         中音区： 
             (funcInput -> 音调)
```

### Comparing `physicsLab-1.2.1/physicsLab/experiment.py` & `physicsLab-1.2.2/physicsLab/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json as _json
 
 import physicsLab._tools as _tools
 import physicsLab.errors as errors
 import physicsLab._colorUtils as _colorUtils
 import physicsLab._fileGlobals as _fileGlobals
 from physicsLab.electricity.element import crt_Element
+import physicsLab.electricity.elementXYZ as _elementXYZ
 
 ### define ###
 
 def print_Elements():
     print(_fileGlobals.Elements)
 
 def print_wires():
@@ -23,33 +24,38 @@
 ### end define ###
 
 # 实验（存档）类，主要与'with'关键字搭配使用
 class experiment:
     def __init__(
             self,
             file: str,
-            read: bool = False # 是否读取存档原有状态
-    ) -> None:
+            read: bool = False, # 是否读取存档原有状态
+            elementXYZ: bool = False
+    ):
         if not (
             isinstance(file, str)
             and isinstance(read, bool)
         ):
             raise TypeError
 
         self.file = file
         self.read = read
+        self.elementXYZ = elementXYZ
 
     # 上下文管理器，搭配with使用
     def __enter__(self):
         try:
             open_Experiment(self.file)
         except errors.openExperimentError: # 如果存档不存在
             crt_Experiment(self.file)
+
         if self.read:
             read_Experiment()
+        if self.elementXYZ:
+            _elementXYZ.set_elementXYZ(True)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         write_Experiment()
 
 # 输入sav文件名并读取（旧函数，不建议使用）
 def old_open_Experiment(file: str) -> None:
     file = file.strip()
```

### Comparing `physicsLab-1.2.1/physicsLab/unionElements/union_music.py` & `physicsLab-1.2.2/physicsLab/electricity/unionElements/unionMusic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #coding=utf-8
 import math as _math
 from typing import Union as _Union
 import physicsLab._tools as _tools
-import physicsLab.electricity as eletricity
+import physicsLab.electricity as _eletricity
 '''
 How do you play music in physics Lab AR?
 Music extension might make it easier than before!
 
     How to use it?
 >>> music(a_list_or_a_tuple)
 >>> write_Experiment()
@@ -29,12 +29,12 @@
     def __init__(
             self,
             x: _tools.numType = 0,
             y: _tools.numType = 0,
             z: _tools.numType = 0,
             musicArray: _Union[list, tuple] = ()
     ):
-        tick = eletricity.Nimp_Gate(x, y + 0.1, z)
-        eletricity.crt_Wire(eletricity.Logic_Input(x, y, z).o, tick.i_up), eletricity.crt_Wire(tick.o, tick.i_low)
-        eletricity.crt_Wire(tick.o, eletricity.Counter(x + 0.2, y, z).i_up)
+        tick = _eletricity.Nimp_Gate(x, y + 0.1, z)
+        _eletricity.crt_Wire(_eletricity.Logic_Input(x, y, z).o, tick.i_up), _eletricity.crt_Wire(tick.o, tick.i_low)
+        _eletricity.crt_Wire(tick.o, _eletricity.Counter(x + 0.2, y, z).i_up)
         side = _math.ceil(_math.sqrt(musicArray.__len__()))
         pass
```

### Comparing `physicsLab-1.2.1/physicsLab.egg-info/PKG-INFO` & `physicsLab-1.2.2/physicsLab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.2.1
+Version: 1.2.2
 Summary: Doing experiments in the physics lab AR by python
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `physicsLab-1.2.1/physicsLab.egg-info/SOURCES.txt` & `physicsLab-1.2.2/physicsLab.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.py
 physicsLab/__init__.py
 physicsLab/_colorUtils.py
 physicsLab/_fileGlobals.py
 physicsLab/_tools.py
 physicsLab/errors.py
 physicsLab/experiment.py
-physicsLab/userlog.py
 physicsLab.egg-info/PKG-INFO
 physicsLab.egg-info/SOURCES.txt
 physicsLab.egg-info/dependency_links.txt
 physicsLab.egg-info/top_level.txt
 physicsLab/astrophysics/__init__.py
 physicsLab/electricity/__init__.py
 physicsLab/electricity/element.py
@@ -21,13 +20,14 @@
 physicsLab/electricity/wire.py
 physicsLab/electricity/elementsClass/__init__.py
 physicsLab/electricity/elementsClass/_elementClassHead.py
 physicsLab/electricity/elementsClass/artificialCircuit.py
 physicsLab/electricity/elementsClass/basicCircuit.py
 physicsLab/electricity/elementsClass/logicCircuit.py
 physicsLab/electricity/elementsClass/otherCircuit.py
-physicsLab/electromagnetism/__init__.py
-physicsLab/unionElements/__init__.py
-physicsLab/unionElements/_unionClassHead.py
-physicsLab/unionElements/unionLogic.py
-physicsLab/unionElements/unionPin.py
-physicsLab/unionElements/union_music.py
+physicsLab/electricity/unionElements/__init__.py
+physicsLab/electricity/unionElements/_unionClassHead.py
+physicsLab/electricity/unionElements/unionLogic.py
+physicsLab/electricity/unionElements/unionMusic.py
+physicsLab/electricity/unionElements/unionPin.py
+physicsLab/electricity/unionElements/wires.py
+physicsLab/electromagnetism/__init__.py
```

### Comparing `physicsLab-1.2.1/pyproject.toml` & `physicsLab-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `physicsLab-1.2.1/setup.py` & `physicsLab-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("D:/program_physicsLab/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="physicsLab",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.2.1",  # 包版本号，便于维护版本
+    version="1.2.2",  # 包版本号，便于维护版本
     author="Goodenough",  # 作者，可以写自己的姓名
     author_email="2381642961@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="Doing experiments in the physics lab AR by python",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://gitee.com/script2000/physicsLab",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

