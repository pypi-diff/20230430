# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.0.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.1.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.0.tar` & `nonebot_plugin_l4d2_server-0.5.1.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0    35823 2023-04-04 06:17:31.531814 nonebot_plugin_l4d2_server-0.5.0/LICENSE
--rw-r--r--   0        0        0    17425 2023-04-28 09:27:53.056386 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     8845 2023-04-28 09:27:46.992526 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     8963 2023-04-28 09:13:46.843089 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-04-04 06:17:32.432688 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-04-04 06:17:32.439653 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-04-04 06:17:32.446667 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1650 2023-04-12 08:10:14.946997 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-04-04 06:17:32.518934 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2150 2023-04-04 06:17:32.520927 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6368 2023-04-24 08:33:07.861726 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6401 2023-04-12 08:10:14.949986 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1571 2023-04-12 08:10:14.951977 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5515 2023-04-24 06:29:14.906083 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-04-24 03:38:03.986578 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     8404 2023-04-04 06:17:32.837979 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-04-24 02:39:20.313753 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     8974 2023-04-28 08:08:47.505874 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1661 2023-04-04 06:17:32.842931 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3085 2023-04-04 06:17:33.045071 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1748 2023-04-20 00:42:41.559778 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      376 2023-04-04 06:17:33.049047 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3332 2023-04-04 06:17:34.075276 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      485 2023-04-04 06:17:34.076270 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0     3308 2023-04-04 06:17:34.078267 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1316 2023-04-04 06:17:34.082274 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4197 2023-04-04 06:17:35.069174 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1962 2023-04-20 02:34:31.279698 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     2947 2023-04-20 02:28:12.756210 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4139 2023-04-28 08:36:18.885635 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4097 2023-04-04 06:17:36.400628 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1070 2023-04-04 06:17:36.401631 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0      968 2023-04-04 06:17:36.402626 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3882 2023-04-12 08:10:14.955477 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1427 2023-04-04 06:17:36.739056 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3905 2023-04-25 06:48:18.748229 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1152 2023-04-27 01:31:26.318282 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0      788 2023-04-20 00:42:41.565761 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    11114 2023-04-28 08:28:21.116819 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1676 2023-04-04 06:17:36.802363 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0     1265 2023-04-28 08:24:33.893547 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1409 2023-04-04 06:17:36.926711 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     8776 2023-04-28 09:27:34.285127 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14389 2023-04-28 09:03:53.538976 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1678 2023-04-04 06:17:37.086862 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0     1025 2023-04-04 06:17:37.088855 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2197 2023-04-28 06:37:36.428815 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8307 2023-04-28 08:09:27.412377 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1522 2023-04-28 09:29:46.218925 nonebot_plugin_l4d2_server-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    11652 2023-04-23 03:26:29.286604 nonebot_plugin_l4d2_server-0.5.0/README.md
--rw-r--r--   0        0        0    13339 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-29 05:42:17.440730 nonebot_plugin_l4d2_server-0.5.1/LICENSE
+-rw-r--r--   0        0        0    17425 2023-04-30 18:53:43.450624 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1715 2023-04-30 18:16:08.781400 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/chrome.py
+-rw-r--r--   0        0        0     8851 2023-04-30 18:22:03.380711 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/command.py
+-rw-r--r--   0        0        0     6339 2023-04-30 18:16:10.020193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/config.py
+-rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1650 2023-04-09 15:09:05.585642 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6368 2023-04-25 12:33:57.826233 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6401 2023-04-09 15:09:04.937399 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1571 2023-04-09 15:08:29.280432 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5515 2023-04-25 12:33:57.876232 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-04-25 12:33:57.877232 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-04-25 12:33:58.077232 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     8974 2023-04-30 18:16:10.020193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1661 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3085 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1748 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      376 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3332 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0     3308 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1316 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4197 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1962 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     2751 2023-04-30 18:16:10.021193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4139 2023-04-30 18:16:10.021193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4097 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1070 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0      968 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3882 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1427 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3905 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1152 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1226 2023-04-30 18:16:10.022193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    11114 2023-04-30 18:16:10.022193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1676 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1265 2023-04-30 18:16:10.023193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1409 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     9369 2023-04-30 18:16:10.023193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14485 2023-04-30 18:16:10.024193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1678 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/message.py
+-rw-r--r--   0        0        0     1025 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/seach.py
+-rw-r--r--   0        0        0     2197 2023-04-30 18:16:10.025193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/txt_to_img.py
+-rw-r--r--   0        0        0     8307 2023-04-30 18:16:10.025193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/utils.py
+-rw-r--r--   0        0        0     1522 2023-04-30 18:53:34.072876 nonebot_plugin_l4d2_server-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    11188 2023-04-30 18:50:40.261224 nonebot_plugin_l4d2_server-0.5.1/README.md
+-rw-r--r--   0        0        0    13003 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.1/setup.py
+-rw-r--r--   0        0        0    12865 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.1/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.0/LICENSE` & `nonebot_plugin_l4d2_server-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 driver = get_driver()
 
 
-__version__ = "0.4.9"
+__version__ = "0.5.1"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
```

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/command.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,29 +26,28 @@
 # 服务器
 # last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
 
 
 
 def wenjian(
 event:NoticeEvent):
-    superuse = config_manager.config.l4_master
     args = event.dict()
     try:
         name: str = args['file']['name']
         usr_id = str(args['user_id'])
     except KeyError:
         return False
     if args['notice_type'] == 'offline_file':
-        if superuse:
-            return name.endswith(file_format) and usr_id in superuse
+        if l4_config.l4_master:
+            return name.endswith(file_format) and usr_id in l4_config.l4_master
         else:
             return name.endswith(file_format)
     elif args['notice_type'] == 'group_upload':
-        if superuse:
-            return usr_id in superuse and name.endswith(file_format)
+        if l4_config.l4_master:
+            return usr_id in l4_config.l4_master and name.endswith(file_format)
         else:
             return False
 
 up = on_notice(rule=wenjian)
 
 
 
@@ -122,19 +121,19 @@
 async def get_des_ip():
     global ALL_HOST
     global ANNE_IP
     global matchers
     if l4_config.l4_tag == None:
         pass
     else:
-        try:
-            qq = l4_config.l4_master[0]
-        except:
-            qq = list(nonebot.get_bot().config.superusers)[0]
-        ALL_HOST.update(await seach_map(msg = l4_config.l4_tag,qq = qq, key=l4_config.l4_key,mode='ip'))
+        # try:
+        #     qq = l4_config.l4_master[0]
+        # except:
+        #     qq = list(nonebot.get_bot().config.superusers)[0]
+        # ALL_HOST.update(await seach_map(msg = l4_config.l4_tag,qq = qq, key=l4_config.l4_key,mode='ip'))
         def count_ips(ip_dict:dict):
             global ANNE_IP
             for key, value in ip_dict.items():
                 if key in ['error_','success_']:
                     ip_dict.pop(key)
                     break
                 count = len(value)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files 19% similar despite different names*

```diff
@@ -57,10 +57,7 @@
     if mode == 'upload':
         await client.upload(local_path, remote_path)
     elif mode == 'read':
         file = await client.read(remote_path)
         return file
     elif mode == 'del':
         await client.delete(remote_path)
-
-if __name__ == '__main__':
-    asyncio.run(remote(mode='upload',host='106.13.207.45',user='root',password='Taojie@114514',local_path='E:\\zhang\\文件\\login_info.txt',remote_path='/home/'))
```

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 7% similar despite different names*

```diff
@@ -167,34 +167,48 @@
                 'msg':    '返回失败，请确保网络连接正常'
             }
 
     @app.get('/l4d2/api/get_l4d2_messages', response_class=JSONResponse, dependencies=[authentication()])
     async def get_l4d2_messages():
         try:
             l4_ipall = config_manager.config.l4_ipall
+<<<<<<< Updated upstream
+            server_list = []
+            config = config_manager.config.dict(exclude={'group_config'})
+            server_list.extend(
+                [{'label': f'{item["server_id"] or item["id_rank"]}({item["host"]})',
+                    'value': item['id_rank']}
+                    for item in l4_ipall])
+            config['server_list'] = server_list
+            return config
+=======
             config = [{'label': item['server_id'] , 'value': item['id_rank']}
                 for item in l4_ipall]
             return {
                 'status': 0,
                 'msg': 'ok',
                 'data': {'server_list':config}
             }
+>>>>>>> Stashed changes
         except ValueError:
             return {
                 'status': -100,
                 'msg':    '返回失败，请确保网络连接正常'
             }
     @app.get('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
     async def get_l4d2_server_config(id_rank :str):
         try:
             l4_ipall = config_manager.config.l4_ipall
             config = {}
             for item in l4_ipall:
                 if item['id_rank'] == id_rank :
+<<<<<<< Updated upstream
+=======
                     item['place'] = item['place'] == 'True' or item['place'] == True
+>>>>>>> Stashed changes
                     config = item
                     break
             return {
                 'status': 0,
                 'msg': 'ok',
                 'data': config
             }
@@ -202,14 +216,18 @@
             return {
                 'status': -100,
                 'msg':    '返回失败，请确保网络连接正常'
             }
         
     @app.post('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
     async def post_l4d2_server_config(id_rank :str,data: dict):
+<<<<<<< Updated upstream
+        print(data)
+=======
+>>>>>>> Stashed changes
         for one in config_manager.config.l4_ipall:
             if one['id_rank']==id_rank:
                 one.update(**data)
         config_manager.save()
         return {
             'status': 0,
             'msg':    '保存成功'
```

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,19 @@
 server_control = Select(label='服务器设置', name='id_rank', source='${server_list}',
                       placeholder='选择服务器')
 
 server_ditail= Form(
     title='',
     api='post:/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
     initApi='/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
+<<<<<<< Updated upstream
+    visibleOn='server_id != null',
+=======
     visibleOn='id_rank != null',
+>>>>>>> Stashed changes
     body=[
         Switch(label='是否是远程服务器', name='place', value='${place}', onText='是的', offText='不是',
                labelRemark=Remark(shape='circle',
                                   content='开启则确认为远程服务器')),
         InputText(label='服务器名称', name='server_id', value='${server_id}',
                   labelRemark=Remark(shape='circle',
                                      content='服务器名字')),
```

#### html2text {}

```diff
@@ -83,18 +83,19 @@
 ( label='ä¿å­è³ææç¾¤', level=LevelEnum.primary,
 confirmText='ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼', api='post:/l4d2/api/
 l4d2_group_config?group_id=all' ), Action(label='éç½®',
 level=LevelEnum.warning, type='reset')] ) server_control = Select
 (label='æå¡å¨è®¾ç½®', name='id_rank', source='${server_list}',
 placeholder='éæ©æå¡å¨') server_ditail= Form( title='', api='post:/l4d2/
 api/l4d2_server_config?id_rank=${id_rank}', initApi='/l4d2/api/
-l4d2_server_config?id_rank=${id_rank}', visibleOn='id_rank != null', body=
-[ Switch(label='æ¯å¦æ¯è¿ç¨æå¡å¨', name='place', value='${place}',
-onText='æ¯ç', offText='ä¸æ¯', labelRemark=Remark(shape='circle',
-content='å¼å¯åç¡®è®¤ä¸ºè¿ç¨æå¡å¨')), InputText
+l4d2_server_config?id_rank=${id_rank}', <<<<<<< Updated upstream
+visibleOn='server_id != null', ======= visibleOn='id_rank != null', >>>>>>>
+Stashed changes body=[ Switch(label='æ¯å¦æ¯è¿ç¨æå¡å¨', name='place',
+value='${place}', onText='æ¯ç', offText='ä¸æ¯', labelRemark=Remark
+(shape='circle', content='å¼å¯åç¡®è®¤ä¸ºè¿ç¨æå¡å¨')), InputText
 (label='æå¡å¨åç§°', name='server_id', value='${server_id}',
 labelRemark=Remark(shape='circle', content='æå¡å¨åå­')), InputText
 (label='æå¡å¨ipå°å', name='host', value='${host}', labelRemark=Remark
 (shape='circle', content='æå¡ç«¯æå¨ipå°å,ä¹å¯ä»¥æ¯åå')),
 InputText(label='æå¨ç«¯å£', name='port', value='${port}',
 labelRemark=Remark(shape='circle', content='æå¡ç«¯æå¨ç«¯å£')),
 InputPassword(label='rconæ§å¶å°å¯ç ', name='rcon', value='${rcon}',
```

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.0/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.0"
+version = "0.5.1"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.0/README.md` & `nonebot_plugin_l4d2_server-0.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,52 +30,47 @@
     <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
 </a>
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 
 </div>
 
-## 快速使用（env示例）
 
-    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
-    # 所有的多选，用逗号隔开
-    l4_master = ['1145149191']            # 允许上传地图的qq号
-    l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
-    l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
-    l4_port = ['20715']                   # 服务器端口
-    l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
-    l4_font = 'simsun.ttc'                # 服务器字体
-    l4_web = True                         # 网页控制台，默认是关闭
 
 ## 主要功能
 
 - 求生服务器-本地多路径操作（传地图）
 - 批量查询指定ip服务器状态和玩家
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
 
-## 如何获取key
 
-为了使得ip不被滥用，我采取这种方式管理。
+## 数据结构
 
-这并不影响正常使用，如果不需要可以忽略
-
-[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
-如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
-
-        l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
-        l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
-
-## 提交自己的服务器？
-
-__本项目原旨在方便自己查询管理服务器，如果你希望提供了ip__
-
-__那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip__
+bot所在文件夹下
+```txt
+举例：
+└── data
+    └── L4D2
+        ├── l4d2.yml
+        ├── l4d2.json
+        ├── sql
+        │   └── L4D2.db
+        ├── image
+        │   └── players
+        │       └── ...
+        └── l4d2
+            ├── 关键词1.json
+            ├── 关键词2.json
+            └── ...
+...
+```
 
 新增一个json文件，格式如下,文件名与需要响应的指令一致
+`l4d2.json`和`关键词1.json`都可以加载
 
         {
         "呆呆": [
                 {
                 "id": 1,
                 "version": "战役",
                 "ip": "43.248.188.17:27031"
@@ -86,35 +81,50 @@
                 "ip": "43.248.188.17:27032"
                 }
         ]
         }
 
 ## 🌐 默认服务器
 
-目前 __已授权__ 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
+由于不可抗力原因，暂时不使用在线的方式获取ip，有需求可以自行添加
+以下仅供参考本人使用的查询服务器
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
-| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4
-| 云 | anne电信服云服 | 东 | 27
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 5
+| 云 | anne电信服云服 | 东 | 19
 | 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
 | 橘 | 橘希实香的小窝 | 橘希实香 | 21
 | 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
 | 音理 | 星空列车与白的旅行 | 音理 | 3
 | 尤 | 尤尤 | 晓音 | 3
 | 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
-| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
+| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 2
 | Air | Air | Air | 15
 | 3ks | 为人民服务 | DK | 14
+| 驴头 | 驴头服 | lvt | 4
+| 尸鬼 | 尸鬼狂潮 | ❀几❀ | 7
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.5.1--2022.5.01
+
+- 解决了main和dev分支的一个严重bug（也许没解决
+- 本地化，更好的添加,删除远程分支
+- 服务器忘了备份，尽力抢救了数据了
+
+### 0.5.0--2022.4.28
+
+- 重构config，并弃用env设置
+- 使用网页控制台来控制配置
+- 新增了很多不会报错的bug
+
 ### 0.4.9--2022.4
 
 - 修复h11版本错误的bug
 - 重写了config，下个版本正式使用yaml替代env设置
 - 新增远程连接测试代码
 
 ### 0.4.8--2022.4.16
@@ -343,7 +353,8 @@
 - ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)
 - [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
   - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
 - [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
 - [日向麻麻](https://github.com/Special-Week)- 代码优化参考
 - [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考
 - 呆呆- 提供三方地图的详细数据
+- ArcPav -积极反馈bug，提供改进思路
```

#### html2text {}

```diff
@@ -1,53 +1,44 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
    # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
-## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼ #
-å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
-# ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] #
-åè®¸ä¸ä¼ å°å¾çqqå· l4_file = ['/home/ubuntu/l4d2/coop'] #
-æ¬å°æå¡å¨è·¯å¾ l4_host = ['127.0.0.1'] #
-æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼ l4_port = ['20715'] #
-æå¡å¨ç«¯å£ l4_rcon = ['1145149191810'] #
-æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´  l4_font =
-'simsun.ttc' # æå¡å¨å­ä½ l4_web = True #
-ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­ ## ä¸»è¦åè½ - æ±çæå¡å¨-
-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
+## ä¸»è¦åè½ - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php) ## å¦ä½è·åkey
-ä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã
-è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
-(https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
-å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
-l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
-l4_key = 'qwertyuiopasdfg' #
-è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ##
-æäº¤èªå·±çæå¡å¨ï¼
-__æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip__
-__é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip__
+ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt ä¸¾ä¾ï¼
+âââ data âââ L4D2 âââ l4d2.yml âââ l4d2.json âââ
+sql â âââ L4D2.db âââ image â âââ players â âââ
+... âââ l4d2 âââ å³é®è¯1.json âââ å³é®è¯2.json
+âââ ... ... ```
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
-{ "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" },
-{ "id": 2, "version": "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð
-é»è®¤æå¡å¨ ç®å __å·²ææ__
-çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
-æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
-ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 4 | äº | anneçµä¿¡æäºæ | ä¸ |
-27 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
-21 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³
-| 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
-ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
-| 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
-0.4.9--2022.4 - ä¿®å¤h11çæ¬éè¯¯çbug -
+`l4d2.json`å`å³é®è¯1.json`é½å¯ä»¥å è½½ { "åå": [ { "id": 1,
+"version": "æå½¹", "ip": "43.248.188.17:27031" }, { "id": 2, "version":
+"æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð é»è®¤æå¡å¨
+ç±äºä¸å¯æååå ï¼ææ¶ä¸ä½¿ç¨å¨çº¿çæ¹å¼è·åipï¼æéæ±å¯ä»¥èªè¡æ·»å 
+ä»¥ä¸ä»ä¾åèæ¬äººä½¿ç¨çæ¥è¯¢æå¡å¨ | æä»¤ | æå¡å¨ | op |
+æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  | ç±ä¸½æ°ç æ³è¦æ¶©æ¶© |
+ç±ä¸½æ°ç  | 5 | äº | anneçµä¿¡æäºæ | ä¸ | 19 | åå |
+ååçå°çª | æè«å¤§é­ç | 15 | æ© | æ©å¸å®é¦çå°çª |
+æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ | 21 | é³ç |
+æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ | 3 | é±¼ |
+é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ | ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿
+| å¤æå°æ | 2 | Air | Air | Air | 15 | 3ks | ä¸ºäººæ°æå¡ | DK | 14 |
+é©´å¤´ | é©´å¤´æ | lvt | 4 | å°¸é¬¼ | å°¸é¬¼çæ½® | âå â | 7 ## ð
+æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.5.1--2022.5.01 -
+è§£å³äºmainådevåæ¯çä¸ä¸ªä¸¥ébugï¼ä¹è®¸æ²¡è§£å³ -
+æ¬å°åï¼æ´å¥½çæ·»å ,å é¤è¿ç¨åæ¯ -
+æå¡å¨å¿äºå¤ä»½ï¼å°½åæ¢æäºæ°æ®äº ### 0.5.0--2022.4.28 -
+éæconfigï¼å¹¶å¼ç¨envè®¾ç½® - ä½¿ç¨ç½é¡µæ§å¶å°æ¥æ§å¶éç½® -
+æ°å¢äºå¾å¤ä¸ä¼æ¥éçbug ### 0.4.9--2022.4 -
+ä¿®å¤h11çæ¬éè¯¯çbug -
 éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½® -
 æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç  ### 0.4.8--2022.4.16 - æ°å¢éè½½ip -
 ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug ### 0.4.7--2022.4.13 -
 æ°å¢æ¨¡å¼æ¥è¯¢ - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯ ### 0.4.6--2022.4.9 -
 æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort()å¤©ä¸ç¬¬ä¸ï¼ -
 é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼ ### 0.4.2--2022.4.9 -
 ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
@@ -137,8 +128,9 @@
 [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://github.com/Agnes4m/VSQ)~~
 (å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq)-
 éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
 MeetWq/mybot)- æå¡å¨å¾çåè - [ç¾¤èå­¦ä¹ ](https://github.com/
 CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè -
 [æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè - [gsuid]
 (https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè -
-åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
+åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ® - ArcPav -
+ç§¯æåé¦bugï¼æä¾æ¹è¿æè·¯
```

### Comparing `nonebot_plugin_l4d2_server-0.5.0/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.0
+Version: 0.5.1
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -78,52 +78,47 @@
     <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
 </a>
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 
 </div>
 
-## 快速使用（env示例）
 
-    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
-    # 所有的多选，用逗号隔开
-    l4_master = ['1145149191']            # 允许上传地图的qq号
-    l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
-    l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
-    l4_port = ['20715']                   # 服务器端口
-    l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
-    l4_font = 'simsun.ttc'                # 服务器字体
-    l4_web = True                         # 网页控制台，默认是关闭
 
 ## 主要功能
 
 - 求生服务器-本地多路径操作（传地图）
 - 批量查询指定ip服务器状态和玩家
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
 
-## 如何获取key
 
-为了使得ip不被滥用，我采取这种方式管理。
+## 数据结构
 
-这并不影响正常使用，如果不需要可以忽略
-
-[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
-如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
-
-        l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
-        l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
-
-## 提交自己的服务器？
-
-__本项目原旨在方便自己查询管理服务器，如果你希望提供了ip__
-
-__那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip__
+bot所在文件夹下
+```txt
+举例：
+└── data
+    └── L4D2
+        ├── l4d2.yml
+        ├── l4d2.json
+        ├── sql
+        │   └── L4D2.db
+        ├── image
+        │   └── players
+        │       └── ...
+        └── l4d2
+            ├── 关键词1.json
+            ├── 关键词2.json
+            └── ...
+...
+```
 
 新增一个json文件，格式如下,文件名与需要响应的指令一致
+`l4d2.json`和`关键词1.json`都可以加载
 
         {
         "呆呆": [
                 {
                 "id": 1,
                 "version": "战役",
                 "ip": "43.248.188.17:27031"
@@ -134,35 +129,50 @@
                 "ip": "43.248.188.17:27032"
                 }
         ]
         }
 
 ## 🌐 默认服务器
 
-目前 __已授权__ 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
+由于不可抗力原因，暂时不使用在线的方式获取ip，有需求可以自行添加
+以下仅供参考本人使用的查询服务器
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
-| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4
-| 云 | anne电信服云服 | 东 | 27
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 5
+| 云 | anne电信服云服 | 东 | 19
 | 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
 | 橘 | 橘希实香的小窝 | 橘希实香 | 21
 | 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
 | 音理 | 星空列车与白的旅行 | 音理 | 3
 | 尤 | 尤尤 | 晓音 | 3
 | 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
-| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
+| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 2
 | Air | Air | Air | 15
 | 3ks | 为人民服务 | DK | 14
+| 驴头 | 驴头服 | lvt | 4
+| 尸鬼 | 尸鬼狂潮 | ❀几❀ | 7
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.5.1--2022.5.01
+
+- 解决了main和dev分支的一个严重bug（也许没解决
+- 本地化，更好的添加,删除远程分支
+- 服务器忘了备份，尽力抢救了数据了
+
+### 0.5.0--2022.4.28
+
+- 重构config，并弃用env设置
+- 使用网页控制台来控制配置
+- 新增了很多不会报错的bug
+
 ### 0.4.9--2022.4
 
 - 修复h11版本错误的bug
 - 重写了config，下个版本正式使用yaml替代env设置
 - 新增远程连接测试代码
 
 ### 0.4.8--2022.4.16
@@ -391,8 +401,8 @@
 - ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)
 - [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
   - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
 - [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
 - [日向麻麻](https://github.com/Special-Week)- 代码优化参考
 - [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考
 - 呆呆- 提供三方地图的详细数据
-
+- ArcPav -积极反馈bug，提供改进思路
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.1 Summary:
 L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -29,53 +29,44 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
    # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
-## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼ #
-å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
-# ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] #
-åè®¸ä¸ä¼ å°å¾çqqå· l4_file = ['/home/ubuntu/l4d2/coop'] #
-æ¬å°æå¡å¨è·¯å¾ l4_host = ['127.0.0.1'] #
-æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼ l4_port = ['20715'] #
-æå¡å¨ç«¯å£ l4_rcon = ['1145149191810'] #
-æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´  l4_font =
-'simsun.ttc' # æå¡å¨å­ä½ l4_web = True #
-ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­ ## ä¸»è¦åè½ - æ±çæå¡å¨-
-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
+## ä¸»è¦åè½ - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php) ## å¦ä½è·åkey
-ä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã
-è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
-(https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
-å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
-l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
-l4_key = 'qwertyuiopasdfg' #
-è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ##
-æäº¤èªå·±çæå¡å¨ï¼
-__æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip__
-__é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip__
+ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt ä¸¾ä¾ï¼
+âââ data âââ L4D2 âââ l4d2.yml âââ l4d2.json âââ
+sql â âââ L4D2.db âââ image â âââ players â âââ
+... âââ l4d2 âââ å³é®è¯1.json âââ å³é®è¯2.json
+âââ ... ... ```
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
-{ "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" },
-{ "id": 2, "version": "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð
-é»è®¤æå¡å¨ ç®å __å·²ææ__
-çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
-æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
-ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 4 | äº | anneçµä¿¡æäºæ | ä¸ |
-27 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
-21 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³
-| 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
-ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
-| 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
-0.4.9--2022.4 - ä¿®å¤h11çæ¬éè¯¯çbug -
+`l4d2.json`å`å³é®è¯1.json`é½å¯ä»¥å è½½ { "åå": [ { "id": 1,
+"version": "æå½¹", "ip": "43.248.188.17:27031" }, { "id": 2, "version":
+"æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð é»è®¤æå¡å¨
+ç±äºä¸å¯æååå ï¼ææ¶ä¸ä½¿ç¨å¨çº¿çæ¹å¼è·åipï¼æéæ±å¯ä»¥èªè¡æ·»å 
+ä»¥ä¸ä»ä¾åèæ¬äººä½¿ç¨çæ¥è¯¢æå¡å¨ | æä»¤ | æå¡å¨ | op |
+æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  | ç±ä¸½æ°ç æ³è¦æ¶©æ¶© |
+ç±ä¸½æ°ç  | 5 | äº | anneçµä¿¡æäºæ | ä¸ | 19 | åå |
+ååçå°çª | æè«å¤§é­ç | 15 | æ© | æ©å¸å®é¦çå°çª |
+æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ | 21 | é³ç |
+æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ | 3 | é±¼ |
+é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ | ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿
+| å¤æå°æ | 2 | Air | Air | Air | 15 | 3ks | ä¸ºäººæ°æå¡ | DK | 14 |
+é©´å¤´ | é©´å¤´æ | lvt | 4 | å°¸é¬¼ | å°¸é¬¼çæ½® | âå â | 7 ## ð
+æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.5.1--2022.5.01 -
+è§£å³äºmainådevåæ¯çä¸ä¸ªä¸¥ébugï¼ä¹è®¸æ²¡è§£å³ -
+æ¬å°åï¼æ´å¥½çæ·»å ,å é¤è¿ç¨åæ¯ -
+æå¡å¨å¿äºå¤ä»½ï¼å°½åæ¢æäºæ°æ®äº ### 0.5.0--2022.4.28 -
+éæconfigï¼å¹¶å¼ç¨envè®¾ç½® - ä½¿ç¨ç½é¡µæ§å¶å°æ¥æ§å¶éç½® -
+æ°å¢äºå¾å¤ä¸ä¼æ¥éçbug ### 0.4.9--2022.4 -
+ä¿®å¤h11çæ¬éè¯¯çbug -
 éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½® -
 æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç  ### 0.4.8--2022.4.16 - æ°å¢éè½½ip -
 ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug ### 0.4.7--2022.4.13 -
 æ°å¢æ¨¡å¼æ¥è¯¢ - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯ ### 0.4.6--2022.4.9 -
 æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort()å¤©ä¸ç¬¬ä¸ï¼ -
 é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼ ### 0.4.2--2022.4.9 -
 ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
@@ -165,8 +156,9 @@
 [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://github.com/Agnes4m/VSQ)~~
 (å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq)-
 éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
 MeetWq/mybot)- æå¡å¨å¾çåè - [ç¾¤èå­¦ä¹ ](https://github.com/
 CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè -
 [æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè - [gsuid]
 (https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè -
-åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
+åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ® - ArcPav -
+ç§¯æåé¦bugï¼æä¾æ¹è¿æè·¯
```

