# Comparing `tmp/Musicreater-0.5.0.1.tar.gz` & `tmp/Musicreater-0.5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-0.5.0.1.tar", last modified: Sat Apr 29 14:03:46 2023, max compression
+gzip compressed data, was "Musicreater-0.5.0.2.tar", last modified: Sun Apr 30 14:35:44 2023, max compression
```

## Comparing `Musicreater-0.5.0.1.tar` & `Musicreater-0.5.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 14:03:46.510571 Musicreater-0.5.0.1/
--rw-rw-rw-   0        0        0    13085 2023-02-05 09:39:58.000000 Musicreater-0.5.0.1/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-29 14:03:46.497614 Musicreater-0.5.0.1/Musicreater/
--rw-rw-rw-   0        0        0      892 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     3197 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0     5479 2023-04-29 11:13:55.000000 Musicreater-0.5.0.1/Musicreater/instConstants.py
--rw-rw-rw-   0        0        0    10696 2023-04-29 11:13:55.000000 Musicreater-0.5.0.1/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    80322 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/Musicreater/main.py
--rw-rw-rw-   0        0        0    13451 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 14:03:46.507581 Musicreater-0.5.0.1/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     7618 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7618 2023-04-29 14:03:46.509574 Musicreater-0.5.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6547 2023-04-29 11:13:55.000000 Musicreater-0.5.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 14:03:46.510571 Musicreater-0.5.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1597 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 14:35:44.345693 Musicreater-0.5.0.2/
+-rw-rw-rw-   0        0        0    13085 2023-02-05 09:39:58.000000 Musicreater-0.5.0.2/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-04-30 14:35:44.328693 Musicreater-0.5.0.2/Musicreater/
+-rw-rw-rw-   0        0        0      892 2023-04-30 14:34:46.000000 Musicreater-0.5.0.2/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     3197 2023-04-29 13:59:22.000000 Musicreater-0.5.0.2/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0     5479 2023-04-29 11:13:55.000000 Musicreater-0.5.0.2/Musicreater/instConstants.py
+-rw-rw-rw-   0        0        0    10696 2023-04-29 11:13:55.000000 Musicreater-0.5.0.2/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    80374 2023-04-30 14:34:46.000000 Musicreater-0.5.0.2/Musicreater/main.py
+-rw-rw-rw-   0        0        0    13570 2023-04-30 14:34:46.000000 Musicreater-0.5.0.2/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-30 14:35:44.342693 Musicreater-0.5.0.2/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     7618 2023-04-30 14:35:43.000000 Musicreater-0.5.0.2/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-30 14:35:44.000000 Musicreater-0.5.0.2/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 14:35:43.000000 Musicreater-0.5.0.2/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-30 14:35:43.000000 Musicreater-0.5.0.2/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 14:35:43.000000 Musicreater-0.5.0.2/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7618 2023-04-30 14:35:44.344693 Musicreater-0.5.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6547 2023-04-30 14:34:46.000000 Musicreater-0.5.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 14:35:44.345693 Musicreater-0.5.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1597 2023-04-29 13:59:22.000000 Musicreater-0.5.0.2/setup.py
```

### Comparing `Musicreater-0.5.0.1/LICENSE.md` & `Musicreater-0.5.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0.1/Musicreater/__init__.py` & `Musicreater-0.5.0.2/Musicreater/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 版权所有 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & 鸣凤鸽子("MingFengPigeon")
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 from .main import *
 
-__version__ = "0.5.0.1"
+__version__ = "0.5.0.2"
 __all__ = []
 __author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"), ("鸣凤鸽子", "MingFengPigeon"))
```

### Comparing `Musicreater-0.5.0.1/Musicreater/exceptions.py` & `Musicreater-0.5.0.2/Musicreater/exceptions.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0.1/Musicreater/instConstants.py` & `Musicreater-0.5.0.2/Musicreater/instConstants.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0.1/Musicreater/magicmain.py` & `Musicreater-0.5.0.2/Musicreater/magicmain.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0.1/Musicreater/main.py` & `Musicreater-0.5.0.2/Musicreater/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1588,14 +1588,16 @@
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
         :param volume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return 成功与否，成功返回(True,未经过压缩的源,结构占用大小)，失败返回(False,str失败原因)
         """
+        
+        from TrimMCStruct import Structure
 
         if self.enable_old_exe_format:
             raise CommandFormatError("使用mcstructure结构文件导出时不支持旧版本的指令格式。")
 
         command_list, max_delay = self.methods_byDelay[method - 1](
             volume,
             speed,
```

### Comparing `Musicreater-0.5.0.1/Musicreater/utils.py` & `Musicreater-0.5.0.2/Musicreater/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import math
 import os
 
-from TrimMCStruct import Structure, Block, TAG_Long, TAG_Byte
 
 bdx_key = {
     "x": [b"\x0f", b"\x0e", b"\x1c", b"\x14", b"\x15"],
     "y": [b"\x11", b"\x10", b"\x1d", b"\x16", b"\x17"],
     "z": [b"\x13", b"\x12", b"\x1e", b"\x18", b"\x19"],
 }
 """key存储了方块移动指令的数据，其中可以用key[x|y|z][0|1]来表示xyz的减或增
@@ -237,14 +236,15 @@
     :param instrument: `str`
         音符盒的乐器
     :param powered: `bool`
         是否已被激活
     :return Block
     """
 
+    from TrimMCStruct import Block, TAG_Byte
     return Block(
         "minecraft",
         "noteblock",
         {
             "instrument": instrument.replace("note.", ""),
             "note": note,
             "powered": powered,
@@ -266,14 +266,16 @@
 ):
     """生成中继器方块
     :param powered:
     :param locked:
     :param facing:
     :param delay: 1~4
     :return Block()"""
+    
+    from TrimMCStruct import Block
 
     return Block(
         "minecraft",
         "unpowered_repeater",
         {
             "repeater_delay": delay,
             "direction": facing,
@@ -334,14 +336,17 @@
         首刻执行(循环指令方块是否激活后立即执行，若为False，则从激活时起延迟后第一次执行)
     :param trackOutput: `bool`
         是否输出
 
     :return:str
     """
 
+    
+    from TrimMCStruct import Block, TAG_Long
+
     return Block(
         "minecraft",
         "command_block"
         if impluse == 0
         else ("repeating_command_block" if impluse == 1 else "chain_command_block"),
         states={"conditional_bit": condition, "facing_direction": particularValue},
         extra_data={
@@ -380,14 +385,17 @@
 ):
     """
     :param commands: 指令列表(指令, 延迟)
     :param max_height: 生成结构最大高度
     :return 成功与否，成功返回(结构类,结构占用大小)，失败返回(False,str失败原因)
     """
 
+    
+    from TrimMCStruct import Structure
+
     _sideLength = bottem_side_length_of_smallest_square_bottom_box(
         len(commands), max_height
     )
 
     struct = Structure(
         (_sideLength, max_height, _sideLength),  # 声明结构大小
     )
```

### Comparing `Musicreater-0.5.0.1/Musicreater.egg-info/PKG-INFO` & `Musicreater-0.5.0.2/Musicreater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.5.0.1
+Version: 0.5.0.2
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -146,10 +146,10 @@
 
 
 
 
 [Bilibili: 金羿ELS]: https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge
 [Bilibili: 诸葛亮与八卦阵]: https://img.shields.io/badge/Bilibili-%E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-00A1E7?style=for-the-badge
 [CodeStyle: black]: https://img.shields.io/badge/code%20style-black-121110.svg?style=for-the-badge
-[python]: https://img.shields.io/badge/python-3.6-AB70FF?style=for-the-badge
+[python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0.1 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0.2 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -88,11 +88,11 @@
 NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR
 MICROSOFT. [Bilibili: éç¾¿ELS]: https://img.shields.io/badge/Bilibili-
 %E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge [Bilibili:
 è¯¸èäº®ä¸å«å¦éµ]: https://img.shields.io/badge/Bilibili-
 %E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-
 00A1E7?style=for-the-badge [CodeStyle: black]: https://img.shields.io/badge/
 code%20style-black-121110.svg?style=for-the-badge [python]: https://
-img.shields.io/badge/python-3.6-AB70FF?style=for-the-badge [release]: https://
+img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge [release]: https://
 img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-
 badge
```

### Comparing `Musicreater-0.5.0.1/PKG-INFO` & `Musicreater-0.5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.5.0.1
+Version: 0.5.0.2
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -146,10 +146,10 @@
 
 
 
 
 [Bilibili: 金羿ELS]: https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge
 [Bilibili: 诸葛亮与八卦阵]: https://img.shields.io/badge/Bilibili-%E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-00A1E7?style=for-the-badge
 [CodeStyle: black]: https://img.shields.io/badge/code%20style-black-121110.svg?style=for-the-badge
-[python]: https://img.shields.io/badge/python-3.6-AB70FF?style=for-the-badge
+[python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0.1 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0.2 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -88,11 +88,11 @@
 NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR
 MICROSOFT. [Bilibili: éç¾¿ELS]: https://img.shields.io/badge/Bilibili-
 %E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge [Bilibili:
 è¯¸èäº®ä¸å«å¦éµ]: https://img.shields.io/badge/Bilibili-
 %E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-
 00A1E7?style=for-the-badge [CodeStyle: black]: https://img.shields.io/badge/
 code%20style-black-121110.svg?style=for-the-badge [python]: https://
-img.shields.io/badge/python-3.6-AB70FF?style=for-the-badge [release]: https://
+img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge [release]: https://
 img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-
 badge
```

### Comparing `Musicreater-0.5.0.1/README.md` & `Musicreater-0.5.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -124,10 +124,10 @@
 
 
 
 
 [Bilibili: 金羿ELS]: https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge
 [Bilibili: 诸葛亮与八卦阵]: https://img.shields.io/badge/Bilibili-%E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-00A1E7?style=for-the-badge
 [CodeStyle: black]: https://img.shields.io/badge/code%20style-black-121110.svg?style=for-the-badge
-[python]: https://img.shields.io/badge/python-3.6-AB70FF?style=for-the-badge
+[python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-badge
```

#### html2text {}

```diff
@@ -73,11 +73,11 @@
 NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR
 MICROSOFT. [Bilibili: éç¾¿ELS]: https://img.shields.io/badge/Bilibili-
 %E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge [Bilibili:
 è¯¸èäº®ä¸å«å¦éµ]: https://img.shields.io/badge/Bilibili-
 %E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-
 00A1E7?style=for-the-badge [CodeStyle: black]: https://img.shields.io/badge/
 code%20style-black-121110.svg?style=for-the-badge [python]: https://
-img.shields.io/badge/python-3.6-AB70FF?style=for-the-badge [release]: https://
+img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge [release]: https://
 img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-
 badge
```

### Comparing `Musicreater-0.5.0.1/setup.py` & `Musicreater-0.5.0.2/setup.py`

 * *Files identical despite different names*

