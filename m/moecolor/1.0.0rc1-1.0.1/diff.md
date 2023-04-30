# Comparing `tmp/moecolor-1.0.0rc1.tar.gz` & `tmp/moecolor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moecolor-1.0.0rc1.tar", last modified: Sat Dec 31 02:56:37 2022, max compression
+gzip compressed data, was "dist\moecolor-1.0.1.tar", last modified: Sun Apr 30 05:37:14 2023, max compression
```

## Comparing `moecolor-1.0.0rc1.tar` & `moecolor-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-31 02:56:37.044904 moecolor-1.0.0rc1/
--rw-rw-rw-   0        0        0     7522 2022-12-31 02:56:37.043907 moecolor-1.0.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0     5728 2022-12-31 02:45:50.000000 moecolor-1.0.0rc1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-31 02:56:37.018974 moecolor-1.0.0rc1/moecolor/
--rw-rw-rw-   0        0        0     5660 2022-12-31 02:56:01.000000 moecolor-1.0.0rc1/moecolor/README.py
--rw-rw-rw-   0        0        0     1259 2022-12-31 01:02:51.000000 moecolor-1.0.0rc1/moecolor/__init__.py
--rw-rw-rw-   0        0        0     9710 2022-12-31 02:56:21.000000 moecolor-1.0.0rc1/moecolor/main.py
--rw-rw-rw-   0        0        0       25 2022-12-31 02:56:34.000000 moecolor-1.0.0rc1/moecolor/version.py
-drwxrwxrwx   0        0        0        0 2022-12-31 02:56:37.042908 moecolor-1.0.0rc1/moecolor.egg-info/
--rw-rw-rw-   0        0        0     7522 2022-12-31 02:56:36.000000 moecolor-1.0.0rc1/moecolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2022-12-31 02:56:36.000000 moecolor-1.0.0rc1/moecolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-31 02:56:36.000000 moecolor-1.0.0rc1/moecolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-12-31 02:56:36.000000 moecolor-1.0.0rc1/moecolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-31 02:56:37.045902 moecolor-1.0.0rc1/setup.cfg
--rw-rw-rw-   0        0        0     1246 2022-12-31 02:47:04.000000 moecolor-1.0.0rc1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:37:14.000000 moecolor-1.0.1/
+-rw-rw-rw-   0        0        0     7518 2023-04-30 05:37:14.000000 moecolor-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5728 2023-01-04 04:46:32.000000 moecolor-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 05:37:14.000000 moecolor-1.0.1/moecolor/
+-rw-rw-rw-   0        0        0     5660 2023-01-04 04:46:32.000000 moecolor-1.0.1/moecolor/README.py
+-rw-rw-rw-   0        0        0      152 2023-02-22 01:27:35.000000 moecolor-1.0.1/moecolor/__init__.py
+-rw-rw-rw-   0        0        0     9767 2023-04-30 05:36:39.000000 moecolor-1.0.1/moecolor/main.py
+-rw-rw-rw-   0        0        0     1196 2023-04-30 05:37:02.000000 moecolor-1.0.1/moecolor/version.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:37:14.000000 moecolor-1.0.1/moecolor.egg-info/
+-rw-rw-rw-   0        0        0     7518 2023-04-30 05:37:14.000000 moecolor-1.0.1/moecolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-30 05:37:14.000000 moecolor-1.0.1/moecolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 05:37:14.000000 moecolor-1.0.1/moecolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 05:37:14.000000 moecolor-1.0.1/moecolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 05:37:14.000000 moecolor-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1245 2023-02-22 04:15:58.000000 moecolor-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `moecolor-1.0.0rc1/PKG-INFO` & `moecolor-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: moecolor
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: Python Libary to print colored and styled text in terminal. Offers color-specific configuration by providing 24bit hex or RGB values as well 256-color mode.
 Home-page: https://github.com/mhamdan91/moecolor
 Author: mhamdan91 (Hamdan, Muhammad)
-Author-email: <mhamdan-91@hotmail.com>
+Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Moecolor (Flexible terminal text coloring and styling)
         =======================================================
         ## Table of Contents
         
          * [Overview](#overview)
          * [Library Installalion](#library-installalion)
@@ -113,15 +113,15 @@
         
         Windows terminals (CMD, PS) support most of attributes, but the following ['blink', 'dim']
         LINUX terminals support all AFAIK
         """
         ```
         
         ----------------------------------------
-        Author: Hamdan, Muhammad (@mhamdan91 - آ©)
+        Author: Hamdan, Muhammad (@mhamdan91 - Â©)
         
 Keywords: python,color,terminal,text,styling,ansi,coloring text,text styling,text formatting,formatting
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `moecolor-1.0.0rc1/README.md` & `moecolor-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `moecolor-1.0.0rc1/moecolor/README.py` & `moecolor-1.0.1/moecolor/README.py`

 * *Files identical despite different names*

### Comparing `moecolor-1.0.0rc1/moecolor/__init__.py` & `moecolor-1.0.1/moecolor/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from .main import print, FormatText, CLEAR_SCREEN
-from .version import __version__
-__author__ = "Muhammad Hamdan <mhamdan-91@hotmail.com>"
+__version__ = "1.0.1"
+__author__ = "Muhammad Hamdan <mhamdan.dev@gmail.com>"
 __copyright__ = """
 MIT License
 
 Copyright (c) 2022 Muhammad Hamdan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `moecolor-1.0.0rc1/moecolor/main.py` & `moecolor-1.0.1/moecolor/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,21 +210,22 @@
             v2 = word2vec(color)
             shared = v1[0].intersection(v2[0])
             # Cos(x, y) = x . y / ||x|| * ||y||
             scores[color] = sum(v1[1][ch]*v2[1][ch] for ch in shared)/v1[2]/v2[2]
         scores = sorted(scores.items(), key=lambda item:item[1], reverse=True)
         return AVAILABLE_COLORS[scores[0][0]] if scores[0][1] > 0.5 else -1
 
-def print(text: str='', color: typing.Any='DEFAULT', attr: typing.Iterable=[], **kwargs):
+def print(text: str='', *args, color: typing.Any='DEFAULT', attr: typing.Iterable=[], **kwargs):
     usage = False
     possible_help = ['h', 'usage', 'show_help', 'help_me', 'use']
     if set(possible_help).intersection(kwargs):
         for h in possible_help:
             if h in kwargs:
                 del kwargs[h]
         usage = True
+    text = (text + ' ' + ' '.join(args)).strip()
     formatted_text = FormatText(text, color, attr=attr, usage=usage)
     if not usage:
         osprint(formatted_text, **kwargs)
 
 print.__doc__ = LONG_DESCRIPTION
 FormatText.__doc__ = LONG_DESCRIPTION
```

### Comparing `moecolor-1.0.0rc1/moecolor.egg-info/PKG-INFO` & `moecolor-1.0.1/moecolor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: moecolor
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: Python Libary to print colored and styled text in terminal. Offers color-specific configuration by providing 24bit hex or RGB values as well 256-color mode.
 Home-page: https://github.com/mhamdan91/moecolor
 Author: mhamdan91 (Hamdan, Muhammad)
-Author-email: <mhamdan-91@hotmail.com>
+Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Moecolor (Flexible terminal text coloring and styling)
         =======================================================
         ## Table of Contents
         
          * [Overview](#overview)
          * [Library Installalion](#library-installalion)
@@ -113,15 +113,15 @@
         
         Windows terminals (CMD, PS) support most of attributes, but the following ['blink', 'dim']
         LINUX terminals support all AFAIK
         """
         ```
         
         ----------------------------------------
-        Author: Hamdan, Muhammad (@mhamdan91 - آ©)
+        Author: Hamdan, Muhammad (@mhamdan91 - Â©)
         
 Keywords: python,color,terminal,text,styling,ansi,coloring text,text styling,text formatting,formatting
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `moecolor-1.0.0rc1/setup.py` & `moecolor-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
               'Offers color-specific configuration by providing 24bit hex '  \
               'or RGB values as well 256-color mode.'
 LONG_DESCRIPTION = open('README.md').read()
 setup(
     name="moecolor",
     version=VERSION,
     author="mhamdan91 (Hamdan, Muhammad)",
-    author_email="<mhamdan-91@hotmail.com>",
+    author_email="<mhamdan.dev@gmail.com>",
     url='https://github.com/mhamdan91/moecolor',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     keywords=['python', 'color', 'terminal', 'text', 'styling', 'ansi',
               'coloring text', 'text styling', 'text formatting', 'formatting'],
```

