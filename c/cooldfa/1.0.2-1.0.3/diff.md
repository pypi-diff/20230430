# Comparing `tmp/cooldfa-1.0.2.tar.gz` & `tmp/cooldfa-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooldfa-1.0.2.tar", last modified: Sat Apr 22 15:49:51 2023, max compression
+gzip compressed data, was "cooldfa-1.0.3.tar", last modified: Sun Apr 30 01:55:05 2023, max compression
```

## Comparing `cooldfa-1.0.2.tar` & `cooldfa-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 cooldfa-1.0.2/LICENSE
--rw-r--r--   0        0        0     1985 2023-04-19 04:33:25.482492 cooldfa-1.0.2/README.md
--rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.2/cooldfa/__init__.py
--rw-r--r--   0        0        0     3692 2023-04-19 04:33:25.482492 cooldfa-1.0.2/cooldfa/_cooldfa.py
--rw-r--r--   0        0        0   478756 2023-04-03 17:12:39.903738 cooldfa-1.0.2/cooldfa/_words/others.json
--rw-r--r--   0        0        0    23166 2023-04-03 17:12:39.906737 cooldfa-1.0.2/cooldfa/_words/politics.json
--rw-r--r--   0        0        0    10325 2023-04-03 17:12:39.909739 cooldfa-1.0.2/cooldfa/_words/sex.json
--rw-r--r--   0        0        0   262857 2023-04-07 01:51:58.429386 cooldfa-1.0.2/cooldfa/_words/url.json
--rw-r--r--   0        0        0     4015 2023-04-03 17:12:39.929739 cooldfa-1.0.2/cooldfa/_words/violence.json
--rw-r--r--   0        0        0      547 2023-04-22 15:46:27.072378 cooldfa-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 cooldfa-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 cooldfa-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1985 2023-04-19 04:33:25.482492 cooldfa-1.0.3/README.md
+-rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.3/cooldfa/__init__.py
+-rw-r--r--   0        0        0     3661 2023-04-30 01:06:28.124524 cooldfa-1.0.3/cooldfa/_cooldfa.py
+-rw-r--r--   0        0        0   478756 2023-04-03 17:12:39.903738 cooldfa-1.0.3/cooldfa/_words/others.json
+-rw-r--r--   0        0        0    23166 2023-04-03 17:12:39.906737 cooldfa-1.0.3/cooldfa/_words/politics.json
+-rw-r--r--   0        0        0    10325 2023-04-03 17:12:39.909739 cooldfa-1.0.3/cooldfa/_words/sex.json
+-rw-r--r--   0        0        0   262857 2023-04-07 01:51:58.429386 cooldfa-1.0.3/cooldfa/_words/url.json
+-rw-r--r--   0        0        0     4015 2023-04-03 17:12:39.929739 cooldfa-1.0.3/cooldfa/_words/violence.json
+-rw-r--r--   0        0        0      547 2023-04-30 01:53:19.907400 cooldfa-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 cooldfa-1.0.3/PKG-INFO
```

### Comparing `cooldfa-1.0.2/LICENSE` & `cooldfa-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.2/README.md` & `cooldfa-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.2/cooldfa/_cooldfa.py` & `cooldfa-1.0.3/cooldfa/_cooldfa.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,31 +3,37 @@
 license: Apache License, Version 2.0
 email: lcctoor@outlook.com
 '''
 
 from copy import deepcopy
 from json import loads
 from pathlib import Path
+from typing import Any
 
 
 # 预置忽略词
 preset_ignore_words = set('''
     `-_=~!@#$%^&*()+[ ]\\{}|;\',./:"<>?·！￥…（）—【】、；‘：“，。《》？
     ～＆＠＃”’〝〞＂＇´﹞﹝＞＜«»‹›〔〕〈〉』『〗〖｝｛」「］［︵︷︹︿︽﹁﹃︻︗＼｜／︘︼﹄﹂︾﹀︺︸︶＿﹏﹍﹎
     \n\r \t¦¡\xad¨ˊ¯￣﹋﹉﹊ˋ︴¿ˇ\u3000
 '''.lower())
 
 # 预置敏感词
 words_dir = Path(__file__).parent / '_words'
-class preset_words:
-    politics = loads((words_dir / 'politics.json').read_text('utf8'))
-    sex = loads((words_dir / 'sex.json').read_text('utf8'))
-    violence = loads((words_dir / 'violence.json').read_text('utf8'))
-    url = loads((words_dir / 'url.json').read_text('utf8'))
-    others = loads((words_dir / 'others.json').read_text('utf8'))
+class PresetWords:
+    politics: list
+    sex: list
+    violence: list
+    url: list
+    others: list
+
+    def __getattr__(self, name):
+        self.__setattr__(name, loads((words_dir / f'{name}.json').read_text('utf8')))
+        return self.__dict__[name]
+preset_words = PresetWords()
 
 # dfa算法
 class dfa():
     ignore_words = preset_ignore_words
     tree = {}
 
     def __init__(self, *words_lists):
```

### Comparing `cooldfa-1.0.2/cooldfa/_words/others.json` & `cooldfa-1.0.3/cooldfa/_words/others.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.2/cooldfa/_words/politics.json` & `cooldfa-1.0.3/cooldfa/_words/politics.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.2/cooldfa/_words/sex.json` & `cooldfa-1.0.3/cooldfa/_words/sex.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.2/cooldfa/_words/url.json` & `cooldfa-1.0.3/cooldfa/_words/url.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.2/cooldfa/_words/violence.json` & `cooldfa-1.0.3/cooldfa/_words/violence.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.2/pyproject.toml` & `cooldfa-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "cooldfa"
-version = "1.0.2"
+version = "1.0.3"
 description = "一个基于DFA算法的敏感词检测器"
 dependencies = []
 keywords = ["cooldfa", "dfa"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `cooldfa-1.0.2/PKG-INFO` & `cooldfa-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cooldfa
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一个基于DFA算法的敏感词检测器
 Keywords: cooldfa,dfa
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/cooldfa
```

