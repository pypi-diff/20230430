# Comparing `tmp/UzSyllable-0.0.5.tar.gz` & `tmp/UzSyllable-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UzSyllable-0.0.5.tar", last modified: Sat Apr 15 01:06:29 2023, max compression
+gzip compressed data, was "UzSyllable-0.0.6.tar", last modified: Sun Apr 30 02:11:02 2023, max compression
```

## Comparing `UzSyllable-0.0.5.tar` & `UzSyllable-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 01:06:29.663219 UzSyllable-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-04-12 11:44:40.000000 UzSyllable-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3358 2023-04-15 01:06:29.661904 UzSyllable-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2686 2023-04-15 00:40:54.000000 UzSyllable-0.0.5/README.md
--rw-rw-rw-   0        0        0       86 2023-04-12 11:44:40.000000 UzSyllable-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 01:06:29.663219 UzSyllable-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-04-15 00:42:03.000000 UzSyllable-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 01:06:29.274529 UzSyllable-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 01:06:29.616942 UzSyllable-0.0.5/src/UzSyllable/
--rw-rw-rw-   0        0        0     4423 2023-04-14 10:55:55.000000 UzSyllable-0.0.5/src/UzSyllable/UzSyllable.py
--rw-rw-rw-   0        0        0       27 2023-04-14 07:45:03.000000 UzSyllable-0.0.5/src/UzSyllable/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 01:06:29.656710 UzSyllable-0.0.5/src/UzSyllable.egg-info/
--rw-rw-rw-   0        0        0     3358 2023-04-15 01:06:29.000000 UzSyllable-0.0.5/src/UzSyllable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-15 01:06:29.000000 UzSyllable-0.0.5/src/UzSyllable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 01:06:29.000000 UzSyllable-0.0.5/src/UzSyllable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-15 01:06:29.000000 UzSyllable-0.0.5/src/UzSyllable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 02:11:02.044363 UzSyllable-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-12 11:44:40.000000 UzSyllable-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-04-30 02:11:02.044363 UzSyllable-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2023-04-30 02:06:10.000000 UzSyllable-0.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-12 11:44:40.000000 UzSyllable-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 02:11:02.044363 UzSyllable-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2023-04-30 02:07:12.000000 UzSyllable-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 02:11:01.983869 UzSyllable-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 02:11:02.037676 UzSyllable-0.0.6/src/UzSyllable/
+-rw-rw-rw-   0        0        0     4683 2023-04-28 05:09:12.000000 UzSyllable-0.0.6/src/UzSyllable/UzSyllable.py
+-rw-rw-rw-   0        0        0      104 2023-04-28 05:00:03.000000 UzSyllable-0.0.6/src/UzSyllable/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 02:11:02.044363 UzSyllable-0.0.6/src/UzSyllable.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-04-30 02:11:01.000000 UzSyllable-0.0.6/src/UzSyllable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-30 02:11:01.000000 UzSyllable-0.0.6/src/UzSyllable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 02:11:01.000000 UzSyllable-0.0.6/src/UzSyllable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-30 02:11:01.000000 UzSyllable-0.0.6/src/UzSyllable.egg-info/top_level.txt
```

### Comparing `UzSyllable-0.0.5/LICENSE` & `UzSyllable-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `UzSyllable-0.0.5/PKG-INFO` & `UzSyllable-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: UzSyllable
-Version: 0.0.5
+Version: 0.0.6
 Summary: UzSyllable | The Syllable Separator, Line breaks and Counter for Uzbek Language
 Home-page: https://github.com/UlugbekSalaev/UzSyllable
 Author: Ulugbek Salaev
 Author-email: ulugbek0302@gmail.com
 Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/UzSyllable/issues
-Keywords: syllabification,end-of-line,line-break,hyphenation,justification,Uzbek language
+Keywords: syllable,line-break,uzbek-language
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,15 +38,15 @@
 
 - Syllabification
 - End-of-Line
 - Count of Syllables
 
 ## Usage
 
-Three options to run UzSyllable:
+Two options to run UzSyllable:
 
 - pip
 - Web interface
 
 ### pip installation
 
 To install UzSyllable, simply run:
@@ -57,14 +57,16 @@
 
 After installation, use in python like following:
 ```yml
 import UzSyllable
 # call syllables method
 print(UzSyllable.syllables('maktabimda'))
 # Output : ['mak-ta-bim-da']
+print(UzSyllable.syllables('мактабимда'))
+# Output : ['мак-та-бим-да']
 # call end-of-line method
 print(UzSyllable.line_break('maktabimda'))
 # Output : ['mak-tabimda', 'makta-bimda', 'maktabim-da']
 # call count of syllables method
 print(UzSyllable.count('maktabimda'))
 # Output : 4
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `UzSyllable-0.0.5/README.md` & `UzSyllable-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 - Syllabification
 - End-of-Line
 - Count of Syllables
 
 ## Usage
 
-Three options to run UzSyllable:
+Two options to run UzSyllable:
 
 - pip
 - Web interface
 
 ### pip installation
 
 To install UzSyllable, simply run:
@@ -41,14 +41,16 @@
 
 After installation, use in python like following:
 ```yml
 import UzSyllable
 # call syllables method
 print(UzSyllable.syllables('maktabimda'))
 # Output : ['mak-ta-bim-da']
+print(UzSyllable.syllables('мактабимда'))
+# Output : ['мак-та-бим-да']
 # call end-of-line method
 print(UzSyllable.line_break('maktabimda'))
 # Output : ['mak-tabimda', 'makta-bimda', 'maktabim-da']
 # call count of syllables method
 print(UzSyllable.count('maktabimda'))
 # Output : 4
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `UzSyllable-0.0.5/setup.py` & `UzSyllable-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="UzSyllable",
-    version="0.0.5",
+    version="0.0.6",
     author="Ulugbek Salaev",
     author_email="ulugbek0302@gmail.com",
     description="UzSyllable | The Syllable Separator, Line breaks and Counter for Uzbek Language",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UlugbekSalaev/UzSyllable",
     project_urls={
         "Bug Tracker": "https://github.com/UlugbekSalaev/UzSyllable/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    keywords=['syllabification', 'end-of-line', 'line-break', 'hyphenation', 'justification', 'Uzbek language'],
+    keywords=['syllable', 'line-break', 'uzbek-language'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     install_requires=[],
     python_requires=">=3.6",
     include_package_data=True,
     #package_data={"": ["*.csv"]},
     #package_data={"": ["cyr_exwords.csv", "lat_exwords.csv"],},
```

### Comparing `UzSyllable-0.0.5/src/UzSyllable/UzSyllable.py` & `UzSyllable-0.0.6/src/UzSyllable/UzSyllable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 def syllables(text):
-    tokens = text.split()
+    tokens = processing(text)
     sylls = list()
     for token in tokens:
         count = 0
-        vowels = set("AaEeUuOoIi")
+        vowels = set("AaEeUuOoIiАаОоУуИиЯяЕеЁёЮюЭэЎў")
         syll = list()
         start = 0
         for letter in token:
             for i in range(65, 91):
                 if ord(letter) == i:
                     count += 1
         if count > 1:
@@ -84,14 +84,19 @@
                 w = w[1:len(w)]
             if w != '':
                 str += w
                 if not w.__contains__('-'):
                     str += '-'
         sylls.append(str[0:len(str)-1])
     return sylls
+def processing(text):
+    text = str(text)
+    text = text.replace("O'", "O‘").replace("o'", "o‘").replace("G'", "G‘").replace("g'", "g‘").replace("'", "’")
+    tokens = text.split()
+    return tokens
 def line_break(text):
     word = text
     syllable = ' '.join(syllables(text))
     begin = end = ''
     if word.__contains__('-'):
         for i in range(0, len(word)):
             if word[i] == '-':
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `UzSyllable-0.0.5/src/UzSyllable.egg-info/PKG-INFO` & `UzSyllable-0.0.6/src/UzSyllable.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: UzSyllable
-Version: 0.0.5
+Version: 0.0.6
 Summary: UzSyllable | The Syllable Separator, Line breaks and Counter for Uzbek Language
 Home-page: https://github.com/UlugbekSalaev/UzSyllable
 Author: Ulugbek Salaev
 Author-email: ulugbek0302@gmail.com
 Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/UzSyllable/issues
-Keywords: syllabification,end-of-line,line-break,hyphenation,justification,Uzbek language
+Keywords: syllable,line-break,uzbek-language
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,15 +38,15 @@
 
 - Syllabification
 - End-of-Line
 - Count of Syllables
 
 ## Usage
 
-Three options to run UzSyllable:
+Two options to run UzSyllable:
 
 - pip
 - Web interface
 
 ### pip installation
 
 To install UzSyllable, simply run:
@@ -57,14 +57,16 @@
 
 After installation, use in python like following:
 ```yml
 import UzSyllable
 # call syllables method
 print(UzSyllable.syllables('maktabimda'))
 # Output : ['mak-ta-bim-da']
+print(UzSyllable.syllables('мактабимда'))
+# Output : ['мак-та-бим-да']
 # call end-of-line method
 print(UzSyllable.line_break('maktabimda'))
 # Output : ['mak-tabimda', 'makta-bimda', 'maktabim-da']
 # call count of syllables method
 print(UzSyllable.count('maktabimda'))
 # Output : 4
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

