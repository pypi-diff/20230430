# Comparing `tmp/discloud-1.0.1.tar.gz` & `tmp/discloud-1.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discloud-1.0.1.tar", last modified: Sun Apr 30 17:28:35 2023, max compression
+gzip compressed data, was "discloud-1.0.3a0.tar", last modified: Wed Jan 12 00:30:29 2022, max compression
```

## Comparing `discloud-1.0.1.tar` & `discloud-1.0.3a0.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 17:28:35.043119 discloud-1.0.1/
--rw-rw-rw-   0        0        0     6420 2023-04-30 17:28:35.038131 discloud-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5791 2023-03-09 19:44:38.000000 discloud-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 17:28:34.909943 discloud-1.0.1/discloud/
--rw-rw-rw-   0        0        0       91 2022-09-09 19:30:31.000000 discloud-1.0.1/discloud/__init__.py
--rw-rw-rw-   0        0        0     8132 2023-03-09 19:05:02.000000 discloud-1.0.1/discloud/client.py
--rw-rw-rw-   0        0        0     5938 2023-04-30 17:17:46.000000 discloud-1.0.1/discloud/discloud.py
--rw-rw-rw-   0        0        0     1636 2023-03-09 19:06:11.000000 discloud-1.0.1/discloud/discloud_typing.py
--rw-rw-rw-   0        0        0      303 2022-09-09 21:27:24.000000 discloud-1.0.1/discloud/errors.py
--rw-rw-rw-   0        0        0    11749 2023-03-09 18:45:19.000000 discloud-1.0.1/discloud/http.py
--rw-rw-rw-   0        0        0     1006 2022-09-09 21:27:24.000000 discloud-1.0.1/discloud/old.py
--rw-rw-rw-   0        0        0     5376 2023-02-19 17:51:22.000000 discloud-1.0.1/discloud/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 17:28:35.035138 discloud-1.0.1/discloud.egg-info/
--rw-rw-rw-   0        0        0     6420 2023-04-30 17:28:34.000000 discloud-1.0.1/discloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-04-30 17:28:34.000000 discloud-1.0.1/discloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 17:28:34.000000 discloud-1.0.1/discloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-30 17:28:34.000000 discloud-1.0.1/discloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 17:28:34.000000 discloud-1.0.1/discloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      746 2023-04-30 17:27:36.000000 discloud-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 17:28:35.044125 discloud-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-04-30 17:24:25.000000 discloud-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-12 00:30:29.102439 discloud-1.0.3a0/
+-rw-rw-rw-   0        0        0     2113 2022-01-12 00:30:29.101441 discloud-1.0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1497 2022-01-12 00:25:53.000000 discloud-1.0.3a0/README.md
+drwxrwxrwx   0        0        0        0 2022-01-12 00:30:29.070527 discloud-1.0.3a0/discloud/
+-rw-rw-rw-   0        0        0      146 2022-01-12 00:25:53.000000 discloud-1.0.3a0/discloud/__init__.py
+-rw-rw-rw-   0        0        0     1280 2022-01-12 00:25:53.000000 discloud-1.0.3a0/discloud/client.py
+-rw-rw-rw-   0        0        0     3753 2022-01-12 00:25:53.000000 discloud-1.0.3a0/discloud/discloud.py
+-rw-rw-rw-   0        0        0      903 2022-01-12 00:25:53.000000 discloud-1.0.3a0/discloud/errors.py
+-rw-rw-rw-   0        0        0     2662 2022-01-12 00:25:53.000000 discloud-1.0.3a0/discloud/http.py
+-rw-rw-rw-   0        0        0      962 2022-01-12 00:25:53.000000 discloud-1.0.3a0/discloud/old.py
+-rw-rw-rw-   0        0        0     4339 2022-01-12 00:25:53.000000 discloud-1.0.3a0/discloud/utils.py
+drwxrwxrwx   0        0        0        0 2022-01-12 00:30:29.095464 discloud-1.0.3a0/discloud.egg-info/
+-rw-rw-rw-   0        0        0     2113 2022-01-12 00:30:28.000000 discloud-1.0.3a0/discloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2022-01-12 00:30:28.000000 discloud-1.0.3a0/discloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-12 00:30:28.000000 discloud-1.0.3a0/discloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-01-12 00:30:28.000000 discloud-1.0.3a0/discloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-12 00:30:29.103437 discloud-1.0.3a0/setup.cfg
+-rw-rw-rw-   0        0        0      767 2022-01-12 00:25:53.000000 discloud-1.0.3a0/setup.py
```

