# Comparing `tmp/PyGPSClient-1.3.8.tar.gz` & `tmp/PyGPSClient-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGPSClient-1.3.8.tar", last modified: Wed Aug 24 17:40:25 2022, max compression
+gzip compressed data, was "PyGPSClient-1.3.9.tar", last modified: Fri Sep  2 09:18:28 2022, max compression
```

## Comparing `PyGPSClient-1.3.8.tar` & `PyGPSClient-1.3.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-08-24 17:40:25.934860 PyGPSClient-1.3.8/
--rw-r--r--   0 stevensmith   (501) staff       (20)     1613 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/LICENSE
--rw-r--r--   0 stevensmith   (501) staff       (20)       98 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/MANIFEST.in
--rw-r--r--   0 stevensmith   (501) staff       (20)    30794 2022-08-24 17:40:25.934466 PyGPSClient-1.3.8/PKG-INFO
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-08-24 17:40:25.902097 PyGPSClient-1.3.8/PyGPSClient.egg-info/
--rw-r--r--   0 stevensmith   (501) staff       (20)    30794 2022-08-24 17:40:25.000000 PyGPSClient-1.3.8/PyGPSClient.egg-info/PKG-INFO
--rw-r--r--   0 stevensmith   (501) staff       (20)     2314 2022-08-24 17:40:25.000000 PyGPSClient-1.3.8/PyGPSClient.egg-info/SOURCES.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)        1 2022-08-24 17:40:25.000000 PyGPSClient-1.3.8/PyGPSClient.egg-info/dependency_links.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       58 2022-08-24 17:40:25.000000 PyGPSClient-1.3.8/PyGPSClient.egg-info/entry_points.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       64 2022-08-24 17:40:25.000000 PyGPSClient-1.3.8/PyGPSClient.egg-info/requires.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)       12 2022-08-24 17:40:25.000000 PyGPSClient-1.3.8/PyGPSClient.egg-info/top_level.txt
--rw-r--r--   0 stevensmith   (501) staff       (20)    29619 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/README.md
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-08-24 17:40:25.922586 PyGPSClient-1.3.8/pygpsclient/
--rw-r--r--   0 stevensmith   (501) staff       (20)      222 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/__init__.py
--rw-r--r--   0 stevensmith   (501) staff       (20)      392 2022-05-23 10:23:09.000000 PyGPSClient-1.3.8/pygpsclient/__main__.py
--rw-r--r--   0 stevensmith   (501) staff       (20)      166 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/pygpsclient/_version.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     5285 2022-07-21 09:22:06.000000 PyGPSClient-1.3.8/pygpsclient/about_dialog.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    22350 2022-07-21 09:22:06.000000 PyGPSClient-1.3.8/pygpsclient/app.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    19942 2022-07-21 09:22:06.000000 PyGPSClient-1.3.8/pygpsclient/banner_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     6060 2022-07-05 16:13:18.000000 PyGPSClient-1.3.8/pygpsclient/console_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9581 2022-08-06 16:57:08.000000 PyGPSClient-1.3.8/pygpsclient/file_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     7940 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/pygpsclient/globals.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     1431 2022-04-22 07:36:03.000000 PyGPSClient-1.3.8/pygpsclient/gnss_status.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     5727 2022-04-29 08:34:24.000000 PyGPSClient-1.3.8/pygpsclient/graphview_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    12956 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/pygpsclient/helpers.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     7732 2022-04-29 08:34:29.000000 PyGPSClient-1.3.8/pygpsclient/map_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     3434 2022-04-29 08:34:32.000000 PyGPSClient-1.3.8/pygpsclient/menu_bar.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    10960 2022-07-21 09:22:06.000000 PyGPSClient-1.3.8/pygpsclient/nmea_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    24832 2022-07-21 09:22:06.000000 PyGPSClient-1.3.8/pygpsclient/ntrip_client_dialog.py
-drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-08-24 17:40:25.933409 PyGPSClient-1.3.8/pygpsclient/resources/
--rw-r--r--   0 stevensmith   (501) staff       (20)     6148 2022-07-06 11:18:44.000000 PyGPSClient-1.3.8/pygpsclient/resources/.DS_Store
--rw-r--r--   0 stevensmith   (501) staff       (20)     9309 2022-07-21 09:22:06.000000 PyGPSClient-1.3.8/pygpsclient/resources/binary-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      575 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/pygpsclient/resources/clear-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     9507 2022-05-02 22:38:07.000000 PyGPSClient-1.3.8/pygpsclient/resources/ethernet-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      946 2022-04-11 07:18:02.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-antenna-6-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      269 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-arrow-12-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      209 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-arrow-80-16.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      844 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-check-mark-8-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      395 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-door-6-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     1037 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-gear-2-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      439 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-location-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     1724 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-location-27-32.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      328 2022-05-02 22:38:07.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-media-control-48-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      125 2022-05-02 22:38:07.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-media-control-50-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)    10472 2022-05-23 10:23:09.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-noclient-10-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     3856 2022-05-23 10:23:09.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-notransmit-10-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      442 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-refresh-6-16.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      875 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-time-6-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      860 2022-05-23 10:23:09.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-transmit-10-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      276 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-triangle-1-16.png
--rw-r--r--   0 stevensmith   (501) staff       (20)      466 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-warning-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     4286 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/pygpsclient.ico
--rw-r--r--   0 stevensmith   (501) staff       (20)     5424 2022-05-02 22:38:07.000000 PyGPSClient-1.3.8/pygpsclient/resources/usbport-1-24.png
--rw-r--r--   0 stevensmith   (501) staff       (20)   327167 2021-05-26 09:31:55.000000 PyGPSClient-1.3.8/pygpsclient/resources/world.png
--rw-r--r--   0 stevensmith   (501) staff       (20)     1315 2022-04-29 08:34:46.000000 PyGPSClient-1.3.8/pygpsclient/rtcm3_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    14416 2022-05-02 22:38:07.000000 PyGPSClient-1.3.8/pygpsclient/serialconfig_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    30284 2022-08-08 08:16:28.000000 PyGPSClient-1.3.8/pygpsclient/settings_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     5341 2022-05-29 08:04:41.000000 PyGPSClient-1.3.8/pygpsclient/skyview_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     4965 2022-05-08 17:41:44.000000 PyGPSClient-1.3.8/pygpsclient/socketconfig_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     3258 2022-05-08 17:41:44.000000 PyGPSClient-1.3.8/pygpsclient/status_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9561 2022-07-21 09:22:06.000000 PyGPSClient-1.3.8/pygpsclient/stream_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     4944 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/pygpsclient/strings.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    16086 2022-08-19 09:45:36.000000 PyGPSClient-1.3.8/pygpsclient/ubx_cfgval_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    11555 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/pygpsclient/ubx_config_dialog.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    17522 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/pygpsclient/ubx_dynamic_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    16832 2022-08-24 17:39:34.000000 PyGPSClient-1.3.8/pygpsclient/ubx_handler.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     6298 2022-07-06 10:42:40.000000 PyGPSClient-1.3.8/pygpsclient/ubx_info_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9794 2022-08-17 08:33:30.000000 PyGPSClient-1.3.8/pygpsclient/ubx_msgrate_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     9559 2022-05-08 17:41:44.000000 PyGPSClient-1.3.8/pygpsclient/ubx_port_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)    18215 2022-05-08 17:41:44.000000 PyGPSClient-1.3.8/pygpsclient/ubx_preset_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)     7362 2022-05-08 17:41:44.000000 PyGPSClient-1.3.8/pygpsclient/ubx_solrate_frame.py
--rw-r--r--   0 stevensmith   (501) staff       (20)       38 2022-08-24 17:40:25.934975 PyGPSClient-1.3.8/setup.cfg
--rw-r--r--   0 stevensmith   (501) staff       (20)     2634 2022-08-22 10:20:23.000000 PyGPSClient-1.3.8/setup.py
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-09-02 09:18:28.797773 PyGPSClient-1.3.9/
+-rw-r--r--   0 stevensmith   (501) staff       (20)     1613 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/LICENSE
+-rw-r--r--   0 stevensmith   (501) staff       (20)       98 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/MANIFEST.in
+-rw-r--r--   0 stevensmith   (501) staff       (20)    30893 2022-09-02 09:18:28.797420 PyGPSClient-1.3.9/PKG-INFO
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-09-02 09:18:28.694334 PyGPSClient-1.3.9/PyGPSClient.egg-info/
+-rw-r--r--   0 stevensmith   (501) staff       (20)    30893 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/PKG-INFO
+-rw-r--r--   0 stevensmith   (501) staff       (20)     2314 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/SOURCES.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)        1 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/dependency_links.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)       58 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/entry_points.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)       64 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/requires.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)       12 2022-09-02 09:18:28.000000 PyGPSClient-1.3.9/PyGPSClient.egg-info/top_level.txt
+-rw-r--r--   0 stevensmith   (501) staff       (20)    29718 2022-08-29 10:34:28.000000 PyGPSClient-1.3.9/README.md
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-09-02 09:18:28.724242 PyGPSClient-1.3.9/pygpsclient/
+-rw-r--r--   0 stevensmith   (501) staff       (20)      222 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/__init__.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)      392 2022-05-23 10:23:09.000000 PyGPSClient-1.3.9/pygpsclient/__main__.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)      166 2022-09-02 09:13:55.000000 PyGPSClient-1.3.9/pygpsclient/_version.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     5285 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/about_dialog.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    22362 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/app.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    19942 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/banner_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     6060 2022-07-05 16:13:18.000000 PyGPSClient-1.3.9/pygpsclient/console_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     9581 2022-08-06 16:57:08.000000 PyGPSClient-1.3.9/pygpsclient/file_handler.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     7940 2022-08-24 17:39:34.000000 PyGPSClient-1.3.9/pygpsclient/globals.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     1431 2022-04-22 07:36:03.000000 PyGPSClient-1.3.9/pygpsclient/gnss_status.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     5727 2022-04-29 08:34:24.000000 PyGPSClient-1.3.9/pygpsclient/graphview_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    12956 2022-08-24 17:39:34.000000 PyGPSClient-1.3.9/pygpsclient/helpers.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     7732 2022-04-29 08:34:29.000000 PyGPSClient-1.3.9/pygpsclient/map_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     3434 2022-04-29 08:34:32.000000 PyGPSClient-1.3.9/pygpsclient/menu_bar.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    10960 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/nmea_handler.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    24328 2022-09-02 09:13:55.000000 PyGPSClient-1.3.9/pygpsclient/ntrip_client_dialog.py
+drwxr-xr-x   0 stevensmith   (501) staff       (20)        0 2022-09-02 09:18:28.796265 PyGPSClient-1.3.9/pygpsclient/resources/
+-rw-r--r--   0 stevensmith   (501) staff       (20)     6148 2022-07-06 11:18:44.000000 PyGPSClient-1.3.9/pygpsclient/resources/.DS_Store
+-rw-r--r--   0 stevensmith   (501) staff       (20)     9309 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/resources/binary-1-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      575 2022-08-24 17:39:34.000000 PyGPSClient-1.3.9/pygpsclient/resources/clear-1-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)     9507 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/resources/ethernet-1-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      946 2022-04-11 07:18:02.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-antenna-6-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      269 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-arrow-12-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      209 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-arrow-80-16.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      844 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-check-mark-8-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      395 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-door-6-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)     1037 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-gear-2-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      439 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-location-1-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)     1724 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-location-27-32.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      328 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-media-control-48-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      125 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-media-control-50-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)    10472 2022-05-23 10:23:09.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-noclient-10-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)     3856 2022-05-23 10:23:09.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-notransmit-10-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      442 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-refresh-6-16.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      875 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-time-6-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      860 2022-05-23 10:23:09.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-transmit-10-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      276 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-triangle-1-16.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)      466 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-warning-1-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)     4286 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/pygpsclient.ico
+-rw-r--r--   0 stevensmith   (501) staff       (20)     5424 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/resources/usbport-1-24.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)   327167 2021-05-26 09:31:55.000000 PyGPSClient-1.3.9/pygpsclient/resources/world.png
+-rw-r--r--   0 stevensmith   (501) staff       (20)     1315 2022-04-29 08:34:46.000000 PyGPSClient-1.3.9/pygpsclient/rtcm3_handler.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    14416 2022-05-02 22:38:07.000000 PyGPSClient-1.3.9/pygpsclient/serialconfig_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    30284 2022-08-08 08:16:28.000000 PyGPSClient-1.3.9/pygpsclient/settings_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     5341 2022-05-29 08:04:41.000000 PyGPSClient-1.3.9/pygpsclient/skyview_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     4965 2022-05-08 17:41:44.000000 PyGPSClient-1.3.9/pygpsclient/socketconfig_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     3258 2022-05-08 17:41:44.000000 PyGPSClient-1.3.9/pygpsclient/status_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     9561 2022-07-21 09:22:06.000000 PyGPSClient-1.3.9/pygpsclient/stream_handler.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     5004 2022-09-02 09:13:55.000000 PyGPSClient-1.3.9/pygpsclient/strings.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    16002 2022-08-29 06:50:48.000000 PyGPSClient-1.3.9/pygpsclient/ubx_cfgval_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    10211 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_config_dialog.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    17058 2022-08-27 14:49:03.000000 PyGPSClient-1.3.9/pygpsclient/ubx_dynamic_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     9315 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_handler.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     7700 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_info_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     9722 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_msgrate_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     9353 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_port_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)    18202 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_preset_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)     7262 2022-08-27 14:45:07.000000 PyGPSClient-1.3.9/pygpsclient/ubx_solrate_frame.py
+-rw-r--r--   0 stevensmith   (501) staff       (20)       38 2022-09-02 09:18:28.797893 PyGPSClient-1.3.9/setup.cfg
+-rw-r--r--   0 stevensmith   (501) staff       (20)     2634 2022-09-02 09:13:55.000000 PyGPSClient-1.3.9/setup.py
```

### Comparing `PyGPSClient-1.3.8/LICENSE` & `PyGPSClient-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/PKG-INFO` & `PyGPSClient-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGPSClient
-Version: 1.3.8
+Version: 1.3.9
 Summary: PyGPSClient GNSS/GPS Graphical Client
 Home-page: https://github.com/semuconsulting/PyGPSClient
 Author: semuadmin
 Author-email: semuadmin@semuconsulting.com
 License: BSD 3-Clause 'Modified' License
 Project-URL: Bug Tracker, https://github.com/semuconsulting/PyGPSClient
 Project-URL: Documentation, https://github.com/semuconsulting/PyGPSClient
@@ -101,15 +101,15 @@
 ## <a name="howtouse">How to Use</a>
 
 * To connect to a listed serial device, select the device from the listbox, set the appropriate serial connection parameters and click 
 ![connect icon](/pygpsclient/resources/usbport-1-24.png). The application will endeavour to pre-select a recognised GNSS/GPS device but this is platform and device dependent. Press the ![refresh](/pygpsclient/resources/iconmonstr-refresh-6-16.png) button to refresh the list of connected devices at any point. *Rate bps is typically the only setting that might need adjusting, but tweaking the timeout setting may improve performance on certain platforms*.
 * To connect to a TCP or UDP socket, enter the server URL and port, select the protocol (defaults to TCP) and click 
 ![connect socket icon](/pygpsclient/resources/ethernet-1-24.png).
 * To stream from a previously-saved binary datalog file, click 
-![connect-file icon](/pygpsclient/resources/binary-1-24.png) and select the file. PyGPSClient datalog files will be named e.g. `pygpsdata-20220427114802.log`, but any binary dump of an GNSS receiver output is acceptable.
+![connect-file icon](/pygpsclient/resources/binary-1-24.png) and select the file type (`*.log, *.ubx, *.*`) and path. PyGPSClient datalog files will be named e.g. `pygpsdata-20220427114802.log`, but any binary dump of an GNSS receiver output is acceptable, including `*.ubx` files produced by u-center.
 * To disconnect from the data stream, click
 ![disconnect icon](/pygpsclient/resources/iconmonstr-media-control-50-24.png).
 * To display the UBX Configuration Dialog (*only functional when connected to a UBX GNSS device via serial port*), click
 ![gear icon](/pygpsclient/resources/iconmonstr-gear-2-24.png), or go to Menu..Options.
 * To display the NTRIP Client Configuration Dialog (*requires internet connection*), click
 ![gear icon](/pygpsclient/resources/iconmonstr-antenna-6-24.png), or go to Menu..Options.
 * To expand or collapse the banner or serial port configuration widgets, click the ![expand icon](/pygpsclient/resources/iconmonstr-arrow-80-16.png)/![expand icon](/pygpsclient/resources/iconmonstr-triangle-1-16.png) buttons.
@@ -132,15 +132,15 @@
 
 ![ubxconfig widget screenshot](/images/ubxconfig_widget.png)
 
 The UBX Configuration Dialog currently supports the following UBX configuration panels:
 1. Version panel shows current device hardware/firmware versions (*via MON-VER and MON-HW polls*).
 1. Protocol Configuration panel (CFG-PRT) sets baud rate and inbound/outbound protocols across all available ports.
 1. Solution Rate panel (CFG-RATE) sets navigation solution interval in ms (e.g. 1000 = 1/second) and measurement ratio (ratio between the number of measurements and the number of navigation solutions, e.g. 5 = five measurements per navigation solution).
-1. For each of the panels above, clicking anywhere in the widget background will refresh the displayed information with the current configuration.
+1. For each of the panels above, clicking anywhere in the panel background will refresh the displayed information with the current configuration.
 1. Message Rate panel (CFG-MSG) sets message rates per port for UBX and NMEA messages. Message rate is relative to navigation solution frequency e.g. a message rate of '4' means 'every 4th navigation solution'.
 1. Other configuration panel (CFG-*) providing structured updates for a range of legacy CFG- configuration commands for pre-Generation 9+ devices. Note: 'X' (byte) type attributes can be entered as integers or hexadecimal strings e.g. 522125312 or 0x1f1f0000.
 1. Configuration Interface widget (CFG-VALSET, CFG-VALDEL and CFG-VALGET) queries and sets configuration for [Generation 9+ devices](https://github.com/semuconsulting/pyubx2#configinterface) e.g. NEO-M9, ZED-F9P, etc.
 1. Preset Commands widget supports a variety of preset and user-defined commands - see [user defined presets](#userdefined)
 
 An icon to the right of each 'SEND' 
 ![send icon](/pygpsclient/resources/iconmonstr-arrow-12-24.png) button indicates the confirmation status of the configuration command; 
@@ -158,15 +158,15 @@
 
 ![ntrip config widget screenshot](/images/ntripconfig_widget.png)
 
 To use:
 1. Enter the required NTRIP server URL (or IP address) and port (defaults to 2101). For services which require authorisation, enter your login username and password.
 1. To retrieve the sourcetable, leave the mountpoint field blank and click connect (*response may take a few seconds*). The required mountpoint may then be selected from the list, or entered manually. Where possible, `PyGPSClient` will automatically identify the closest mountpoint to the current location.
 1. For NTRIP services which require client position data via NMEA GGA sentences, select the appropriate sentence transmission interval in seconds. The default is 'None' (no GGA sentences sent). A value of 10 or 60 seconds is typical.
-1. If GGA sentence transmission is enabled, GGA sentences can either be populated from live navigation data (*assuming a receiver is connected and outputting valid position data*) or from manual settings entered in the NTRIP configuration panel (latitude, longitude, elevation and separation - all four manual settings must be provided).
+1. If GGA sentence transmission is enabled, GGA sentences can either be populated from live navigation data (*assuming a receiver is connected and outputting valid position data*) or from fixed reference settings entered in the NTRIP configuration panel (latitude, longitude, elevation and geoid separation - all four reference settings must be provided).
 1. To connect to the NTRIP server, click ![connect icon](/pygpsclient/resources/iconmonstr-media-control-48-24.png). To disconnect, click ![disconnect icon](/pygpsclient/resources/iconmonstr-media-control-50-24.png).
 1. If NTRIP data is being successfully received, the banner '**dgps:**' status indicator should change to 'YES' and indicate the age and reference station of the correction data (where available) ![dgps status](/images/dgps_status.png). Note that DGPS status is typically maintained for up to 60 seconds after loss of correction signal.
 1. Some NTRIP services may output RTCM3 correction messages at a high rate, flooding the GUI console display. To suppress these messages in the console, de-select the 'RTCM' option in 'Protocols Shown' - the RTCM3 messages will continue to be processed in the background.
 
 Below is a illustrative NTRIP DGPS data log, showing:
 * Outgoing NMEA GPGGA (client position) sentence.
 * Incoming RTCM3 correction messages; in this case - 1006 (Ref station ARP (*DF003=2690*) with antenna height), 1008 (Antenna descriptor), 1033 (Receiver descriptor), 1075 (GPS MSM5), 1085 (GLONASS MSM5), 1095 (Galileo MSM5), 1125 (BeiDou MSM5) and 1230 (GLONASS Code-Phase Biases)
```

### Comparing `PyGPSClient-1.3.8/PyGPSClient.egg-info/PKG-INFO` & `PyGPSClient-1.3.9/PyGPSClient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGPSClient
-Version: 1.3.8
+Version: 1.3.9
 Summary: PyGPSClient GNSS/GPS Graphical Client
 Home-page: https://github.com/semuconsulting/PyGPSClient
 Author: semuadmin
 Author-email: semuadmin@semuconsulting.com
 License: BSD 3-Clause 'Modified' License
 Project-URL: Bug Tracker, https://github.com/semuconsulting/PyGPSClient
 Project-URL: Documentation, https://github.com/semuconsulting/PyGPSClient
@@ -101,15 +101,15 @@
 ## <a name="howtouse">How to Use</a>
 
 * To connect to a listed serial device, select the device from the listbox, set the appropriate serial connection parameters and click 
 ![connect icon](/pygpsclient/resources/usbport-1-24.png). The application will endeavour to pre-select a recognised GNSS/GPS device but this is platform and device dependent. Press the ![refresh](/pygpsclient/resources/iconmonstr-refresh-6-16.png) button to refresh the list of connected devices at any point. *Rate bps is typically the only setting that might need adjusting, but tweaking the timeout setting may improve performance on certain platforms*.
 * To connect to a TCP or UDP socket, enter the server URL and port, select the protocol (defaults to TCP) and click 
 ![connect socket icon](/pygpsclient/resources/ethernet-1-24.png).
 * To stream from a previously-saved binary datalog file, click 
-![connect-file icon](/pygpsclient/resources/binary-1-24.png) and select the file. PyGPSClient datalog files will be named e.g. `pygpsdata-20220427114802.log`, but any binary dump of an GNSS receiver output is acceptable.
+![connect-file icon](/pygpsclient/resources/binary-1-24.png) and select the file type (`*.log, *.ubx, *.*`) and path. PyGPSClient datalog files will be named e.g. `pygpsdata-20220427114802.log`, but any binary dump of an GNSS receiver output is acceptable, including `*.ubx` files produced by u-center.
 * To disconnect from the data stream, click
 ![disconnect icon](/pygpsclient/resources/iconmonstr-media-control-50-24.png).
 * To display the UBX Configuration Dialog (*only functional when connected to a UBX GNSS device via serial port*), click
 ![gear icon](/pygpsclient/resources/iconmonstr-gear-2-24.png), or go to Menu..Options.
 * To display the NTRIP Client Configuration Dialog (*requires internet connection*), click
 ![gear icon](/pygpsclient/resources/iconmonstr-antenna-6-24.png), or go to Menu..Options.
 * To expand or collapse the banner or serial port configuration widgets, click the ![expand icon](/pygpsclient/resources/iconmonstr-arrow-80-16.png)/![expand icon](/pygpsclient/resources/iconmonstr-triangle-1-16.png) buttons.
@@ -132,15 +132,15 @@
 
 ![ubxconfig widget screenshot](/images/ubxconfig_widget.png)
 
 The UBX Configuration Dialog currently supports the following UBX configuration panels:
 1. Version panel shows current device hardware/firmware versions (*via MON-VER and MON-HW polls*).
 1. Protocol Configuration panel (CFG-PRT) sets baud rate and inbound/outbound protocols across all available ports.
 1. Solution Rate panel (CFG-RATE) sets navigation solution interval in ms (e.g. 1000 = 1/second) and measurement ratio (ratio between the number of measurements and the number of navigation solutions, e.g. 5 = five measurements per navigation solution).
-1. For each of the panels above, clicking anywhere in the widget background will refresh the displayed information with the current configuration.
+1. For each of the panels above, clicking anywhere in the panel background will refresh the displayed information with the current configuration.
 1. Message Rate panel (CFG-MSG) sets message rates per port for UBX and NMEA messages. Message rate is relative to navigation solution frequency e.g. a message rate of '4' means 'every 4th navigation solution'.
 1. Other configuration panel (CFG-*) providing structured updates for a range of legacy CFG- configuration commands for pre-Generation 9+ devices. Note: 'X' (byte) type attributes can be entered as integers or hexadecimal strings e.g. 522125312 or 0x1f1f0000.
 1. Configuration Interface widget (CFG-VALSET, CFG-VALDEL and CFG-VALGET) queries and sets configuration for [Generation 9+ devices](https://github.com/semuconsulting/pyubx2#configinterface) e.g. NEO-M9, ZED-F9P, etc.
 1. Preset Commands widget supports a variety of preset and user-defined commands - see [user defined presets](#userdefined)
 
 An icon to the right of each 'SEND' 
 ![send icon](/pygpsclient/resources/iconmonstr-arrow-12-24.png) button indicates the confirmation status of the configuration command; 
@@ -158,15 +158,15 @@
 
 ![ntrip config widget screenshot](/images/ntripconfig_widget.png)
 
 To use:
 1. Enter the required NTRIP server URL (or IP address) and port (defaults to 2101). For services which require authorisation, enter your login username and password.
 1. To retrieve the sourcetable, leave the mountpoint field blank and click connect (*response may take a few seconds*). The required mountpoint may then be selected from the list, or entered manually. Where possible, `PyGPSClient` will automatically identify the closest mountpoint to the current location.
 1. For NTRIP services which require client position data via NMEA GGA sentences, select the appropriate sentence transmission interval in seconds. The default is 'None' (no GGA sentences sent). A value of 10 or 60 seconds is typical.
-1. If GGA sentence transmission is enabled, GGA sentences can either be populated from live navigation data (*assuming a receiver is connected and outputting valid position data*) or from manual settings entered in the NTRIP configuration panel (latitude, longitude, elevation and separation - all four manual settings must be provided).
+1. If GGA sentence transmission is enabled, GGA sentences can either be populated from live navigation data (*assuming a receiver is connected and outputting valid position data*) or from fixed reference settings entered in the NTRIP configuration panel (latitude, longitude, elevation and geoid separation - all four reference settings must be provided).
 1. To connect to the NTRIP server, click ![connect icon](/pygpsclient/resources/iconmonstr-media-control-48-24.png). To disconnect, click ![disconnect icon](/pygpsclient/resources/iconmonstr-media-control-50-24.png).
 1. If NTRIP data is being successfully received, the banner '**dgps:**' status indicator should change to 'YES' and indicate the age and reference station of the correction data (where available) ![dgps status](/images/dgps_status.png). Note that DGPS status is typically maintained for up to 60 seconds after loss of correction signal.
 1. Some NTRIP services may output RTCM3 correction messages at a high rate, flooding the GUI console display. To suppress these messages in the console, de-select the 'RTCM' option in 'Protocols Shown' - the RTCM3 messages will continue to be processed in the background.
 
 Below is a illustrative NTRIP DGPS data log, showing:
 * Outgoing NMEA GPGGA (client position) sentence.
 * Incoming RTCM3 correction messages; in this case - 1006 (Ref station ARP (*DF003=2690*) with antenna height), 1008 (Antenna descriptor), 1033 (Receiver descriptor), 1075 (GPS MSM5), 1085 (GLONASS MSM5), 1095 (Galileo MSM5), 1125 (BeiDou MSM5) and 1230 (GLONASS Code-Phase Biases)
```

### Comparing `PyGPSClient-1.3.8/PyGPSClient.egg-info/SOURCES.txt` & `PyGPSClient-1.3.9/PyGPSClient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/README.md` & `PyGPSClient-1.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 ## <a name="howtouse">How to Use</a>
 
 * To connect to a listed serial device, select the device from the listbox, set the appropriate serial connection parameters and click 
 ![connect icon](/pygpsclient/resources/usbport-1-24.png). The application will endeavour to pre-select a recognised GNSS/GPS device but this is platform and device dependent. Press the ![refresh](/pygpsclient/resources/iconmonstr-refresh-6-16.png) button to refresh the list of connected devices at any point. *Rate bps is typically the only setting that might need adjusting, but tweaking the timeout setting may improve performance on certain platforms*.
 * To connect to a TCP or UDP socket, enter the server URL and port, select the protocol (defaults to TCP) and click 
 ![connect socket icon](/pygpsclient/resources/ethernet-1-24.png).
 * To stream from a previously-saved binary datalog file, click 
-![connect-file icon](/pygpsclient/resources/binary-1-24.png) and select the file. PyGPSClient datalog files will be named e.g. `pygpsdata-20220427114802.log`, but any binary dump of an GNSS receiver output is acceptable.
+![connect-file icon](/pygpsclient/resources/binary-1-24.png) and select the file type (`*.log, *.ubx, *.*`) and path. PyGPSClient datalog files will be named e.g. `pygpsdata-20220427114802.log`, but any binary dump of an GNSS receiver output is acceptable, including `*.ubx` files produced by u-center.
 * To disconnect from the data stream, click
 ![disconnect icon](/pygpsclient/resources/iconmonstr-media-control-50-24.png).
 * To display the UBX Configuration Dialog (*only functional when connected to a UBX GNSS device via serial port*), click
 ![gear icon](/pygpsclient/resources/iconmonstr-gear-2-24.png), or go to Menu..Options.
 * To display the NTRIP Client Configuration Dialog (*requires internet connection*), click
 ![gear icon](/pygpsclient/resources/iconmonstr-antenna-6-24.png), or go to Menu..Options.
 * To expand or collapse the banner or serial port configuration widgets, click the ![expand icon](/pygpsclient/resources/iconmonstr-arrow-80-16.png)/![expand icon](/pygpsclient/resources/iconmonstr-triangle-1-16.png) buttons.
@@ -95,15 +95,15 @@
 
 ![ubxconfig widget screenshot](/images/ubxconfig_widget.png)
 
 The UBX Configuration Dialog currently supports the following UBX configuration panels:
 1. Version panel shows current device hardware/firmware versions (*via MON-VER and MON-HW polls*).
 1. Protocol Configuration panel (CFG-PRT) sets baud rate and inbound/outbound protocols across all available ports.
 1. Solution Rate panel (CFG-RATE) sets navigation solution interval in ms (e.g. 1000 = 1/second) and measurement ratio (ratio between the number of measurements and the number of navigation solutions, e.g. 5 = five measurements per navigation solution).
-1. For each of the panels above, clicking anywhere in the widget background will refresh the displayed information with the current configuration.
+1. For each of the panels above, clicking anywhere in the panel background will refresh the displayed information with the current configuration.
 1. Message Rate panel (CFG-MSG) sets message rates per port for UBX and NMEA messages. Message rate is relative to navigation solution frequency e.g. a message rate of '4' means 'every 4th navigation solution'.
 1. Other configuration panel (CFG-*) providing structured updates for a range of legacy CFG- configuration commands for pre-Generation 9+ devices. Note: 'X' (byte) type attributes can be entered as integers or hexadecimal strings e.g. 522125312 or 0x1f1f0000.
 1. Configuration Interface widget (CFG-VALSET, CFG-VALDEL and CFG-VALGET) queries and sets configuration for [Generation 9+ devices](https://github.com/semuconsulting/pyubx2#configinterface) e.g. NEO-M9, ZED-F9P, etc.
 1. Preset Commands widget supports a variety of preset and user-defined commands - see [user defined presets](#userdefined)
 
 An icon to the right of each 'SEND' 
 ![send icon](/pygpsclient/resources/iconmonstr-arrow-12-24.png) button indicates the confirmation status of the configuration command; 
@@ -121,15 +121,15 @@
 
 ![ntrip config widget screenshot](/images/ntripconfig_widget.png)
 
 To use:
 1. Enter the required NTRIP server URL (or IP address) and port (defaults to 2101). For services which require authorisation, enter your login username and password.
 1. To retrieve the sourcetable, leave the mountpoint field blank and click connect (*response may take a few seconds*). The required mountpoint may then be selected from the list, or entered manually. Where possible, `PyGPSClient` will automatically identify the closest mountpoint to the current location.
 1. For NTRIP services which require client position data via NMEA GGA sentences, select the appropriate sentence transmission interval in seconds. The default is 'None' (no GGA sentences sent). A value of 10 or 60 seconds is typical.
-1. If GGA sentence transmission is enabled, GGA sentences can either be populated from live navigation data (*assuming a receiver is connected and outputting valid position data*) or from manual settings entered in the NTRIP configuration panel (latitude, longitude, elevation and separation - all four manual settings must be provided).
+1. If GGA sentence transmission is enabled, GGA sentences can either be populated from live navigation data (*assuming a receiver is connected and outputting valid position data*) or from fixed reference settings entered in the NTRIP configuration panel (latitude, longitude, elevation and geoid separation - all four reference settings must be provided).
 1. To connect to the NTRIP server, click ![connect icon](/pygpsclient/resources/iconmonstr-media-control-48-24.png). To disconnect, click ![disconnect icon](/pygpsclient/resources/iconmonstr-media-control-50-24.png).
 1. If NTRIP data is being successfully received, the banner '**dgps:**' status indicator should change to 'YES' and indicate the age and reference station of the correction data (where available) ![dgps status](/images/dgps_status.png). Note that DGPS status is typically maintained for up to 60 seconds after loss of correction signal.
 1. Some NTRIP services may output RTCM3 correction messages at a high rate, flooding the GUI console display. To suppress these messages in the console, de-select the 'RTCM' option in 'Protocols Shown' - the RTCM3 messages will continue to be processed in the background.
 
 Below is a illustrative NTRIP DGPS data log, showing:
 * Outgoing NMEA GPGGA (client position) sentence.
 * Incoming RTCM3 correction messages; in this case - 1006 (Ref station ARP (*DF003=2690*) with antenna height), 1008 (Antenna descriptor), 1033 (Receiver descriptor), 1075 (GPS MSM5), 1085 (GLONASS MSM5), 1095 (Galileo MSM5), 1125 (BeiDou MSM5) and 1230 (GLONASS Code-Phase Biases)
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/about_dialog.py` & `PyGPSClient-1.3.9/pygpsclient/about_dialog.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/app.py` & `PyGPSClient-1.3.9/pygpsclient/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Created on 12 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 
-import logging
+# import logging
 from threading import Thread
 from queue import Queue, Empty
 from datetime import datetime, timedelta
 from tkinter import Frame, N, S, E, W, PhotoImage, font
 from serial import SerialException, SerialTimeoutException
 from pyubx2 import (
     protocol,
@@ -65,15 +65,15 @@
 from pygpsclient.status_frame import StatusFrame
 from pygpsclient.ubx_config_dialog import UBXConfigDialog
 from pygpsclient.ntrip_client_dialog import NTRIPConfigDialog
 from pygpsclient.nmea_handler import NMEAHandler
 from pygpsclient.ubx_handler import UBXHandler
 
 
-LOGGING = logging.INFO
+# LOGGING = logging.INFO
 
 
 class App(Frame):  # pylint: disable=too-many-ancestors
     """
     Main PyGPSClient GUI Application Class
     """
 
@@ -82,18 +82,18 @@
         Set up main application and add frames
 
         :param tkinter.Tk master: reference to Tk root
         :param args: optional args to pass to Frame parent class
         :param kwargs: optional kwargs to pass to Frame parent class
         """
 
-        logging.basicConfig(
-            format="%(asctime)-15s [%(levelname)s] %(funcName)s: %(message)s",
-            level=LOGGING,
-        )
+        # logging.basicConfig(
+        #     format="%(asctime)-15s [%(levelname)s] %(funcName)s: %(message)s",
+        #     level=LOGGING,
+        # )
 
         self.__master = master
 
         Frame.__init__(self, self.__master, *args, **kwargs)
 
         self.__master.protocol("WM_DELETE_WINDOW", self.on_exit)
         self.__master.title(TITLE)
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/banner_frame.py` & `PyGPSClient-1.3.9/pygpsclient/banner_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/console_frame.py` & `PyGPSClient-1.3.9/pygpsclient/console_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/file_handler.py` & `PyGPSClient-1.3.9/pygpsclient/file_handler.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/globals.py` & `PyGPSClient-1.3.9/pygpsclient/globals.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/gnss_status.py` & `PyGPSClient-1.3.9/pygpsclient/gnss_status.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/graphview_frame.py` & `PyGPSClient-1.3.9/pygpsclient/graphview_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/helpers.py` & `PyGPSClient-1.3.9/pygpsclient/helpers.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/map_frame.py` & `PyGPSClient-1.3.9/pygpsclient/map_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/menu_bar.py` & `PyGPSClient-1.3.9/pygpsclient/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/nmea_handler.py` & `PyGPSClient-1.3.9/pygpsclient/nmea_handler.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/ntrip_client_dialog.py` & `PyGPSClient-1.3.9/pygpsclient/ntrip_client_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 NTRIP client container dialog
 
 This is the pop-up dialog containing the various
 NTRIP client configuration functions.
 
+NB: the NTRIP handler gnssntripclient is part of the separate
+pygnssutils  package.
+
 Created on 2 Apr 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
@@ -18,15 +21,17 @@
     Frame,
     Button,
     Label,
     Entry,
     Spinbox,
     Listbox,
     Scrollbar,
+    Radiobutton,
     StringVar,
+    IntVar,
     N,
     S,
     E,
     W,
     NORMAL,
     DISABLED,
     END,
@@ -47,30 +52,30 @@
     UBX_CFGRATE,
     UBX_CFGMSG,
     UBX_CFGVAL,
     UBX_PRESET,
     ENTCOL,
     READONLY,
     POPUP_TRANSIENT,
-    DISCONNECTED,
-    CONNECTED,
     UI,
     UIK,
     GGA_INTERVALS,
 )
 from pygpsclient.strings import (
     DLGNTRIPCONFIG,
     LBLNTRIPSERVER,
     LBLNTRIPPORT,
     LBLNTRIPVERSION,
     LBLNTRIPMOUNT,
     LBLNTRIPUSER,
     LBLNTRIPPWD,
     LBLNTRIPGGAINT,
     LBLNTRIPSTR,
+    LBLGGALIVE,
+    LBLGGAFIXED,
 )
 from pygpsclient.helpers import (
     valid_entry,
     VALINT,
     VALFLOAT,
     VALURL,
     MAXPORT,
@@ -122,27 +127,27 @@
         self._ntrip_server = StringVar()
         self._ntrip_port = StringVar()
         self._ntrip_mountpoint = StringVar()
         self._ntrip_mpdist = StringVar()
         self._ntrip_user = StringVar()
         self._ntrip_password = StringVar()
         self._ntrip_gga_interval = StringVar()
+        self._ntrip_gga_mode = IntVar()
         self._ntrip_gga_lat = StringVar()
         self._ntrip_gga_lon = StringVar()
         self._ntrip_gga_alt = StringVar()
         self._ntrip_gga_sep = StringVar()
         self._settings = {}
         self._connected = False
         self._sourcetable = None
 
         self._body()
         self._do_layout()
         self._attach_events()
         self._reset()
-        # self._centre()
 
     def _body(self):
         """
         Set up frame and widgets.
         """
         # pylint: disable=unnecessary-lambda
 
@@ -244,43 +249,51 @@
             values=(GGA_INTERVALS),
             width=5,
             readonlybackground=ENTCOL,
             wrap=True,
             textvariable=self._ntrip_gga_interval,
             state=READONLY,
         )
-
-        self._lbl_lat = Label(self._frm_container, text="GGA Latitude")
+        self._rad_ggalive = Radiobutton(
+            self._frm_container, text=LBLGGALIVE, variable=self._ntrip_gga_mode, value=0
+        )
+        self._rad_ggafixed = Radiobutton(
+            self._frm_container,
+            text=LBLGGAFIXED,
+            variable=self._ntrip_gga_mode,
+            value=1,
+        )
+        self._lbl_lat = Label(self._frm_container, text="Ref Latitude")
         self._ent_lat = Entry(
             self._frm_container,
             textvariable=self._ntrip_gga_lat,
             bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=15,
         )
-        self._lbl_lon = Label(self._frm_container, text="GGA Longitude")
+        self._lbl_lon = Label(self._frm_container, text="Ref Longitude")
         self._ent_lon = Entry(
             self._frm_container,
             textvariable=self._ntrip_gga_lon,
             bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=15,
         )
-        self._lbl_alt = Label(self._frm_container, text="GGA Elevation m")
+        self._lbl_alt = Label(self._frm_container, text="Ref Elevation m")
         self._ent_alt = Entry(
             self._frm_container,
             textvariable=self._ntrip_gga_alt,
             bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=15,
         )
-        self._lbl_sep = Label(self._frm_container, text="GGA Separation m")
+        self._lbl_sep = Label(self._frm_container, text="Ref Separation m")
         self._ent_sep = Entry(
             self._frm_container,
             textvariable=self._ntrip_gga_sep,
             bg=ENTCOL,
             state=NORMAL,
             relief="sunken",
             width=15,
@@ -347,30 +360,32 @@
         ttk.Separator(self._frm_container).grid(
             column=0, row=12, columnspan=3, padx=3, pady=3, sticky=(W, E)
         )
         self._lbl_ntripggaint.grid(column=0, row=13, padx=2, pady=3, sticky=W)
         self._spn_ntripggaint.grid(
             column=1, row=13, padx=3, pady=2, rowspan=2, sticky=W
         )
-        self._lbl_lat.grid(column=0, row=15, padx=3, pady=2, sticky=W)
-        self._ent_lat.grid(column=1, row=15, padx=3, pady=2, sticky=W)
-        self._lbl_lon.grid(column=0, row=16, padx=3, pady=2, sticky=W)
-        self._ent_lon.grid(column=1, row=16, padx=3, pady=2, sticky=W)
-        self._lbl_alt.grid(column=0, row=17, padx=3, pady=2, sticky=W)
-        self._ent_alt.grid(column=1, row=17, padx=3, pady=2, sticky=W)
-        self._lbl_sep.grid(column=0, row=18, padx=3, pady=2, sticky=W)
-        self._ent_sep.grid(column=1, row=18, padx=3, pady=2, sticky=W)
+        self._rad_ggalive.grid(column=0, row=15, padx=3, pady=2, sticky=W)
+        self._rad_ggafixed.grid(column=1, row=15, padx=3, pady=2, sticky=W)
+        self._lbl_lat.grid(column=0, row=16, padx=3, pady=2, sticky=W)
+        self._ent_lat.grid(column=1, row=16, padx=3, pady=2, sticky=W)
+        self._lbl_lon.grid(column=0, row=17, padx=3, pady=2, sticky=W)
+        self._ent_lon.grid(column=1, row=17, padx=3, pady=2, sticky=W)
+        self._lbl_alt.grid(column=0, row=18, padx=3, pady=2, sticky=W)
+        self._ent_alt.grid(column=1, row=18, padx=3, pady=2, sticky=W)
+        self._lbl_sep.grid(column=0, row=19, padx=3, pady=2, sticky=W)
+        self._ent_sep.grid(column=1, row=19, padx=3, pady=2, sticky=W)
         ttk.Separator(self._frm_container).grid(
-            column=0, row=19, columnspan=3, padx=3, pady=3, sticky=(W, E)
+            column=0, row=20, columnspan=3, padx=3, pady=3, sticky=(W, E)
         )
-        self._btn_connect.grid(column=0, row=20, padx=3, pady=3, sticky=W)
-        self._btn_disconnect.grid(column=1, row=20, padx=3, pady=3, sticky=W)
+        self._btn_connect.grid(column=0, row=21, padx=3, pady=3, sticky=W)
+        self._btn_disconnect.grid(column=1, row=21, padx=3, pady=3, sticky=W)
 
         # bottom of grid
-        row = 21
+        row = 22
         col = 0
         (colsp, rowsp) = self._frm_container.grid_size()
         self._frm_status.grid(column=col, row=row, columnspan=colsp, sticky=(W, E))
         self._lbl_status.grid(
             column=0, row=0, columnspan=colsp - 1, ipadx=3, ipady=3, sticky=(W, E)
         )
         self._btn_exit.grid(column=colsp - 1, row=0, ipadx=3, ipady=3, sticky=(E))
@@ -440,14 +455,16 @@
                 self._ent_mountpoint,
                 self._ent_user,
                 self._ent_password,
                 self._ent_lat,
                 self._ent_lon,
                 self._ent_alt,
                 self._ent_sep,
+                self._rad_ggalive,
+                self._rad_ggafixed,
                 self._lbx_sourcetable,
             ):
                 ctl.config(state=(DISABLED if connected else NORMAL))
             # refresh sourcetable listbox ! NB PLACEMENT OF THIS CALL IS IMPORTANT !
             self.update_sourcetable(self._settings["sourcetable"])
             # update closest mountpoint name and distance (if available)
             lat, lon = self._get_coordinates()
@@ -458,28 +475,14 @@
                     self._settings["sourcetable"],
                     self._settings["mountpoint"],
                 )
                 self.set_mp_dist(mindist, mpname)
         except TclError:  # fudge during thread termination
             pass
 
-    def _centre(self):
-        """
-        Roughly center dialog in master window
-        NB: behaviour is slightly different across Windows, MacOS and Linux
-        """
-
-        dw = self.winfo_width()
-        dh = self.winfo_height()
-        mx = self.__master.winfo_x()
-        my = self.__master.winfo_y()
-        mw = self.__master.winfo_width()
-        mh = self.__master.winfo_height()
-        self.geometry(f"+{int(mx + (mw/2 - dw/2))}+{int(my + (mh/2 - dh/2))}")
-
     def set_status(self, message: str, color: str = "blue"):
         """
         Set status message.
 
         :param str message: message to be displayed
         :param str color: rgb color of text (blue)
         """
@@ -542,25 +545,22 @@
         self._settings = self.__app.ntrip_handler.settings
         self._ntrip_server.set(self._settings["server"])
         self._ntrip_port.set(self._settings["port"])
         self._ntrip_mountpoint.set(self._settings["mountpoint"])
         self._ntrip_version.set(self._settings["version"])
         self._ntrip_user.set(self._settings["user"])
         self._ntrip_password.set(self._settings["password"])
-        self._ntrip_gga_interval.set(
-            "None"
-            if self._settings["ggainterval"] == NOGGA
-            else self._settings["ggainterval"]
-        )
+        ggaint = self._settings["ggainterval"]
+        self._ntrip_gga_interval.set("None" if ggaint == NOGGA else ggaint)
+        self._ntrip_gga_mode.set(self._settings["ggamode"])
         self._ntrip_gga_lat.set(self._settings["reflat"])
         self._ntrip_gga_lon.set(self._settings["reflon"])
         self._ntrip_gga_alt.set(self._settings["refalt"])
         self._ntrip_gga_sep.set(self._settings["refsep"])
 
-        # mindist, mpname = self.find_mp_distance(self._settings["mountpoint"])
         lat, lon = self._get_coordinates()
         mpname, mindist = find_mp_distance(
             lat, lon, self._settings["sourcetable"], self._settings["mountpoint"]
         )
         self.set_mp_dist(mindist, mpname)
 
     def _set_settings(self):
@@ -575,52 +575,50 @@
         self._settings["user"] = self._ntrip_user.get()
         self._settings["password"] = self._ntrip_password.get()
         self._settings["ggainterval"] = (
             NOGGA
             if self._ntrip_gga_interval.get() == "None"
             else self._ntrip_gga_interval.get()
         )
+        self._settings["ggamode"] = self._ntrip_gga_mode.get()
         self._settings["reflat"] = self._ntrip_gga_lat.get()
         self._settings["reflon"] = self._ntrip_gga_lon.get()
         self._settings["refalt"] = self._ntrip_gga_alt.get()
         self._settings["refsep"] = self._ntrip_gga_sep.get()
 
-        # self.__app.ntrip_handler.settings = self._settings
-
     def update_sourcetable(self, stable: list):
         """
         Update sourcetable listbox for this NTRIP server.
 
         :param list stable: sourcetable
         """
 
         self._lbx_sourcetable.unbind("<<ListboxSelect>>")
         self._lbx_sourcetable.delete(0, END)
         for item in stable:
             self._lbx_sourcetable.insert(END, item)
-        # self._lbx_sourcetable.update_idletasks()
         self._lbx_sourcetable.bind("<<ListboxSelect>>", self._on_select_mp)
 
     def _connect(self):
         """
         Connect to NTRIP Server. NTRIP handler will invoke set_controls()
         with connection status in due course.
         """
 
         if self._valid_settings():
             self._set_settings()
-            # self.__app.ntrip_handler.settings = self._settings
             self.__app.ntrip_handler.run(
                 server=self._settings["server"],
                 port=self._settings["port"],
                 mountpoint=self._settings["mountpoint"],
                 version=self._settings["version"],
                 user=self._settings["user"],
                 password=self._settings["password"],
                 ggainterval=self._settings["ggainterval"],
+                ggamode=self._settings["ggamode"],
                 reflat=self._settings["reflat"],
                 reflon=self._settings["reflon"],
                 refalt=self._settings["refalt"],
                 refsep=self._settings["refsep"],
                 output=self.__app.ntripqueue,
             )
             self.set_controls(True)
@@ -641,32 +639,19 @@
         :return: valid True/False
         :rtype: bool
         """
 
         valid = True
         valid = valid & valid_entry(self._ent_server, VALURL)
         valid = valid & valid_entry(self._ent_port, VALINT, 1, MAXPORT)
-
-        if self._ntrip_gga_interval.get() != "None":  # sending GGA
-            # either use all 4 fixed settings to construct GGA sentence,
-            # or use live readings from connected receiver
-            # valid = valid & valid_entry(self._ent_mountpoint, VALNONBLANK)
-            fxd = (
-                self._ent_lat.get()
-                + self._ent_lon.get()
-                + self._ent_alt.get()
-                + self._ent_sep.get()
-            )
-            if self.__app.conn_status != CONNECTED or (
-                self.__app.conn_status == CONNECTED and fxd != ""
-            ):
-                valid = valid & valid_entry(self._ent_lat, VALFLOAT, -90.0, 90.0)
-                valid = valid & valid_entry(self._ent_lon, VALFLOAT, -180.0, 180.0)
-                valid = valid & valid_entry(self._ent_alt, VALFLOAT, -MAXALT, MAXALT)
-                valid = valid & valid_entry(self._ent_sep, VALFLOAT, -MAXALT, MAXALT)
+        if self._settings["ggamode"] == 1:  # fixed reference
+            valid = valid & valid_entry(self._ent_lat, VALFLOAT, -90.0, 90.0)
+            valid = valid & valid_entry(self._ent_lon, VALFLOAT, -180.0, 180.0)
+            valid = valid & valid_entry(self._ent_alt, VALFLOAT, -MAXALT, MAXALT)
+            valid = valid & valid_entry(self._ent_sep, VALFLOAT, -MAXALT, MAXALT)
 
         if not valid:
             self.set_status("ERROR - invalid settings", "red")
 
         return valid
 
     def set_mp_dist(self, dist: float, name: str = ""):
@@ -688,23 +673,22 @@
             dist_l = f"Distance {dist:,.1f} {dist_u}"
 
         self._ntrip_mountpoint.set(name)
         self._ntrip_mpdist.set(dist_l)
 
     def _get_coordinates(self) -> tuple:
         """
-        Get current coordinates. If not available,
-        return fixed reference coordinates, or ""
-        if not available.
+        Get coordinates from receiver or fixed reference settings.
 
         :returns: tuple (lat,lon)
         :rtype: tuple
         """
 
         try:
-            conn_status, lat, lon, _, _ = self.__app.get_coordinates()
-            if conn_status == DISCONNECTED:
+            if self._settings.get("ggamode", 0) == 0:  # live position
+                _, lat, lon, _, _ = self.__app.get_coordinates()
+            else:  # fixed reference
                 lat = float(self._settings["reflat"])
                 lon = float(self._settings["reflon"])
             return lat, lon
         except (ValueError, TypeError):
             return "", ""
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/.DS_Store` & `PyGPSClient-1.3.9/pygpsclient/resources/.DS_Store`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/binary-1-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/binary-1-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/clear-1-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/clear-1-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/ethernet-1-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/ethernet-1-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-antenna-6-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-antenna-6-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-check-mark-8-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-check-mark-8-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-gear-2-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-gear-2-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-location-27-32.png` & `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-location-27-32.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-noclient-10-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-noclient-10-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-notransmit-10-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-notransmit-10-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-time-6-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-time-6-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/iconmonstr-transmit-10-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/iconmonstr-transmit-10-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/pygpsclient.ico` & `PyGPSClient-1.3.9/pygpsclient/resources/pygpsclient.ico`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/usbport-1-24.png` & `PyGPSClient-1.3.9/pygpsclient/resources/usbport-1-24.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/resources/world.png` & `PyGPSClient-1.3.9/pygpsclient/resources/world.png`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/rtcm3_handler.py` & `PyGPSClient-1.3.9/pygpsclient/rtcm3_handler.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/serialconfig_frame.py` & `PyGPSClient-1.3.9/pygpsclient/serialconfig_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/settings_frame.py` & `PyGPSClient-1.3.9/pygpsclient/settings_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/skyview_frame.py` & `PyGPSClient-1.3.9/pygpsclient/skyview_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/socketconfig_frame.py` & `PyGPSClient-1.3.9/pygpsclient/socketconfig_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/status_frame.py` & `PyGPSClient-1.3.9/pygpsclient/status_frame.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/stream_handler.py` & `PyGPSClient-1.3.9/pygpsclient/stream_handler.py`

 * *Files identical despite different names*

### Comparing `PyGPSClient-1.3.8/pygpsclient/strings.py` & `PyGPSClient-1.3.9/pygpsclient/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 BTNRST = "Reset"
 
 # Label text
 LBLPROTDISP = "Protocols Shown"
 LBLDATADISP = "Console Display"
 LBLUBXCONFIG = "UBX\nConfig"
 LBLNTRIPCONFIG = "NTRIP\nClient"
-LBLNTRIPGGAINT = "GGA Interval"
+LBLNTRIPGGAINT = "GGA Interval s"
 LBLCTL = "Controls"
 LBLSET = "Settings"
 LBLCFGPRT = "CFG-PRT Protocol Configuration"
 LBLCFGRATE = "CFG-RATE Navigation Solution Rate Configuration"
 LBLCFGMSG = "CFG-MSG Message Rate Configuration"
 LBLPRESET = "Preset UBX Configuration Commands"
 LBLDATALOG = "DataLogging"
@@ -105,14 +105,16 @@
 LBLNTRIPPWD = "Password"
 LBLNTRIPSTR = "Sourcetable"
 LBLSOCKSERVE = "Socket Server /\nNTRIP Caster   "  # padded to align
 LBLSERVERPORT = "Port"
 LBLDEGFORMAT = "Degrees Format"
 LBLSERVERMODE = "Mode"
 LBLCFGDYN = "CFG-* Other Configuration"
+LBLGGALIVE = "Receiver"
+LBLGGAFIXED = "Fixed Reference"
 
 # Dialog text
 DLGUBXCONFIG = "UBX Configuration"
 DLGNTRIPCONFIG = "NTRIP Client Configuration"
 DLGABOUT = "PyGPSClient"
 DLGHOWTO = "How To Use PyGPSCLient"
 DLGRESET = "Confirm Reset"
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/ubx_cfgval_frame.py` & `PyGPSClient-1.3.9/pygpsclient/ubx_cfgval_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-UBX Configuration widget for CFG-VAL commands
+UBX Configuration frame for CFG-VAL commands
 
 Created on 22 Dec 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
@@ -401,15 +401,16 @@
 
         if valid_entry:
             msg = UBXMessage.config_set(layers, transaction, cfgData)
             self.__app.stream_handler.serial_write(msg.serialize())
             self._ent_val.configure(bg=ENTCOL)
             self._lbl_send_command.config(image=self._img_pending)
             self.__container.set_status("CFG-VALSET SET message sent", "blue")
-            self.__container.set_pending(UBX_CFGVAL, ("ACK-ACK", "ACK-NAK"))
+            for msgid in ("ACK-ACK", "ACK-NAK"):
+                self.__container.set_pending(msgid, UBX_CFGVAL)
         else:
             self._ent_val.configure(bg=ERRCOL)
             self._lbl_send_command.config(image=self._img_warn)
             typ = ATTDICT[att]
             self.__container.set_status(
                 (
                     "INVALID ENTRY - must conform to parameter "
@@ -437,15 +438,16 @@
             self._cfgval_keyname,
         ]
         msg = UBXMessage.config_del(layers, transaction, key)
         self.__app.stream_handler.serial_write(msg.serialize())
         self._ent_val.configure(bg=ENTCOL)
         self._lbl_send_command.config(image=self._img_pending)
         self.__container.set_status("CFG-VALDEL SET message sent", "blue")
-        self.__container.set_pending(UBX_CFGVAL, ("ACK-ACK", "ACK-NAK"))
+        for msgid in ("ACK-ACK", "ACK-NAK"):
+            self.__container.set_pending(msgid, UBX_CFGVAL)
 
     def _do_valget(self):
         """
         Send a CFG-VALGET message.
         """
 
         layers = self._cfglayer.get()
@@ -462,33 +464,33 @@
             self._cfgval_keyname,
         ]
         msg = UBXMessage.config_poll(layers, transaction, keys)
         self.__app.stream_handler.serial_write(msg.serialize())
         self._ent_val.configure(bg=ENTCOL)
         self._lbl_send_command.config(image=self._img_pending)
         self.__container.set_status("CFG-VALGET POLL message sent", "blue")
-        self.__container.set_pending(UBX_CFGVAL, ("CFG-VALGET", "ACK-ACK", "ACK-NAK"))
+        for msgid in ("CFG-VALGET", "ACK-ACK", "ACK-NAK"):
+            self.__container.set_pending(msgid, UBX_CFGVAL)
 
-    def update_status(self, cfgtype, **kwargs):  # pylint: disable=unused-argument
+    def update_status(self, msg: UBXMessage):  # pylint: disable=unused-argument
         """
         Update pending confirmation status.
 
-        :param str cfgtype: identity of UBX message containing config info
-        :param kwargs: status keywords and values from UBX config message
+        :param UBXMessage msg: UBX config message
         """
 
-        if cfgtype == "CFG-VALGET":
+        if msg.identity == "CFG-VALGET":
             self._lbl_send_command.config(image=self._img_confirmed)
-            data = kwargs.get("data", None)
-            if data is not None:
-                val = getattr(data, self._cfgval_keyname, None)
-                if val is not None:
-                    if isinstance(val, bytes):
-                        val = val.hex()
-                    self._cfgval.set(val)
-            self.__container.set_status(f"{cfgtype} GET message received", "green")
-        elif cfgtype == "ACK-ACK":
+            val = getattr(msg, self._cfgval_keyname, None)
+            if val is not None:
+                if isinstance(val, bytes):
+                    val = val.hex()
+                self._cfgval.set(val)
+            self.__container.set_status("CFG-VALGET GET message received", "green")
+
+        elif msg.identity == "ACK-ACK":
             self._lbl_send_command.config(image=self._img_confirmed)
-            self.__container.set_status(f"{cfgtype} GET message received", "green")
-        elif cfgtype == "ACK-NAK":
+            self.__container.set_status("CFG-VAL command acknowledged", "green")
+
+        elif msg.identity == "ACK-NAK":
             self._lbl_send_command.config(image=self._img_warn)
-            self.__container.set_status("CFG-VAL message rejected", "red")
+            self.__container.set_status("CFG-VAL command rejected", "red")
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/ubx_config_dialog.py` & `PyGPSClient-1.3.9/pygpsclient/ubx_config_dialog.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """
 UBX configuration container dialog
 
 This is the pop-up dialog containing the various
-UBX configuration command widgets.
+UBX configuration command frames.
 
 NB: Individual UBX configuration commands do not have uniquely
 identifiable synchronous or asynchronous responses (e.g. unique
 txn ID). The way we keep tabs on confirmation status is to
 maintain a list of all commands sent and the responses they're
 expecting. When we receive a response, we check against the list
 of awaited responses of the same type and flag the first one we
-find as 'confirmed'. This is generally reliable but not absolutely
-foolproof - if several commands awaiting the same response type are
-sent in quick succession, it's possible their responses may arrive
-out of order (or not at all) and we may flag the wrong command as
-'confirmed', or leave a confirmed command as 'pending'.
+find as 'confirmed'.
 
 Created on 19 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
@@ -32,14 +28,15 @@
     StringVar,
     N,
     S,
     E,
     W,
 )
 from PIL import ImageTk, Image
+from pyubx2 import UBXMessage
 from pygpsclient.globals import (
     ICON_EXIT,
     UBX_MONVER,
     UBX_MONHW,
     UBX_CFGPRT,
     UBX_CFGRATE,
     UBX_CFGMSG,
@@ -80,30 +77,21 @@
         if POPUP_TRANSIENT:
             self.transient(self.__app)
         self.resizable(True, True)  # allow for MacOS resize glitches
         self.title(DLGUBXCONFIG)  # pylint: disable=E1102
         self.protocol("WM_DELETE_WINDOW", self.on_exit)
         self._img_exit = ImageTk.PhotoImage(Image.open(ICON_EXIT))
         self._cfg_msg_command = None
-        self._pending_confs = {
-            UBX_MONVER: (),
-            UBX_MONHW: (),
-            UBX_CFGPRT: (),
-            UBX_CFGMSG: (),
-            UBX_CFGVAL: (),
-            UBX_PRESET: (),
-            UBX_CFGRATE: (),
-        }
+        self._pending_confs = {}
         self._status = StringVar()
         self._status_cfgmsg = StringVar()
 
         self._body()
         self._do_layout()
         self._reset()
-        # self._centre()
 
     def _body(self):
         """
         Set up frame and widgets.
         """
 
         self._frm_container = Frame(self, borderwidth=2, relief="groove")
@@ -235,71 +223,55 @@
         self._frm_config_rate.reset()
         self._frm_config_port.reset()
         self._frm_config_dynamic.reset()
         self._frm_device_info.reset()
         if self.__app.conn_status != CONNECTED:
             self.set_status("Device not connected", "red")
 
-    def _centre(self):
+    def set_pending(self, msgid: int, ubxfrm: int):
         """
-        Roughly center dialog in master window
-        NB: behaviour is slightly different across Windows, MacOS and Linux
-        """
-
-        dw = self.winfo_width()
-        dh = self.winfo_height()
-        mx = self.__master.winfo_x()
-        my = self.__master.winfo_y()
-        mw = self.__master.winfo_width()
-        mh = self.__master.winfo_height()
-        self.geometry(f"+{int(mx + (mw/2 - dw/2))}+{int(my + (mh/2 - dh/2))}")
-
-    def set_pending(self, key: int, val: list):
-        """
-        Set pending confirmation flag for configuration widget to
+        Set pending confirmation flag for UBX configuration frame to
         signify that it's waiting for a confirmation message.
 
-        :param int key: integer representing UBX configuration widget (0-6)
-        :param list val: list of confirmation messages that widget is awaiting
+        :param int msgid: UBX message identity
+        :param int ubxfrm: integer representing UBX configuration frame (0-6)
         """
 
-        self._pending_confs[key] = val
+        self._pending_confs[msgid] = ubxfrm
 
-    def update_pending(self, cfgtype, **kwargs):
+    def update_pending(self, msg: UBXMessage):
         """
         Receives polled confirmation message from the ubx_handler and
-        updates the widget that is waiting for this confirmation.
+        updates whichever UBX config frame is waiting for this confirmation.
 
-        :param str cfgtype: identity of UBX message containing config info
-        :param kwargs: status keywords and values from UBX config message
+        :param UBXMessage msg: UBX config message
         """
 
-        for (key, val) in self._pending_confs.items():
-            if cfgtype in val:
-                self.set_status(
-                    f"{cfgtype} GET message received",
-                    "red" if cfgtype == "ACK-NAK" else "green",
-                )
-                self._pending_confs[key] = ()  # reset awaiting conf flag
-                if key == UBX_MONVER:
-                    self._frm_device_info.update_status(cfgtype, **kwargs)
-                elif key == UBX_MONHW:
-                    self._frm_device_info.update_status(cfgtype, **kwargs)
-                elif key == UBX_CFGPRT:
-                    self._frm_config_port.update_status(cfgtype, **kwargs)
-                elif key == UBX_CFGRATE:
-                    self._frm_config_rate.update_status(cfgtype, **kwargs)
-                elif key == UBX_CFGMSG:
-                    self._frm_config_msg.update_status(cfgtype, **kwargs)
-                elif key == UBX_CFGVAL:
-                    self._frm_configdb.update_status(cfgtype, **kwargs)
-                elif key == UBX_PRESET:
-                    self._frm_preset.update_status(cfgtype, **kwargs)
-                elif key == UBX_CFGOTHER:
-                    self._frm_config_dynamic.update_status(cfgtype, **kwargs)
+        ubxfrm = self._pending_confs.get(msg.identity, None)
+
+        if ubxfrm is not None:
+            if ubxfrm in (UBX_MONVER, UBX_MONHW):
+                self._frm_device_info.update_status(msg)
+            elif ubxfrm == UBX_CFGPRT:
+                self._frm_config_port.update_status(msg)
+            elif ubxfrm == UBX_CFGRATE:
+                self._frm_config_rate.update_status(msg)
+            elif ubxfrm == UBX_CFGMSG:
+                self._frm_config_msg.update_status(msg)
+            elif ubxfrm == UBX_CFGVAL:
+                self._frm_configdb.update_status(msg)
+            elif ubxfrm == UBX_PRESET:
+                self._frm_preset.update_status(msg)
+            elif ubxfrm == UBX_CFGOTHER:
+                self._frm_config_dynamic.update_status(msg)
+
+            # reset all confirmation flags for this frame
+            for msgid in (msg.identity, "ACK-ACK", "ACK-NAK"):
+                if self._pending_confs.get(msgid, None) == ubxfrm:
+                    self._pending_confs.pop(msgid)
 
     def set_status(self, message: str, color: str = "blue"):
         """
         Set status message.
 
         :param str message: message to be displayed
         :param str color: rgb color of text (blue)
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/ubx_dynamic_frame.py` & `PyGPSClient-1.3.9/pygpsclient/ubx_dynamic_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     atttyp,
     X1,
     X2,
     X4,
     X6,
     X8,
     X24,
-    U1,
 )
 from .globals import (
     ENTCOL,
     ICON_SEND,
     ICON_WARNING,
     ICON_PENDING,
     ICON_CONFIRMED,
@@ -67,15 +66,14 @@
 from .helpers import stringvar2val
 
 # dimensions of scrollable attribute window
 SCROLLX = 300
 SCROLLY = 300
 # following CFG types exluded from selection...
 CFG_EXCLUDED = (
-    # "CFG-CFG",  # handled via Preset panel
     "CFG-DAT-NUM",  # deprecated
     "CFG-GEOFENCE",  # 'variable by size' groups not yet implemented - use pyubx2
     "CFG-MSG",  # handled via existing CFG-MSG panel
     "CFG-NMEAv0",  # deprecated
     "CFG-NMEAvX",  # deprecated
     "CFG-PRT",  # handled via existing CFG-PRT panel
     "CFG-RATE",  # handled via existing CFG-RATE panel
@@ -206,15 +204,14 @@
         self._frm_attrs.bind("<Configure>", self._setscroll)
 
     def reset(self):
         """
         Reset panel to initial settings
         """
 
-        # populate CFG listbox with range of CFG message types
         self._lbx_cfg_cmd.delete(0, END)
         for i, cmd in enumerate(UBX_PAYLOADS_SET):
             if cmd[0:3] == "CFG" and cmd not in CFG_EXCLUDED:
                 self._lbx_cfg_cmd.insert(i, cmd)
 
         self._clear_widgets()
         self._lbl_send_command.config(image=self._img_unknown)
@@ -241,35 +238,33 @@
         self._do_poll_cfg()
         self._lbl_command.config(text=self._cfg_id)
 
         self._clear_widgets()
         self._add_widgets(None, UBX_PAYLOADS_SET[self._cfg_id], 1, 0)
         self.update()
 
-    def update_status(self, cfgtype, **kwargs):
+    def update_status(self, msg: UBXMessage):
         """
         UBXHandler module receives CFG SET/POLL response and forwards it
         on to this module; confirmation status updated accordingly.
 
-        :param str cfgtype: identity of UBX CFG message
-        :param kwargs: status keywords and values from UBX config message
+        :param UBXMessage msg: UBX config message
         """
 
-        if cfgtype == self._cfg_id:
+        if msg.identity == self._cfg_id:
             self._lbl_send_command.config(image=self._img_confirmed)
-            self.__container.set_status(f"{cfgtype} GET message received", "green")
-            msg = kwargs.get("msg", None)  # CFG POLL response message
+            self.__container.set_status(f"{msg.identity} GET message received", "green")
             self._clear_widgets()
             self._add_widgets(msg, UBX_PAYLOADS_SET[self._cfg_id], 1, 0)
             self.update()
-        elif cfgtype == "ACK-NAK":
-            self.__container.set_status(f"{cfgtype} POLL message rejected", "red")
+        elif msg.identity == "ACK-NAK":
+            self.__container.set_status(f"{self._cfg_id} message rejected", "red")
             self._lbl_send_command.config(image=self._img_warn)
-        elif cfgtype == "ACK-ACK":
-            self.__container.set_status(f"{cfgtype} SET message accepted", "green")
+        elif msg.identity == "ACK-ACK":
+            self.__container.set_status(f"{self._cfg_id} message acknowledged", "green")
             self._lbl_send_command.config(image=self._img_confirmed)
 
     def _clear_widgets(self):
         """
         Clear dynamically generated Entry widgets from panel.
         """
 
@@ -340,39 +335,38 @@
         :return: last row used
         :rtype: int
         """
 
         numr, attd = att
 
         if index == 1:
-            # if 'variable by size' group, add entry field to
+            # TODO if 'variable by size' group, add entry field to
             # allow user to specify size of group
-            # TODO not currently fully implemented
-            if numr == "None":
-                self._cfg_atts[nam] = (StringVar(), U1)
-                Label(self._frm_attrs, text="Group Size:").grid(
-                    column=0, row=row, sticky=(E)
-                )
-                Entry(
-                    self._frm_attrs,
-                    readonlybackground=ENTCOL,
-                    textvariable=self._cfg_atts[nam],
-                    relief="sunken",
-                    bg=ENTCOL,
-                ).grid(column=1, row=row, sticky=(W))
-                Label(self._frm_attrs, text=U1).grid(column=2, row=row, sticky=(W))
-                row += 1
-            # otherwise add label indicating the integer or existing attribute
-            # which represents the group size
-            else:
-                Label(self._frm_attrs, text="Group Size:").grid(
-                    column=0, row=row, sticky=(E)
-                )
-                Label(self._frm_attrs, text=numr).grid(column=1, row=row, sticky=(W))
-                row += 1
+            # if numr == "None":
+            #     self._cfg_atts[nam] = (StringVar(), U1)
+            #     Label(self._frm_attrs, text="Group Size:").grid(
+            #         column=0, row=row, sticky=(E)
+            #     )
+            #     Entry(
+            #         self._frm_attrs,
+            #         readonlybackground=ENTCOL,
+            #         textvariable=self._cfg_atts[nam],
+            #         relief="sunken",
+            #         bg=ENTCOL,
+            #     ).grid(column=1, row=row, sticky=(W))
+            #     Label(self._frm_attrs, text=U1).grid(column=2, row=row, sticky=(W))
+            #     row += 1
+            #     otherwise add label indicating the integer or existing attribute
+            #     which represents the group size
+            # else:
+            Label(self._frm_attrs, text="Group Size:").grid(
+                column=0, row=row, sticky=(E)
+            )
+            Label(self._frm_attrs, text=numr).grid(column=1, row=row, sticky=(W))
+            row += 1
 
         row = self._add_widgets(msg, attd, row, index)
 
         return row
 
     def _add_widgets_single(
         self,
@@ -401,26 +395,24 @@
             return row
 
         if index > 0:  # if part of group, add index suffix e.g. '_02'
             nam += f"_{index:02d}"
         if isinstance(att, list):  # (type, scale factor)
             att = att[0]
 
-        # create and populate StringVar for this attribute
         self._cfg_atts[nam] = (StringVar(), att)
         if msg is not None:  # set initial value from POLL response
             mval = getattr(msg, nam)
             if nam == "bdsTalkerId":  # fudge for default CFG-NMEA bdsTalkerId
                 if mval == b"\x00\x00":
                     mval = ""
-            if atttyp(att) == "X":  # convert bytes to hex string for display
+            if atttyp(att) == "X":
                 mval = hex(int.from_bytes(mval, "big"))
             self._cfg_atts[nam][0].set(mval)
 
-        # add Entry widget with labels
         Label(self._frm_attrs, text=nam).grid(column=0, row=row, sticky=(E))
         Entry(
             self._frm_attrs,
             readonlybackground=ENTCOL,
             textvariable=self._cfg_atts[nam][0],
             relief="sunken",
             bg=ENTCOL,
@@ -428,16 +420,15 @@
         Label(self._frm_attrs, text=att).grid(column=2, row=row, sticky=(W))
         row += 1
 
         return row
 
     def _on_send_cfg(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
-        Populate CFG SET message from Entry fields on panel, send to device,
-        then send CFG POLL to confirm update.
+        Populate CFG SET message from Entry fields on panel and send to device.
         """
 
         nam = ""
         ent = StringVar().set("")
         try:
 
             # create dict of attribute keyword arguments from
@@ -450,18 +441,16 @@
             # create UBXMessage using these keyword arguments
             msg = UBXMessage("CFG", self._cfg_id, SET, **vals)
 
             # send message, update status and await response
             self.__app.stream_handler.serial_write(msg.serialize())
             self._lbl_send_command.config(image=self._img_pending)
             self.__container.set_status(f"{self._cfg_id} SET message sent", "blue")
-            self.__container.set_pending(UBX_CFGOTHER, ("ACK-ACK", "ACK-NAK"))
-
-            # POLL to confirm update
-            self._do_poll_cfg()
+            for msgid in ("ACK-ACK", "ACK-NAK"):
+                self.__container.set_pending(msgid, UBX_CFGOTHER)
 
         except ValueError as err:
             self.__container.set_status(
                 f"INVALID! {nam}, {att}: {err}",
                 "red",
             )
 
@@ -471,11 +460,12 @@
         """
 
         if self._cfg_id in UBX_PAYLOADS_POLL:  # CFG is POLLable
             msg = UBXMessage("CFG", self._cfg_id, POLL)
             self.__app.stream_handler.serial_write(msg.serialize())
             self.__container.set_status(f"{self._cfg_id} POLL message sent", "blue")
             self._lbl_send_command.config(image=self._img_pending)
-            self.__container.set_pending(UBX_CFGOTHER, (self._cfg_id, "ACK-NAK"))
+            for msgid in (self._cfg_id, "ACK-NAK"):
+                self.__container.set_pending(msgid, UBX_CFGOTHER)
         else:  # CFG cannot be POLLed
             self.__container.set_status(f"{self._cfg_id} No POLL available", "blue")
             self._lbl_send_command.config(image=self._img_unknown)
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/ubx_info_frame.py` & `PyGPSClient-1.3.9/pygpsclient/ubx_info_frame.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-UBX Configuration widget for MON-VER and MON-HW messages
+UBX Configuration frame for MON-VER and MON-HW messages
 
 Created on 22 Dec 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
@@ -127,39 +127,74 @@
         """
         Reset panel to initial settings
         """
 
         if self.__app.conn_status == CONNECTED:
             self._do_poll_ver()
 
-    def update_status(self, cfgtype, **kwargs):
+    def update_status(self, msg: UBXMessage):
         """
         Update pending confirmation status.
 
-        :param str cfgtype: identity of UBX message containing config info
-        :param kwargs: status keywords and values from UBX config message
+        :param UBXMessage msg: UBX config message
         """
 
         # MON-VER information (for firmware version)
-        if cfgtype == "MON-VER":
-            self._sw_version.set(kwargs.get("swversion", ""))
-            self._hw_version.set(kwargs.get("hwversion", ""))
-            self._fw_version.set(kwargs.get("fwversion", ""))
-            self._protocol.set(kwargs.get("protocol", ""))
-            self._gnss_supported.set(kwargs.get("gnsssupported", ""))
+        if msg.identity == "MON-VER":
+
+            exts = []
+            fw_version = b"n/a"
+            protocol = b"n/a"
+            gnss_supported = b""
+            model = b""
+            sw_version = getattr(msg, "swVersion", b"n/a")
+            sw_version = sw_version.replace(b"\x00", b"")
+            sw_version = sw_version.replace(b"ROM CORE", b"ROM")
+            sw_version = sw_version.replace(b"EXT CORE", b"Flash")
+            hw_version = getattr(msg, "hwVersion", b"n/a")
+            hw_version = hw_version.replace(b"\x00", b"")
+
+            for i in range(9):
+                idx = f"_{i+1:02d}"
+                ext = getattr(msg, "extension" + idx, b"")
+                ext = ext.replace(b"\x00", b"")
+                exts.append(ext)
+                if b"FWVER=" in exts[i]:
+                    fw_version = exts[i].replace(b"FWVER=", b"")
+                if b"PROTVER=" in exts[i]:
+                    protocol = exts[i].replace(b"PROTVER=", b"")
+                if b"PROTVER " in exts[i]:
+                    protocol = exts[i].replace(b"PROTVER ", b"")
+                if b"MOD=" in exts[i]:
+                    model = exts[i].replace(b"MOD=", b"")
+                    hw_version = model + b" " + hw_version
+                for gnss in (b"GPS", b"GLO", b"GAL", b"BDS", b"SBAS", b"IMES", b"QZSS"):
+                    if gnss in exts[i]:
+                        gnss_supported = gnss_supported + gnss + b" "
+
+            self._sw_version.set(sw_version)
+            self._hw_version.set(hw_version)
+            self._fw_version.set(fw_version)
+            self._protocol.set(protocol)
+            self._gnss_supported.set(gnss_supported)
 
         # MON-HW information (for antenna status)
-        if cfgtype == "MON-HW":
-            self._ant_status.set(ANTSTATUS[kwargs.get("antstatus", 1)])
-            self._ant_power.set(ANTPOWER[kwargs.get("antpower", 2)])
+        if msg.identity == "MON-HW":
+
+            ant_status = getattr(msg, "aStatus", 1)
+            ant_power = getattr(msg, "aPower", 2)
+            self._ant_status.set(ANTSTATUS[ant_status])
+            self._ant_power.set(ANTPOWER[ant_power])
+
+        self.__container.set_status(f"{msg.identity} GET message received", "green")
 
     def _do_poll_ver(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Poll MON-VER & MON-HW
         """
 
         for msgtype in ("MON-VER", "MON-HW"):
             msg = UBXMessage(msgtype[0:3], msgtype, POLL)
             self.__app.stream_handler.serial.write(msg.serialize())
             self.__container.set_status(f"{msgtype} POLL message sent", "blue")
-        self.__container.set_pending(UBX_MONVER, ("MON-VER",))
-        self.__container.set_pending(UBX_MONHW, ("MON-HW",))
+        self.__container.set_pending("MON-VER", UBX_MONVER)
+        self.__container.set_pending("MON-HW", UBX_MONHW)
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/ubx_msgrate_frame.py` & `PyGPSClient-1.3.9/pygpsclient/ubx_msgrate_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-UBX Configuration widget for CFG-MSG commands
+UBX Configuration frame for CFG-MSG commands
 
 Created on 22 Dec 2020
 
 Created on 22 Sep 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
@@ -29,15 +29,15 @@
 from PIL import ImageTk, Image
 from pyubx2 import (
     UBXMessage,
     POLL,
     SET,
     UBX_MSGIDS,
 )
-from pyubx2.ubxhelpers import key_from_val
+from pyubx2.ubxhelpers import key_from_val, msgclass2bytes
 from pygpsclient.globals import (
     ENTCOL,
     ICON_SEND,
     ICON_WARNING,
     ICON_PENDING,
     ICON_CONFIRMED,
     READONLY,
@@ -210,31 +210,32 @@
 
         idx = 0
         for _, val in UBX_MSGIDS.items():
             if val[0:3] not in ("ACK", "CFG", "AID", "MGA", "UPD", "FOO"):
                 self._lbx_cfg_msg.insert(idx, val)
                 idx += 1
 
-    def update_status(self, cfgtype, **kwargs):
+    def update_status(self, msg: UBXMessage):
         """
         Update pending confirmation status.
 
-        :param str cfgtype: identity of UBX message containing config info
-        :param kwargs: status keywords and values from UBX config message
+        :param UBXMessage msg: UBX config message
         """
 
-        if cfgtype == "CFG-MSG":
+        if msg.identity == "CFG-MSG":
+
             self.__container.set_status("CFG-MSG GET message received", "green")
-            self._ddc_rate.set(kwargs.get("ddcrate", 0))
-            self._uart1_rate.set(kwargs.get("uart1rate", 0))
-            self._uart2_rate.set(kwargs.get("uart2rate", 0))
-            self._usb_rate.set(kwargs.get("usbrate", 0))
-            self._spi_rate.set(kwargs.get("spirate", 0))
+            self._ddc_rate.set(msg.rateDDC)
+            self._uart1_rate.set(msg.rateUART1)
+            self._uart2_rate.set(msg.rateUART2)
+            self._usb_rate.set(msg.rateUSB)
+            self._spi_rate.set(msg.rateSPI)
             self._lbl_send_command.config(image=self._img_confirmed)
-        elif cfgtype == "ACK-NAK":
+
+        elif msg.identity == "ACK-NAK":
             self.__container.set_status("CFG-MSG POLL message rejected", "red")
             self._lbl_send_command.config(image=self._img_warn)
 
     def _on_select_cfg_msg(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         CFG-MSG command has been selected.
         """
@@ -270,21 +271,23 @@
             rateUART2=rateUART2,
             rateUSB=rateUSB,
             rateSPI=rateSPI,
         )
         self.__app.stream_handler.serial_write(data.serialize())
         self._lbl_send_command.config(image=self._img_pending)
         self.__container.set_status("CFG-MSG SET message sent", "green")
-        self.__container.set_pending(UBX_CFGMSG, ("ACK-ACK", "ACK-NAK"))
+        for msgid in ("ACK-ACK", "ACK-NAK"):
+            self.__container.set_pending(msgid, UBX_CFGMSG)
 
         self._do_poll_msg(msg)
 
     def _do_poll_msg(self, msg):
         """
         Poll message rate.
         """
 
         data = UBXMessage("CFG", "CFG-MSG", POLL, payload=msg)  # poll for a response
         self.__app.stream_handler.serial_write(data.serialize())
         self._lbl_send_command.config(image=self._img_pending)
         self.__container.set_status("CFG-MSG POLL message sent", "blue")
-        self.__container.set_pending(UBX_CFGMSG, ("CFG-MSG", "ACK-NAK"))
+        for msgid in ("CFG-MSG", "ACK-NAK"):
+            self.__container.set_pending(msgid, UBX_CFGMSG)
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/ubx_port_frame.py` & `PyGPSClient-1.3.9/pygpsclient/ubx_port_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-UBX Configuration widget for CFG-PRT commands
+UBX Configuration frame for CFG-PRT commands
 
 Created on 22 Dec 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
@@ -188,36 +188,34 @@
         """
         Reset panel to initial settings
         """
 
         if self.__app.conn_status == CONNECTED:
             self._do_poll_prt()
 
-    def update_status(self, cfgtype, **kwargs):
+    def update_status(self, msg: UBXMessage):
         """
         Update pending confirmation status.
 
-        :param str cfgtype: identity of UBX message containing config info
-        :param kwargs: status keywords and values from UBX config message
+        :param UBXMessage msg: UBX config message
         """
 
-        if cfgtype == "CFG-PRT":
-            self._bpsrate.set(str(kwargs.get("bpsrate", 0)))
-            (inUBX, inNMEA, inRTCM, inRTCM3) = kwargs.get("inprot", (1, 1, 0, 1))
-            (outUBX, outNMEA, outRTCM3) = kwargs.get("outprot", (1, 1, 0))
-            self._inprot_ubx.set(inUBX)
-            self._inprot_nmea.set(inNMEA)
-            self._inprot_rtcm2.set(inRTCM)
-            self._inprot_rtcm3.set(inRTCM3)
-            self._outprot_ubx.set(outUBX)
-            self._outprot_nmea.set(outNMEA)
-            self._outprot_rtcm3.set(outRTCM3)
+        if msg.identity == "CFG-PRT":
+            self._bpsrate.set(msg.baudRate)
+            self._inprot_ubx.set(msg.inUBX)
+            self._inprot_nmea.set(msg.inNMEA)
+            self._inprot_rtcm2.set(msg.inRTCM)
+            self._inprot_rtcm3.set(msg.inRTCM3)
+            self._outprot_ubx.set(msg.outUBX)
+            self._outprot_nmea.set(msg.outNMEA)
+            self._outprot_rtcm3.set(msg.outRTCM3)
             self._lbl_send_command.config(image=self._img_confirmed)
             self.__container.set_status("CFG-PRT GET message received", "green")
-        elif cfgtype == "ACK-NAK":
+
+        elif msg.identity == "ACK-NAK":
             self.__container.set_status("CFG-PRT POLL message rejected", "red")
             self._lbl_send_command.config(image=self._img_warn)
 
     def _on_select_portid(self):
         """
         Handle portid selection.
         """
@@ -268,8 +266,9 @@
         """
 
         portID = int(self._portid.get()[0:1])
         msg = UBXMessage("CFG", "CFG-PRT", POLL, portID=portID)
         self.__app.stream_handler.serial_write(msg.serialize())
         self._lbl_send_command.config(image=self._img_pending)
         self.__container.set_status("CFG-PRT POLL message sent", "blue")
-        self.__container.set_pending(UBX_CFGPRT, ("CFG-PRT", "ACK-NAK"))
+        for msgid in ("CFG-PRT", "ACK-NAK"):
+            self.__container.set_pending(msgid, UBX_CFGPRT)
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/ubx_preset_frame.py` & `PyGPSClient-1.3.9/pygpsclient/ubx_preset_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-UBX Configuration widget for preset and user-defined commands
+UBX Configuration frame for preset and user-defined commands
 
 Created on 22 Dec 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
@@ -212,14 +212,15 @@
 
     def _on_send_preset(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Preset command send button has been clicked.
         """
 
         confirmed = True
+        confids = ("MON-VER", "ACK-ACK")
         try:
 
             if self._preset_command == PSTRESET:
                 confirmed = self._do_factory_reset()
             elif self._preset_command == PSTSAVE:
                 confirmed = self._do_save_config()
             elif self._preset_command == PSTMINNMEAON:
@@ -255,22 +256,22 @@
             elif self._preset_command == PSTPOLLINFO:
                 self._do_poll_inf()
             elif self._preset_command == PSTPOLLALLCFG:
                 self._do_poll_all_CFG()
             elif self._preset_command == PSTPOLLALLNAV:
                 self._do_poll_all_NAV()
             else:
+                confids = ("MON-VER", "ACK-ACK", "ACK-NAK")
                 self._do_user_defined(self._preset_command)
 
             if confirmed:
                 self._lbl_send_command.config(image=self._img_pending)
                 self.__container.set_status("Command(s) sent", "blue")
-                self.__container.set_pending(
-                    UBX_PRESET, ("ACK-ACK", "ACK-NAK", "MON-VER")
-                )
+                for msgid in confids:
+                    self.__container.set_pending(msgid, UBX_PRESET)
             else:
                 self.__container.set_status("Command(s) cancelled", "blue")
 
         except Exception as err:  # pylint: disable=broad-except
             self.__container.set_status(f"Error {err}", "red")
             self._lbl_send_command.config(image=self._img_warn)
 
@@ -540,21 +541,20 @@
                 else:
                     msg = UBXMessage(ubx_class, ubx_id, mode)
                 self.__app.stream_handler.serial_write(msg.serialize())
         except Exception as err:  # pylint: disable=broad-except
             self.__app.set_status(f"Error {err}", "red")
             self._lbl_send_command.config(image=self._img_warn)
 
-    def update_status(self, cfgtype, **kwargs):
+    def update_status(self, msg: UBXMessage):
         """
         Update pending confirmation status.
 
-        :param str cfgtype: identity of UBX message containing config info
-        :param kwargs: status keywords and values from UBX config message
+        :param UBXMessage msg: UBX config message
         """
 
-        if cfgtype in ("ACK-ACK", "MON-VER"):
+        if msg.identity in ("ACK-ACK", "MON-VER"):
             self._lbl_send_command.config(image=self._img_confirmed)
-            self.__container.set_status(f"{cfgtype} GET message received", "green")
-        elif cfgtype == "ACK-NAK":
+            self.__container.set_status("Preset command(s) acknowledged", "green")
+        elif msg.identity == "ACK-NAK":
             self._lbl_send_command.config(image=self._img_warn)
-            self.__container.set_status("PRESET command rejected", "red")
+            self.__container.set_status("Preset command(s) rejected", "red")
```

### Comparing `PyGPSClient-1.3.8/pygpsclient/ubx_solrate_frame.py` & `PyGPSClient-1.3.9/pygpsclient/ubx_solrate_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-UBX Configuration widget for CFG-RATE commands
+UBX Configuration frame for CFG-RATE commands
 
 Created on 19 Feb 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
@@ -169,29 +169,29 @@
         """
         Reset panel to initial settings.
         """
 
         if self.__app.conn_status == CONNECTED:
             self._do_poll_rate()
 
-    def update_status(self, cfgtype, **kwargs):
+    def update_status(self, msg: UBXMessage):
         """
         Update pending confirmation status.
 
-        :param str cfgtype: identity of UBX message containing config info
-        :param kwargs: status keywords and values from UBX config message
+        :param UBXMessage msg: UBX config message
         """
 
-        if cfgtype == "CFG-RATE":
-            self._measint.set(kwargs.get("measrate", 1000))
-            self._navrate.set(kwargs.get("navrate", 1))
-            self._timeref.set(TIMEREFS[kwargs.get("timeref", 0)])
+        if msg.identity == "CFG-RATE":
+            self._measint.set(msg.measRate)
+            self._navrate.set(msg.navRate)
+            self._timeref.set(TIMEREFS[msg.timeRef])
             self._lbl_send_command.config(image=self._img_confirmed)
             self.__container.set_status("CFG-RATE GET message received", "green")
-        elif cfgtype == "ACK-NAK":
+
+        elif msg.identity == "ACK-NAK":
             self.__container.set_status("CFG-RATE POLL message rejected", "red")
             self._lbl_send_command.config(image=self._img_warn)
 
     def _on_send_rate(self, *args, **kwargs):  # pylint: disable=unused-argument
         """
         Handle Send rate config button press.
         """
@@ -222,8 +222,9 @@
         Poll RATE message configuration.
         """
 
         msg = UBXMessage("CFG", "CFG-RATE", POLL)
         self.__app.stream_handler.serial_write(msg.serialize())
         self._lbl_send_command.config(image=self._img_pending)
         self.__container.set_status("CFG-RATE POLL message sent", "blue")
-        self.__container.set_pending(UBX_CFGRATE, ("CFG-RATE", "ACK-NAK"))
+        for msgid in ("CFG-RATE", "ACK-NAK"):
+            self.__container.set_pending(msgid, UBX_CFGRATE)
```

### Comparing `PyGPSClient-1.3.8/setup.py` & `PyGPSClient-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     name="PyGPSClient",
     version=VERSION,
     packages=find_namespace_packages(
         exclude=["tests", "references", "images", "docs", "examples"],
     ),
     install_requires=[
-        "pygnssutils>=0.3.1",
+        "pygnssutils>=0.3.2",
         "requests>=2.24.0",
         "Pillow>=7.2.0",
         "pyserial>=3.5",
     ],
     package_data={
         "pygpsclient": [
             "resources/*.gif",
```

