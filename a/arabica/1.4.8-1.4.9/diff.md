# Comparing `tmp/arabica-1.4.8.tar.gz` & `tmp/arabica-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.4.8.tar", last modified: Sat Apr 29 01:38:00 2023, max compression
+gzip compressed data, was "arabica-1.4.9.tar", last modified: Sat Apr 29 23:03:07 2023, max compression
```

## Comparing `arabica-1.4.8.tar` & `arabica-1.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 01:38:00.702672 arabica-1.4.8/
--rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.8/LICENSE
--rw-rw-rw-   0        0        0     7537 2023-04-29 01:38:00.702672 arabica-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 01:38:00.687149 arabica-1.4.8/arabica/
--rw-rw-rw-   0        0        0      105 2023-04-21 14:06:32.000000 arabica-1.4.8/arabica/__init__.py
--rw-rw-rw-   0        0        0    11414 2023-04-29 01:02:05.000000 arabica-1.4.8/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    29525 2023-04-20 22:52:23.000000 arabica-1.4.8/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.8/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.8/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.8/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.8/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.8/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.8/arabica/sentiment.py
--rw-rw-rw-   0        0        0      768 2023-04-29 01:02:05.000000 arabica-1.4.8/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-04-29 01:38:00.702672 arabica-1.4.8/arabica.egg-info/
--rw-rw-rw-   0        0        0     7537 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-04-29 01:36:53.000000 arabica-1.4.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 01:38:00.702672 arabica-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-04-29 01:36:53.000000 arabica-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:03:07.921467 arabica-1.4.9/
+-rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0     7537 2023-04-29 23:03:07.921467 arabica-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 23:03:07.921467 arabica-1.4.9/arabica/
+-rw-rw-rw-   0        0        0      105 2023-04-21 14:06:32.000000 arabica-1.4.9/arabica/__init__.py
+-rw-rw-rw-   0        0        0    12373 2023-04-29 22:20:26.000000 arabica-1.4.9/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    29525 2023-04-20 22:52:23.000000 arabica-1.4.9/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.9/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.9/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.9/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.9/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.9/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.9/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      823 2023-04-29 21:16:55.000000 arabica-1.4.9/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:03:07.921467 arabica-1.4.9/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7537 2023-04-29 23:03:07.000000 arabica-1.4.9/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-29 23:03:07.000000 arabica-1.4.9/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 23:03:07.000000 arabica-1.4.9/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-04-29 23:03:07.000000 arabica-1.4.9/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 23:03:07.000000 arabica-1.4.9/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-04-29 23:02:48.000000 arabica-1.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 23:03:07.921467 arabica-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-04-29 23:02:48.000000 arabica-1.4.9/setup.py
```

### Comparing `arabica-1.4.8/PKG-INFO` & `arabica-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
```

### Comparing `arabica-1.4.8/README.md` & `arabica-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `arabica-1.4.8/arabica/arabica_freq.py` & `arabica-1.4.9/arabica/arabica_freq.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,32 +38,57 @@
         data['time']=data['time'].astype(str)
         data['time'] = pd.to_datetime(data['time'], dayfirst=True)
 
     elif date_format == 'us':
         data['time']=data['time'].astype(str)
         data['time'] = pd.to_datetime(data['time'], dayfirst=False)
 
+    # cleaning - blank rows
     data=data.set_index(data['time'])
     data.replace("", float("NaN"), inplace=True)
     data.dropna(subset = ["text"], inplace=True)
 
+    # cleaning - unwanted strings
     if skip is not None:
         data['text'] = data.text.str.replace('|'.join(skip), '.', regex=True).str.strip()
 
+    # cleaning - futher processing
+    data['text'] = data['text'].str.replace("."," . ")
+    data['text'] = data['text'].str.replace("!"," ! ")
+    data['text'] = data['text'].str.replace("?"," ? ")
+    data['text'] = data['text'].str.replace("."," . ")
+    data['text'] = data['text'].str.replace(","," , ")
+    data['text'] = data['text'].str.replace("#"," # ")
+
+    # cleaning - stop words
+    data.replace("", float("NaN"), inplace=True)
+    data.dropna(subset = ["text"], inplace=True)
     if stopwords is not None:
         data['text'] = data.text.map(lambda x: remove_stopwords(x,stopwords=[stopwords]))
 
-    if lower_case is True:
-        data['text'] = np.vectorize(lower_casing)(data['text'])
-
+    # cleaning - punctuation
+    data.replace("", float("NaN"), inplace=True)
+    data.dropna(subset = ["text"], inplace=True)
     data['text'] = np.vectorize(preprocess)(data['text'])
 
+
+    # cleaning - numbers
+    data.replace("", float("NaN"), inplace=True)
+    data.dropna(subset = ["text"], inplace=True)
     if numbers is True:
         data['text'] = np.vectorize(remove_numbers)(data['text'])
 
+
+    # cleaning - lowercasing
+    data.replace("", float("NaN"), inplace=True)
+    data.dropna(subset = ["text"], inplace=True)
+    if lower_case is True:
+        data['text'] = np.vectorize(lower_casing)(data['text'])
+
+
     periods = []
     unigrams_freq = []
     bigrams_freq = []
     trigrams_freq = []
 
     for i, row in data.iterrows():
         period = row[1]
```

### Comparing `arabica-1.4.8/arabica/cappuccino.py` & `arabica-1.4.9/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.8/arabica/clean_ngram.py` & `arabica-1.4.9/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.8/arabica/coffee_break.py` & `arabica-1.4.9/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.8/arabica/group.py` & `arabica-1.4.9/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.8/arabica/preprocess.py` & `arabica-1.4.9/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.8/arabica/stopwords.py` & `arabica-1.4.9/arabica/stopwords.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 List of provided languages:
 from nltk.corpus import stopwords
 print(stopwords.fileids())
 """
 
 from nltk.corpus import stopwords as st
 
-additional_stopwords = set(["i'm","i'd","i've","we'd","we've","he'd","she'd","it'd","they'd"])
 
 def remove_stopwords(text: str,
                      stopwords = []):
 
+    additional_stopwords = set(["i'm","i'd","i've","we'd","we've","he'd","she'd","it'd",
+                                "they'd","it'll","it's"])
+
     for language in stopwords:
         stops= set(st.words(language))
         if 'english' in language :
             stops_extended = stops.union(additional_stopwords)
             filtered_words = [word for word in text.split() if word.lower() not in stops_extended]
         else:
             filtered_words = [word for word in text.split() if word.lower() not in stops]
```

### Comparing `arabica-1.4.8/arabica.egg-info/PKG-INFO` & `arabica-1.4.9/arabica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
```

### Comparing `arabica-1.4.8/pyproject.toml` & `arabica-1.4.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.4.8"
+version = "1.4.9"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.4.8/setup.py` & `arabica-1.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.4.8",
+        version="1.4.9",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

