# Comparing `tmp/maestral-cocoa-1.7.2.tar.gz` & `tmp/maestral-cocoa-1.7.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral-cocoa-1.7.2.tar", last modified: Sun Apr 30 21:33:21 2023, max compression
+gzip compressed data, was "maestral-cocoa-1.7.2.dev2.tar", last modified: Sun Apr 30 13:07:55 2023, max compression
```

## Comparing `maestral-cocoa-1.7.2.tar` & `maestral-cocoa-1.7.2.dev2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.835112 maestral-cocoa-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-30 21:33:21.835112 maestral-cocoa-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-30 21:33:21.835112 maestral-cocoa-1.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.823112 maestral-cocoa-1.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.827112 maestral-cocoa-1.7.2/src/maestral_cocoa/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/autostart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/bandwidth_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/dbx_location_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.831112 maestral-cocoa-1.7.2/src/maestral_cocoa/private/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.831112 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.831112 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/cocoa/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/cocoa/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29146 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/cocoa/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.831112 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/gtk/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/gtk/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/private/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.835112 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48199 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/faceholder.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   842676 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/maestral.icns
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/release_notes.css
--rw-r--r--   0 runner    (1001) docker     (123)    51081 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-disconnected.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    47443 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-error.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    52917 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-idle.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    52604 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-info.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    46340 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-paused.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    50085 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-syncing.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/selective_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/selective_sync_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/settings_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/setup_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/syncissues.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-30 21:33:04.000000 maestral-cocoa-1.7.2/src/maestral_cocoa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:33:21.831112 maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-30 21:33:21.000000 maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-30 21:33:21.000000 maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 21:33:21.000000 maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-30 21:33:21.000000 maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 21:33:21.000000 maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-30 21:33:21.000000 maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 21:33:21.000000 maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.873165 maestral-cocoa-1.7.2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-30 13:07:55.873165 maestral-cocoa-1.7.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-30 13:07:55.873165 maestral-cocoa-1.7.2.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.857164 maestral-cocoa-1.7.2.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.865165 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/bandwidth_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/dbx_location_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.865165 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.869165 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.869165 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/cocoa/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29146 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/cocoa/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.869165 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/gtk/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/gtk/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20827 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.873165 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48199 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/faceholder.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   842676 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/maestral.icns
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/release_notes.css
+-rw-r--r--   0 runner    (1001) docker     (123)    51081 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-disconnected.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    47443 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-error.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    52917 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-idle.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    52604 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-info.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    46340 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-paused.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    50085 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-syncing.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/selective_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/selective_sync_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/settings_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/setup_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/syncissues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-30 13:07:39.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 13:07:55.865165 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-30 13:07:55.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-30 13:07:55.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:07:55.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-30 13:07:55.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 13:07:55.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-30 13:07:55.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 13:07:55.000000 maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/top_level.txt
```

### Comparing `maestral-cocoa-1.7.2/LICENSE.txt` & `maestral-cocoa-1.7.2.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/PKG-INFO` & `maestral-cocoa-1.7.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-cocoa
-Version: 1.7.2
+Version: 1.7.2.dev2
 Summary: Open-source Dropbox client for macOS and Linux.
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `maestral-cocoa-1.7.2/pyproject.toml` & `maestral-cocoa-1.7.2.dev2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.briefcase]
 project_name = "Maestral"
 bundle = "com.samschott.maestral"
-version = "1.7.2"
+version = "1.7.2.dev2"
 url = "https://maestral.app"
 license = "MIT license"
 author = "Sam Schott"
 author_email = "sam.schott@outlook.com"
 template = "https://github.com/samschott/briefcase-macOS-Xcode-template.git"
 template_branch = "maestral"
 
@@ -14,27 +14,27 @@
 description = "An open-source Dropbox client for macOS and Linux"
 icon = "icon/maestral"
 sources = ["src/maestral_cocoa"]
 requires = [
     "chardet==5.1.0",
     "click==8.1.3",
     "importlib_metadata;python_version<'3.8'",
-    "maestral==1.7.2",
-    "markdown2==2.4.8",
-    "rubicon-objc==0.4.6",
+    "maestral==1.7.2.dev2",
+    "markdown2==2.4.6",
+    "rubicon-objc==0.4.5",
     "toga==0.3.1",
 ]
 sparkle_feed_url = "https://maestral.app/appcast.xml"
 sparkle_public_key = "RugM2eM14xHixaeHpl5uWSq7+sDZvYi52Xpz4IXpAdA="
 
 [tool.briefcase.app.maestral-cocoa.macOS]
 requires = [
     "toga-cocoa==0.3.1",
 ]
-build = "85"
+build = "84"
 
 [tool.briefcase.app.maestral-cocoa.linux]
 supported = false
 
 [tool.black]
 line-length = 88
 target-version = ["py37", "py38", "py39", "py310", "py311"]
```

### Comparing `maestral-cocoa-1.7.2/setup.cfg` & `maestral-cocoa-1.7.2.dev2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = maestral-cocoa
-version = 1.7.2
+version = 1.7.2.dev2
 author = Sam Schott
 author_email = sam.schott@outlook.com
 license = MIT
 description = Open-source Dropbox client for macOS and Linux.
 url = https://maestral.app
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -24,15 +24,15 @@
 packages = find:
 package_dir = 
 	= src
 zip_safe = False
 setup_requires = build
 install_requires = 
 	click
-	maestral>=1.7.2
+	maestral>=1.7.2.dev2
 	markdown2
 	toga==0.3.1
 	rubicon-objc>=0.4.5
 python_requires = >=3.7
 
 [options.packages.find]
 where = src
```

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/__main__.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/__main__.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/activity.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/activity.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,53 +24,52 @@
 
 PADDING = 10
 ICON_SIZE = 32
 WINDOW_SIZE = (700, 600)
 
 
 class SyncEventRow:
-    _reveal_button: FreestandingIconButton | None
+    _reveal: FreestandingIconButton | None
 
     def __init__(self, sync_event: SyncEvent) -> None:
         self.sync_event = sync_event
 
         dirname, basename = osp.split(self.sync_event.local_path)
         dt = datetime.fromtimestamp(self.sync_event.change_time_or_sync_time)
 
         # attributes for table column values
+        self._basename = basename
+        self._icon: Icon | None = None
         self.location = osp.basename(dirname)
         self.type = self.sync_event.change_type.value.capitalize()
         self.time = dt.strftime("%d %b %Y %H:%M")
         self.username = self.sync_event.change_user_name
-
-        self._basename = basename
-        self._icon: Icon | None = None
-        self._reveal_button = None
+        self._reveal = None
 
     @property
     def filename(self) -> tuple[Icon, str]:
         if not self._icon:
             if self.sync_event.item_type is ItemType.Folder:
                 self._icon = Icon(for_path="/usr")
             else:
                 self._icon = Icon(for_path=self.sync_event.local_path)
 
         return self._icon, sanitize_string(self._basename)
 
     @property
     def reveal(self) -> FreestandingIconButton:
-        if not self._reveal_button:
-            self._reveal_button = FreestandingIconButton(
+        if not self._reveal:
+            self._reveal = FreestandingIconButton(
                 text="",
                 icon=Icon(template=ImageTemplate.Reveal),
                 on_press=self.on_reveal_pressed,
             )
-            self._reveal_button.enabled = osp.exists(self.sync_event.local_path)
+            self._reveal.enabled = osp.exists(self.sync_event.local_path)
 
-        return self._reveal_button
+        return self._reveal
 
     def on_reveal_pressed(self, widget: Any) -> None:
         click.launch(self.sync_event.local_path, locate=True)
 
     def refresh(self) -> None:
         self.reveal.enabled = osp.exists(self.sync_event.local_path)
```

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/app.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/app.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/autostart.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/autostart.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/bandwidth.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/bandwidth.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/bandwidth_gui.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/bandwidth_gui.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/dbx_location_dialog.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/dbx_location_dialog.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/dialogs.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/cocoa/constants.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/cocoa/constants.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/cocoa/dialogs.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/cocoa/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/private/implementation/cocoa/factory.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/implementation/cocoa/factory.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/private/platform.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/platform.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/private/widgets.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/private/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,23 +173,14 @@
 
         # Set all the properties
         self.text = text
         self.on_press = on_press
         self.icon = icon
 
     @property
-    def on_press(self):
-        """The handler to invoke when the button is pressed."""
-        return self._on_press
-
-    @on_press.setter
-    def on_press(self, handler):
-        self._on_press = wrapped_handler(self, handler)
-
-    @property
     def text(self):
         """
         Returns:
             The button text as a ``str``
         """
         return self._text
 
@@ -212,14 +203,33 @@
 
     @icon.setter
     def icon(self, value):
         self._icon = value
         self._impl.set_icon(value)
         self._impl.rehint()
 
+    @property
+    def on_press(self):
+        """The handler to invoke when the button is pressed.
+
+        Returns:
+            The function ``callable`` that is called on button press.
+        """
+        return self._on_press
+
+    @on_press.setter
+    def on_press(self, handler):
+        """Set the handler to invoke when the button is pressed.
+
+        Args:
+            handler (:obj:`callable`): The handler to invoke when the button is pressed.
+        """
+        self._on_press = wrapped_handler(self, handler)
+        self._impl.set_on_press(self._on_press)
+
 
 class FollowLinkButton(FreestandingIconButton):
     def __init__(
         self,
         text,
         url=None,
         locate=False,
```

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/__init__.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/faceholder.pdf` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/faceholder.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/maestral.icns` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/maestral.icns`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-disconnected.pdf` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-disconnected.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-error.pdf` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-error.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-idle.pdf` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-idle.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-info.pdf` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-info.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-paused.pdf` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-paused.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/resources/systray-syncing.pdf` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/resources/systray-syncing.pdf`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/selective_sync.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/selective_sync.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/selective_sync_gui.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/selective_sync_gui.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/settings.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/settings.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/settings_gui.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/settings_gui.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/setup.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/setup.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/setup_gui.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/setup_gui.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/syncissues.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/syncissues.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/updater.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/updater.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa/utils.py` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa/utils.py`

 * *Files identical despite different names*

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/PKG-INFO` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral-cocoa
-Version: 1.7.2
+Version: 1.7.2.dev2
 Summary: Open-source Dropbox client for macOS and Linux.
 Home-page: https://maestral.app
 Author: Sam Schott
 Author-email: sam.schott@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `maestral-cocoa-1.7.2/src/maestral_cocoa.egg-info/SOURCES.txt` & `maestral-cocoa-1.7.2.dev2/src/maestral_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

