# Comparing `tmp/nlptoolssna-0.3.6.tar.gz` & `tmp/nlptoolssna-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.3.6.tar", last modified: Sat Apr 29 08:50:52 2023, max compression
+gzip compressed data, was "nlptoolssna-0.3.7.tar", last modified: Sun Apr 30 06:10:02 2023, max compression
```

## Comparing `nlptoolssna-0.3.6.tar` & `nlptoolssna-0.3.7.tar`

### file list

```diff
@@ -1,75 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.318354 nlptoolssna-0.3.6/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-29 08:50:52.318354 nlptoolssna-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.146482 nlptoolssna-0.3.6/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.3.6/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.093352 nlptoolssna-0.3.6/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.093407 nlptoolssna-0.3.6/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.146482 nlptoolssna-0.3.6/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.6/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.178885 nlptoolssna-0.3.6/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.6/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.3.6/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.3.6/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.3.6/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.3.6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.223258 nlptoolssna-0.3.6/docs/source/
--rw-rw-rw-   0        0        0      318 2023-04-27 09:55:38.000000 nlptoolssna-0.3.6/docs/source/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.234340 nlptoolssna-0.3.6/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.6/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.235367 nlptoolssna-0.3.6/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.266745 nlptoolssna-0.3.6/docs/source/api/morph/
--rw-rw-rw-   0        0        0       48 2023-04-26 20:02:35.000000 nlptoolssna-0.3.6/docs/source/api/morph/charsets.rst
--rw-rw-rw-   0        0        0       66 2023-04-26 20:02:52.000000 nlptoolssna-0.3.6/docs/source/api/morph/lemmatizeSentence.rst
--rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.3.6/docs/source/api/morph/morph_tagger.rst
--rw-rw-rw-   0        0        0       65 2023-04-26 20:03:13.000000 nlptoolssna-0.3.6/docs/source/api/morph/tokenizers_words.rst
--rw-rw-rw-   0        0        0      280 2023-04-27 12:17:19.000000 nlptoolssna-0.3.6/docs/source/api/morph.rst
--rw-rw-rw-   0        0        0      140 2023-04-26 20:11:06.000000 nlptoolssna-0.3.6/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.3.6/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.3.6/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.3.6/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.3.6/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.270939 nlptoolssna-0.3.6/nlptools/
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.275109 nlptoolssna-0.3.6/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.6/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     2527 2023-04-27 21:39:46.000000 nlptoolssna-0.3.6/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.276639 nlptoolssna-0.3.6/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.6/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.284828 nlptoolssna-0.3.6/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.6/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.6/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.293431 nlptoolssna-0.3.6/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.6/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.3.6/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     7467 2023-04-29 08:48:51.000000 nlptoolssna-0.3.6/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.6/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.6/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.293431 nlptoolssna-0.3.6/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.6/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.6/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.301537 nlptoolssna-0.3.6/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.6/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.6/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.6/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.310194 nlptoolssna-0.3.6/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1479 2023-04-29 08:50:52.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 08:50:51.000000 nlptoolssna-0.3.6/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-04-29 08:50:52.318354 nlptoolssna-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1843 2023-04-18 21:50:46.000000 nlptoolssna-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:50:52.318354 nlptoolssna-0.3.6/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.6/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.847293 nlptoolssna-0.3.7/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-04-30 06:10:02.848292 nlptoolssna-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.740569 nlptoolssna-0.3.7/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.3.7/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.703097 nlptoolssna-0.3.7/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.704277 nlptoolssna-0.3.7/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.743710 nlptoolssna-0.3.7/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.7/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.751781 nlptoolssna-0.3.7/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.7/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.3.7/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.3.7/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.3.7/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.3.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.765830 nlptoolssna-0.3.7/docs/source/
+-rw-rw-rw-   0        0        0      318 2023-04-27 09:55:38.000000 nlptoolssna-0.3.7/docs/source/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.767831 nlptoolssna-0.3.7/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.3.7/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.769836 nlptoolssna-0.3.7/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.778576 nlptoolssna-0.3.7/docs/source/api/morph/
+-rw-rw-rw-   0        0        0       48 2023-04-26 20:02:35.000000 nlptoolssna-0.3.7/docs/source/api/morph/charsets.rst
+-rw-rw-rw-   0        0        0       66 2023-04-26 20:02:52.000000 nlptoolssna-0.3.7/docs/source/api/morph/lemmatizeSentence.rst
+-rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.3.7/docs/source/api/morph/morph_tagger.rst
+-rw-rw-rw-   0        0        0       65 2023-04-26 20:03:13.000000 nlptoolssna-0.3.7/docs/source/api/morph/tokenizers_words.rst
+-rw-rw-rw-   0        0        0      280 2023-04-27 12:17:19.000000 nlptoolssna-0.3.7/docs/source/api/morph.rst
+-rw-rw-rw-   0        0        0      140 2023-04-26 20:11:06.000000 nlptoolssna-0.3.7/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.3.7/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.3.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.3.7/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.3.7/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.784880 nlptoolssna-0.3.7/nlptools/
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.789319 nlptoolssna-0.3.7/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.3.7/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     2527 2023-04-27 21:39:46.000000 nlptoolssna-0.3.7/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.790316 nlptoolssna-0.3.7/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.3.7/nlptools/arabiner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.794415 nlptoolssna-0.3.7/nlptools/arabiner/bin/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.3.7/nlptools/arabiner/bin/__init__.py
+-rw-rw-rw-   0        0        0     1350 2023-04-30 05:53:08.000000 nlptoolssna-0.3.7/nlptools/arabiner/bin/infer.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.800965 nlptoolssna-0.3.7/nlptools/arabiner/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.3.7/nlptools/arabiner/utils/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-03-29 20:22:54.000000 nlptoolssna-0.3.7/nlptools/arabiner/utils/data.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.3.7/nlptools/arabiner/utils/helpers.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.803634 nlptoolssna-0.3.7/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.3.7/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.807469 nlptoolssna-0.3.7/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.3.7/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.3.7/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.818335 nlptoolssna-0.3.7/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.3.7/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.3.7/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     7629 2023-04-29 19:50:22.000000 nlptoolssna-0.3.7/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.3.7/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.3.7/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.821883 nlptoolssna-0.3.7/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.3.7/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.3.7/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.829839 nlptoolssna-0.3.7/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.3.7/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.3.7/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.3.7/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.840259 nlptoolssna-0.3.7/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-04-30 06:10:02.000000 nlptoolssna-0.3.7/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1677 2023-04-30 06:10:02.000000 nlptoolssna-0.3.7/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 06:10:02.000000 nlptoolssna-0.3.7/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-30 06:10:02.000000 nlptoolssna-0.3.7/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.3.7/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      101 2023-04-30 06:10:02.000000 nlptoolssna-0.3.7/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 06:10:02.000000 nlptoolssna-0.3.7/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-04-30 06:10:02.849913 nlptoolssna-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2036 2023-04-30 06:09:18.000000 nlptoolssna-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 06:10:02.846300 nlptoolssna-0.3.7/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.3.7/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.3.6/CONTRIBUTING.rst` & `nlptoolssna-0.3.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/LICENSE` & `nlptoolssna-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/PKG-INFO` & `nlptoolssna-0.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 nlptools
 ========
```

### Comparing `nlptoolssna-0.3.6/README.rst` & `nlptoolssna-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/docs/Makefile` & `nlptoolssna-0.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/docs/build/html/_images/download.png` & `nlptoolssna-0.3.7/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/docs/build/html/_static/download.png` & `nlptoolssna-0.3.7/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/docs/make.bat` & `nlptoolssna-0.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/docs/source/_static/download.png` & `nlptoolssna-0.3.7/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/docs/source/conf.py` & `nlptoolssna-0.3.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/docs/source/installation.rst` & `nlptoolssna-0.3.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.3.7/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptools/data/my_data.pickle` & `nlptoolssna-0.3.7/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.3.7/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptools/morph/charsets.py` & `nlptoolssna-0.3.7/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.3.7/nlptools/morph/morph_tagger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pickle
 from nlptools.morph import settings 
 import re
 from nlptools.morph.tokenizers_words import simple_word_tokenize
 from nlptools.parse.parser import arStrip
 import os.path
 from nlptools.DataDownload import downloader
+from tqdm.auto import tqdm
 
 def load_ALMA_dic():
    # Open the Pickle file in binary mode
     filename = 'ALMA27012000.pickle'
     path =downloader.get_appdatadir()
     file_path = os.path.join(path, filename)
     
@@ -59,19 +60,19 @@
          - task is pos, then the morphological soltuion is only the pos.
          - task is full, the the morphological soltuion is both the lemma and the pos.
      
     The language arguemet is used to help the morphological analysis to return more accurate solutions, for example if the text is MSA, or dialects (Palestinian dilect, pppp).
    
     Args:
           - text (str): The input text to morphologicaly analyzed.
-          - language (str): The language of the input text (e.g., 'MSA').
-          - task (str): The type of task being performed (e.g., 'lemmatizer', 'pos', or 'full').
+          - language (str): The language of the input text (e.g., `MSA`).
+          - task (str): The type of task being performed (e.g., `lemmatizer`, `pos`, or `full`).
          
     Returns:
-    - output_list (list): A list of morphological solution for each token in the input text.
+          - output_list (list): A list of morphological solution for each token in the input text.
 
     **Example:**
 
     .. highlight:: python
     .. code-block:: python
 
          from nlptools.morph import morph_tagger
@@ -79,16 +80,18 @@
          # Return the morpological solution for each token in this text
          morph_tagger.tagger('ذهب الولد الى المدرسة')
     """
 
    output_list = []
    # tokenize sentence into words
    words = simple_word_tokenize(text)
+   # create tqdm progress bar
+   progress_bar = tqdm(words, desc='Lemmatizing Sentence', leave=False)
    # for each word 
-   for word in words:
+   for word in progress_bar:
          result_word =[]
          # Trim spaces 
          word = word.strip()
          # Remove smallDiac
          word = arStrip(word , False , True , False , False , False , False) 
          # Unify ٱ 
          word = re.sub('[ٱ]','ﺍ',word)
@@ -144,19 +147,19 @@
    return output_list               
         
 def tagger(text: str, task = 'full', language = 'MSA') -> list:
 
     """
     This method takes an Arabic text as input, tokenize it into tokens and calles the morphological tagger to return the morpological solution for each token in this text.
     There is no limit for the text size, but one should be resonable based on the available resources (computational power).
-   
-    Args:
-        - text (str): The input Arabic text to be morphologically analyzed and tagged.
-        - task (str): The type of morphological analysis and tagging to be performed. Default is 'full'.
-        - language (str): The language of the input text. Default is 'MSA' (Modern Standard Arabic).
+    
+        Args:
+            - text (str): The input Arabic text to be morphologically analyzed and tagged.
+            - task (str): The type of morphological analysis and tagging to be performed. Default is `full`.
+            - language (str): The language of the input text. Default is 'MSA' (Modern Standard Arabic).
         
     Returns:
         list: A list of lists, where each sublist contains information about a token in the input text, including the original tokem, its lemma, its part of speech (POS) tag, its lemma frequency, the task and the language.
     """
     
     # Check if the ALMA dictionary has been loaded
     if settings.flag == True:
```

### Comparing `nlptoolssna-0.3.6/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.3.7/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptools/parse/parser.py` & `nlptoolssna-0.3.7/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptools/salma/implication.py` & `nlptoolssna-0.3.7/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.3.7/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.3.7/nlptoolssna.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 nlptools
 ========
```

### Comparing `nlptoolssna-0.3.6/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.3.7/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 docs/source/api/morph/morph_tagger.rst
 docs/source/api/morph/tokenizers_words.rst
 nlptools/__init__.py
 nlptools/cli.py
 nlptools/nlptools.py
 nlptools/DataDownload/__init__.py
 nlptools/DataDownload/downloader.py
+nlptools/arabiner/__init__.py
+nlptools/arabiner/bin/__init__.py
+nlptools/arabiner/bin/infer.py
+nlptools/arabiner/utils/__init__.py
+nlptools/arabiner/utils/data.py
+nlptools/arabiner/utils/helpers.py
 nlptools/data/my_data.pickle
 nlptools/jaccard/__init__.py
 nlptools/jaccard/jaccardFunction.py
 nlptools/morph/__init__.py
 nlptools/morph/charsets.py
 nlptools/morph/morph_tagger.py
 nlptools/morph/settings.py
```

### Comparing `nlptoolssna-0.3.6/setup.cfg` & `nlptoolssna-0.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.3.6/setup.py` & `nlptoolssna-0.3.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 
 requirements = [
     'six',
     'farasapy',
     'tqdm',
     'requests',
     'regex',
-    'pathlib'
+    'pathlib',
+    'torchtext==0.14.0',
+    'transformers==4.24.0',
+    'seqeval==1.2.2',
+    'torch'
 ]
 
 test_requirements = [ ]
 
 setup(
     author="Alaa' Omar",
     author_email='alaa.omer2009@gmail.com',
@@ -34,14 +38,16 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
     entry_points={
         'console_scripts': [
             'nlptools=nlptools.cli:main',
         ],
     },
```

