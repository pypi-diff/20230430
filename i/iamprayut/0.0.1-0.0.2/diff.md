# Comparing `tmp/iamprayut-0.0.1.tar.gz` & `tmp/iamprayut-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamprayut-0.0.1.tar", last modified: Sun Apr 30 07:18:31 2023, max compression
+gzip compressed data, was "iamprayut-0.0.2.tar", last modified: Sun Apr 30 07:57:10 2023, max compression
```

## Comparing `iamprayut-0.0.1.tar` & `iamprayut-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 07:18:31.292535 iamprayut-0.0.1/
--rw-rw-rw-   0        0        0     1063 2023-04-30 07:02:50.000000 iamprayut-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1084 2023-04-30 07:02:48.000000 iamprayut-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1581 2023-04-30 07:18:31.292535 iamprayut-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-04-30 07:12:53.000000 iamprayut-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 07:18:31.271264 iamprayut-0.0.1/iamprayut/
--rw-rw-rw-   0        0        0       35 2023-04-30 07:02:54.000000 iamprayut-0.0.1/iamprayut/__init__.py
--rw-rw-rw-   0        0        0     2307 2023-04-30 07:02:52.000000 iamprayut-0.0.1/iamprayut/prayut.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:18:31.290654 iamprayut-0.0.1/iamprayut.egg-info/
--rw-rw-rw-   0        0        0     1581 2023-04-30 07:18:31.000000 iamprayut-0.0.1/iamprayut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-30 07:18:31.000000 iamprayut-0.0.1/iamprayut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 07:18:31.000000 iamprayut-0.0.1/iamprayut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-30 07:18:31.000000 iamprayut-0.0.1/iamprayut.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-30 07:18:31.297524 iamprayut-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-04-30 07:06:11.000000 iamprayut-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 07:57:10.644691 iamprayut-0.0.2/
+-rw-rw-rw-   0        0        0     1063 2023-04-30 07:55:36.000000 iamprayut-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1084 2023-04-30 07:55:37.000000 iamprayut-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1603 2023-04-30 07:57:10.644691 iamprayut-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-04-30 07:55:41.000000 iamprayut-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 07:57:10.633681 iamprayut-0.0.2/iamprayut/
+-rw-rw-rw-   0        0        0       35 2023-04-30 07:55:33.000000 iamprayut-0.0.2/iamprayut/__init__.py
+-rw-rw-rw-   0        0        0     2753 2023-04-30 07:55:31.000000 iamprayut-0.0.2/iamprayut/prayut.py
+drwxrwxrwx   0        0        0        0 2023-04-30 07:57:10.643690 iamprayut-0.0.2/iamprayut.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-04-30 07:57:10.000000 iamprayut-0.0.2/iamprayut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-30 07:57:10.000000 iamprayut-0.0.2/iamprayut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 07:57:10.000000 iamprayut-0.0.2/iamprayut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-30 07:57:10.000000 iamprayut-0.0.2/iamprayut.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-30 07:57:10.645687 iamprayut-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2023-04-30 07:47:54.000000 iamprayut-0.0.2/setup.py
```

### Comparing `iamprayut-0.0.1/LICENSE` & `iamprayut-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamprayut-0.0.1/LICENSE.txt` & `iamprayut-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iamprayut-0.0.1/PKG-INFO` & `iamprayut-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: iamprayut
-Version: 0.0.1
+Version: 0.0.2
 Summary: Who is Prayut Chan-O-Cha
-Home-page: https://github.com/Prayut
-Download-URL: https://github.com/Prayut
+Home-page: https://github.com/Nissorn/iamprayut
+Download-URL: https://github.com/Nissorn/iamprayut
 Author: Prayut
 Author-email: prayut@proton.me
 License: MIT
 Keywords: Prayut,Uncle Engineer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Utilities
```

### Comparing `iamprayut-0.0.1/README.rst` & `iamprayut-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `iamprayut-0.0.1/iamprayut/prayut.py` & `iamprayut-0.0.2/iamprayut/prayut.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+import random
 class Prayut:
     """
     คลาสPrayutคือข้อมูลที่เกี่ยวข้องกับประยุทธ์ จันโอชา
+
+    mayor = Prayut() #Class
+    mayor.show_name() #show name
+    mayor.show_page() #show facebook page
+    mayor.about() #show about him
+    mayor.show_art() #show ascii art
+    mayor.dice()
     """
     def __init__(self):
         self.name = 'Prayut Chan-o-cha'
         self.page = 'https://www.facebook.com/prayutofficial/'
 
     def show_name(self):
         print(f'Hello my name is {self.name}')
@@ -34,16 +42,22 @@
         No Bullshit,          / |  / |       \______/
         Please...            \ |  \ |        \ |  \ |
                             __| |__| |      __| |__| |
                             |___||___|      |___||___|
         """
         print(text)
 
+    def dice(self):
+        dice_list = ['⚀','⚁','⚂','⚃','⚄','⚅']
+        first = random.choice(dice_list)
+        second = random.choice(dice_list)
+        print(f'Your dice is {first} {second}')
     
 
 
 if __name__ == '__main__':
     mayor = Prayut()
     mayor.show_name()
     mayor.show_page()
     mayor.about()
-    mayor.show_art()
+    mayor.show_art()
+    mayor.dice()
```

### Comparing `iamprayut-0.0.1/iamprayut.egg-info/PKG-INFO` & `iamprayut-0.0.2/iamprayut.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: iamprayut
-Version: 0.0.1
+Version: 0.0.2
 Summary: Who is Prayut Chan-O-Cha
-Home-page: https://github.com/Prayut
-Download-URL: https://github.com/Prayut
+Home-page: https://github.com/Nissorn/iamprayut
+Download-URL: https://github.com/Nissorn/iamprayut
 Author: Prayut
 Author-email: prayut@proton.me
 License: MIT
 Keywords: Prayut,Uncle Engineer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Utilities
```

### Comparing `iamprayut-0.0.1/setup.py` & `iamprayut-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'iamprayut',      
   packages = ['iamprayut'], 
-  version = '0.0.1', 
+  version = '0.0.2', 
   license='MIT', 
   description = 'Who is Prayut Chan-O-Cha',
   long_description=DESCRIPTION,
   author = 'Prayut',                 
   author_email = 'prayut@proton.me',     
-  url = 'https://github.com/Prayut',  
-  download_url = 'https://github.com/Prayut',  
+  url = 'https://github.com/Nissorn/iamprayut',  
+  download_url = 'https://github.com/Nissorn/iamprayut',  
   keywords = ['Prayut', 'Uncle Engineer'],
   classifiers=[
     'Development Status :: 3 - Alpha',     
     'Intended Audience :: Education',     
     'Topic :: Utilities',
     'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3',
```

