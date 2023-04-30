# Comparing `tmp/QPUIQ-0.1.7.tar.gz` & `tmp/QPUIQ-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.1.7.tar", last modified: Sat Apr 29 21:13:42 2023, max compression
+gzip compressed data, was "QPUIQ-0.1.8.tar", last modified: Sun Apr 30 05:52:49 2023, max compression
```

## Comparing `QPUIQ-0.1.7.tar` & `QPUIQ-0.1.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.781408 QPUIQ-0.1.7/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.7/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-04-29 21:13:42.781267 QPUIQ-0.1.7/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.768460 QPUIQ-0.1.7/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.770999 QPUIQ-0.1.7/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)      857 2023-04-29 20:10:13.000000 QPUIQ-0.1.7/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.1.7/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     1188 2023-04-29 16:10:01.000000 QPUIQ-0.1.7/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.7/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2138 2023-04-29 14:36:14.000000 QPUIQ-0.1.7/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.7/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      543 2023-04-26 17:57:33.000000 QPUIQ-0.1.7/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.7/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.7/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-04-29 16:58:24.000000 QPUIQ-0.1.7/PUI/PySide6/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.773580 QPUIQ-0.1.7/PUI/Qt5/
--rw-r--r--   0 Bug        (504) staff       (20)      417 2023-04-29 17:06:45.000000 QPUIQ-0.1.7/PUI/Qt5/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      496 2023-04-29 18:30:13.000000 QPUIQ-0.1.7/PUI/Qt5/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     1139 2023-04-29 17:07:47.000000 QPUIQ-0.1.7/PUI/Qt5/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.7/PUI/Qt5/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.7/PUI/Qt5/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.7/PUI/Qt5/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.7/PUI/Qt5/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.7/PUI/Qt5/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.7/PUI/Qt5/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1297 2023-04-29 17:05:56.000000 QPUIQ-0.1.7/PUI/Qt5/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      486 2023-04-29 21:13:28.000000 QPUIQ-0.1.7/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      458 2023-04-29 06:46:04.000000 QPUIQ-0.1.7/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-29 19:40:07.000000 QPUIQ-0.1.7/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.776066 QPUIQ-0.1.7/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      452 2023-04-29 19:08:30.000000 QPUIQ-0.1.7/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      551 2023-04-29 19:19:55.000000 QPUIQ-0.1.7/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.7/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.7/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.7/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.7/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.7/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.7/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      482 2023-04-29 19:19:13.000000 QPUIQ-0.1.7/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     3075 2023-04-29 20:53:50.000000 QPUIQ-0.1.7/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)     8973 2023-04-29 20:54:27.000000 QPUIQ-0.1.7/PUI/state.py
--rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.7/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.778418 QPUIQ-0.1.7/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      414 2023-04-29 18:25:14.000000 QPUIQ-0.1.7/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      568 2023-04-29 18:55:09.000000 QPUIQ-0.1.7/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-04-29 19:57:02.000000 QPUIQ-0.1.7/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.7/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      954 2023-04-29 19:31:18.000000 QPUIQ-0.1.7/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.7/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1636 2023-04-29 19:55:02.000000 QPUIQ-0.1.7/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.7/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.7/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1530 2023-04-29 19:56:35.000000 QPUIQ-0.1.7/PUI/tkinter/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.780417 QPUIQ-0.1.7/PUI/urwid/
--rw-r--r--   0 Bug        (504) staff       (20)      429 2023-04-29 17:20:40.000000 QPUIQ-0.1.7/PUI/urwid/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     1246 2023-04-29 19:07:03.000000 QPUIQ-0.1.7/PUI/urwid/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.7/PUI/urwid/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.7/PUI/urwid/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.7/PUI/urwid/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.7/PUI/urwid/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.7/PUI/urwid/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      315 2023-04-29 19:07:06.000000 QPUIQ-0.1.7/PUI/urwid/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     2604 2023-04-29 21:12:02.000000 QPUIQ-0.1.7/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-29 21:13:42.781069 QPUIQ-0.1.7/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-04-29 21:13:42.000000 QPUIQ-0.1.7/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1251 2023-04-29 21:13:42.000000 QPUIQ-0.1.7/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-29 21:13:42.000000 QPUIQ-0.1.7/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-29 21:13:42.000000 QPUIQ-0.1.7/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2629 2023-04-29 21:00:52.000000 QPUIQ-0.1.7/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-29 21:13:42.781449 QPUIQ-0.1.7/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.1.7/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.775992 QPUIQ-0.1.8/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.8/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-04-30 05:52:49.775860 QPUIQ-0.1.8/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.769022 QPUIQ-0.1.8/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.770354 QPUIQ-0.1.8/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)      891 2023-04-30 05:45:53.000000 QPUIQ-0.1.8/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.1.8/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1187 2023-04-30 05:12:20.000000 QPUIQ-0.1.8/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.8/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2838 2023-04-30 05:45:40.000000 QPUIQ-0.1.8/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.8/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      543 2023-04-26 17:57:33.000000 QPUIQ-0.1.8/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.8/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.8/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-04-29 16:58:24.000000 QPUIQ-0.1.8/PUI/PySide6/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.771678 QPUIQ-0.1.8/PUI/Qt5/
+-rw-r--r--   0 Bug        (504) staff       (20)      417 2023-04-29 17:06:45.000000 QPUIQ-0.1.8/PUI/Qt5/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      496 2023-04-29 18:30:13.000000 QPUIQ-0.1.8/PUI/Qt5/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1138 2023-04-30 05:12:20.000000 QPUIQ-0.1.8/PUI/Qt5/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.8/PUI/Qt5/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.8/PUI/Qt5/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.8/PUI/Qt5/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.8/PUI/Qt5/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.8/PUI/Qt5/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.8/PUI/Qt5/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1297 2023-04-29 17:05:56.000000 QPUIQ-0.1.8/PUI/Qt5/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      486 2023-04-30 05:52:33.000000 QPUIQ-0.1.8/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      458 2023-04-29 06:46:04.000000 QPUIQ-0.1.8/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-29 19:40:07.000000 QPUIQ-0.1.8/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.772838 QPUIQ-0.1.8/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      452 2023-04-29 19:08:30.000000 QPUIQ-0.1.8/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      551 2023-04-29 19:19:55.000000 QPUIQ-0.1.8/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.8/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.8/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.8/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.8/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.8/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.8/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      482 2023-04-29 19:19:13.000000 QPUIQ-0.1.8/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3075 2023-04-29 20:53:50.000000 QPUIQ-0.1.8/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)     8973 2023-04-29 20:54:27.000000 QPUIQ-0.1.8/PUI/state.py
+-rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.8/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.774165 QPUIQ-0.1.8/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      414 2023-04-29 18:25:14.000000 QPUIQ-0.1.8/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      568 2023-04-29 18:55:09.000000 QPUIQ-0.1.8/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-04-29 19:57:02.000000 QPUIQ-0.1.8/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.8/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      954 2023-04-29 19:31:18.000000 QPUIQ-0.1.8/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.8/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1636 2023-04-29 19:55:02.000000 QPUIQ-0.1.8/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.8/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.8/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1530 2023-04-29 19:56:35.000000 QPUIQ-0.1.8/PUI/tkinter/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.775198 QPUIQ-0.1.8/PUI/urwid/
+-rw-r--r--   0 Bug        (504) staff       (20)      429 2023-04-29 17:20:40.000000 QPUIQ-0.1.8/PUI/urwid/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1246 2023-04-29 19:07:03.000000 QPUIQ-0.1.8/PUI/urwid/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.8/PUI/urwid/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.8/PUI/urwid/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.8/PUI/urwid/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.8/PUI/urwid/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.8/PUI/urwid/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      315 2023-04-29 19:07:06.000000 QPUIQ-0.1.8/PUI/urwid/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2604 2023-04-30 05:49:42.000000 QPUIQ-0.1.8/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.775682 QPUIQ-0.1.8/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-04-30 05:52:49.000000 QPUIQ-0.1.8/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1251 2023-04-30 05:52:49.000000 QPUIQ-0.1.8/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-30 05:52:49.000000 QPUIQ-0.1.8/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-30 05:52:49.000000 QPUIQ-0.1.8/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2629 2023-04-29 21:00:52.000000 QPUIQ-0.1.8/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-30 05:52:49.776027 QPUIQ-0.1.8/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.1.8/setup.py
```

### Comparing `QPUIQ-0.1.7/LICENSE.txt` & `QPUIQ-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PKG-INFO` & `QPUIQ-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.7
+Version: 0.1.8
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `QPUIQ-0.1.7/PUI/PySide6/__init__.py` & `QPUIQ-0.1.8/PUI/PySide6/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 HBox = QtHBox
 VBox = QtVBox
 Label = QtLabel
 Button = QtButton
 Canvas = QtCanvas
 CanvasText = QtCanvasText
 CanvasLine = QtCanvasLine
+CanvasPolyline = QtCanvasPolyline
 TextField = QtLineEdit
 ProgressBar = QtProgressBar
 
 def PUI(func):
     def func_wrapper(*args):
         class PUIViewWrapper(QPUIView):
             def __init__(self, name):
```

### Comparing `QPUIQ-0.1.7/PUI/PySide6/base.py` & `QPUIQ-0.1.8/PUI/PySide6/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,12 +29,12 @@
                 params["stretch"] = child.layout_weight
             self.ui.addWidget(child.ui, **params)
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
-            self.box.removeItem(child.ui)
+            self.ui.removeItem(child.ui)
         elif isinstance(child, QtBaseWidget):
             child.ui.setParent(None)
         elif child.children:
             self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.1.7/PUI/PySide6/button.py` & `QPUIQ-0.1.8/PUI/PySide6/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/PySide6/canvas.py` & `QPUIQ-0.1.8/PUI/Qt5/canvas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from .. import *
 from .base import *
 
-from PySide6 import QtWidgets
-from PySide6.QtGui import QPainter, QColor
-from PySide6.QtCore import QPoint
+from PyQt5 import QtWidgets
+from PyQt5.QtGui import QPainter, QColor
+from PyQt5.QtCore import QPoint
 
 class PUIQtCanvas(QtWidgets.QWidget):
-    def __init__(self, puinode, width=None, height=None):
+    def __init__(self, puinode):
         self.puinode = puinode
-        self.width = width
-        self.height = height
         super().__init__()
 
-    def sizeHint(self):
-        return QtCore.QSize(self.width, self.height)
-
     def paintEvent(self, event):
         qpainter = QPainter()
         qpainter.begin(self)
 
         for c in self.puinode.children:
             c.draw(qpainter)
 
         qpainter.end()
 
 class QtCanvas(QtBaseWidget):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.ui = None
+    def __init__(self, size=None, **kwargs):
+        super().__init__(**kwargs)
+        self.size = size
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
             self.ui.puinode = self
         else:
-            self.ui = PUIQtCanvas(self, self.layout_width or 0, self.layout_height or 0)
-        self.ui.resize(self.layout_width or 0, self.layout_height or 0)
+            self.ui = PUIQtCanvas(self)
+        x = 0
+        y = 0
+        w = 0
+        h = 0
+        if not self.size is None:
+            w, h = self.size
+        self.ui.setGeometry(x, y, w, h)
         self.ui.update()
 
 class QtCanvasText(PUINode):
     def __init__(self, x, y, text):
         super().__init__()
         self.x = x
         self.y = y
@@ -48,32 +49,17 @@
     def update(self, prev):
         pass
 
     def draw(self, qpainter):
         qpainter.drawText(QPoint(int(self.x), int(self.y)), self.text)
 
 class QtCanvasLine(PUINode):
-    def __init__(self, x1, y1, x2, y2, color=None, width=None):
+    def __init__(self, *args, **kwargs):
         super().__init__()
-        self.x1 = x1
-        self.y1 = y1
-        self.x2 = x2
-        self.y2 = y2
-        self.color = color
-        self.width = width
+        self.args = args
+        self.kwargs = kwargs
 
     def update(self, prev):
         pass
 
     def draw(self, qpainter):
-        pen = qpainter.pen()
-        color = pen.color()
-        width = pen.width()
-        if not self.color is None:
-            pen.setColor(QColor(self.color))
-        if not self.width is None:
-            pen.setWidth(self.width)
-        qpainter.setPen(pen)
-        qpainter.drawLine(self.x1, self.y1, self.x2, self.y2)
-        pen.setColor(color)
-        pen.setWidth(width)
-        qpainter.setPen(pen)
+        qpainter.drawLine(*self.args)
```

### Comparing `QPUIQ-0.1.7/PUI/PySide6/layout.py` & `QPUIQ-0.1.8/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/PySide6/textfield.py` & `QPUIQ-0.1.8/PUI/PySide6/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/PySide6/window.py` & `QPUIQ-0.1.8/PUI/PySide6/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/Qt5/base.py` & `QPUIQ-0.1.8/PUI/Qt5/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,12 +27,12 @@
                 params["stretch"] = child.layout_weight
             self.ui.addWidget(child.ui, **params)
         else:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
-            self.box.removeItem(child.ui)
+            self.ui.removeItem(child.ui)
         elif isinstance(child, QtBaseWidget):
             child.ui.setParent(None)
         else:
             self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.1.7/PUI/Qt5/button.py` & `QPUIQ-0.1.8/PUI/Qt5/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/Qt5/layout.py` & `QPUIQ-0.1.8/PUI/Qt5/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/Qt5/textfield.py` & `QPUIQ-0.1.8/PUI/Qt5/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/Qt5/window.py` & `QPUIQ-0.1.8/PUI/Qt5/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/dom.py` & `QPUIQ-0.1.8/PUI/dom.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/flet/application.py` & `QPUIQ-0.1.8/PUI/flet/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/flet/button.py` & `QPUIQ-0.1.8/PUI/flet/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/flet/layout.py` & `QPUIQ-0.1.8/PUI/flet/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/flet/textfield.py` & `QPUIQ-0.1.8/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/node.py` & `QPUIQ-0.1.8/PUI/node.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/state.py` & `QPUIQ-0.1.8/PUI/state.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/timeline.py` & `QPUIQ-0.1.8/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/tkinter/application.py` & `QPUIQ-0.1.8/PUI/tkinter/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/tkinter/base.py` & `QPUIQ-0.1.8/PUI/tkinter/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/tkinter/button.py` & `QPUIQ-0.1.8/PUI/tkinter/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/tkinter/canvas.py` & `QPUIQ-0.1.8/PUI/tkinter/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/tkinter/layout.py` & `QPUIQ-0.1.8/PUI/tkinter/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/tkinter/textfield.py` & `QPUIQ-0.1.8/PUI/tkinter/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/tkinter/window.py` & `QPUIQ-0.1.8/PUI/tkinter/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/urwid/application.py` & `QPUIQ-0.1.8/PUI/urwid/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/urwid/button.py` & `QPUIQ-0.1.8/PUI/urwid/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/urwid/layout.py` & `QPUIQ-0.1.8/PUI/urwid/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/PUI/view.py` & `QPUIQ-0.1.8/PUI/view.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.1.8/QPUIQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.7
+Version: 0.1.8
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `QPUIQ-0.1.7/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.1.8/QPUIQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/README.md` & `QPUIQ-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.7/setup.py` & `QPUIQ-0.1.8/setup.py`

 * *Files identical despite different names*

