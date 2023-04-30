# Comparing `tmp/bnconverter-0.0.2.tar.gz` & `tmp/bnconverter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnconverter-0.0.2.tar", last modified: Sat Apr 29 07:45:30 2023, max compression
+gzip compressed data, was "bnconverter-0.0.3.tar", last modified: Sun Apr 30 19:01:13 2023, max compression
```

## Comparing `bnconverter-0.0.2.tar` & `bnconverter-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 nadeem     (501) staff       (20)        0 2023-04-29 07:45:30.567573 bnconverter-0.0.2/
--rw-r--r--   0 nadeem     (501) staff       (20)     1476 2023-04-29 07:45:30.567178 bnconverter-0.0.2/PKG-INFO
--rw-r--r--   0 nadeem     (501) staff       (20)      902 2023-04-29 07:11:22.000000 bnconverter-0.0.2/README.md
-drwxr-xr-x   0 nadeem     (501) staff       (20)        0 2023-04-29 07:45:30.563451 bnconverter-0.0.2/bnconverter.egg-info/
--rw-r--r--   0 nadeem     (501) staff       (20)     1476 2023-04-29 07:45:30.000000 bnconverter-0.0.2/bnconverter.egg-info/PKG-INFO
--rw-r--r--   0 nadeem     (501) staff       (20)      257 2023-04-29 07:45:30.000000 bnconverter-0.0.2/bnconverter.egg-info/SOURCES.txt
--rw-r--r--   0 nadeem     (501) staff       (20)        1 2023-04-29 07:45:30.000000 bnconverter-0.0.2/bnconverter.egg-info/dependency_links.txt
--rw-r--r--   0 nadeem     (501) staff       (20)        6 2023-04-29 07:45:30.000000 bnconverter-0.0.2/bnconverter.egg-info/requires.txt
--rw-r--r--   0 nadeem     (501) staff       (20)       10 2023-04-29 07:45:30.000000 bnconverter-0.0.2/bnconverter.egg-info/top_level.txt
-drwxr-xr-x   0 nadeem     (501) staff       (20)        0 2023-04-29 07:45:30.565882 bnconverter-0.0.2/bnunicode/
--rw-r--r--   0 nadeem     (501) staff       (20)       50 2023-04-29 07:35:34.000000 bnconverter-0.0.2/bnunicode/__init__.py
--rw-r--r--   0 nadeem     (501) staff       (20)      711 2023-04-29 07:08:22.000000 bnconverter-0.0.2/bnunicode/bnconverter.py
--rw-r--r--   0 nadeem     (501) staff       (20)    20390 2023-04-26 13:06:04.000000 bnconverter-0.0.2/bnunicode/util.py
--rw-r--r--   0 nadeem     (501) staff       (20)       38 2023-04-29 07:45:30.567707 bnconverter-0.0.2/setup.cfg
--rw-r--r--   0 nadeem     (501) staff       (20)     1122 2023-04-29 07:36:28.000000 bnconverter-0.0.2/setup.py
+drwxr-xr-x   0 nadeem     (501) staff       (20)        0 2023-04-30 19:01:13.744134 bnconverter-0.0.3/
+-rw-r--r--   0 nadeem     (501) staff       (20)     1476 2023-04-30 19:01:13.743478 bnconverter-0.0.3/PKG-INFO
+-rw-r--r--   0 nadeem     (501) staff       (20)      901 2023-04-30 18:48:08.000000 bnconverter-0.0.3/README.md
+drwxr-xr-x   0 nadeem     (501) staff       (20)        0 2023-04-30 19:01:13.739848 bnconverter-0.0.3/bnconverter.egg-info/
+-rw-r--r--   0 nadeem     (501) staff       (20)     1476 2023-04-30 19:01:13.000000 bnconverter-0.0.3/bnconverter.egg-info/PKG-INFO
+-rw-r--r--   0 nadeem     (501) staff       (20)      339 2023-04-30 19:01:13.000000 bnconverter-0.0.3/bnconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 nadeem     (501) staff       (20)        1 2023-04-30 19:01:13.000000 bnconverter-0.0.3/bnconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 nadeem     (501) staff       (20)        6 2023-04-30 19:01:13.000000 bnconverter-0.0.3/bnconverter.egg-info/requires.txt
+-rw-r--r--   0 nadeem     (501) staff       (20)       10 2023-04-30 19:01:13.000000 bnconverter-0.0.3/bnconverter.egg-info/top_level.txt
+drwxr-xr-x   0 nadeem     (501) staff       (20)        0 2023-04-30 19:01:13.740639 bnconverter-0.0.3/bnunicode/
+-rw-r--r--   0 nadeem     (501) staff       (20)       40 2023-04-30 18:50:37.000000 bnconverter-0.0.3/bnunicode/__init__.py
+-rw-r--r--   0 nadeem     (501) staff       (20)      699 2023-04-30 18:59:19.000000 bnconverter-0.0.3/bnunicode/bnunibtob.py
+drwxr-xr-x   0 nadeem     (501) staff       (20)        0 2023-04-30 19:01:13.742704 bnconverter-0.0.3/bnunicode/util/
+-rw-r--r--   0 nadeem     (501) staff       (20)       60 2023-04-30 18:39:33.000000 bnconverter-0.0.3/bnunicode/util/__init__.py
+-rw-r--r--   0 nadeem     (501) staff       (20)    16530 2023-04-30 18:09:40.000000 bnconverter-0.0.3/bnunicode/util/common.py
+-rw-r--r--   0 nadeem     (501) staff       (20)      711 2023-04-30 18:33:03.000000 bnconverter-0.0.3/bnunicode/util/decode.py
+-rw-r--r--   0 nadeem     (501) staff       (20)     1131 2023-04-30 18:32:43.000000 bnconverter-0.0.3/bnunicode/util/encode.py
+-rw-r--r--   0 nadeem     (501) staff       (20)       38 2023-04-30 19:01:13.744319 bnconverter-0.0.3/setup.cfg
+-rw-r--r--   0 nadeem     (501) staff       (20)     1122 2023-04-30 18:53:29.000000 bnconverter-0.0.3/setup.py
```

### Comparing `bnconverter-0.0.2/PKG-INFO` & `bnconverter-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnconverter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python converting Bangla <=> Unicode (UTF-8) for Bengali to Bangla.
 Author: Nazrul Islam (Nadeem)
 Author-email: <nazrul.devs@gmail.com>
 Keywords: python,converting,Unicode,Bengali to Bangla
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bnconverter-0.0.2/README.md` & `bnconverter-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     result=data.convertBnUniCodeToDecode(unicode_bangla_text)
     print(result)
     # আমার সোনার বাংলা, আমি তোমায় ভালোবাসি। চিরদিন তোমার আকাশ, তোমার বাতাস, আমার প্রাণে বাজায় বাঁশি॥
     toPrint=test.convertBnUniCodeToDecode(result)
     print(toPrint)
 
 ## References:
-https://github.com/sh-sabbir/UnicodeToBijoy
+https://github.com/sh-sabbir/UnicodeToBijoy
```

### Comparing `bnconverter-0.0.2/bnconverter.egg-info/PKG-INFO` & `bnconverter-0.0.3/bnconverter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnconverter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python converting Bangla <=> Unicode (UTF-8) for Bengali to Bangla.
 Author: Nazrul Islam (Nadeem)
 Author-email: <nazrul.devs@gmail.com>
 Keywords: python,converting,Unicode,Bengali to Bangla
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bnconverter-0.0.2/bnunicode/bnconverter.py` & `bnconverter-0.0.3/bnunicode/bnunibtob.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 class UnicodeStreaming:
 
     # main conversion def
     def convertBnUniCodeToDecode(self, srcString):
         if not srcString:
             return srcString
 
-        srcString = util.doCharMapDecode(srcString)
+        srcString = util.uniDecode(srcString)
         return srcString
 
     def convertBnUniCodeToEncode(self, srcString):
         if not srcString:
             return srcString
-        srcString = util.doCharMapEncode(srcString)
+        srcString = util.uniEncode(srcString)
         
         return srcString
     
     def bnReplaceUniCodeFont(self,srcString):
         convertEncodeText= self.convertBnUniCodeToEncode(srcString)
         convertDecodeTxt = self.convertBnUniCodeToDecode(convertEncodeText)
         return convertDecodeTxt
```

### Comparing `bnconverter-0.0.2/setup.py` & `bnconverter-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Python converting Bangla <=> Unicode (UTF-8) for Bengali to Bangla.'
 LONG_DESCRIPTION = 'Python converting Bangla <=> Unicode (UTF-8) for Bengali to Bangla.'
 
 # Setting up
 setup(
     name="bnconverter",
     version=VERSION,
```

