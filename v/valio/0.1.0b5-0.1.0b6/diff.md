# Comparing `tmp/valio-0.1.0b5.tar.gz` & `tmp/valio-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valio-0.1.0b5.tar", max compression
+gzip compressed data, was "valio-0.1.0b6.tar", max compression
```

## Comparing `valio-0.1.0b5.tar` & `valio-0.1.0b6.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1061 2022-06-27 14:25:44.856917 valio-0.1.0b5/LICENSE
--rw-r--r--   0        0        0      559 2022-07-25 04:01:38.207751 valio-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0      319 2022-07-25 04:01:01.957750 valio-0.1.0b5/valio/__init__.py
--rwxr-xr-x   0        0        0      149 2022-06-27 14:28:24.819166 valio-0.1.0b5/valio/descriptor/__init__.py
--rwxr-xr-x   0        0        0    11812 2022-06-27 14:41:25.628061 valio-0.1.0b5/valio/descriptor/descriptors.py
--rwxr-xr-x   0        0        0      144 2022-06-27 14:28:39.539012 valio-0.1.0b5/valio/error/__init__.py
--rwxr-xr-x   0        0        0     2906 2022-06-27 14:32:02.132994 valio-0.1.0b5/valio/error/errors.py
--rwxr-xr-x   0        0        0      144 2022-06-27 20:09:16.877522 valio-0.1.0b5/valio/field/__init__.py
--rwxr-xr-x   0        0        0    29720 2022-06-27 20:10:31.581408 valio-0.1.0b5/valio/field/fields.py
--rwxr-xr-x   0        0        0      145 2022-06-27 14:32:24.492267 valio-0.1.0b5/valio/logger/__init__.py
--rwxr-xr-x   0        0        0    19928 2022-06-27 14:41:48.058072 valio-0.1.0b5/valio/logger/color_format.py
--rwxr-xr-x   0        0        0     6505 2022-06-27 16:20:55.105806 valio-0.1.0b5/valio/logger/loggers.py
--rwxr-xr-x   0        0        0      164 2022-06-27 14:33:32.166750 valio-0.1.0b5/valio/regexer/__init__.py
--rwxr-xr-x   0        0        0    17621 2022-06-27 17:10:39.464428 valio-0.1.0b5/valio/regexer/regexps.py
--rwxr-xr-x   0        0        0      373 2022-07-24 15:36:56.199330 valio-0.1.0b5/valio/regexer/relib/__init__.py
--rw-r--r--   0        0        0     1244 2022-06-27 14:34:10.286175 valio-0.1.0b5/valio/regexer/relib/aadhaarcard.py
--rw-r--r--   0        0        0     3057 2022-07-25 04:02:42.131324 valio-0.1.0b5/valio/regexer/relib/colors.py
--rwxr-xr-x   0        0        0     2581 2022-06-27 14:34:34.734681 valio-0.1.0b5/valio/regexer/relib/control_chars.py
--rw-r--r--   0        0        0    14553 2022-07-24 15:35:18.754752 valio-0.1.0b5/valio/regexer/relib/dates.py
--rwxr-xr-x   0        0        0     1770 2022-06-27 14:34:57.610726 valio-0.1.0b5/valio/regexer/relib/emails.py
--rw-r--r--   0        0        0     8789 2022-06-27 14:35:14.205561 valio-0.1.0b5/valio/regexer/relib/ipaddresses.py
--rw-r--r--   0        0        0     4572 2022-07-08 07:31:29.262732 valio-0.1.0b5/valio/regexer/relib/pancard.py
--rwxr-xr-x   0        0        0     8381 2022-07-08 06:09:24.681383 valio-0.1.0b5/valio/regexer/relib/patterns.py
--rw-r--r--   0        0        0     5470 2022-06-27 14:36:00.625073 valio-0.1.0b5/valio/regexer/relib/paymentcards.py
--rwxr-xr-x   0        0        0     1185 2022-06-27 14:36:13.118994 valio-0.1.0b5/valio/regexer/relib/special_chars.py
--rwxr-xr-x   0        0        0      120 2022-06-27 14:39:41.985791 valio-0.1.0b5/valio/regexer/tests/__init__.py
--rwxr-xr-x   0        0        0     6979 2022-06-27 14:39:50.666718 valio-0.1.0b5/valio/regexer/tests/regex_test.py
--rwxr-xr-x   0        0        0      173 2022-06-27 14:37:40.471345 valio-0.1.0b5/valio/schema/__init__.py
--rwxr-xr-x   0        0        0     7975 2022-06-27 14:37:42.635628 valio-0.1.0b5/valio/schema/schemas.py
--rwxr-xr-x   0        0        0     5783 2022-06-27 14:37:06.246722 valio-0.1.0b5/valio/schema/schemas_v2.py
--rw-r--r--   0        0        0      120 2022-06-27 14:38:20.376411 valio-0.1.0b5/valio/tests/__init__.py
--rw-r--r--   0        0        0      122 2022-06-27 14:38:38.986662 valio-0.1.0b5/valio/tests/descriptor/__init__.py
--rw-r--r--   0        0        0     8808 2022-06-27 14:38:57.204799 valio-0.1.0b5/valio/tests/descriptor/test_descriptors.py
--rw-r--r--   0        0        0      122 2022-06-27 14:27:06.943999 valio-0.1.0b5/valio/tests/validator/__init__.py
--rw-r--r--   0        0        0    29851 2022-07-25 04:01:20.318761 valio-0.1.0b5/valio/tests/validator/test_validators.py
--rwxr-xr-x   0        0        0      148 2022-06-27 14:27:58.923439 valio-0.1.0b5/valio/validator/__init__.py
--rwxr-xr-x   0        0        0    76576 2022-07-25 03:00:23.471961 valio-0.1.0b5/valio/validator/validators.py
--rw-r--r--   0        0        0     1001 2022-07-25 04:07:28.735893 valio-0.1.0b5/setup.py
--rw-r--r--   0        0        0      458 2022-07-25 04:07:28.736533 valio-0.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-06-27 14:25:44.856917 valio-0.1.0b6/LICENSE
+-rw-r--r--   0        0        0      580 2023-04-30 19:02:33.955101 valio-0.1.0b6/pyproject.toml
+-rw-r--r--   0        0        0      320 2023-04-30 19:02:55.467050 valio-0.1.0b6/valio/__init__.py
+-rwxr-xr-x   0        0        0      149 2022-06-27 14:28:24.819166 valio-0.1.0b6/valio/descriptor/__init__.py
+-rwxr-xr-x   0        0        0    11812 2022-06-27 14:41:25.628061 valio-0.1.0b6/valio/descriptor/descriptors.py
+-rwxr-xr-x   0        0        0      144 2022-06-27 14:28:39.539012 valio-0.1.0b6/valio/error/__init__.py
+-rwxr-xr-x   0        0        0     2906 2022-06-27 14:32:02.132994 valio-0.1.0b6/valio/error/errors.py
+-rwxr-xr-x   0        0        0      144 2022-06-27 20:09:16.877522 valio-0.1.0b6/valio/field/__init__.py
+-rwxr-xr-x   0        0        0    29720 2022-06-27 20:10:31.581408 valio-0.1.0b6/valio/field/fields.py
+-rwxr-xr-x   0        0        0      145 2022-06-27 14:32:24.492267 valio-0.1.0b6/valio/logger/__init__.py
+-rwxr-xr-x   0        0        0    19928 2022-06-27 14:41:48.058072 valio-0.1.0b6/valio/logger/color_format.py
+-rwxr-xr-x   0        0        0     6505 2022-11-15 11:09:37.992219 valio-0.1.0b6/valio/logger/loggers.py
+-rwxr-xr-x   0        0        0      164 2022-06-27 14:33:32.166750 valio-0.1.0b6/valio/regexer/__init__.py
+-rwxr-xr-x   0        0        0    17621 2022-06-27 17:10:39.464428 valio-0.1.0b6/valio/regexer/regexps.py
+-rwxr-xr-x   0        0        0      373 2022-07-24 15:36:56.199330 valio-0.1.0b6/valio/regexer/relib/__init__.py
+-rw-r--r--   0        0        0     1244 2022-06-27 14:34:10.286175 valio-0.1.0b6/valio/regexer/relib/aadhaarcard.py
+-rw-r--r--   0        0        0     3057 2022-07-25 04:02:42.131324 valio-0.1.0b6/valio/regexer/relib/colors.py
+-rwxr-xr-x   0        0        0     2581 2022-06-27 14:34:34.734681 valio-0.1.0b6/valio/regexer/relib/control_chars.py
+-rw-r--r--   0        0        0    14553 2022-07-24 15:35:18.754752 valio-0.1.0b6/valio/regexer/relib/dates.py
+-rwxr-xr-x   0        0        0     1770 2022-06-27 14:34:57.610726 valio-0.1.0b6/valio/regexer/relib/emails.py
+-rw-r--r--   0        0        0     8789 2022-06-27 14:35:14.205561 valio-0.1.0b6/valio/regexer/relib/ipaddresses.py
+-rw-r--r--   0        0        0     4572 2022-07-08 07:31:29.262732 valio-0.1.0b6/valio/regexer/relib/pancard.py
+-rwxr-xr-x   0        0        0     8381 2022-07-08 06:09:24.681383 valio-0.1.0b6/valio/regexer/relib/patterns.py
+-rw-r--r--   0        0        0     5470 2022-06-27 14:36:00.625073 valio-0.1.0b6/valio/regexer/relib/paymentcards.py
+-rwxr-xr-x   0        0        0     1185 2022-06-27 14:36:13.118994 valio-0.1.0b6/valio/regexer/relib/special_chars.py
+-rwxr-xr-x   0        0        0      120 2022-06-27 14:39:41.985791 valio-0.1.0b6/valio/regexer/tests/__init__.py
+-rwxr-xr-x   0        0        0     6979 2022-06-27 14:39:50.666718 valio-0.1.0b6/valio/regexer/tests/regex_test.py
+-rwxr-xr-x   0        0        0      173 2022-06-27 14:37:40.471345 valio-0.1.0b6/valio/schema/__init__.py
+-rwxr-xr-x   0        0        0     7975 2022-06-27 14:37:42.635628 valio-0.1.0b6/valio/schema/schemas.py
+-rwxr-xr-x   0        0        0     5783 2022-06-27 14:37:06.246722 valio-0.1.0b6/valio/schema/schemas_v2.py
+-rw-r--r--   0        0        0      120 2022-06-27 14:38:20.376411 valio-0.1.0b6/valio/tests/__init__.py
+-rw-r--r--   0        0        0      122 2022-06-27 14:38:38.986662 valio-0.1.0b6/valio/tests/descriptor/__init__.py
+-rw-r--r--   0        0        0     8808 2022-06-27 14:38:57.204799 valio-0.1.0b6/valio/tests/descriptor/test_descriptors.py
+-rw-r--r--   0        0        0      122 2022-06-27 14:27:06.943999 valio-0.1.0b6/valio/tests/validator/__init__.py
+-rw-r--r--   0        0        0    29851 2022-07-25 04:01:20.318761 valio-0.1.0b6/valio/tests/validator/test_validators.py
+-rwxr-xr-x   0        0        0      148 2022-06-27 14:27:58.923439 valio-0.1.0b6/valio/validator/__init__.py
+-rwxr-xr-x   0        0        0    76576 2022-07-25 03:00:23.471961 valio-0.1.0b6/valio/validator/validators.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 valio-0.1.0b6/PKG-INFO
```

### Comparing `valio-0.1.0b5/LICENSE` & `valio-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/descriptor/descriptors.py` & `valio-0.1.0b6/valio/descriptor/descriptors.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/error/errors.py` & `valio-0.1.0b6/valio/error/errors.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/field/fields.py` & `valio-0.1.0b6/valio/field/fields.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/logger/color_format.py` & `valio-0.1.0b6/valio/logger/color_format.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/logger/loggers.py` & `valio-0.1.0b6/valio/logger/loggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             if not os.path.exists(folder_path):
                 os.makedirs(folder_path)
         else:
             folder_path.mkdir(parents=True, exist_ok=True)
         return folder_path
 
     def get_logger(self, subdir=None, record_prefix=None):
-        if self.logger is None or True:
+        if self.logger in [None, True]:
             module_name = os.path.splitext(
                 os.path.basename(sys.modules["__main__"].__file__)
             )[0]
             class_name = (
                 type(self).__name__
                 if subdir is None
                 else os.path.splitext(os.path.basename(subdir))[0]
```

### Comparing `valio-0.1.0b5/valio/regexer/regexps.py` & `valio-0.1.0b6/valio/regexer/regexps.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/aadhaarcard.py` & `valio-0.1.0b6/valio/regexer/relib/aadhaarcard.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/colors.py` & `valio-0.1.0b6/valio/regexer/relib/colors.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/control_chars.py` & `valio-0.1.0b6/valio/regexer/relib/control_chars.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/dates.py` & `valio-0.1.0b6/valio/regexer/relib/dates.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/emails.py` & `valio-0.1.0b6/valio/regexer/relib/emails.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/ipaddresses.py` & `valio-0.1.0b6/valio/regexer/relib/ipaddresses.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/pancard.py` & `valio-0.1.0b6/valio/regexer/relib/pancard.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/patterns.py` & `valio-0.1.0b6/valio/regexer/relib/patterns.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/paymentcards.py` & `valio-0.1.0b6/valio/regexer/relib/paymentcards.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/relib/special_chars.py` & `valio-0.1.0b6/valio/regexer/relib/special_chars.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/regexer/tests/regex_test.py` & `valio-0.1.0b6/valio/regexer/tests/regex_test.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/schema/schemas.py` & `valio-0.1.0b6/valio/schema/schemas.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/schema/schemas_v2.py` & `valio-0.1.0b6/valio/schema/schemas_v2.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/tests/descriptor/test_descriptors.py` & `valio-0.1.0b6/valio/tests/descriptor/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/tests/validator/test_validators.py` & `valio-0.1.0b6/valio/tests/validator/test_validators.py`

 * *Files identical despite different names*

### Comparing `valio-0.1.0b5/valio/validator/validators.py` & `valio-0.1.0b6/valio/validator/validators.py`

 * *Files identical despite different names*

