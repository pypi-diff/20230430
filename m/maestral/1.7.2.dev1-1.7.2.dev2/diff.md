# Comparing `tmp/maestral-1.7.2.dev1.tar.gz` & `tmp/maestral-1.7.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral-1.7.2.dev1.tar", last modified: Sun Apr 30 12:47:11 2023, max compression
+gzip compressed data, was "maestral-1.7.2.dev2.tar", last modified: Sun Apr 30 12:47:14 2023, max compression
```

## Comparing `maestral-1.7.2.dev1.tar` & `maestral-1.7.2.dev2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.883341 maestral-1.7.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-30 12:47:11.883341 maestral-1.7.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:47:11.883341 maestral-1.7.2.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.875342 maestral-1.7.2.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.875342 maestral-1.7.2.dev1/src/maestral/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/autostart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.879341 maestral-1.7.2.dev1/src/maestral/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/cli_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/cli_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/cli_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    69523 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.879341 maestral-1.7.2.dev1/src/maestral/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/config/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.879341 maestral-1.7.2.dev1/src/maestral/database/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/database/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17525 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/database/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/database/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/database/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/errorhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.879341 maestral-1.7.2.dev1/src/maestral/fsevents/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/fsevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/fsevents/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63172 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29677 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.879341 maestral-1.7.2.dev1/src/maestral/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   137001 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/resources/maestral.png
--rw-r--r--   0 runner    (1001) docker     (123)   147935 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.883341 maestral-1.7.2.dev1/src/maestral/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/utils/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/utils/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/utils/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-04-30 12:46:50.000000 maestral-1.7.2.dev1/src/maestral/utils/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:11.879341 maestral-1.7.2.dev1/src/maestral.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-30 12:47:11.000000 maestral-1.7.2.dev1/src/maestral.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-30 12:47:11.000000 maestral-1.7.2.dev1/src/maestral.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:47:11.000000 maestral-1.7.2.dev1/src/maestral.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 12:47:11.000000 maestral-1.7.2.dev1/src/maestral.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-30 12:47:11.000000 maestral-1.7.2.dev1/src/maestral.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 12:47:11.000000 maestral-1.7.2.dev1/src/maestral.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.423205 maestral-1.7.2.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.427205 maestral-1.7.2.dev2/src/maestral/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/autostart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.427205 maestral-1.7.2.dev2/src/maestral/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69523 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/config/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17525 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/errorhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/fsevents/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/fsevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/fsevents/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63172 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29677 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137001 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/resources/maestral.png
+-rw-r--r--   0 runner    (1001) docker     (123)   147935 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.427205 maestral-1.7.2.dev2/src/maestral.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/top_level.txt
```

### Comparing `maestral-1.7.2.dev1/LICENSE.txt` & `maestral-1.7.2.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/PKG-INFO` & `maestral-1.7.2.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral
-Version: 1.7.2.dev1
+Version: 1.7.2.dev2
 Summary: Open-source Dropbox client for macOS and Linux.
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://maestral.app
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
```

### Comparing `maestral-1.7.2.dev1/README.md` & `maestral-1.7.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/pyproject.toml` & `maestral-1.7.2.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maestral"
-version = "1.7.2.dev1"
+version = "1.7.2.dev2"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Open-source Dropbox client for macOS and Linux."
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: Unix",
     "Programming Language :: Python",
```

### Comparing `maestral-1.7.2.dev1/src/maestral/autostart.py` & `maestral-1.7.2.dev2/src/maestral/autostart.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/cli_core.py` & `maestral-1.7.2.dev2/src/maestral/cli/cli_core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/cli_info.py` & `maestral-1.7.2.dev2/src/maestral/cli/cli_info.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/cli_main.py` & `maestral-1.7.2.dev2/src/maestral/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/cli_maintenance.py` & `maestral-1.7.2.dev2/src/maestral/cli/cli_maintenance.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/cli_settings.py` & `maestral-1.7.2.dev2/src/maestral/cli/cli_settings.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/common.py` & `maestral-1.7.2.dev2/src/maestral/cli/common.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/core.py` & `maestral-1.7.2.dev2/src/maestral/cli/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/dialogs.py` & `maestral-1.7.2.dev2/src/maestral/cli/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/cli/output.py` & `maestral-1.7.2.dev2/src/maestral/cli/output.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/client.py` & `maestral-1.7.2.dev2/src/maestral/client.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/config/__init__.py` & `maestral-1.7.2.dev2/src/maestral/config/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/config/main.py` & `maestral-1.7.2.dev2/src/maestral/config/main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/config/user.py` & `maestral-1.7.2.dev2/src/maestral/config/user.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/constants.py` & `maestral-1.7.2.dev2/src/maestral/constants.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/core.py` & `maestral-1.7.2.dev2/src/maestral/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/daemon.py` & `maestral-1.7.2.dev2/src/maestral/daemon.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/database/core.py` & `maestral-1.7.2.dev2/src/maestral/database/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/database/orm.py` & `maestral-1.7.2.dev2/src/maestral/database/orm.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/database/query.py` & `maestral-1.7.2.dev2/src/maestral/database/query.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/database/types.py` & `maestral-1.7.2.dev2/src/maestral/database/types.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/errorhandling.py` & `maestral-1.7.2.dev2/src/maestral/errorhandling.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/exceptions.py` & `maestral-1.7.2.dev2/src/maestral/exceptions.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/fsevents/__init__.py` & `maestral-1.7.2.dev2/src/maestral/fsevents/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/fsevents/polling.py` & `maestral-1.7.2.dev2/src/maestral/fsevents/polling.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/keyring.py` & `maestral-1.7.2.dev2/src/maestral/keyring.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/logging.py` & `maestral-1.7.2.dev2/src/maestral/logging.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/main.py` & `maestral-1.7.2.dev2/src/maestral/main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/manager.py` & `maestral-1.7.2.dev2/src/maestral/manager.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/models.py` & `maestral-1.7.2.dev2/src/maestral/models.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/notify.py` & `maestral-1.7.2.dev2/src/maestral/notify.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/resources/maestral.png` & `maestral-1.7.2.dev2/src/maestral/resources/maestral.png`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/sync.py` & `maestral-1.7.2.dev2/src/maestral/sync.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/utils/__init__.py` & `maestral-1.7.2.dev2/src/maestral/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/utils/appdirs.py` & `maestral-1.7.2.dev2/src/maestral/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/utils/caches.py` & `maestral-1.7.2.dev2/src/maestral/utils/caches.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/utils/hashing.py` & `maestral-1.7.2.dev2/src/maestral/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/utils/integration.py` & `maestral-1.7.2.dev2/src/maestral/utils/integration.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral/utils/path.py` & `maestral-1.7.2.dev2/src/maestral/utils/path.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral.egg-info/PKG-INFO` & `maestral-1.7.2.dev2/src/maestral.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral
-Version: 1.7.2.dev1
+Version: 1.7.2.dev2
 Summary: Open-source Dropbox client for macOS and Linux.
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://maestral.app
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
```

### Comparing `maestral-1.7.2.dev1/src/maestral.egg-info/SOURCES.txt` & `maestral-1.7.2.dev2/src/maestral.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev1/src/maestral.egg-info/requires.txt` & `maestral-1.7.2.dev2/src/maestral.egg-info/requires.txt`

 * *Files identical despite different names*

