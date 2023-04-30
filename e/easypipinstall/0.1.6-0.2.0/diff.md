# Comparing `tmp/easypipinstall-0.1.6.tar.gz` & `tmp/easypipinstall-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypipinstall-0.1.6.tar", last modified: Tue Feb 14 15:29:03 2023, max compression
+gzip compressed data, was "easypipinstall-0.2.0.tar", last modified: Sun Apr 30 08:21:32 2023, max compression
```

## Comparing `easypipinstall-0.1.6.tar` & `easypipinstall-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-14 15:29:03.076387 easypipinstall-0.1.6/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 06:31:54.000000 easypipinstall-0.1.6/LICENSE
--rw-r--r--   0 nicolasdao   (501) staff       (20)     2585 2023-02-14 15:29:03.076456 easypipinstall-0.1.6/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1915 2023-02-14 15:27:54.000000 easypipinstall-0.1.6/README.md
--rw-r--r--   0 nicolasdao   (501) staff       (20)      179 2023-02-14 06:47:32.000000 easypipinstall-0.1.6/pyproject.toml
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1078 2023-02-14 15:29:03.076823 easypipinstall-0.1.6/setup.cfg
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-14 15:29:03.074732 easypipinstall-0.1.6/src/
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-14 15:29:03.075493 easypipinstall-0.1.6/src/easypipinstall/
--rw-r--r--   0 nicolasdao   (501) staff       (20)       48 2023-02-14 13:18:32.000000 easypipinstall-0.1.6/src/easypipinstall/__init__.py
--rw-r--r--   0 nicolasdao   (501) staff       (20)    10264 2023-02-14 14:52:55.000000 easypipinstall-0.1.6/src/easypipinstall/install.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-14 15:29:03.076277 easypipinstall-0.1.6/src/easypipinstall.egg-info/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     2585 2023-02-14 15:29:03.000000 easypipinstall-0.1.6/src/easypipinstall.egg-info/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)      357 2023-02-14 15:29:03.000000 easypipinstall-0.1.6/src/easypipinstall.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-02-14 15:29:03.000000 easypipinstall-0.1.6/src/easypipinstall.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       82 2023-02-14 15:29:03.000000 easypipinstall-0.1.6/src/easypipinstall.egg-info/entry_points.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       32 2023-02-14 15:29:03.000000 easypipinstall-0.1.6/src/easypipinstall.egg-info/requires.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       15 2023-02-14 15:29:03.000000 easypipinstall-0.1.6/src/easypipinstall.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:21:32.673605 easypipinstall-0.2.0/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 06:31:54.000000 easypipinstall-0.2.0/LICENSE
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    11843 2023-04-30 08:21:32.673671 easypipinstall-0.2.0/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    11174 2023-04-30 08:16:27.000000 easypipinstall-0.2.0/README.md
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      179 2023-02-14 06:47:32.000000 easypipinstall-0.2.0/pyproject.toml
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1091 2023-04-30 08:21:32.674047 easypipinstall-0.2.0/setup.cfg
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:21:32.671592 easypipinstall-0.2.0/src/
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:21:32.672723 easypipinstall-0.2.0/src/easypipinstall/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       85 2023-04-29 07:55:46.000000 easypipinstall-0.2.0/src/easypipinstall/__init__.py
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    10532 2023-04-29 15:37:21.000000 easypipinstall-0.2.0/src/easypipinstall/install.py
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    14295 2023-04-30 08:18:41.000000 easypipinstall-0.2.0/src/easypipinstall/version.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-30 08:21:32.673500 easypipinstall-0.2.0/src/easypipinstall.egg-info/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    11843 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      387 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       82 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/entry_points.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       32 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/requires.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       15 2023-04-30 08:21:32.000000 easypipinstall-0.2.0/src/easypipinstall.egg-info/top_level.txt
```

### Comparing `easypipinstall-0.1.6/LICENSE` & `easypipinstall-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easypipinstall-0.1.6/setup.cfg` & `easypipinstall-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easypipinstall
-version = 0.1.6
+version = 0.2.0
 author = Nicolas Dao
 author_email = nicolas.dao@gmail.com
 description = easypipinstall installs Python packages similarly to NPM in NodeJS. It automatically maintains the `requirements.txt`, `prod-requirements.txt` and `setup.cfg` files. It also easily uninstalls all the dependencies from those files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicolasdao/easypipinstall
 readme = README.md
@@ -32,14 +32,14 @@
 
 [options.entry_points]
 console_scripts = 
 	easyi = easypipinstall:install
 	easyu = easypipinstall:uninstall
 
 [flake8]
-extend-ignore = W191,E501,E302,E231,W291,E305,W391
-exclude = .git,__pycache__,.venv,build,dist
+extend-ignore = W191,E501,E302,E231,W291,E305,W391,E722
+exclude = .git,__pycache__,.venv,build,dist,test.py
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `easypipinstall-0.1.6/src/easypipinstall/install.py` & `easypipinstall-0.2.0/src/easypipinstall/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,35 +4,39 @@
 import re
 import os
 from functools import partial
 import importlib
 
 # Defines constants
 SETUP_FILE = "setup.cfg"
-LIB_COMPARATOR_REGEX = r"[>=<\n\s,]"
+LIB_COMPARATOR_REGEX = r"[>=<\r\n\s,]"
 GLOBAL_REQUIREMENTS = "requirements.txt"
 PROD_REQUIREMENTS = "prod-requirements.txt"
 PROD_SECTION = "options"
 PROD_SECTION_REQUIRE = "install_requires"
 DEV_SECTION = "options.extras_require"
 DEV_SECTION_REQUIRE = "dev"
 
 
 def getItems(s=""):
     """Gets the unique items in a list where the separator is a new line"""
     if not s:
         return ([], [])
-    items = list(set(x for x in re.split("\n", s) if x))
+    items = list(set(x for x in re.split(os.linesep, s) if x))
     names = [getLibNameOnly(x) for x in items]
     return (items, names)
 
 
-def freeze():
-    with open(GLOBAL_REQUIREMENTS, "w") as f:
-        f.write(subprocess.check_output(("pip", "freeze")).decode("UTF-8"))
+def freeze(inspect_only=False):
+    content = subprocess.check_output(("pip", "freeze")).decode("UTF-8")
+    if inspect_only:
+        print(content)
+    else:
+        with open(GLOBAL_REQUIREMENTS, "w") as f:
+            f.write(content)
 
 
 def getConfig(config, section, property):
     val = (
         ""
         if section not in config or property not in config[section]
         else config[section][property]
@@ -82,29 +86,28 @@
                     lib (string):	e.g., 'numpy' or 'flake8==6.0.0'.
                     dev (boolean):	Default False. When False, the prod-requirements.txt is also updated.
     """
     subprocess.check_call(["pip", "install", lib])
     freeze()
     if not dev:
         requirements = getFileContent(GLOBAL_REQUIREMENTS)
-        print(requirements)
         deps = getExactDeps(requirements, lib)
         if len(deps):
+            prodRequirements = getFileContent(PROD_REQUIREMENTS)
             with open(PROD_REQUIREMENTS, "w") as pfile:
-                prodRequirements = getFileContent(PROD_REQUIREMENTS)
                 prodDeps, prodNames = getItems(prodRequirements)
                 for dependency in deps:
                     libName = getLibNameOnly(dependency)
                     if libName not in prodNames:
                         prodDeps.append(dependency)
                     else:
                         prodDeps[prodNames.index(libName)] = dependency
                 prodDeps = list(set(prodDeps))
-                prodDeps.sort()
-                pfile.write("\n".join(prodDeps))
+                prodDeps = sorted(prodDeps, key=str.casefold)
+                pfile.write(os.linesep.join(prodDeps))
 
 
 def pip_uninstall(lib):
     """
     Uninstalls library 'lib' and freeze the dependencies in both requirements.txt and prod-requirements.txt.
     The strategy used to uninstall the dependencies in prod mode is as follow:
     1.	Check which dependencies were removed from requirements.txt. It's safer to do that rather than
@@ -122,24 +125,24 @@
     for dep in uninstallDeps:
         subprocess.check_call(["pip", "uninstall", dep, "-y"])
 
     freeze()
     newRequirements = getFileContent(GLOBAL_REQUIREMENTS)
     deletedLines = getDeletedLines(oldRequirements, newRequirements)
     if len(deletedLines):
+        oldProdRequirements = getFileContent(PROD_REQUIREMENTS)
         with open(PROD_REQUIREMENTS, "w") as pfile:
-            oldProdRequirements = getFileContent(PROD_REQUIREMENTS)
-            prodLines = oldProdRequirements.split("\n")
+            prodLines = oldProdRequirements.split(os.linesep)
             newProdLines = []
             for line in prodLines:
                 if line not in deletedLines:
                     newProdLines.append(line)
             newProdLines = list(set(newProdLines))
             newProdLines.sort()
-            pfile.write("\n".join(newProdLines))
+            pfile.write(os.linesep.join(newProdLines))
 
 
 def getIsolatedDeps(lib):
     """Gets lib's dependencies that are only used by lib any nobody else in the requirements.txt"""
     libName = getLibNameOnly(lib)
     requirements = getFileContent(GLOBAL_REQUIREMENTS)
     # Gets lib's dependencies
@@ -163,33 +166,33 @@
 
 def getFileContent(file):
     content = ""
     if not file:
         return content
 
     if os.path.exists(file):
-        with open(file) as f:
+        with open(file, "r") as f:
             content = f.read()
 
     return content
 
 
 def getDiffLines(oldContent="", newContent="", mode="new"):
-    oldLines = oldContent.split("\n")
-    newLines = newContent.split("\n")
+    oldLines = oldContent.split(os.linesep)
+    newLines = newContent.split(os.linesep)
     lines = []
     ls1, ls2 = (newLines, oldLines) if mode == "new" else (oldLines, newLines)
     for line in ls1:
         if line not in ls2:
             lines.append(line)
     return lines
 
 
 def getExactDeps(requirementsContent, lib, recursive=False, skipDeps=[]):
-    requirements = requirementsContent.split("\n")
+    requirements = requirementsContent.split(os.linesep)
     deps = getPackageDeps(lib)
     libName = getLibNameOnly(lib)
     deps.append(libName)
     exactDeps = []
     findDeps = partial(find, items=requirements)
     for dep in deps:
         if dep not in skipDeps:
@@ -212,20 +215,21 @@
     return exactDeps
 
 
 getNewLines = partial(getDiffLines, mode="new")
 getDeletedLines = partial(getDiffLines, mode="deleted")
 
 
-def main(mode="install"):
+def main(*libs, mode="install"):
     """Main program"""
     # Reads the 'setup.cfg' file
 
-    # Gets the terminal inputs
-    _, *libs = sys.argv
+    if not (len(libs)):
+        # Gets the terminal inputs
+        _, *libs = sys.argv
 
     # Exists if no inputs were provided
     if not (len(libs)):
         exit()
 
     # Filters the inputs between libraries and options (e.g., -D for dev dependencies)
     libDefs = []
@@ -285,22 +289,26 @@
                     prodDeps.append(cleanName)
             pip_install(lib, dev)
 
     if prodChanged:
         initConfig(config, PROD_SECTION, PROD_SECTION_REQUIRE)
         if len(prodDeps):
             prodDeps.sort()
-            config[PROD_SECTION][PROD_SECTION_REQUIRE] = "\n" + "\n".join(prodDeps)
+            config[PROD_SECTION][PROD_SECTION_REQUIRE] = os.linesep + os.linesep.join(
+                prodDeps
+            )
         else:
             del config[PROD_SECTION][PROD_SECTION_REQUIRE]
     if devChanged:
         initConfig(config, DEV_SECTION, DEV_SECTION_REQUIRE)
         if len(devDeps):
             devDeps.sort()
-            config[DEV_SECTION][DEV_SECTION_REQUIRE] = "\n" + "\n".join(devDeps)
+            config[DEV_SECTION][DEV_SECTION_REQUIRE] = os.linesep + os.linesep.join(
+                devDeps
+            )
         else:
             del config[DEV_SECTION][DEV_SECTION_REQUIRE]
 
     with open(SETUP_FILE, "w") as configfile:
         config.write(configfile)
```

