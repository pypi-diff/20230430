# Comparing `tmp/loxt_models-0.1.0.tar.gz` & `tmp/loxt_models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loxt_models-0.1.0.tar", max compression
+gzip compressed data, was "loxt_models-0.1.1.tar", max compression
```

## Comparing `loxt_models-0.1.0.tar` & `loxt_models-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,27 @@
--rw-r--r--   0        0        0        0 2023-03-01 21:20:33.321433 loxt_models-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-01 20:51:58.516046 loxt_models-0.1.0/loxt_models/__init__.py
--rw-r--r--   0        0        0      378 2023-03-01 21:07:31.052547 loxt_models-0.1.0/loxt_models/deck.py
--rw-r--r--   0        0        0     1010 2023-03-01 21:07:31.064547 loxt_models-0.1.0/loxt_models/extension.py
--rw-r--r--   0        0        0      380 2023-03-01 21:07:31.072546 loxt_models-0.1.0/loxt_models/panel.py
--rw-r--r--   0        0        0      205 2023-03-01 21:07:31.060547 loxt_models-0.1.0/loxt_models/sidebar.py
--rw-r--r--   0        0        0      309 2023-03-01 20:51:06.559788 loxt_models-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 loxt_models-0.1.0/setup.py
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 loxt_models-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-01 21:20:33.321433 loxt_models-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-31 20:53:35.668768 loxt_models-0.1.1/loxt_models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:27:03.860786 loxt_models-0.1.1/loxt_models/controls/__init__.py
+-rw-r--r--   0        0        0      158 2023-03-09 22:28:52.476217 loxt_models-0.1.1/loxt_models/controls/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1178 2023-04-01 16:08:03.907168 loxt_models-0.1.1/loxt_models/controls/__pycache__/button_control.cpython-310.pyc
+-rw-r--r--   0        0        0     2054 2023-04-30 09:31:58.261126 loxt_models-0.1.1/loxt_models/controls/__pycache__/control_base.cpython-310.pyc
+-rw-r--r--   0        0        0     1076 2023-03-12 21:11:40.067110 loxt_models-0.1.1/loxt_models/controls/__pycache__/edit_control.cpython-310.pyc
+-rw-r--r--   0        0        0     1086 2023-03-12 21:11:40.067110 loxt_models-0.1.1/loxt_models/controls/__pycache__/label_control.cpython-310.pyc
+-rw-r--r--   0        0        0     1254 2023-03-09 21:23:26.117132 loxt_models-0.1.1/loxt_models/controls/__pycache__/property_value.cpython-310.pyc
+-rw-r--r--   0        0        0      796 2023-04-01 16:04:42.514487 loxt_models-0.1.1/loxt_models/controls/button_control.py
+-rw-r--r--   0        0        0     1604 2023-04-30 09:40:36.462705 loxt_models-0.1.1/loxt_models/controls/control_base.py
+-rw-r--r--   0        0        0      662 2023-03-12 21:11:04.390783 loxt_models-0.1.1/loxt_models/controls/edit_control.py
+-rw-r--r--   0        0        0      726 2023-04-30 09:41:48.405072 loxt_models-0.1.1/loxt_models/controls/label_control.py
+-rw-r--r--   0        0        0      896 2023-03-09 21:19:45.668270 loxt_models-0.1.1/loxt_models/controls/property_value.py
+-rw-r--r--   0        0        0     2810 2023-04-28 20:55:02.981936 loxt_models-0.1.1/loxt_models/deck.py
+-rw-r--r--   0        0        0     1517 2023-04-02 21:15:22.193846 loxt_models-0.1.1/loxt_models/extension.py
+-rw-r--r--   0        0        0        0 2023-04-01 15:19:27.162490 loxt_models-0.1.1/loxt_models/listeners/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-01 15:56:53.120433 loxt_models-0.1.1/loxt_models/listeners/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      874 2023-04-01 15:56:53.120433 loxt_models-0.1.1/loxt_models/listeners/__pycache__/action_listener.cpython-310.pyc
+-rw-r--r--   0        0        0      382 2023-04-01 15:25:53.369178 loxt_models-0.1.1/loxt_models/listeners/action_listener.py
+-rw-r--r--   0        0        0     3845 2023-04-30 14:00:20.996495 loxt_models-0.1.1/loxt_models/panel.py
+-rw-r--r--   0        0        0      320 2023-03-24 21:26:27.547294 loxt_models-0.1.1/loxt_models/sidebar.py
+-rw-r--r--   0        0        0      524 2023-03-31 21:04:54.972685 loxt_models-0.1.1/loxt_models/utils.py
+-rw-r--r--   0        0        0     1874 2023-04-28 20:47:24.397948 loxt_models-0.1.1/loxt_models/x_ui_panel.py
+-rw-r--r--   0        0        0      370 2023-04-30 14:02:42.097159 loxt_models-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 loxt_models-0.1.1/setup.py
+-rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 loxt_models-0.1.1/PKG-INFO
```

