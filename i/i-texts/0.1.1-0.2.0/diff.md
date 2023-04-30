# Comparing `tmp/i-texts-0.1.1.tar.gz` & `tmp/i-texts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i-texts-0.1.1.tar", last modified: Fri Apr 14 18:55:54 2023, max compression
+gzip compressed data, was "i-texts-0.2.0.tar", last modified: Sun Apr 30 06:46:42 2023, max compression
```

## Comparing `i-texts-0.1.1.tar` & `i-texts-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0       48 2023-04-14 17:47:10.481893 i-texts-0.1.1/i_texts/__init__.py
--rw-r--r--   0        0        0      710 2023-04-14 18:54:17.413781 i-texts-0.1.1/i_texts/core.py
--rw-r--r--   0        0        0      169 2023-04-14 18:21:43.478803 i-texts-0.1.1/i_texts/main.py
--rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 i-texts-0.1.1/i_texts/py.typed
--rw-r--r--   0        0        0      491 2023-04-14 18:55:13.631243 i-texts-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      434 2023-04-14 18:55:44.354629 i-texts-0.1.1/README.md
--rw-r--r--   0        0        0      214 2023-04-14 18:54:29.966911 i-texts-0.1.1/tests/__main__.py
--rw-r--r--   0        0        0       48 2023-04-14 18:53:06.818508 i-texts-0.1.1/tests/locales/ru.yml
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 i-texts-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-04-14 17:47:10.481893 i-texts-0.2.0/i_texts/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-14 18:54:17.413781 i-texts-0.2.0/i_texts/core.py
+-rw-r--r--   0        0        0      246 2023-04-30 06:32:44.638490 i-texts-0.2.0/i_texts/main.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 i-texts-0.2.0/i_texts/py.typed
+-rw-r--r--   0        0        0      645 2023-04-30 06:46:26.780845 i-texts-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-04-30 06:40:39.299330 i-texts-0.2.0/README.md
+-rw-r--r--   0        0        0      214 2023-04-14 18:54:29.966911 i-texts-0.2.0/tests/__main__.py
+-rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 i-texts-0.2.0/PKG-INFO
```

### Comparing `i-texts-0.1.1/i_texts/core.py` & `i-texts-0.2.0/i_texts/core.py`

 * *Files identical despite different names*

### Comparing `i-texts-0.1.1/PKG-INFO` & `i-texts-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: i-texts
-Version: 0.1.1
+Version: 0.2.0
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# I18n texts loader
-
 Use `pip install i-texts`
 
-- Requires `LOCALE` and `LOCALES_PATH` (default: `./locales`) environment variables.
-- Loads texts from "{`LOCALES_PATH`}/{`LOCALE`}.yml"
+**Requires:**
+
+- or `$TEXTS_PATH`
+- or `$LOCALE` and `$LOCALES_PATH` (default: `./locales`).
+
+**Loads texts from:**
+
+- or `$TEXTS_PATH`
+- or {`$LOCALES_PATH`}/{`$LOCALE`}.yml"
 
-## Example
+### Example
 
 ```py
 from i_texts import texts
 
 assert texts.dict == {1: "1", "a": "a", "words": "a b c", "ru": "русский"}
 assert texts[1] == "1"
 assert texts["a"] == "a"
```

