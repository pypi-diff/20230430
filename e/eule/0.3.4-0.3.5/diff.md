# Comparing `tmp/eule-0.3.4.tar.gz` & `tmp/eule-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eule-0.3.4.tar", max compression
+gzip compressed data, was "eule-0.3.5.tar", max compression
```

## Comparing `eule-0.3.4.tar` & `eule-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-0.3.4/LICENSE
--rw-r--r--   0        0        0     1794 2023-03-19 15:49:57.253200 eule-0.3.4/README.md
--rw-r--r--   0        0        0      205 2023-03-27 14:19:19.843506 eule-0.3.4/eule/__init__.py
--rw-r--r--   0        0        0     5684 2023-04-17 21:01:38.628319 eule-0.3.4/eule/eule.py
--rw-r--r--   0        0        0     2841 2023-04-17 20:46:01.004663 eule-0.3.4/eule/utils.py
--rw-r--r--   0        0        0     1358 2023-04-17 21:02:16.396466 eule-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 eule-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1873 2023-04-23 22:40:19.368385 eule-0.3.5/README.md
+-rw-r--r--   0        0        0      222 2023-04-30 12:36:21.742153 eule-0.3.5/eule/__init__.py
+-rw-r--r--   0        0        0     5697 2023-04-18 19:12:36.364911 eule-0.3.5/eule/eule.py
+-rw-r--r--   0        0        0     2856 2023-04-18 19:12:36.364911 eule-0.3.5/eule/utils.py
+-rw-r--r--   0        0        0     1358 2023-04-30 12:37:25.166400 eule-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2942 1970-01-01 00:00:00.000000 eule-0.3.5/PKG-INFO
```

### Comparing `eule-0.3.4/LICENSE` & `eule-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eule-0.3.4/README.md` & `eule-0.3.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -42,10 +42,18 @@
     'b': [2, 3, 4],
     'c': [3, 4, 5],
     'd': [3, 5, 6]
 }
 
 diagram = eule.euler(set)
 
-# Euler dictionary: {'a,b': [2], 'b,c': [4], 'a,b,c,d': [3], 'c,d': [5], 'd': [6], 'a': [1]}
+# Euler dictionary:
+# {
+#     ('a', 'b'): [2], 
+#     ('b', 'c'): [4], 
+#     ('a', 'b', 'c', 'd'): [3], 
+#     ('d',): [6], 
+#     ('c', 'd'): [5], 
+#     ('a',): [1]
+# }
 print(diagram)
 ```
```

### Comparing `eule-0.3.4/eule/eule.py` & `eule-0.3.5/eule/eule.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         msg_2 = 'It must be either a dict or array of arrays object!'
         raise TypeError(msg_1 + msg_2)
 
     is_unique_set_arr = [
         len(uniq(values)) == len(values) for values in sets_.values()
     ]
 
-    and_map = lambda a, b: a and b
+    def and_map(a, b):
+        return (a and b)
 
     if not reduc(and_map, is_unique_set_arr, True):
         warn('Each array MUST NOT have duplicates')
         sets = {key: uniq(values) for key, values in sets.items()}
 
     # Only a set
     if len(sets_.keys()) == 1:
```

### Comparing `eule-0.3.4/eule/utils.py` & `eule-0.3.5/eule/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 def clear(sets):
     """This map returns a set with non-empty values
 
     :param dict set:  
     :returns: a set universe with  
     :rtype: dict
     """
-    non_empty_mask=lambda key: len(sets[key]) != 0
+    def non_empty_mask(key):
+        return (len(sets[key]) != 0)
 
     return list(filter(non_empty_mask, sets.keys(), ),)
 
 def update_tuple(tuple_, value):
     """This map updates and sorts a tuple with a value
 
     :param tuple of elements:
```

### Comparing `eule-0.3.4/pyproject.toml` & `eule-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eule"
-version = "0.3.4"
+version = "0.3.5"
 description = "Euler diagrams in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "eule"}]
 homepage = "https://pypi.org/project/eule/"
 repository = "https://github.com/trouchet/eule"
```

### Comparing `eule-0.3.4/PKG-INFO` & `eule-0.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eule
-Version: 0.3.4
+Version: 0.3.5
 Summary: Euler diagrams in python
 Home-page: https://pypi.org/project/eule/
 License: MIT
 Keywords: euler-diagram,sets
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -70,11 +70,19 @@
     'b': [2, 3, 4],
     'c': [3, 4, 5],
     'd': [3, 5, 6]
 }
 
 diagram = eule.euler(set)
 
-# Euler dictionary: {'a,b': [2], 'b,c': [4], 'a,b,c,d': [3], 'c,d': [5], 'd': [6], 'a': [1]}
+# Euler dictionary:
+# {
+#     ('a', 'b'): [2], 
+#     ('b', 'c'): [4], 
+#     ('a', 'b', 'c', 'd'): [3], 
+#     ('d',): [6], 
+#     ('c', 'd'): [5], 
+#     ('a',): [1]
+# }
 print(diagram)
 ```
```

