# Comparing `tmp/picods-0.1.5.tar.gz` & `tmp/picods-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picods-0.1.5.tar", max compression
+gzip compressed data, was "picods-0.1.6.tar", max compression
```

## Comparing `picods-0.1.5.tar` & `picods-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3157 2023-04-28 12:58:26.332181 picods-0.1.5/README.md
--rw-r--r--   0        0        0       93 2023-04-28 12:58:26.332181 picods-0.1.5/picods/__init__.py
--rw-r--r--   0        0        0       51 2023-04-28 12:58:26.332181 picods-0.1.5/picods/plot/__init__.py
--rw-r--r--   0        0        0      988 2023-04-28 12:58:26.332181 picods-0.1.5/picods/plot/plot.py
--rw-r--r--   0        0        0       54 2023-04-28 12:58:26.332181 picods-0.1.5/picods/table/__init__.py
--rw-r--r--   0        0        0      856 2023-04-28 12:58:26.332181 picods-0.1.5/picods/table/table.py
--rw-r--r--   0        0        0      418 2023-04-28 12:58:55.528330 picods-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 picods-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3157 2023-04-30 19:24:59.880106 picods-0.1.6/README.md
+-rw-r--r--   0        0        0       93 2023-04-30 19:24:59.880106 picods-0.1.6/picods/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-30 19:24:59.880106 picods-0.1.6/picods/plot/__init__.py
+-rw-r--r--   0        0        0      988 2023-04-30 19:24:59.880106 picods-0.1.6/picods/plot/plot.py
+-rw-r--r--   0        0        0       54 2023-04-30 19:24:59.880106 picods-0.1.6/picods/table/__init__.py
+-rw-r--r--   0        0        0      856 2023-04-30 19:24:59.880106 picods-0.1.6/picods/table/table.py
+-rw-r--r--   0        0        0      418 2023-04-30 19:25:23.648452 picods-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 picods-0.1.6/PKG-INFO
```

### Comparing `picods-0.1.5/README.md` & `picods-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `picods-0.1.5/picods/plot/plot.py` & `picods-0.1.6/picods/plot/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,11 +38,11 @@
 
     if x_lim:
         plt.xlim(0, x_lim)
     if y_lim:
         plt.ylim(0, y_lim)
 
     for x, y, color in zip(xs, ys, colors):
-        plt.plot(y, x, color=color)
+        plt.plot(x, y, color=color)
 
     plt.legend(legends)
     plt.show()
```

### Comparing `picods-0.1.5/picods/table/table.py` & `picods-0.1.6/picods/table/table.py`

 * *Files identical despite different names*

### Comparing `picods-0.1.5/PKG-INFO` & `picods-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picods
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pico Data Science: A small, personal use case, Data Science library.
 License: MIT
 Author: Pablo
 Author-email: pablohuggem@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

