# Comparing `tmp/splittr-0.0.0.tar.gz` & `tmp/splittr-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splittr-0.0.0.tar", last modified: Fri Apr 28 17:16:13 2023, max compression
+gzip compressed data, was "splittr-0.0.1.tar", last modified: Sun Apr 30 13:34:53 2023, max compression
```

## Comparing `splittr-0.0.0.tar` & `splittr-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:16:13.245423 splittr-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 17:16:00.000000 splittr-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:16:13.245423 splittr-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 17:16:00.000000 splittr-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 17:16:13.245423 splittr-0.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3408 2023-04-28 17:16:00.000000 splittr-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:16:13.245423 splittr-0.0.0/splittr/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-28 17:16:00.000000 splittr-0.0.0/splittr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:16:13.245423 splittr-0.0.0/splittr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:16:13.000000 splittr-0.0.0/splittr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-28 17:16:13.000000 splittr-0.0.0/splittr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:16:13.000000 splittr-0.0.0/splittr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 17:16:13.000000 splittr-0.0.0/splittr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:34:53.963757 splittr-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-30 13:34:42.000000 splittr-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-30 13:34:53.963757 splittr-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-30 13:34:42.000000 splittr-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 13:34:53.963757 splittr-0.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3408 2023-04-30 13:34:42.000000 splittr-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:34:53.963757 splittr-0.0.1/splittr/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-30 13:34:42.000000 splittr-0.0.1/splittr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:34:53.963757 splittr-0.0.1/splittr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-30 13:34:53.000000 splittr-0.0.1/splittr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-30 13:34:53.000000 splittr-0.0.1/splittr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:34:53.000000 splittr-0.0.1/splittr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 13:34:53.000000 splittr-0.0.1/splittr.egg-info/top_level.txt
```

### Comparing `splittr-0.0.0/LICENSE` & `splittr-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splittr-0.0.0/setup.py` & `splittr-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.0"
+VERSION = "0.0.1"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `splittr-0.0.0/splittr/__init__.py` & `splittr-0.0.1/splittr/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,130 @@
-import os, sys, hashlib, zipfile
+import os, sys, hashlib, zipfile, jsons, shutil
 from glob import glob as re
 
-file = 'python_threeten'
-prefix = file.replace('.zip','') + '_broken_up_'
-hash_file = file + '.sums'
-CHUNK_SIZE =  1_000_000  #1MB for testing #100_000_000 #100MB
-hash_function = hashlib.sha1
-
-def create_zip_file(source_file, zip_file_name):
-    with zipfile.ZipFile(zip_file_name, 'w', compression=zipfile.ZIP_DEFLATED) as zip_file:
-        zip_file.write(source_file, source_file)
-
 def build():
     hash()
     split()
 
-def hash():
+def hash(foil, hash_function = hashlib.sha1):
     hashing = hash_function()
-    with open(file, 'rb') as f:
+    with open(foil, 'rb') as f:
         for chunk in iter(lambda: f.read(4096), b""):
             hashing.update(chunk)
-    with open(hash_file, 'a') as f:
-        f.write(hashing.hexdigest() + '  ' + file + '\n')
+    with open(foil + '.sums', 'a') as f:
+        json.dumps(
+            str({
+                "hash":hashing.hexdigest()
+            }),
+            f
+        )
+
+def verify(foil, hash_function = hashlib.sha1):
+    verified, set_hash = False, 0
+
+    with open(foil + '.sums', 'r') as f:
+        set_hash = json.loads(f)['hash']
 
-def verify():
-    print('Verifying the sums file')
     with open(hash, 'r') as f:
-        if not hash_function(open(file, 'rb').read()).hexdigest() == f.readline().split()[0]:
-            print("Hash doesn't match")
-            return
-    print("Hash matches")
+        verified = hash_function(open(foil, 'rb').read()).hexdigest() == set_hash:
+
+    if verified:
+        os.remove(foil + '.sums')
 
-def split():
+    return verified
+
+def split(foil, CHUNK_SIZE = 100_000_000): #100MB
     #https://www.tutorialspoint.com/How-to-spilt-a-binary-file-into-multiple-files-using-Python
     failure = False
     file_number = 1
-    with open(file,'rb') as f:
-        print("Starting to split")
+    with open(foil,'rb') as f:
         try:
             chunk = f.read(CHUNK_SIZE)
             while chunk:
 
-                current_file = prefix + str(str(file_number).zfill(6))
+                current_file = foil.replace('.zip','') + '_broken_up_' + str(str(file_number).zfill(10))
 
                 with open(current_file, "wb+") as chunk_file:
                     chunk_file.write(chunk)
 
-                create_zip_file(current_file, current_file+".zip")
+                with zipfile.ZipFile(current_file+".zip", 'w', compression=zipfile.ZIP_DEFLATED) as zip_file:
+                    zip_file.write(current_file, current_file)
+
                 os.remove(current_file)
                 file_number += 1
                 chunk = f.read(CHUNK_SIZE)
         except Exception as e:
             print(f"Exception :> {e}")
             failure = True
 
     if not failure:
-        os.remove(file)
+        os.remove(foil)
 
-"""
-with open('Output.bin', 'wb') as fp:
-    fp.write(input1)
-"""
-
-def join():
-    foils = re(prefix + "*.zip")
-    foils.sort()
+def join(foil):
+    mini_foils,current_binary = re(prefix + "*.zip"),None
+    mini_foils.sort()
     #https://stackoverflow.com/questions/62050356/merge-two-binary-files-into-third-binary-file
 
-    current_binary = None
-    for foil in foils:
-        raw_foil = foil.replace('.zip','')
-        print(foil)
-        print(raw_foil)
+    for mini_foil in mini_foils:
+        raw_foil = mini_foil.replace('.zip','')
 
-        with zipfile.ZipFile(foil,"r") as f:
+        with zipfile.ZipFile(mini_foil,"r") as f:
             f.extractall(members = [raw_foil])
 
         if current_binary is None:
             current_binary = open(raw_foil, 'rb').read()
         else:
             current_binary += open(raw_foil, 'rb').read()
 
-        [os.remove(x) for x in [foil, raw_foil]]
+        [os.remove(x) for x in [mini_foil, raw_foil]]
+
+    with open(foil, 'wb') as fp:
+        fp.write(current_binary)
 
+def arguments():
+    import argparse
+	parser = argparse.ArgumentParser(description=f"Enabling the capability to stretch a single large file into many smaller files")
+
+	parser.add_argument("-f","--file", help="The name of the file", nargs='*')
+	parser.add_argument("--split", help="Split the file up", action="store_true",default=False)
+	parser.add_argument("--join", help="Recreate the file", action="store_true",default=False)
+	parser.add_argument("--template", help="Create a copy of this file specific to a large file", action="store_true",default=False)
+
+	return parser.parse_args()
+
+def main(foil:str,splitfile:bool=False, joinfile:bool=False):
+    if splitfile:
+        hash(foil)
+        split(foil)
+    elif joinfile:
+        join(foil)
+        verify(foil)
+
+if __name__ == '__main__':
+    argz = arguments()
+    workingfoil = args.file[0]
+
+    if args.template:
+        contents = []
+        with open(__file__, "r") as reader:
+            contents = reader.readlines()
+
+        with open(foil + ".py", "w+") as writer:
+            for line in contents:
+                line = line.rstrip()
+                if "workingfoil = args.file[0]" in line:
+                    line = line.replace("args.file[0]", "\""+foil+"\"")
+        
+        print(foil + ".py")
+    else:
+        if args.split and args.join:
+            print("Cannot use both both split and join")
+            return
+        elif not os.path.exists(args.file[0])
+            print("The file {file} does not exist".format(file=args.file[0]))
+            return
 
-    with open(file, 'wb') as fp:
-        fp.write(current_binary)
+        main(
+            workingfoil,
+            splitfile=args.split,
+            joinfile=args.join,
+        )
```

