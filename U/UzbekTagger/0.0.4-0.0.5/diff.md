# Comparing `tmp/UzbekTagger-0.0.4.tar.gz` & `tmp/UzbekTagger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzbekTagger-0.0.4.tar", last modified: Mon Mar 13 13:17:40 2023, max compression
+gzip compressed data, was "UzbekTagger-0.0.5.tar", last modified: Sun Apr 30 09:21:21 2023, max compression
```

## Comparing `UzbekTagger-0.0.4.tar` & `UzbekTagger-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 13:17:40.538629 UzbekTagger-0.0.4/
--rw-rw-rw-   0        0        0    11558 2022-12-22 05:23:51.000000 UzbekTagger-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      480 2023-03-13 13:17:40.538629 UzbekTagger-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-03-02 11:43:55.000000 UzbekTagger-0.0.4/README.md
--rw-rw-rw-   0        0        0      461 2023-03-13 13:16:23.000000 UzbekTagger-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-13 13:17:40.538629 UzbekTagger-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-13 13:17:40.538629 UzbekTagger-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-13 13:17:40.538629 UzbekTagger-0.0.4/src/UzbekTagger/
--rw-rw-rw-   0        0        0     4590 2023-03-13 13:05:14.000000 UzbekTagger-0.0.4/src/UzbekTagger/UzbekTagger.py
--rw-rw-rw-   0        0        0        0 2023-03-01 09:00:01.000000 UzbekTagger-0.0.4/src/UzbekTagger/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-03-13 10:27:15.000000 UzbekTagger-0.0.4/src/UzbekTagger/service_to_uzbek_text.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:17:40.538629 UzbekTagger-0.0.4/src/UzbekTagger.egg-info/
--rw-rw-rw-   0        0        0      480 2023-03-13 13:17:40.000000 UzbekTagger-0.0.4/src/UzbekTagger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-03-13 13:17:40.000000 UzbekTagger-0.0.4/src/UzbekTagger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 13:17:40.000000 UzbekTagger-0.0.4/src/UzbekTagger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-03-13 13:17:40.000000 UzbekTagger-0.0.4/src/UzbekTagger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 09:21:21.255285 UzbekTagger-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2022-12-22 05:23:51.000000 UzbekTagger-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      716 2023-04-30 09:21:21.255285 UzbekTagger-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-03-02 11:43:55.000000 UzbekTagger-0.0.5/README.md
+-rw-rw-rw-   0        0        0      502 2023-04-30 03:43:09.000000 UzbekTagger-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 09:21:21.255285 UzbekTagger-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1213 2023-04-30 09:18:27.000000 UzbekTagger-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:21:21.218707 UzbekTagger-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 09:21:21.223991 UzbekTagger-0.0.5/src/UzbekTagger/
+-rw-rw-rw-   0        0        0     4687 2023-04-30 03:43:09.000000 UzbekTagger-0.0.5/src/UzbekTagger/UzbekTagger.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 03:55:06.000000 UzbekTagger-0.0.5/src/UzbekTagger/__init__.py
+-rw-rw-rw-   0        0        0     1339 2023-03-13 10:27:15.000000 UzbekTagger-0.0.5/src/UzbekTagger/service_to_uzbek_text.py
+-rw-rw-rw-   0        0        0  4038555 2023-04-30 03:38:16.000000 UzbekTagger-0.0.5/src/UzbekTagger/word.xml
+drwxrwxrwx   0        0        0        0 2023-04-30 09:21:21.255285 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/
+-rw-rw-rw-   0        0        0      716 2023-04-30 09:21:21.000000 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-30 09:21:21.000000 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 09:21:21.000000 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-30 09:21:21.000000 UzbekTagger-0.0.5/src/UzbekTagger.egg-info/top_level.txt
```

### Comparing `UzbekTagger-0.0.4/LICENSE` & `UzbekTagger-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `UzbekTagger-0.0.4/src/UzbekTagger/UzbekTagger.py` & `UzbekTagger-0.0.5/src/UzbekTagger/UzbekTagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from UzbekTagger import service_to_uzbek_text
+import service_to_uzbek_text
 import xml.etree.ElementTree as et
 from pathlib import Path
+from lxml import etree
+
 
 class pos:
     __this_directory = Path(__file__).parent
-    __dir = __this_directory.joinpath('Words.xml')
-    __tree = et.parse(__dir)
+    #__dir = __this_directory.joinpath('words.xml')
+    __tree = et.parse(__this_directory/"word.xml")
     __root = __tree.getroot()
+
     def __double_words(a):
 
         a = list(a)
         verb = ["edi", "ekan", "emish","kerak"]
         l1 = len(a)
         l2 = len(verb)
         i = 0
@@ -36,15 +39,15 @@
             i = i + 1
 
         return a
 
     def __check_with_affix(a):
         #a = list(a)
         verb = ['di', 'lan','lash','lashtir','lantir']
-        noun = ['lig', 'lik', 'vchi']
+        noun = ['lig', 'lik', 'vchi','ga','ka','qa','dan']
         for v in verb:
             if (v in a["affix"]):
                 if (a['pos'] == 'VERB'):
                     break
                 else:
                     a['pos'] = 'VERB'
         for v in noun:
@@ -77,16 +80,14 @@
                     a["affix"] = a["word"][l:]
                 elif (l > len(a["root"])):
                     a["pos"] = str(dic.attrib["classId"])
                     a["root"] = s
                     a["affix"] = a["word"][l:]
         return a
 
-
-
     def __check_with_lar(a, root):
         if(len(a['affix'])==0):
             return a
 
         if (str(a['root'])[-2:] == 'la') and (str(a['affix'])[0] == 'r'):
             b = {'word': a['root'][:-1], 'pos': "null", 'root': 'null', 'affix': 'null'}
             b = pos.__tag_word(b, root)
@@ -127,7 +128,9 @@
             for i in range(len(tagged_list)):
 
                 tagged_sent=tagged_sent+' '+tagged_list[i]['word']+'/'+tagged_list[i]['pos']
             tagged_sent=tagged_sent+' '+punk+'/PUNCT\n'
             tagged_text=tagged_text+tagged_sent
             #print(tagged_sent)
         return tagged_text
+
+#print(pos.tagger("Men bugun uyga bordim."))
```

### Comparing `UzbekTagger-0.0.4/src/UzbekTagger/service_to_uzbek_text.py` & `UzbekTagger-0.0.5/src/UzbekTagger/service_to_uzbek_text.py`

 * *Files identical despite different names*

