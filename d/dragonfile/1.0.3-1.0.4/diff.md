# Comparing `tmp/dragonfile-1.0.3.tar.gz` & `tmp/dragonfile-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonfile-1.0.3.tar", last modified: Sat Apr 22 05:07:30 2023, max compression
+gzip compressed data, was "dragonfile-1.0.4.tar", last modified: Sun Apr 30 02:57:51 2023, max compression
```

## Comparing `dragonfile-1.0.3.tar` & `dragonfile-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 05:07:30.781914 dragonfile-1.0.3/
--rw-rw-rw-   0        0        0     1086 2023-04-20 21:04:35.000000 dragonfile-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      771 2023-04-22 05:07:30.778914 dragonfile-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2091 2023-04-22 02:49:35.000000 dragonfile-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 05:07:30.721949 dragonfile-1.0.3/dragonfile/
--rw-rw-rw-   0        0        0     4128 2023-04-22 05:07:21.000000 dragonfile-1.0.3/dragonfile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 05:07:30.766928 dragonfile-1.0.3/dragonfile.egg-info/
--rw-rw-rw-   0        0        0      771 2023-04-22 05:07:30.000000 dragonfile-1.0.3/dragonfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-22 05:07:30.000000 dragonfile-1.0.3/dragonfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 05:07:30.000000 dragonfile-1.0.3/dragonfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-22 05:07:30.000000 dragonfile-1.0.3/dragonfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 05:07:30.783917 dragonfile-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-04-22 05:07:12.000000 dragonfile-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 05:07:30.773918 dragonfile-1.0.3/tests/
--rw-rw-rw-   0        0        0        8 2023-04-22 04:26:27.000000 dragonfile-1.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 02:57:51.550401 dragonfile-1.0.4/
+-rw-rw-rw-   0        0        0     1086 2023-04-20 21:04:35.000000 dragonfile-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-04-30 02:57:51.542405 dragonfile-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-04-22 02:49:35.000000 dragonfile-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 02:57:51.426476 dragonfile-1.0.4/dragonfile/
+-rw-rw-rw-   0        0        0     5439 2023-04-30 02:54:53.000000 dragonfile-1.0.4/dragonfile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 02:57:51.525414 dragonfile-1.0.4/dragonfile.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-04-30 02:57:50.000000 dragonfile-1.0.4/dragonfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-30 02:57:51.000000 dragonfile-1.0.4/dragonfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 02:57:50.000000 dragonfile-1.0.4/dragonfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-30 02:57:50.000000 dragonfile-1.0.4/dragonfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 02:57:51.551399 dragonfile-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-04-30 02:57:21.000000 dragonfile-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 02:57:51.537409 dragonfile-1.0.4/tests/
+-rw-rw-rw-   0        0        0        8 2023-04-22 04:26:27.000000 dragonfile-1.0.4/tests/__init__.py
```

### Comparing `dragonfile-1.0.3/LICENSE` & `dragonfile-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfile-1.0.3/PKG-INFO` & `dragonfile-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 1.0.3
+Version: 1.0.4
 Summary: Read CSV - Version Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dragonfile-1.0.3/README.md` & `dragonfile-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dragonfile-1.0.3/dragonfile/__init__.py` & `dragonfile-1.0.4/dragonfile/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 import csv
 
-class dragonfile:
-    def __init__ (self, dFile, nColumn, dSep=",", coding="utf-8", dictD={}):
+class DragonFile:
+    def __init__ (self, dFile, nColumn, dSep=",", coding="utf-8", dictD={}, validate=False):
         self.dFile = dFile
         self.nColumn = nColumn
         self.dSep = dSep
         self.coding = coding
         self.dictD = dictD
+        self.validate = validate
     
     def readFile(self):
         columns = []
 
         with open(self.dFile, encoding=self.coding) as file:
             reader = csv.reader(file, delimiter=self.dSep)
             header = next(reader)
             nameColumn = header[self.nColumn]
 
             for i, row in enumerate(reader):
                 columns.append(row[self.nColumn])
 
         dictDaux = {nameColumn: columns}
         self.dictD.update(dictDaux)
-        print("Termino",self.nColumn)
+
+        if self.validate == True:
+            print("Termino",self.nColumn)
+        
         self.nColumn += 1
 
         return self.dictD, self.nColumn
 
-    def readFileSetPeriod(self, varOp0="", varOp1="Valor1", varOp2="Valor2", varOp3="Valor3", varLog0="1", varLog1="6", varLog2="12", twoColumn=False):
+    def readFileSetPeriod(self, varOp0="", varOp1="Manhã", varOp2="Tarde", varOp3="Noite", varLog0="6", varLog1="12", varLog2="18", twoColumn=False):
         columns = []
         columnsTwo = []
 
         with open(self.dFile, encoding=self.coding) as file:
             reader = csv.reader(file, delimiter=self.dSep)
             header = next(reader)
             nameColumn = header[self.nColumn]
             extraColum = "New"+header[self.nColumn]
             
             for i, row in enumerate(reader):
                 word = row[self.nColumn]
 
-                if word != varOp0:
+                if word != "":
                     word = int(word[0]+word[1])
                 else:
                     word = varOp0
 
-                if word != varOp0:
+                if word != varOp0 :
 
                     if word > varLog0 and word <= varLog1:
                         word = varOp1
 
                     elif word > varLog1 and word < varLog2:
                         word = varOp2
 
@@ -60,66 +64,101 @@
                 
                 columns.append(word)
                 columnsTwo.append(row[self.nColumn])
 
             if twoColumn == False:
                 dictDaux = {extraColum: columns}
                 self.dictD.update(dictDaux)
-                print("Termino",self.nColumn)
+
+                if self.validate == True:
+                    print("Termino",self.nColumn)
+
                 self.nColumn += 1
             else:
                 dictDaux1 = {nameColumn: columnsTwo}
                 dictDaux2 = {extraColum: columns}
 
                 dictDaux1.update(dictDaux2)
                 self.dictD.update(dictDaux1)
 
-                print("Termino",self.nColumn)
+                if self.validate == True:
+                    print("Termino",self.nColumn)
+
                 self.nColumn += 1
             
             return self.dictD, self.nColumn
 
-    def readFileRename(self, nameRow=[], renameRow=[]):
+    def readFileRename(self, nameRow=[], renameRow=[], mode=False, varOp0=""):
         columns = []
 
         with open(self.dFile, encoding=self.coding) as file:
             reader = csv.reader(file, delimiter=self.dSep)
             header = next(reader)
             nameColumn = header[self.nColumn]
 
-            for i, row in enumerate(reader):
-                j = 0
-                while j < len(nameRow):
-                    if row[self.nColumn] == nameRow[j]:
-                        columns.append(renameRow[j])
-                        j += 1
+            for row in reader:
+                if mode == False:
+                    if row[self.nColumn] in nameRow:
+                        index = nameRow.index(row[self.nColumn])
+                        columns.append(renameRow[index])
                     else:
-                        j += 1
-
-                if j > len(nameRow):
-                    find = False
+                        columns.append(row[self.nColumn])
                 else:
-                    find = True
+                    if row[self.nColumn] in nameRow:
+                        index = nameRow.index(row[self.nColumn])
+                        columns.append(renameRow[index])
+                    else:
+                        columns.append(varOp0)
+
+            dictDaux = {nameColumn: columns}
+            self.dictD.update(dictDaux)
+
+            if self.validate == True:
+                    print("Termino",self.nColumn)
+
+            self.nColumn += 1
+
+            return self.dictD, self.nColumn
+        
+    def readValues(self):   
+        columns = []
+
+        with open(self.dFile, encoding=self.coding) as file:
+            reader = csv.reader(file, delimiter=self.dSep)
+            header = next(reader)
+            nameColumn = header[self.nColumn]
+
+            for i, row in enumerate(reader):
+                valor = row[self.nColumn]
                 
-                if find == False:
-                    columns.append(row[self.nColumn])
-                else:
-                    pass
+                valor = valor.replace(".", "")
+                valor = valor.replace(",", ".")
+                columns.append(valor)
+                        
 
         dictDaux = {nameColumn: columns}
         self.dictD.update(dictDaux)
-        print("Termino",self.nColumn)
+
+        if self.validate == True:
+            print("Termino",self.nColumn)
+        
         self.nColumn += 1
 
         return self.dictD, self.nColumn
 
     def fileToCsv(self):
         with open(self.dFile, 'w', newline='', encoding='utf-8') as file:
             writer = csv.writer(file)
             writer.writerow(self.dictD.keys())
             writer.writerows(zip(*self.dictD.values()))
 
     def lenColumns(self):
         with open(self.dFile, 'r', encoding='utf-8') as file:
             reader = csv.reader(file, delimiter=self.dSep)
             first_row = next(reader)
-            return len(first_row)
+            return len(first_row)
+        
+dragonfile = DragonFile
+
+class dataDict(dragonfile):
+    def __init__(self, dFile, nColumn, dSep=",", coding="utf-8", dictD={}, validate=False):
+        super().__init__(dFile, nColumn, dSep, coding, dictD, validate)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dragonfile-1.0.3/dragonfile.egg-info/PKG-INFO` & `dragonfile-1.0.4/dragonfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfile
-Version: 1.0.3
+Version: 1.0.4
 Summary: Read CSV - Version Test
 Author: Gabriel Arantd Felipe
 Author-email: grantd.ctt@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dragonfile-1.0.3/setup.py` & `dragonfile-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dragonfile',
-    version='1.0.3',
+    version='1.0.4',
     description='Read CSV - Version Test',
     author='Gabriel Arantd Felipe',
     author_email='grantd.ctt@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

