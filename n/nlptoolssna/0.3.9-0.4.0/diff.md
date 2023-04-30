# Comparing `tmp/nlptoolssna-0.3.9.tar.gz` & `tmp/nlptoolssna-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.3.9.tar", last modified: Sun Apr 30 09:12:19 2023, max compression
+gzip compressed data, was "nlptoolssna-0.4.0.tar", last modified: Sun Apr 30 09:44:38 2023, max compression
```

## Comparing `nlptoolssna-0.3.9.tar` & `nlptoolssna-0.4.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.922585 nlptoolssna-0.3.9/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-04-30 09:12:19.922585 nlptoolssna-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.838945 nlptoolssna-0.3.9/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.3.9/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.810791 nlptoolssna-0.3.9/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.811859 nlptoolssna-0.3.9/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.840943 nlptoolssna-0.3.9/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.9/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.846379 nlptoolssna-0.3.9/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.9/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.3.9/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.3.9/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.3.9/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.3.9/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.858115 nlptoolssna-0.3.9/docs/source/
--rw-rw-rw-   0        0        0      318 2023-04-27 09:55:38.000000 nlptoolssna-0.3.9/docs/source/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.860494 nlptoolssna-0.3.9/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.9/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.861693 nlptoolssna-0.3.9/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.867713 nlptoolssna-0.3.9/docs/source/api/morph/
--rw-rw-rw-   0        0        0       48 2023-04-26 20:02:35.000000 nlptoolssna-0.3.9/docs/source/api/morph/charsets.rst
--rw-rw-rw-   0        0        0       66 2023-04-26 20:02:52.000000 nlptoolssna-0.3.9/docs/source/api/morph/lemmatizeSentence.rst
--rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.3.9/docs/source/api/morph/morph_tagger.rst
--rw-rw-rw-   0        0        0       65 2023-04-26 20:03:13.000000 nlptoolssna-0.3.9/docs/source/api/morph/tokenizers_words.rst
--rw-rw-rw-   0        0        0      280 2023-04-27 12:17:19.000000 nlptoolssna-0.3.9/docs/source/api/morph.rst
--rw-rw-rw-   0        0        0      140 2023-04-26 20:11:06.000000 nlptoolssna-0.3.9/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.3.9/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.3.9/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.3.9/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.3.9/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.872696 nlptoolssna-0.3.9/nlptools/
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.876100 nlptoolssna-0.3.9/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.9/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     2527 2023-04-27 21:39:46.000000 nlptoolssna-0.3.9/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.888087 nlptoolssna-0.3.9/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.3.9/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.3.9/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.3.9/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.3.9/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.3.9/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-04-30 06:31:23.000000 nlptoolssna-0.3.9/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.890277 nlptoolssna-0.3.9/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.9/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.894252 nlptoolssna-0.3.9/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.9/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.9/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.900519 nlptoolssna-0.3.9/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.9/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.3.9/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     7629 2023-04-29 19:50:22.000000 nlptoolssna-0.3.9/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.9/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.9/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.903552 nlptoolssna-0.3.9/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.9/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.9/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.908068 nlptoolssna-0.3.9/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.9/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.9/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.9/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.918071 nlptoolssna-0.3.9/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-04-30 09:12:19.000000 nlptoolssna-0.3.9/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1653 2023-04-30 09:12:19.000000 nlptoolssna-0.3.9/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 09:12:19.000000 nlptoolssna-0.3.9/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-30 09:12:19.000000 nlptoolssna-0.3.9/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.9/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      121 2023-04-30 09:12:19.000000 nlptoolssna-0.3.9/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 09:12:19.000000 nlptoolssna-0.3.9/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-04-30 09:12:19.924597 nlptoolssna-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     2064 2023-04-30 09:06:38.000000 nlptoolssna-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 09:12:19.920583 nlptoolssna-0.3.9/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.9/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.850461 nlptoolssna-0.4.0/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-04-30 09:44:38.850461 nlptoolssna-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.758409 nlptoolssna-0.4.0/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.721590 nlptoolssna-0.4.0/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.724108 nlptoolssna-0.4.0/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.761007 nlptoolssna-0.4.0/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.0/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.770098 nlptoolssna-0.4.0/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.0/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.0/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.0/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.0/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.784126 nlptoolssna-0.4.0/docs/source/
+-rw-rw-rw-   0        0        0      318 2023-04-27 09:55:38.000000 nlptoolssna-0.4.0/docs/source/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.785836 nlptoolssna-0.4.0/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.0/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.788559 nlptoolssna-0.4.0/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.797837 nlptoolssna-0.4.0/docs/source/api/morph/
+-rw-rw-rw-   0        0        0       48 2023-04-26 20:02:35.000000 nlptoolssna-0.4.0/docs/source/api/morph/charsets.rst
+-rw-rw-rw-   0        0        0       66 2023-04-26 20:02:52.000000 nlptoolssna-0.4.0/docs/source/api/morph/lemmatizeSentence.rst
+-rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.4.0/docs/source/api/morph/morph_tagger.rst
+-rw-rw-rw-   0        0        0       65 2023-04-26 20:03:13.000000 nlptoolssna-0.4.0/docs/source/api/morph/tokenizers_words.rst
+-rw-rw-rw-   0        0        0      280 2023-04-27 12:17:19.000000 nlptoolssna-0.4.0/docs/source/api/morph.rst
+-rw-rw-rw-   0        0        0      140 2023-04-26 20:11:06.000000 nlptoolssna-0.4.0/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.0/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.0/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.803871 nlptoolssna-0.4.0/nlptools/
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.807728 nlptoolssna-0.4.0/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.0/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     2527 2023-04-27 21:39:46.000000 nlptoolssna-0.4.0/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.817621 nlptoolssna-0.4.0/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.0/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.0/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.0/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.0/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.0/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-04-30 06:31:23.000000 nlptoolssna-0.4.0/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.818615 nlptoolssna-0.4.0/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.0/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.821619 nlptoolssna-0.4.0/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.0/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.0/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.830357 nlptoolssna-0.4.0/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.4.0/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.0/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     7629 2023-04-29 19:50:22.000000 nlptoolssna-0.4.0/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.0/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.4.0/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.832357 nlptoolssna-0.4.0/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.0/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.0/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.836357 nlptoolssna-0.4.0/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.0/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.0/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.4.0/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.847462 nlptoolssna-0.4.0/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-04-30 09:44:38.000000 nlptoolssna-0.4.0/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1653 2023-04-30 09:44:38.000000 nlptoolssna-0.4.0/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 09:44:38.000000 nlptoolssna-0.4.0/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-30 09:44:38.000000 nlptoolssna-0.4.0/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.0/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      137 2023-04-30 09:44:38.000000 nlptoolssna-0.4.0/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 09:44:38.000000 nlptoolssna-0.4.0/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-04-30 09:44:38.851481 nlptoolssna-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2088 2023-04-30 09:44:22.000000 nlptoolssna-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:44:38.849462 nlptoolssna-0.4.0/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.0/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.3.9/CONTRIBUTING.rst` & `nlptoolssna-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/LICENSE` & `nlptoolssna-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/PKG-INFO` & `nlptoolssna-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.9
+Version: 0.4.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.3.9/README.rst` & `nlptoolssna-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/docs/Makefile` & `nlptoolssna-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/docs/build/html/_images/download.png` & `nlptoolssna-0.4.0/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/docs/build/html/_static/download.png` & `nlptoolssna-0.4.0/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/docs/make.bat` & `nlptoolssna-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/docs/source/_static/download.png` & `nlptoolssna-0.4.0/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/docs/source/conf.py` & `nlptoolssna-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/docs/source/installation.rst` & `nlptoolssna-0.4.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.4.0/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/arabiner/data.py` & `nlptoolssna-0.4.0/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/arabiner/datasets.py` & `nlptoolssna-0.4.0/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/arabiner/helpers.py` & `nlptoolssna-0.4.0/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/arabiner/infer.py` & `nlptoolssna-0.4.0/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/arabiner/transforms.py` & `nlptoolssna-0.4.0/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/data/my_data.pickle` & `nlptoolssna-0.4.0/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.4.0/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/morph/charsets.py` & `nlptoolssna-0.4.0/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.4.0/nlptools/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.4.0/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/parse/parser.py` & `nlptoolssna-0.4.0/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/salma/implication.py` & `nlptoolssna-0.4.0/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.4.0/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.4.0/nlptoolssna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.9
+Version: 0.4.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.3.9/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.4.0/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/setup.cfg` & `nlptoolssna-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.9/setup.py` & `nlptoolssna-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     'requests',
     'regex',
     'pathlib',
     'torchtext==0.14.0',
     'transformers==4.24.0',
     'seqeval==1.2.2',
     'torchvision==0.14.0',
+    'pytorch==1.13.0',
     'torch'
 ]
 
 test_requirements = [ ]
 
 setup(
     author="Alaa' Omar",
```

