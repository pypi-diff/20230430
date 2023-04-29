# Comparing `tmp/ibonds-1.0.0.tar.gz` & `tmp/ibonds-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibonds-1.0.0.tar", last modified: Tue Apr 11 04:47:21 2023, max compression
+gzip compressed data, was "ibonds-1.0.1.tar", last modified: Sat Apr 29 23:52:47 2023, max compression
```

## Comparing `ibonds-1.0.0.tar` & `ibonds-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-11 04:47:21.363296 ibonds-1.0.0/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1071 2023-04-03 03:32:07.000000 ibonds-1.0.0/LICENSE
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       35 2023-04-11 04:27:26.000000 ibonds-1.0.0/MANIFEST.in
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1854 2023-04-11 04:47:21.363296 ibonds-1.0.0/PKG-INFO
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1311 2023-04-11 04:42:03.000000 ibonds-1.0.0/README.md
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-11 04:47:21.363296 ibonds-1.0.0/ibonds/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     6888 2023-04-11 04:02:39.000000 ibonds-1.0.0/ibonds/__init__.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1302 2023-04-07 04:29:48.000000 ibonds-1.0.0/ibonds/interest_rates.yaml
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-11 04:47:21.363296 ibonds-1.0.0/ibonds.egg-info/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1854 2023-04-11 04:47:21.000000 ibonds-1.0.0/ibonds.egg-info/PKG-INFO
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      254 2023-04-11 04:47:21.000000 ibonds-1.0.0/ibonds.egg-info/SOURCES.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        1 2023-04-11 04:47:21.000000 ibonds-1.0.0/ibonds.egg-info/dependency_links.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       27 2023-04-11 04:47:21.000000 ibonds-1.0.0/ibonds.egg-info/requires.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        7 2023-04-11 04:47:21.000000 ibonds-1.0.0/ibonds.egg-info/top_level.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       38 2023-04-11 04:47:21.363296 ibonds-1.0.0/setup.cfg
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1004 2023-04-11 04:46:17.000000 ibonds-1.0.0/setup.py
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-11 04:47:21.363296 ibonds-1.0.0/tests/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     5032 2023-04-10 07:29:46.000000 ibonds-1.0.0/tests/test_ibonds.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-29 23:52:47.983502 ibonds-1.0.1/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1071 2023-04-03 03:32:07.000000 ibonds-1.0.1/LICENSE
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       35 2023-04-11 04:27:26.000000 ibonds-1.0.1/MANIFEST.in
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1854 2023-04-29 23:52:47.980169 ibonds-1.0.1/PKG-INFO
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1311 2023-04-11 04:42:03.000000 ibonds-1.0.1/README.md
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-29 23:52:47.980169 ibonds-1.0.1/ibonds/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     6966 2023-04-11 05:01:51.000000 ibonds-1.0.1/ibonds/__init__.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1328 2023-04-29 00:47:18.000000 ibonds-1.0.1/ibonds/interest_rates.yaml
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-29 23:52:47.980169 ibonds-1.0.1/ibonds.egg-info/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1854 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/PKG-INFO
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      254 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        1 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       27 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/requires.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        7 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/top_level.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       38 2023-04-29 23:52:47.983502 ibonds-1.0.1/setup.cfg
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1004 2023-04-29 23:52:21.000000 ibonds-1.0.1/setup.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-29 23:52:47.980169 ibonds-1.0.1/tests/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     5108 2023-04-29 00:54:03.000000 ibonds-1.0.1/tests/test_ibonds.py
```

### Comparing `ibonds-1.0.0/LICENSE` & `ibonds-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibonds-1.0.0/PKG-INFO` & `ibonds-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibonds
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to calculate the current value of a Series I savings bond
 Home-page: https://github.com/sarvjeets/ibonds
 Author: Sarvjeet Singh
 Author-email: sarvjeet@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ibonds-1.0.0/README.md` & `ibonds-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ibonds-1.0.0/ibonds/__init__.py` & `ibonds-1.0.1/ibonds/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,18 +159,19 @@
 
     def value(self, d=date.today()):
         """Returns value of this I Bond on date d."""
         assert (d - self.issue_date) >= timedelta(days=1), (
             f'Cannot compute value on {d} which is before the issue date '
             f'{self.issue_date}')
 
-        # All bond values are multiple of $25 bond
+        # All bond values are multiple of $25 bond.
         value_25 = 25.0
         value_on = _YearMonth(self.issue_date.year, self.issue_date.month)
         months_left = _YearMonth(d.year, d.month) - value_on
+        months_left = min(months_left, 12 * 30)  # No interest after 30 yrs.
 
         if months_left < 12 * 5:   # 5 year penalty
             months_left -= 3
             if months_left < 0:
                 months_left = 0
 
         # Rate changes every 6 months. Interest accrues monthly and compounds
```

### Comparing `ibonds-1.0.0/ibonds/interest_rates.yaml` & `ibonds-1.0.1/ibonds/interest_rates.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -144,7 +144,10 @@
 - 3.56
 2022-05-01:
 - 0.00
 - 4.81
 2022-11-01:
 - 0.40
 - 3.24
+2023-05-01:
+- 0.90
+- 1.69
```

### Comparing `ibonds-1.0.0/ibonds.egg-info/PKG-INFO` & `ibonds-1.0.1/ibonds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibonds
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to calculate the current value of a Series I savings bond
 Home-page: https://github.com/sarvjeets/ibonds
 Author: Sarvjeet Singh
 Author-email: sarvjeet@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ibonds-1.0.0/setup.py` & `ibonds-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='ibonds',
-    version='1.0.0',
+    version='1.0.1',
     author='Sarvjeet Singh',
     author_email='sarvjeet@gmail.com',
     description=('Library to calculate the current value of a '
                  'Series I savings bond'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sarvjeets/ibonds',
```

### Comparing `ibonds-1.0.0/tests/test_ibonds.py` & `ibonds-1.0.1/tests/test_ibonds.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import unittest
 from datetime import date
 
 from ibonds import IBond, InterestRates, _YearMonth
 
-INTEREST_RATE_DATA = """2021-05-01:
+INTEREST_RATE_DATA = """
+2020-11-01:
+- 0.00
+- 0.84
+2021-05-01:
 - 0.00
 - 1.77
 2021-11-01:
 - 0.00
 - 3.56
 2022-05-01:
 - 0.00
@@ -98,15 +102,16 @@
         d = _YearMonth(2022, 12) + 1
         self.assertEqual(date(2023, 1, 1), d.date())
 
         d = _YearMonth(2022, 11) + 6
         self.assertEqual(date(2023, 5, 1), d.date())
 
     def test_ibond_composite_rate(self):
-        ib = IBond('01/2021', 100)
+        i = InterestRates(INTEREST_RATE_DATA)
+        ib = IBond('01/2021', 100, i)
         self.assertEqual(6.48, ib.composite_rate(date(2023, 5, 1)))
         self.assertIsNone(ib.composite_rate(date(2023, 7, 1)))
 
     def test_value_with_bad_date(self):
         with self.assertRaisesRegex(
             AssertionError, 'Cannot compute value on 2023-03-12 which is '
                             'before the issue date 2023-04-01'):
```

