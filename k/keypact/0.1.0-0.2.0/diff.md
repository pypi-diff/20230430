# Comparing `tmp/keypact-0.1.0.tar.gz` & `tmp/keypact-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.1.0.tar", last modified: Sun Apr 23 16:51:15 2023, max compression
+gzip compressed data, was "keypact-0.2.0.tar", last modified: Sun Apr 30 11:22:31 2023, max compression
```

## Comparing `keypact-0.1.0.tar` & `keypact-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:51:15.588070 keypact-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-23 16:51:05.000000 keypact-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-23 16:51:15.588070 keypact-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 16:51:05.000000 keypact-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:51:15.588070 keypact-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-23 16:51:05.000000 keypact-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:51:15.584070 keypact-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:51:15.584070 keypact-0.1.0/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 16:51:05.000000 keypact-0.1.0/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-23 16:51:05.000000 keypact-0.1.0/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:51:15.588070 keypact-0.1.0/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-23 16:51:15.000000 keypact-0.1.0/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-23 16:51:15.000000 keypact-0.1.0/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:51:15.000000 keypact-0.1.0/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 16:51:15.000000 keypact-0.1.0/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:51:15.000000 keypact-0.1.0/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 16:51:15.000000 keypact-0.1.0/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 16:51:15.000000 keypact-0.1.0/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:22:31.332641 keypact-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-30 11:22:14.000000 keypact-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-30 11:22:31.332641 keypact-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-30 11:22:14.000000 keypact-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 11:22:31.332641 keypact-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-30 11:22:14.000000 keypact-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:22:31.332641 keypact-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:22:31.332641 keypact-0.2.0/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-30 11:22:14.000000 keypact-0.2.0/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-30 11:22:14.000000 keypact-0.2.0/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 11:22:31.332641 keypact-0.2.0/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-30 11:22:31.000000 keypact-0.2.0/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-30 11:22:31.000000 keypact-0.2.0/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:22:31.000000 keypact-0.2.0/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-30 11:22:31.000000 keypact-0.2.0/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 11:22:31.000000 keypact-0.2.0/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 11:22:31.000000 keypact-0.2.0/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 11:22:31.000000 keypact-0.2.0/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.1.0/LICENSE` & `keypact-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.1.0/PKG-INFO` & `keypact-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.1.0
+Version: 0.2.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -39,18 +39,18 @@
         
         print(my_keypact.get("Onur"))
         ```
         
         ### Console
         
         ```console	
-        keypact client_addresses set Onur Sivas
+        keypact --name=client_addresses set Onur Sivas
         ```
         ```console
-        keypact client_addresses get Onur
+        keypact --name=client_addresses get Onur
         ```
         
         
         ## Contributing
         Contributions to Keypact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
         
         ## License
```

### Comparing `keypact-0.1.0/README.md` & `keypact-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 
 print(my_keypact.get("Onur"))
 ```
 
 ### Console
 
 ```console	
-keypact client_addresses set Onur Sivas
+keypact --name=client_addresses set Onur Sivas
 ```
 ```console
-keypact client_addresses get Onur
+keypact --name=client_addresses get Onur
 ```
 
 
 ## Contributing
 Contributions to Keypact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
 
 ## License
```

### Comparing `keypact-0.1.0/setup.py` & `keypact-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.1.0',
+version='0.2.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `keypact-0.1.0/src/keypact/keypact.py` & `keypact-0.2.0/src/keypact/keypact.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,29 +28,56 @@
 
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
 
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
 
         with open(os.path.join(self.location, key_location), "wb") as f:
-            pickle.dump(value, f)
+            pickle.dump({"key":key,"value":value}, f)
 
-    def get(self, key: str):
-        key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
+    def get(self, key: str, custom_key_location: str = None):
+        key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == None else custom_key_location
 
         if not os.path.isfile(os.path.join(self.location, key_location)):
             raise FileNotFoundError("Key not found")
 
         with open(os.path.join(self.location, key_location), "rb") as f:
-            return pickle.load(f)
-        
+            result = pickle.load(f)
+            try:
+                total_result = result["value"]
+            except TypeError:
+                total_result = result
+            return total_result
+
+    def get_key(self, key_location: str):
+       
+
+        if not os.path.isfile(os.path.join(self.location, key_location)):
+            raise FileNotFoundError("Key not found")
+
+        with open(os.path.join(self.location, key_location), "rb") as f:
+            result = pickle.load(f)
+            try:
+                total_result = result["key"]
+            except TypeError:
+                total_result = False
+            return total_result
+
     def delete(self, key: str):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
 
         try:
             os.remove(os.path.join(self.location, key_location))
         except OSError:
             pass
 
 
+    def dict(self):
+        result ={}
+        for key in os.listdir(self.location):
+            the_key = self.get_key(key)
+            if the_key != False:
+                result[the_key] = self.get(the_key)
+        return result
+
 def main():
     fire.Fire(KeyPact)
```

### Comparing `keypact-0.1.0/src/keypact.egg-info/PKG-INFO` & `keypact-0.2.0/src/keypact.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.1.0
+Version: 0.2.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -39,18 +39,18 @@
         
         print(my_keypact.get("Onur"))
         ```
         
         ### Console
         
         ```console	
-        keypact client_addresses set Onur Sivas
+        keypact --name=client_addresses set Onur Sivas
         ```
         ```console
-        keypact client_addresses get Onur
+        keypact --name=client_addresses get Onur
         ```
         
         
         ## Contributing
         Contributions to Keypact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
         
         ## License
```

