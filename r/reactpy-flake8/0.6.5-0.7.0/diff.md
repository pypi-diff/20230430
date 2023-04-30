# Comparing `tmp/reactpy_flake8-0.6.5-py3-none-any.whl.zip` & `tmp/reactpy_flake8-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9561 bytes, number of entries: 12
--rw-r--r--  2.0 unx      426 b- defN 23-Apr-30 03:48 reactpy_flake8/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 23-Apr-30 03:48 reactpy_flake8/common.py
--rw-r--r--  2.0 unx     7865 b- defN 23-Apr-30 03:48 reactpy_flake8/exhaustive_deps.py
--rw-r--r--  2.0 unx     2614 b- defN 23-Apr-30 03:48 reactpy_flake8/flake8_plugin.py
--rw-r--r--  2.0 unx     4662 b- defN 23-Apr-30 03:48 reactpy_flake8/rules_of_hooks.py
--rw-r--r--  2.0 unx      854 b- defN 23-Apr-30 03:48 reactpy_flake8/run.py
--rw-r--r--  2.0 unx     1083 b- defN 23-Apr-30 03:48 reactpy_flake8-0.6.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3517 b- defN 23-Apr-30 03:48 reactpy_flake8-0.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 03:48 reactpy_flake8-0.6.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-30 03:48 reactpy_flake8-0.6.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-30 03:48 reactpy_flake8-0.6.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1030 b- defN 23-Apr-30 03:48 reactpy_flake8-0.6.5.dist-info/RECORD
-12 files, 24006 bytes uncompressed, 7811 bytes compressed:  67.5%
+Zip file size: 9553 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      426 b- defN 23-Apr-30 04:05 reactpy_flake8/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 23-Apr-30 04:05 reactpy_flake8/common.py
+-rw-r--r--  2.0 unx     7865 b- defN 23-Apr-30 04:05 reactpy_flake8/exhaustive_deps.py
+-rw-r--r--  2.0 unx     2614 b- defN 23-Apr-30 04:05 reactpy_flake8/flake8_plugin.py
+-rw-r--r--  2.0 unx     4662 b- defN 23-Apr-30 04:05 reactpy_flake8/rules_of_hooks.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Apr-30 04:05 reactpy_flake8/run.py
+-rw-r--r--  2.0 unx     1083 b- defN 23-Apr-30 04:05 reactpy_flake8-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3517 b- defN 23-Apr-30 04:05 reactpy_flake8-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 04:05 reactpy_flake8-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Apr-30 04:05 reactpy_flake8-0.7.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-30 04:05 reactpy_flake8-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1030 b- defN 23-Apr-30 04:05 reactpy_flake8-0.7.0.dist-info/RECORD
+12 files, 24002 bytes uncompressed, 7803 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: reactpy_flake8/rules_of_hooks.py
 Comment: 
 
 Filename: reactpy_flake8/run.py
 Comment: 
 
-Filename: reactpy_flake8-0.6.5.dist-info/LICENSE
+Filename: reactpy_flake8-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: reactpy_flake8-0.6.5.dist-info/METADATA
+Filename: reactpy_flake8-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: reactpy_flake8-0.6.5.dist-info/WHEEL
+Filename: reactpy_flake8-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: reactpy_flake8-0.6.5.dist-info/entry_points.txt
+Filename: reactpy_flake8-0.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: reactpy_flake8-0.6.5.dist-info/top_level.txt
+Filename: reactpy_flake8-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: reactpy_flake8-0.6.5.dist-info/RECORD
+Filename: reactpy_flake8-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `reactpy_flake8-0.6.5.dist-info/LICENSE` & `reactpy_flake8-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `reactpy_flake8-0.6.5.dist-info/METADATA` & `reactpy_flake8-0.7.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-flake8
-Version: 0.6.5
+Version: 0.7.0
 Summary: Flake8 plugin to enforce the rules of hooks for ReactPy
 Home-page: https://github.com/reactive-python/reactpy-flake8
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Platform: Linux
 Platform: Mac OS X
@@ -13,15 +13,15 @@
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flake8 (>=3.7)
 Requires-Dist: black
 
 # `reactpy-flake8`
```

### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: reactpy-flake8 Version: 0.6.5 Summary: Flake8
+Metadata-Version: 2.1 Name: reactpy-flake8 Version: 0.7.0 Summary: Flake8
 plugin to enforce the rules of hooks for ReactPy Home-page: https://github.com/
 reactive-python/reactpy-flake8 Author: Ryan Morshead Author-email:
 ryan.morshead@gmail.com License: MIT Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Environment :: Console Classifier: Framework ::
 Flake8 Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Software
-Development :: Quality Assurance Requires-Python: >=3.6 Description-Content-
+Development :: Quality Assurance Requires-Python: >=3.7 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: flake8 (>=3.7)
 Requires-Dist: black # `reactpy-flake8` A Flake8 plugin that enforces the
 ["rules of hooks"](https://reactjs.org/docs/hooks-rules.html) for [ReactPy]
 (https://github.com/reactive-python/reactpy). The implementation is based on
 React's own ESLint [plugin for hooks](https://github.com/facebook/react/tree/
 master/packages/eslint-plugin-react-hooks). # Install ```bash pip install
 reactpy-flake8 ``` # Developer Installation ```bash pip install -
```

## Comparing `reactpy_flake8-0.6.5.dist-info/RECORD` & `reactpy_flake8-0.7.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 reactpy_flake8/__init__.py,sha256=QAwM8iwcbB9BJhozHoYapaKwApLa3GaOBJ6I5j1NdMk,426
 reactpy_flake8/common.py,sha256=o-dQxM67CbH5oZygf5qWY50_pCofaP8SsLn3UdHJ93E,1797
 reactpy_flake8/exhaustive_deps.py,sha256=Cp0GG8AHNwIM5ELHa-8ta823c8UkdEjfvOCoZgUraLQ,7865
 reactpy_flake8/flake8_plugin.py,sha256=qHa8XVlfGIlWzp4EJuKiV7KrFW3LL5SZvmodi_VP5EM,2614
 reactpy_flake8/rules_of_hooks.py,sha256=tvZ_RX4PfLAPtZlOb606XYzSeyVWSWIav5jom0cgz-E,4662
 reactpy_flake8/run.py,sha256=X9-Jo6IwopdWIs331g6qCJIvq-8ig4zh9O9GXGKEpoA,854
-reactpy_flake8-0.6.5.dist-info/LICENSE,sha256=2g6gYokLtgiM_s7J3Jv41vRMaEfQ_GgkvQ718EqXxdQ,1083
-reactpy_flake8-0.6.5.dist-info/METADATA,sha256=Wgq2la6X2-cUos6jq4KDDtIv6QoDwKrqnkvlLMg26Qc,3517
-reactpy_flake8-0.6.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-reactpy_flake8-0.6.5.dist-info/entry_points.txt,sha256=Sm1jyYEJVEq39SnEh5p91xSl2kiZqxuClP6DwXOYkuo,51
-reactpy_flake8-0.6.5.dist-info/top_level.txt,sha256=qZD2vkry1Ob5lpltNmDnew5fn4v-lOTigVKpHhzNnb8,15
-reactpy_flake8-0.6.5.dist-info/RECORD,,
+reactpy_flake8-0.7.0.dist-info/LICENSE,sha256=2g6gYokLtgiM_s7J3Jv41vRMaEfQ_GgkvQ718EqXxdQ,1083
+reactpy_flake8-0.7.0.dist-info/METADATA,sha256=r1_-0jCBAOEFzkH6xiUTEvRVEwMicfyq68yNmHy_geM,3517
+reactpy_flake8-0.7.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+reactpy_flake8-0.7.0.dist-info/entry_points.txt,sha256=i0Eglr5rRBzR7I6OweugeAIls3_kc_wgI0o3CyQ5zVQ,47
+reactpy_flake8-0.7.0.dist-info/top_level.txt,sha256=qZD2vkry1Ob5lpltNmDnew5fn4v-lOTigVKpHhzNnb8,15
+reactpy_flake8-0.7.0.dist-info/RECORD,,
```

