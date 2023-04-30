# Comparing `tmp/backtrader_binance-1.0.3.tar.gz` & `tmp/backtrader_binance-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtrader_binance-1.0.3.tar", last modified: Sun Apr 30 08:00:37 2023, max compression
+gzip compressed data, was "backtrader_binance-1.0.4.tar", last modified: Sun Apr 30 08:27:33 2023, max compression
```

## Comparing `backtrader_binance-1.0.3.tar` & `backtrader_binance-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 08:00:37.121945 backtrader_binance-1.0.3/
--rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_binance-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    23238 2023-04-30 08:00:37.121945 backtrader_binance-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    21996 2023-04-21 11:23:24.000000 backtrader_binance-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 08:00:37.116949 backtrader_binance-1.0.3/backtrader_binance/
--rw-rw-rw-   0        0        0       40 2021-06-25 01:58:20.000000 backtrader_binance-1.0.3/backtrader_binance/__init__.py
--rw-rw-rw-   0        0        0     6397 2023-04-05 12:42:51.000000 backtrader_binance-1.0.3/backtrader_binance/binance_broker.py
--rw-rw-rw-   0        0        0     5048 2023-04-05 03:54:03.000000 backtrader_binance-1.0.3/backtrader_binance/binance_feed.py
--rw-rw-rw-   0        0        0     6586 2023-04-30 07:50:22.000000 backtrader_binance-1.0.3/backtrader_binance/binance_store.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:00:37.120945 backtrader_binance-1.0.3/backtrader_binance.egg-info/
--rw-rw-rw-   0        0        0    23238 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 08:00:37.122945 backtrader_binance-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2163 2023-04-30 07:55:31.000000 backtrader_binance-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:27:33.818684 backtrader_binance-1.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_binance-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    23941 2023-04-30 08:27:33.818684 backtrader_binance-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    22689 2023-04-30 08:26:04.000000 backtrader_binance-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 08:27:33.813684 backtrader_binance-1.0.4/backtrader_binance/
+-rw-rw-rw-   0        0        0       40 2021-06-25 01:58:20.000000 backtrader_binance-1.0.4/backtrader_binance/__init__.py
+-rw-rw-rw-   0        0        0     6397 2023-04-05 12:42:51.000000 backtrader_binance-1.0.4/backtrader_binance/binance_broker.py
+-rw-rw-rw-   0        0        0     5048 2023-04-05 03:54:03.000000 backtrader_binance-1.0.4/backtrader_binance/binance_feed.py
+-rw-rw-rw-   0        0        0     6586 2023-04-30 07:50:22.000000 backtrader_binance-1.0.4/backtrader_binance/binance_store.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:27:33.817685 backtrader_binance-1.0.4/backtrader_binance.egg-info/
+-rw-rw-rw-   0        0        0    23941 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 08:27:33.819686 backtrader_binance-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2163 2023-04-30 08:27:08.000000 backtrader_binance-1.0.4/setup.py
```

### Comparing `backtrader_binance-1.0.3/LICENSE` & `backtrader_binance-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.3/PKG-INFO` & `backtrader_binance-1.0.4/backtrader_binance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: backtrader_binance
-Version: 1.0.3
+Name: backtrader-binance
+Version: 1.0.4
 Summary: Binance API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_binance
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
 Keywords: trading,development
@@ -46,14 +46,19 @@
 pip install git+https://github.com/WISEPLAT/backtrader_binance.git
 ```
 
 2) Please use backtrader from my repository (as your can push your commits in it). Install it:
 ```shell
 pip install git+https://github.com/WISEPLAT/backtrader.git
 ```
+-- Can I use your binance interface with original backtrader?
+
+-- Yes, you can use original backtrader, as the author of original backtrader had approved all my changes. 
+
+Here is the link: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
 
 3) We have some dependencies, you need to install them: 
 ```shell
 pip install python-binance pandas matplotlib
 ```
 
 ### Getting started
@@ -183,14 +188,19 @@
 pip install git+https://github.com/WISEPLAT/backtrader_binance.git
 ```
 
 2) Пожалуйста, используйте backtrader из моего репозитория (так как вы можете размещать в нем свои коммиты). Установите его:
 ```shell
 pip install git+https://github.com/WISEPLAT/backtrader.git
 ```
+-- Могу ли я использовать ваш интерфейс binance с оригинальным backtrader?
+
+-- Да, вы можете использовать оригинальный backtrader, так как автор оригинального backtrader одобрил все мои изменения.
+
+Вот ссылка: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
 
 3) У нас есть некоторые зависимости, вам нужно их установить:
 ```shell
 pip install python-binance pandas matplotlib
 ```
 
 ### Начало работы
```

### Comparing `backtrader_binance-1.0.3/README.md` & `backtrader_binance-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 pip install git+https://github.com/WISEPLAT/backtrader_binance.git
 ```
 
 2) Please use backtrader from my repository (as your can push your commits in it). Install it:
 ```shell
 pip install git+https://github.com/WISEPLAT/backtrader.git
 ```
+-- Can I use your binance interface with original backtrader?
+
+-- Yes, you can use original backtrader, as the author of original backtrader had approved all my changes. 
+
+Here is the link: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
 
 3) We have some dependencies, you need to install them: 
 ```shell
 pip install python-binance pandas matplotlib
 ```
 
 ### Getting started
@@ -159,14 +164,19 @@
 pip install git+https://github.com/WISEPLAT/backtrader_binance.git
 ```
 
 2) Пожалуйста, используйте backtrader из моего репозитория (так как вы можете размещать в нем свои коммиты). Установите его:
 ```shell
 pip install git+https://github.com/WISEPLAT/backtrader.git
 ```
+-- Могу ли я использовать ваш интерфейс binance с оригинальным backtrader?
+
+-- Да, вы можете использовать оригинальный backtrader, так как автор оригинального backtrader одобрил все мои изменения.
+
+Вот ссылка: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
 
 3) У нас есть некоторые зависимости, вам нужно их установить:
 ```shell
 pip install python-binance pandas matplotlib
 ```
 
 ### Начало работы
```

### Comparing `backtrader_binance-1.0.3/backtrader_binance/binance_broker.py` & `backtrader_binance-1.0.4/backtrader_binance/binance_broker.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.3/backtrader_binance/binance_feed.py` & `backtrader_binance-1.0.4/backtrader_binance/binance_feed.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.3/backtrader_binance/binance_store.py` & `backtrader_binance-1.0.4/backtrader_binance/binance_store.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.3/backtrader_binance.egg-info/PKG-INFO` & `backtrader_binance-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: backtrader-binance
-Version: 1.0.3
+Name: backtrader_binance
+Version: 1.0.4
 Summary: Binance API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_binance
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
 Keywords: trading,development
@@ -46,14 +46,19 @@
 pip install git+https://github.com/WISEPLAT/backtrader_binance.git
 ```
 
 2) Please use backtrader from my repository (as your can push your commits in it). Install it:
 ```shell
 pip install git+https://github.com/WISEPLAT/backtrader.git
 ```
+-- Can I use your binance interface with original backtrader?
+
+-- Yes, you can use original backtrader, as the author of original backtrader had approved all my changes. 
+
+Here is the link: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
 
 3) We have some dependencies, you need to install them: 
 ```shell
 pip install python-binance pandas matplotlib
 ```
 
 ### Getting started
@@ -183,14 +188,19 @@
 pip install git+https://github.com/WISEPLAT/backtrader_binance.git
 ```
 
 2) Пожалуйста, используйте backtrader из моего репозитория (так как вы можете размещать в нем свои коммиты). Установите его:
 ```shell
 pip install git+https://github.com/WISEPLAT/backtrader.git
 ```
+-- Могу ли я использовать ваш интерфейс binance с оригинальным backtrader?
+
+-- Да, вы можете использовать оригинальный backtrader, так как автор оригинального backtrader одобрил все мои изменения.
+
+Вот ссылка: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
 
 3) У нас есть некоторые зависимости, вам нужно их установить:
 ```shell
 pip install python-binance pandas matplotlib
 ```
 
 ### Начало работы
```

### Comparing `backtrader_binance-1.0.3/setup.py` & `backtrader_binance-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the relevant file
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='backtrader_binance',
-      version='1.0.3',
+      version='1.0.4',
       author='wiseplat',
       author_email='oshpagin@gmail.com',
       license='MIT License',
       description='Binance API integration with Backtrader',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/WISEPLAT/backtrader_binance',
```

