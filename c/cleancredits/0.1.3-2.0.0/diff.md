# Comparing `tmp/cleancredits-0.1.3.tar.gz` & `tmp/cleancredits-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleancredits-0.1.3.tar", last modified: Mon Nov  2 18:37:05 2020, max compression
+gzip compressed data, was "cleancredits-2.0.0.tar", last modified: Sun Apr 30 20:36:26 2023, max compression
```

## Comparing `cleancredits-0.1.3.tar` & `cleancredits-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2020-11-02 18:37:05.964910 cleancredits-0.1.3/
--rw-r--r--   0 user       (502) staff       (20)     1950 2020-11-02 18:37:05.964525 cleancredits-0.1.3/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)     1309 2020-11-02 04:36:27.000000 cleancredits-0.1.3/README.txt
-drwxr-xr-x   0 user       (502) staff       (20)        0 2020-11-02 18:37:05.953551 cleancredits-0.1.3/cleancredits/
--rw-r--r--   0 user       (502) staff       (20)        0 2020-11-02 03:05:07.000000 cleancredits-0.1.3/cleancredits/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     2264 2020-11-02 17:02:30.000000 cleancredits-0.1.3/cleancredits/__main__.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2020-11-02 18:37:05.963920 cleancredits-0.1.3/cleancredits.egg-info/
--rw-r--r--   0 user       (502) staff       (20)     1950 2020-11-02 18:37:05.000000 cleancredits-0.1.3/cleancredits.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      213 2020-11-02 18:37:05.000000 cleancredits-0.1.3/cleancredits.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2020-11-02 18:37:05.000000 cleancredits-0.1.3/cleancredits.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)       13 2020-11-02 18:37:05.000000 cleancredits-0.1.3/cleancredits.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)       38 2020-11-02 18:37:05.965016 cleancredits-0.1.3/setup.cfg
--rw-r--r--   0 user       (502) staff       (20)      472 2020-11-02 18:36:48.000000 cleancredits-0.1.3/setup.py
+drwxr-xr-x   0 madelyn    (501) staff       (20)        0 2023-04-30 20:36:26.592494 cleancredits-2.0.0/
+-rw-rw-r--   0 madelyn    (501) staff       (20)    35149 2023-04-30 17:47:04.000000 cleancredits-2.0.0/LICENSE
+-rw-rw-r--   0 madelyn    (501) staff       (20)       25 2023-04-30 17:47:04.000000 cleancredits-2.0.0/MANIFEST.in
+-rw-r--r--   0 madelyn    (501) staff       (20)     4478 2023-04-30 20:36:26.592395 cleancredits-2.0.0/PKG-INFO
+-rw-rw-r--   0 madelyn    (501) staff       (20)     3865 2023-04-30 17:47:04.000000 cleancredits-2.0.0/README.md
+drwxr-xr-x   0 madelyn    (501) staff       (20)        0 2023-04-30 20:36:26.591438 cleancredits-2.0.0/cleancredits/
+-rw-rw-r--   0 madelyn    (501) staff       (20)        2 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/__init__.py
+-rw-rw-r--   0 madelyn    (501) staff       (20)       22 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/__version__.py
+-rw-rw-r--   0 madelyn    (501) staff       (20)     6880 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/cli.py
+-rw-rw-r--   0 madelyn    (501) staff       (20)     2164 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/cli_test.py
+-rw-rw-r--   0 madelyn    (501) staff       (20)    21431 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/gui.py
+-rw-rw-r--   0 madelyn    (501) staff       (20)     3374 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/helpers.py
+-rw-rw-r--   0 madelyn    (501) staff       (20)     3285 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/helpers_test.py
+-rw-rw-r--   0 madelyn    (501) staff       (20)     1498 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/param_types.py
+-rw-rw-r--   0 madelyn    (501) staff       (20)     2069 2023-04-30 17:47:04.000000 cleancredits-2.0.0/cleancredits/param_types_test.py
+drwxr-xr-x   0 madelyn    (501) staff       (20)        0 2023-04-30 20:36:26.592250 cleancredits-2.0.0/cleancredits.egg-info/
+-rw-r--r--   0 madelyn    (501) staff       (20)     4478 2023-04-30 20:36:26.000000 cleancredits-2.0.0/cleancredits.egg-info/PKG-INFO
+-rw-r--r--   0 madelyn    (501) staff       (20)      488 2023-04-30 20:36:26.000000 cleancredits-2.0.0/cleancredits.egg-info/SOURCES.txt
+-rw-r--r--   0 madelyn    (501) staff       (20)        1 2023-04-30 20:36:26.000000 cleancredits-2.0.0/cleancredits.egg-info/dependency_links.txt
+-rw-r--r--   0 madelyn    (501) staff       (20)       54 2023-04-30 20:36:26.000000 cleancredits-2.0.0/cleancredits.egg-info/entry_points.txt
+-rw-r--r--   0 madelyn    (501) staff       (20)       61 2023-04-30 20:36:26.000000 cleancredits-2.0.0/cleancredits.egg-info/requires.txt
+-rw-r--r--   0 madelyn    (501) staff       (20)       13 2023-04-30 20:36:26.000000 cleancredits-2.0.0/cleancredits.egg-info/top_level.txt
+-rw-r--r--   0 madelyn    (501) staff       (20)       38 2023-04-30 20:36:26.592526 cleancredits-2.0.0/setup.cfg
+-rw-rw-r--   0 madelyn    (501) staff       (20)     3635 2023-04-30 17:47:04.000000 cleancredits-2.0.0/setup.py
```

