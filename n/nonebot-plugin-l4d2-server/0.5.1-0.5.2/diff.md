# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.1.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.2.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.1.tar` & `nonebot_plugin_l4d2_server-0.5.2.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0    35823 2023-04-29 05:42:17.440730 nonebot_plugin_l4d2_server-0.5.1/LICENSE
--rw-r--r--   0        0        0    17425 2023-04-30 18:53:43.450624 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     1715 2023-04-30 18:16:08.781400 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/chrome.py
--rw-r--r--   0        0        0     8851 2023-04-30 18:22:03.380711 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     6339 2023-04-30 18:16:10.020193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1650 2023-04-09 15:09:05.585642 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6368 2023-04-25 12:33:57.826233 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6401 2023-04-09 15:09:04.937399 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1571 2023-04-09 15:08:29.280432 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5515 2023-04-25 12:33:57.876232 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-04-25 12:33:57.877232 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-04-25 12:33:58.077232 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     8974 2023-04-30 18:16:10.020193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1661 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3085 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1748 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      376 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3332 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      485 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0     3308 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1316 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4197 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1962 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     2751 2023-04-30 18:16:10.021193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4139 2023-04-30 18:16:10.021193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4097 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1070 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0      968 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3882 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1427 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3905 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1152 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1226 2023-04-30 18:16:10.022193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    11114 2023-04-30 18:16:10.022193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1676 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0     1265 2023-04-30 18:16:10.023193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1409 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     9369 2023-04-30 18:16:10.023193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14485 2023-04-30 18:16:10.024193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1678 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0     1025 2023-04-30 18:08:47.000000 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2197 2023-04-30 18:16:10.025193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8307 2023-04-30 18:16:10.025193 nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1522 2023-04-30 18:53:34.072876 nonebot_plugin_l4d2_server-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    11188 2023-04-30 18:50:40.261224 nonebot_plugin_l4d2_server-0.5.1/README.md
--rw-r--r--   0        0        0    13003 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.1/setup.py
--rw-r--r--   0        0        0    12865 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-30 19:40:30.775975 nonebot_plugin_l4d2_server-0.5.2/LICENSE
+-rw-r--r--   0        0        0    10994 2023-04-30 19:40:30.775975 nonebot_plugin_l4d2_server-0.5.2/README.md
+-rw-r--r--   0        0        0    17425 2023-04-30 19:40:30.779975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1671 2023-04-30 19:40:30.779975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/chrome.py
+-rw-r--r--   0        0        0     8619 2023-04-30 19:40:30.779975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/command.py
+-rw-r--r--   0        0        0     6129 2023-04-30 19:40:30.779975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/config.py
+-rw-r--r--   0        0        0   158357 2023-04-30 19:40:30.779975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     8723 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-04-30 19:40:30.783975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1683 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3241 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0     3221 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1284 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4075 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     2688 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4036 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     3996 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0      936 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3791 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1109 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10826 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1237 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     8542 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14148 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1620 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/message.py
+-rw-r--r--   0        0        0      992 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/seach.py
+-rw-r--r--   0        0        0     2133 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/txt_to_img.py
+-rw-r--r--   0        0        0     8035 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/utils.py
+-rw-r--r--   0        0        0     1470 2023-04-30 19:40:30.787975 nonebot_plugin_l4d2_server-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    13030 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.2/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/LICENSE` & `nonebot_plugin_l4d2_server-0.5.2/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 driver = get_driver()
 
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/chrome.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/chrome.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-try:
-    from selenium import webdriver
-    from selenium.webdriver.chrome.options import Options
-    from selenium.webdriver.common.by import By
-except:
-    pass
-url = 'https://server.trygek.com/index.php'
-
-
-def get_anne_server():
-    chrome_options = Options()  
-    chrome_options.add_argument('--no-sandbox') #“–no-sandbox”参数是让Chrome在root权限下跑
-    chrome_options.add_argument('--ignore-certificate-errors')
-    chrome_options.add_argument('--disable-dev-shm-usage')
-    chrome_options.add_argument('-ignore-certificate-errors')
-    chrome_options.add_argument('--headless') #“–headless”参数是不用打开图形界面  
-    driver = webdriver.Chrome(chrome_options=chrome_options) 
-    print('启动成功')
-    # browser.get(url)
-    # browser.add_cookie({'name':'token','value':token_value})
-    driver.get(url)
-    print('网页已打开，正在浏览')
-    i = 0
-    n = 1
-    msg = ''
-    while i <= 40:
-        try:
-            i += 1
-            mes =''
-            xpath1 = '//*[@id="host_{}"]'.format(i)
-            xpath2 = '/html/body/main/div[3]/div[5]/div/div/table/tbody/tr[{}]/td[5]'.format(n)
-            xpath3 = '//*[@id="players_{}"]'.format(i)
-            xpath4 = '//*[@id="map_{}"]'.format(i)
-            xpath = [xpath1,xpath2,xpath3,xpath4]
-            names = ['服务器名称','服务器ip','玩家','地图']
-            for x in range(5):
-                name:str = driver.find_element(By.XPATH,xpath[x-1]).text
-                mes += names[x-1] + '' + name + '\n'
-            msg += mes
-            msg += '--------------------\n'
-            n += 2
-        except :
-            continue
-    return msg
+try:
+    from selenium import webdriver
+    from selenium.webdriver.chrome.options import Options
+    from selenium.webdriver.common.by import By
+except:
+    pass
+url = 'https://server.trygek.com/index.php'
+
+
+def get_anne_server():
+    chrome_options = Options()  
+    chrome_options.add_argument('--no-sandbox') #“–no-sandbox”参数是让Chrome在root权限下跑
+    chrome_options.add_argument('--ignore-certificate-errors')
+    chrome_options.add_argument('--disable-dev-shm-usage')
+    chrome_options.add_argument('-ignore-certificate-errors')
+    chrome_options.add_argument('--headless') #“–headless”参数是不用打开图形界面  
+    driver = webdriver.Chrome(chrome_options=chrome_options) 
+    print('启动成功')
+    # browser.get(url)
+    # browser.add_cookie({'name':'token','value':token_value})
+    driver.get(url)
+    print('网页已打开，正在浏览')
+    i = 0
+    n = 1
+    msg = ''
+    while i <= 40:
+        try:
+            i += 1
+            mes =''
+            xpath1 = '//*[@id="host_{}"]'.format(i)
+            xpath2 = '/html/body/main/div[3]/div[5]/div/div/table/tbody/tr[{}]/td[5]'.format(n)
+            xpath3 = '//*[@id="players_{}"]'.format(i)
+            xpath4 = '//*[@id="map_{}"]'.format(i)
+            xpath = [xpath1,xpath2,xpath3,xpath4]
+            names = ['服务器名称','服务器ip','玩家','地图']
+            for x in range(5):
+                name:str = driver.find_element(By.XPATH,xpath[x-1]).text
+                mes += names[x-1] + '' + name + '\n'
+            msg += mes
+            msg += '--------------------\n'
+            n += 2
+        except :
+            continue
+    return msg
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/command.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/command.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-import re
-import asyncio
-from typing import Type
-from time import sleep
-
-from nonebot import on_notice,on_command,on_regex,on_keyword,MatcherGroup
-from nonebot.params import CommandArg,RawCommand,CommandStart
-from nonebot.matcher import Matcher
-import nonebot
-from nonebot.adapters.onebot.v11 import (
-    GroupUploadNoticeEvent,
-    NoticeEvent,
-    MessageEvent,
-    Message,
-    MessageSegment,
-    GroupMessageEvent,
-    )
-
-from .l4d2_anne.server import server_key,ANNE_IP
-from .config import *
-from .l4d2_queries.qqgroup import split_maohao
-# from .utils import qq_ip_queries_pic,json_server_to_tag_dict,get_anne_server_ip,get_tan_jian
-from .utils import *
-help_ = on_command('l4_help',aliases={'求生帮助'},priority=20,block=True)
-
-# 服务器
-# last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
-
-
-
-def wenjian(
-event:NoticeEvent):
-    args = event.dict()
-    try:
-        name: str = args['file']['name']
-        usr_id = str(args['user_id'])
-    except KeyError:
-        return False
-    if args['notice_type'] == 'offline_file':
-        if l4_config.l4_master:
-            return name.endswith(file_format) and usr_id in l4_config.l4_master
-        else:
-            return name.endswith(file_format)
-    elif args['notice_type'] == 'group_upload':
-        if l4_config.l4_master:
-            return usr_id in l4_config.l4_master and name.endswith(file_format)
-        else:
-            return False
-
-up = on_notice(rule=wenjian)
-
-
-
-rename_vpk = on_regex(
-        r"^求生地图\s*(\S+.*?)\s*(改|改名)?\s*(\S+.*?)\s*$",
-    flags=  re.S,
-    block= True,
-    priority= 20,
-    permission= Master,
-)
-
-find_vpk = on_command("l4_map",aliases={"求生地图","查看求生地图"},priority=25,block=True)
-del_vpk = on_command("l4_del_map",aliases={"求生地图删除","地图删除"},priority=20,block=True,permission= Master)
-rcon_to_server = on_command('rcon',aliases={"求生服务器指令","服务器指令","求生服务器控制台"},block=True,permission= Master)
-check_path = on_command('l4_check',aliases={'求生路径'},priority=20,block=True,permission= Master)
-smx_file = on_command('l4_smx',aliases={'求生插件'},priority=20,block=True,permission= Master)
-
-# anne
-anne_player = on_command('Ranne',aliases={"求生anne"},priority=25,block=True)
-anne_bind = on_command('Rbind',aliases={'steam绑定','求生绑定','anne绑定'},priority=20,block=True)
-del_bind = on_command('del_bind',aliases={'steam解绑','求生解绑','anne解绑'},priority=20,block=True)
-prison = on_command('zl',aliases={'坐牢'},priority=20,block=True)
-open_prison = on_command('kl',aliases={'开牢'},priority=20,block=True)
-
-# updata = on_command('updata',aliases={'求生更新'},priority=20,block=True,permission= Master)
-tan_jian = on_command('tj',aliases={'探监'},priority=20,block=True)
-
-# 查询
-queries = on_command('queries',aliases={'求生ip','求生IP'},priority=20,block=True)
-add_queries = on_command('addq',aliases={"求生添加订阅"},priority=20,block=True,permission= Master)
-del_queries = on_command('delq',aliases={"求生取消订阅"},priority=20,block=True,permission= Master)
-show_queries = on_command('showq',aliases={"求生订阅"},priority=20,block=True)
-join_server = on_command('ld_jr',aliases={"求生加入"},priority=20,block=True)
-connect_rcon = on_command("Rrcon", aliases={"求生连接", '求生链接','求生rcon'}, priority=50, block=False)
-end_connect = ['stop', '结束', '连接结束', '结束连接']
-search_api = on_command('search',aliases={'求生三方'}, priority=20, block=True,permission= Master)
-which_map = on_keyword(("是什么图"),priority=20, block=False)
-reload_ip = on_command('l4_reload',aliases={'重载ip'},priority=30,permission=Master)
-
-# 下载内容
-up_workshop = on_command('workshop',aliases={'创意工坊下载','求生创意工坊'},priority=20,block=True)
-vtf_make = on_command('vtf_make',aliases={'求生喷漆'},priority=20,block=True)
-
-@help_.handle()
-async def _():
-    msg = [
-        '=====求生机器人帮助=====',
-        '1、电信服战绩查询【求生anne[id/steamid/@]】',
-        '2、电信服绑定【求生绑定[id/steamid]】',
-        '3、电信服状态查询【云xx】'
-        '4、创意工坊下载【创意工坊下载[物品id/链接]】',
-        '5、指定ip查询【求生ip[ip]】(可以是域名)',
-        '6、求生喷漆制作【求生喷漆】',
-        '6、本地服务器操作(略，详情看项目地址)',
-    ]
-    messgae = ''
-    for i in msg:
-        messgae += i + '\n'
-    await help_.finish(messgae)
-
-def get_session_id(event: MessageEvent) -> str:
-    if isinstance(event, GroupMessageEvent):
-        return f"group_{event.group_id}"
-    else:
-        return f"private_{event.user_id}"
-
-matchers: Dict[str, List[Type[Matcher]]] = {}
-
-
-    
-async def get_des_ip():
-    global ALL_HOST
-    global ANNE_IP
-    global matchers
-    if l4_config.l4_tag == None:
-        pass
-    else:
-        # try:
-        #     qq = l4_config.l4_master[0]
-        # except:
-        #     qq = list(nonebot.get_bot().config.superusers)[0]
-        # ALL_HOST.update(await seach_map(msg = l4_config.l4_tag,qq = qq, key=l4_config.l4_key,mode='ip'))
-        def count_ips(ip_dict:dict):
-            global ANNE_IP
-            for key, value in ip_dict.items():
-                if key in ['error_','success_']:
-                    ip_dict.pop(key)
-                    break
-                count = len(value)
-                logger.info(f'已加载：{key} | {count}个')
-                if key == '云':
-                    ANNE_IP = {key:value}
-        sleep(1)
-        count_ips(ALL_HOST)
-        ip_anne_list=[] 
-        try:
-            ips = ALL_HOST['云']
-            ip_anne_list = []
-            for one_ip in ips:
-                host,port = split_maohao(one_ip['ip'])
-                ip_anne_list.append((one_ip['id'],host,port))
-        except KeyError:
-            pass
-    
-    
-    get_ip = on_command('anne',aliases=server_key(),priority=80,block=True)
-    @get_ip.handle()
-    async def _(matcher:Matcher,start:str = CommandStart(),command: str = RawCommand(),args:Message = CommandArg()):
-        global matchers
-        if get_ip.plugin_name not in matchers:
-            matchers[get_ip.plugin_name] = []
-        matchers[get_ip.plugin_name].append(get_ip)
-        if start:
-            command = command.replace(start,'')
-        if command == 'anne':
-            command = '云'
-        msg:str = args.extract_plain_text()
-        if not msg:
-            # 以图片输出全部当前
-            if command in gamemode_list:
-                this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
-                igr = True
-            else:
-                this_ips:list = ALL_HOST[command]
-                igr = False
-            if not this_ips:
-                matcher.finish('')
-            ip_list = []
-            for one_ip in this_ips:
-                host,port = split_maohao(one_ip['ip'])
-                ip_list.append((one_ip['id'],host,port))
-            img = await qq_ip_queries_pic(ip_list,igr)
-            if img:
-                await matcher.finish(MessageSegment.image(img)) 
-            else:
-                await matcher.finish("服务器无响应")
-        else:
-            if not msg[0].isdigit():
-                if any(mode in msg for mode in gamemode_list):
-                    pass
-                else:
-                    return
-            message = await json_server_to_tag_dict(command,msg)
-            if len(message) == 0:
-                # 关键词不匹配，忽略
-                return
-            ip = str(message['ip'])
-            logger.info(ip)
-            try:
-                msg= await get_anne_server_ip(ip)
-                await matcher.finish(msg)
-            except (OSError,asyncio.exceptions.TimeoutError):
-                await matcher.finish('服务器无响应')
-    
-           
-    @tan_jian.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
-        msg = await get_tan_jian(ip_anne_list,1)
-        await matcher.finish(msg)  
-        
-    @prison.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
-        msg = await get_tan_jian(ip_anne_list,2)
-        await matcher.finish(msg)
-
-    @open_prison.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
-
-        msg = await get_tan_jian(ip_anne_list,3)
-        await matcher.finish(msg)
-        
-    
-    
-async def init():
-    global matchers
-    # print('启动辣')
-    await get_des_ip()
-    
-   
-    
-@driver.on_bot_connect
-async def _():
+import re
+import asyncio
+from typing import Type
+from time import sleep
+
+from nonebot import on_notice,on_command,on_regex,on_keyword,MatcherGroup
+from nonebot.params import CommandArg,RawCommand,CommandStart
+from nonebot.matcher import Matcher
+import nonebot
+from nonebot.adapters.onebot.v11 import (
+    GroupUploadNoticeEvent,
+    NoticeEvent,
+    MessageEvent,
+    Message,
+    MessageSegment,
+    GroupMessageEvent,
+    )
+
+from .l4d2_anne.server import server_key,ANNE_IP
+from .config import *
+from .l4d2_queries.qqgroup import split_maohao
+# from .utils import qq_ip_queries_pic,json_server_to_tag_dict,get_anne_server_ip,get_tan_jian
+from .utils import *
+help_ = on_command('l4_help',aliases={'求生帮助'},priority=20,block=True)
+
+# 服务器
+# last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
+
+
+
+def wenjian(
+event:NoticeEvent):
+    args = event.dict()
+    try:
+        name: str = args['file']['name']
+        usr_id = str(args['user_id'])
+    except KeyError:
+        return False
+    if args['notice_type'] == 'offline_file':
+        if l4_config.l4_master:
+            return name.endswith(file_format) and usr_id in l4_config.l4_master
+        else:
+            return name.endswith(file_format)
+    elif args['notice_type'] == 'group_upload':
+        if l4_config.l4_master:
+            return usr_id in l4_config.l4_master and name.endswith(file_format)
+        else:
+            return False
+
+up = on_notice(rule=wenjian)
+
+
+
+rename_vpk = on_regex(
+        r"^求生地图\s*(\S+.*?)\s*(改|改名)?\s*(\S+.*?)\s*$",
+    flags=  re.S,
+    block= True,
+    priority= 20,
+    permission= Master,
+)
+
+find_vpk = on_command("l4_map",aliases={"求生地图","查看求生地图"},priority=25,block=True)
+del_vpk = on_command("l4_del_map",aliases={"求生地图删除","地图删除"},priority=20,block=True,permission= Master)
+rcon_to_server = on_command('rcon',aliases={"求生服务器指令","服务器指令","求生服务器控制台"},block=True,permission= Master)
+check_path = on_command('l4_check',aliases={'求生路径'},priority=20,block=True,permission= Master)
+smx_file = on_command('l4_smx',aliases={'求生插件'},priority=20,block=True,permission= Master)
+
+# anne
+anne_player = on_command('Ranne',aliases={"求生anne"},priority=25,block=True)
+anne_bind = on_command('Rbind',aliases={'steam绑定','求生绑定','anne绑定'},priority=20,block=True)
+del_bind = on_command('del_bind',aliases={'steam解绑','求生解绑','anne解绑'},priority=20,block=True)
+prison = on_command('zl',aliases={'坐牢'},priority=20,block=True)
+open_prison = on_command('kl',aliases={'开牢'},priority=20,block=True)
+
+# updata = on_command('updata',aliases={'求生更新'},priority=20,block=True,permission= Master)
+tan_jian = on_command('tj',aliases={'探监'},priority=20,block=True)
+
+# 查询
+queries = on_command('queries',aliases={'求生ip','求生IP'},priority=20,block=True)
+add_queries = on_command('addq',aliases={"求生添加订阅"},priority=20,block=True,permission= Master)
+del_queries = on_command('delq',aliases={"求生取消订阅"},priority=20,block=True,permission= Master)
+show_queries = on_command('showq',aliases={"求生订阅"},priority=20,block=True)
+join_server = on_command('ld_jr',aliases={"求生加入"},priority=20,block=True)
+connect_rcon = on_command("Rrcon", aliases={"求生连接", '求生链接','求生rcon'}, priority=50, block=False)
+end_connect = ['stop', '结束', '连接结束', '结束连接']
+search_api = on_command('search',aliases={'求生三方'}, priority=20, block=True,permission= Master)
+which_map = on_keyword(("是什么图"),priority=20, block=False)
+reload_ip = on_command('l4_reload',aliases={'重载ip'},priority=30,permission=Master)
+
+# 下载内容
+up_workshop = on_command('workshop',aliases={'创意工坊下载','求生创意工坊'},priority=20,block=True)
+vtf_make = on_command('vtf_make',aliases={'求生喷漆'},priority=20,block=True)
+
+@help_.handle()
+async def _():
+    msg = [
+        '=====求生机器人帮助=====',
+        '1、电信服战绩查询【求生anne[id/steamid/@]】',
+        '2、电信服绑定【求生绑定[id/steamid]】',
+        '3、电信服状态查询【云xx】'
+        '4、创意工坊下载【创意工坊下载[物品id/链接]】',
+        '5、指定ip查询【求生ip[ip]】(可以是域名)',
+        '6、求生喷漆制作【求生喷漆】',
+        '6、本地服务器操作(略，详情看项目地址)',
+    ]
+    messgae = ''
+    for i in msg:
+        messgae += i + '\n'
+    await help_.finish(messgae)
+
+def get_session_id(event: MessageEvent) -> str:
+    if isinstance(event, GroupMessageEvent):
+        return f"group_{event.group_id}"
+    else:
+        return f"private_{event.user_id}"
+
+matchers: Dict[str, List[Type[Matcher]]] = {}
+
+
+    
+async def get_des_ip():
+    global ALL_HOST
+    global ANNE_IP
+    global matchers
+    if l4_config.l4_tag == None:
+        pass
+    else:
+        # try:
+        #     qq = l4_config.l4_master[0]
+        # except:
+        #     qq = list(nonebot.get_bot().config.superusers)[0]
+        # ALL_HOST.update(await seach_map(msg = l4_config.l4_tag,qq = qq, key=l4_config.l4_key,mode='ip'))
+        def count_ips(ip_dict:dict):
+            global ANNE_IP
+            for key, value in ip_dict.items():
+                if key in ['error_','success_']:
+                    ip_dict.pop(key)
+                    break
+                count = len(value)
+                logger.info(f'已加载：{key} | {count}个')
+                if key == '云':
+                    ANNE_IP = {key:value}
+        sleep(1)
+        count_ips(ALL_HOST)
+        ip_anne_list=[] 
+        try:
+            ips = ALL_HOST['云']
+            ip_anne_list = []
+            for one_ip in ips:
+                host,port = split_maohao(one_ip['ip'])
+                ip_anne_list.append((one_ip['id'],host,port))
+        except KeyError:
+            pass
+    
+    
+    get_ip = on_command('anne',aliases=server_key(),priority=80,block=True)
+    @get_ip.handle()
+    async def _(matcher:Matcher,start:str = CommandStart(),command: str = RawCommand(),args:Message = CommandArg()):
+        global matchers
+        if get_ip.plugin_name not in matchers:
+            matchers[get_ip.plugin_name] = []
+        matchers[get_ip.plugin_name].append(get_ip)
+        if start:
+            command = command.replace(start,'')
+        if command == 'anne':
+            command = '云'
+        msg:str = args.extract_plain_text()
+        if not msg:
+            # 以图片输出全部当前
+            if command in gamemode_list:
+                this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
+                igr = True
+            else:
+                this_ips:list = ALL_HOST[command]
+                igr = False
+            if not this_ips:
+                matcher.finish('')
+            ip_list = []
+            for one_ip in this_ips:
+                host,port = split_maohao(one_ip['ip'])
+                ip_list.append((one_ip['id'],host,port))
+            img = await qq_ip_queries_pic(ip_list,igr)
+            if img:
+                await matcher.finish(MessageSegment.image(img)) 
+            else:
+                await matcher.finish("服务器无响应")
+        else:
+            if not msg[0].isdigit():
+                if any(mode in msg for mode in gamemode_list):
+                    pass
+                else:
+                    return
+            message = await json_server_to_tag_dict(command,msg)
+            if len(message) == 0:
+                # 关键词不匹配，忽略
+                return
+            ip = str(message['ip'])
+            logger.info(ip)
+            try:
+                msg= await get_anne_server_ip(ip)
+                await matcher.finish(msg)
+            except (OSError,asyncio.exceptions.TimeoutError):
+                await matcher.finish('服务器无响应')
+    
+           
+    @tan_jian.handle()
+    async def _(matcher:Matcher,event:MessageEvent):
+        msg = await get_tan_jian(ip_anne_list,1)
+        await matcher.finish(msg)  
+        
+    @prison.handle()
+    async def _(matcher:Matcher,event:MessageEvent):
+        msg = await get_tan_jian(ip_anne_list,2)
+        await matcher.finish(msg)
+
+    @open_prison.handle()
+    async def _(matcher:Matcher,event:MessageEvent):
+
+        msg = await get_tan_jian(ip_anne_list,3)
+        await matcher.finish(msg)
+        
+    
+    
+async def init():
+    global matchers
+    # print('启动辣')
+    await get_des_ip()
+    
+   
+    
+@driver.on_bot_connect
+async def _():
     await init()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/config.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/config.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-from pathlib import Path
-from typing import List,Dict,Union
-import ast
-import platform
-import os
-from ruamel import yaml
-from pydantic import Extra,BaseModel,Field
-try:
-    import ujson as json
-except:
-    import json
-
-from nonebot.permission import SUPERUSER
-from nonebot import get_driver
-from nonebot.log import logger
-from nonebot.adapters.onebot.v11.permission import (
-    GROUP_ADMIN,
-    GROUP_OWNER,
-    PRIVATE_FRIEND,
-)
-
-from .l4d2_queries.ohter import ALL_HOST    
-from .l4d2_queries.api import seach_map,map_dict_to_str
-file_format = (".vpk",".zip",".7z",'rar')
-# 权限
-
-driver = get_driver()
-COMMAND_START = list[driver.config.command_start]
-try:
-    NICKNAME: str = list(driver.config.nickname)[0]
-except Exception:
-    NICKNAME = 'bot'
-CHECK_FILE:int = 0
-
-
-reMaster = SUPERUSER | GROUP_OWNER 
-Master = SUPERUSER | GROUP_ADMIN | GROUP_OWNER 
-ADMINISTRATOR = SUPERUSER | GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND
-# file 填写求生服务器所在路径
-
-
-
-
-CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
-CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
-
-class L4d2GroupConfig(BaseModel):
-    enable: bool = Field(True, alias='是否启用求生功能')
-    map_master: List[str] = Field([], alias='分群地图管理员')
-
-    def update(self, **kwargs):
-        for key, value in kwargs.items():
-            if key in self.__fields__:
-                self.__setattr__(key, value)
-
-class L4d2Config(BaseModel):
-    total_enable: bool = Field(True, alias='是否全局启用求生功能')
-    map_path: List[str] = Field([], alias='求生地图路径')
-    web_username: str = Field('l4d2', alias='后台管理用户名')
-    web_password: str = Field('admin', alias='后台管理密码')
-    l4_style: str = Field("standard", alias='图片风格')
-    # l4_file: List[str] = Field(	["/home/ubuntu/l4d2/coop"], alias='本地求生服务器地址')
-    # l4_host: List[str] = Field(['127.0.0.1'], alias='求生服务器地址')
-    # l4_port: List[str] = Field(['20715'], alias='求生服务器端口')
-    # l4_rcon: List[str] = Field(['114514'], alias='求生服务器rcon密码')
-    
-    l4_ipall: List[Dict[str,Union[str,int,bool]]] = Field(
-        [{
-        'id_rank':'1',
-        'place': False,
-        'location':'C:\\l4d2',
-        'host':'127.0.0.1',
-        'port':'20715',
-        'rcon':'114514',
-        'server_id':'本地地图',
-        },{
-        'id_rank':'2',
-        'place': True,
-        'location':'/home/unbuntu/coop',
-        'host':'11.4.51.4',
-        'port':'20715',
-        'rcon':'9191810',
-        'account':'root',
-        'password':'114514',
-        'server_id':'远程地图',
-        }],
-          alias='l4服务器ip集合')
-    web_secret_key: str = Field('49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0',
-                                alias='后台管理token密钥')
-    l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
-    # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
-    l4_font: str = Field('simsun.ttc', alias='字体')
-    l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
-    l4_tag: List[str] = Field(['呆呆','橘'], alias='查服的名')
-    l4_key: str = Field('q1145149191810', alias='key')
-    group_config: Dict[int, L4d2GroupConfig] = Field({}, alias='分群配置')
-
-    def update(self, **kwargs):
-        for key, value in kwargs.items():
-            if key in self.__fields__:
-                self.__setattr__(key, value)
-                
-class L4d2ConfigManager:
-
-    def __init__(self):
-        self.file_path = CONFIG_PATH
-        if self.file_path.exists():
-            self.config = L4d2Config.parse_obj(
-                yaml.load(self.file_path.read_text(encoding='utf-8'), Loader=yaml.Loader))
-        else:
-            self.config = L4d2Config()
-        self.save()
-
-    def get_group_config(self, group_id: int) -> L4d2GroupConfig:
-        if group_id not in self.config.group_config:
-            self.config.group_config[group_id] = L4d2GroupConfig()
-            self.save()
-        return self.config.group_config[group_id]
-
-    @property
-    def config_list(self) -> List[str]:
-        return list(self.config.dict(by_alias=True).keys())
-
-    def save(self):
-        with self.file_path.open('w', encoding='utf-8') as f:
-            yaml.dump(
-                self.config.dict(by_alias=True),
-                f,
-                indent=2,
-                Dumper=yaml.RoundTripDumper,
-                allow_unicode=True)
-
-# 参数设置为全局变量
-global config_manager,l4_config            
-config_manager = L4d2ConfigManager()
-l4_config = config_manager.config
-
-class UserModel(BaseModel):
-    username: str
-    password: str
-
-     
-'''
-地图路径
-'''
-vpk_path = "left4dead2/addons"
-
-
-PLAYERSDATA = Path() / "data/L4D2/image/players"
-"""用户数据路径"""
-TEXT_PATH = Path(__file__).parent / 'data/L4D2/image'
-"""图片存储路径"""
-TEXT_XPATH = Path() / 'data/L4D2/image'
-"""内置图片路径"""
-
-
-
-PLAYERSDATA = Path() / "data/L4D2/sql"
-"""数据库路径"""
-DATASQLITE = Path().parent / "data/L4D2/sql/L4D2.db"
-"""数据库！"""  
-
-table_data = ["L4d2_players","L4D2_server"]
-"""数据库表"""
-L4d2_players_tag = ['qq', 'nickname', 'steamid']
-"""数据库表1"""
-L4d2_server_tag = ['id','qqgroup', 'host', 'port', 'rcon']
-"""数据库表2"""
-L4d2_INTEGER = ['id','qq','qqgroup','port']
-"""INITEGER的表头"""
-L4d2_TEXT = ['nickname','steamid','host','rcon','path']
-"""TEXT的表头"""
-L4d2_BOOLEAN = ['use']
-"""BOOLEAN的表头"""
-
-tables_columns = {
-    table_data[0]:L4d2_players_tag,
-    table_data[1]:L4d2_server_tag
-}
-
-# 求生anne服务器
-anne_url = "https://server.trygek.com/"
-
-gamemode_list = [
-    '纯净',
-    '魔改战役',
-    '多特',
-    '魔改多特',
-    '写专',
-    '对抗',
-    '魔改对抗',
-    '药役',
-    '药抗',
-    '包抗',
-    '绝境',
-    '死专',
-    'ast',
-    '清道夫',
-]
-
-# 系统
-if platform.system() == 'Windows':
-    systems:str = 'win'
-elif platform.system() == 'Linux':
-    systems:str = 'linux'
-else:
-    systems:str = 'others'
-ANNE_IP = {}
-
-
+from pathlib import Path
+from typing import List,Dict,Union
+import ast
+import platform
+import os
+from ruamel import yaml
+from pydantic import Extra,BaseModel,Field
+try:
+    import ujson as json
+except:
+    import json
+
+from nonebot.permission import SUPERUSER
+from nonebot import get_driver
+from nonebot.log import logger
+from nonebot.adapters.onebot.v11.permission import (
+    GROUP_ADMIN,
+    GROUP_OWNER,
+    PRIVATE_FRIEND,
+)
+
+from .l4d2_queries.ohter import ALL_HOST    
+from .l4d2_queries.api import seach_map,map_dict_to_str
+file_format = (".vpk",".zip",".7z",'rar')
+# 权限
+
+driver = get_driver()
+COMMAND_START = list[driver.config.command_start]
+try:
+    NICKNAME: str = list(driver.config.nickname)[0]
+except Exception:
+    NICKNAME = 'bot'
+CHECK_FILE:int = 0
+
+
+reMaster = SUPERUSER | GROUP_OWNER 
+Master = SUPERUSER | GROUP_ADMIN | GROUP_OWNER 
+ADMINISTRATOR = SUPERUSER | GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND
+# file 填写求生服务器所在路径
+
+
+
+
+CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
+CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
+
+class L4d2GroupConfig(BaseModel):
+    enable: bool = Field(True, alias='是否启用求生功能')
+    map_master: List[str] = Field([], alias='分群地图管理员')
+
+    def update(self, **kwargs):
+        for key, value in kwargs.items():
+            if key in self.__fields__:
+                self.__setattr__(key, value)
+
+class L4d2Config(BaseModel):
+    total_enable: bool = Field(True, alias='是否全局启用求生功能')
+    map_path: List[str] = Field([], alias='求生地图路径')
+    web_username: str = Field('l4d2', alias='后台管理用户名')
+    web_password: str = Field('admin', alias='后台管理密码')
+    l4_style: str = Field("standard", alias='图片风格')
+    # l4_file: List[str] = Field(	["/home/ubuntu/l4d2/coop"], alias='本地求生服务器地址')
+    # l4_host: List[str] = Field(['127.0.0.1'], alias='求生服务器地址')
+    # l4_port: List[str] = Field(['20715'], alias='求生服务器端口')
+    # l4_rcon: List[str] = Field(['114514'], alias='求生服务器rcon密码')
+    
+    l4_ipall: List[Dict[str,Union[str,int,bool]]] = Field(
+        [{
+        'id_rank':'1',
+        'place': False,
+        'location':'C:\\l4d2',
+        'host':'127.0.0.1',
+        'port':'20715',
+        'rcon':'114514',
+        'server_id':'本地地图',
+        },{
+        'id_rank':'2',
+        'place': True,
+        'location':'/home/unbuntu/coop',
+        'host':'11.4.51.4',
+        'port':'20715',
+        'rcon':'9191810',
+        'account':'root',
+        'password':'114514',
+        'server_id':'远程地图',
+        }],
+          alias='l4服务器ip集合')
+    web_secret_key: str = Field('49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0',
+                                alias='后台管理token密钥')
+    l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
+    # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
+    l4_font: str = Field('simsun.ttc', alias='字体')
+    l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
+    l4_tag: List[str] = Field(['呆呆','橘'], alias='查服的名')
+    l4_key: str = Field('q1145149191810', alias='key')
+    group_config: Dict[int, L4d2GroupConfig] = Field({}, alias='分群配置')
+
+    def update(self, **kwargs):
+        for key, value in kwargs.items():
+            if key in self.__fields__:
+                self.__setattr__(key, value)
+                
+class L4d2ConfigManager:
+
+    def __init__(self):
+        self.file_path = CONFIG_PATH
+        if self.file_path.exists():
+            self.config = L4d2Config.parse_obj(
+                yaml.load(self.file_path.read_text(encoding='utf-8'), Loader=yaml.Loader))
+        else:
+            self.config = L4d2Config()
+        self.save()
+
+    def get_group_config(self, group_id: int) -> L4d2GroupConfig:
+        if group_id not in self.config.group_config:
+            self.config.group_config[group_id] = L4d2GroupConfig()
+            self.save()
+        return self.config.group_config[group_id]
+
+    @property
+    def config_list(self) -> List[str]:
+        return list(self.config.dict(by_alias=True).keys())
+
+    def save(self):
+        with self.file_path.open('w', encoding='utf-8') as f:
+            yaml.dump(
+                self.config.dict(by_alias=True),
+                f,
+                indent=2,
+                Dumper=yaml.RoundTripDumper,
+                allow_unicode=True)
+
+# 参数设置为全局变量
+global config_manager,l4_config            
+config_manager = L4d2ConfigManager()
+l4_config = config_manager.config
+
+class UserModel(BaseModel):
+    username: str
+    password: str
+
+     
+'''
+地图路径
+'''
+vpk_path = "left4dead2/addons"
+
+
+PLAYERSDATA = Path() / "data/L4D2/image/players"
+"""用户数据路径"""
+TEXT_PATH = Path(__file__).parent / 'data/L4D2/image'
+"""图片存储路径"""
+TEXT_XPATH = Path() / 'data/L4D2/image'
+"""内置图片路径"""
+
+
+
+PLAYERSDATA = Path() / "data/L4D2/sql"
+"""数据库路径"""
+DATASQLITE = Path().parent / "data/L4D2/sql/L4D2.db"
+"""数据库！"""  
+
+table_data = ["L4d2_players","L4D2_server"]
+"""数据库表"""
+L4d2_players_tag = ['qq', 'nickname', 'steamid']
+"""数据库表1"""
+L4d2_server_tag = ['id','qqgroup', 'host', 'port', 'rcon']
+"""数据库表2"""
+L4d2_INTEGER = ['id','qq','qqgroup','port']
+"""INITEGER的表头"""
+L4d2_TEXT = ['nickname','steamid','host','rcon','path']
+"""TEXT的表头"""
+L4d2_BOOLEAN = ['use']
+"""BOOLEAN的表头"""
+
+tables_columns = {
+    table_data[0]:L4d2_players_tag,
+    table_data[1]:L4d2_server_tag
+}
+
+# 求生anne服务器
+anne_url = "https://server.trygek.com/"
+
+gamemode_list = [
+    '纯净',
+    '魔改战役',
+    '多特',
+    '魔改多特',
+    '写专',
+    '对抗',
+    '魔改对抗',
+    '药役',
+    '药抗',
+    '包抗',
+    '绝境',
+    '死专',
+    'ast',
+    '清道夫',
+]
+
+# 系统
+if platform.system() == 'Windows':
+    systems:str = 'win'
+elif platform.system() == 'Linux':
+    systems:str = 'linux'
+else:
+    systems:str = 'others'
+ANNE_IP = {}
+
+
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-<!DOCTYPE html>
-<head>
-	<link rel="stylesheet" type="text/css" href="vue.css">
-</head>
-</br>
-<body style="background-image: url('back.png'); background-size: cover;">
-	<font color="yellow">
-	{% for item in data %}
-	<h1 ><center>求生药役anne电信服数据</center></h1>
-	<div class="scissors" style="border-top:1px dashed orange;">
-	</div><h3><center>
-		{% for msg_one in item.one_msg %}
-			{{ msg_one }}<br>
-		{% endfor %}</center></h3>
-	</font>
-	<div class="scissors" style="border-top:1px dashed orange;">
-	</div>
-	<div class="myinfo">
-		<table class="transparent-bg">
-			<tbody>
-				<tr>
-					<td rowspan="6">
-						<img src={{item.header}}  width="200" height="200" style="border-radius: 50%;">
-					</td>
-					<td>昵&emsp;&emsp;称 | {{item.name}}</td>
-					<td>Steam id | {{item.Steam_ID}}</td>
-			</tr>
-			<tr>
-				<td>游玩时间 | {{item.play_time}}</td>
-				<td>最后上线 | {{item.last_online}}</td>
-			</tr>
-			<tr>
-				<td>排&emsp;&emsp;行 | {{item.rank}}</td>
-				
-				<td>分&emsp;&emsp;数 | {{item.points}}</td>
-			</tr>
-			<tr>
-				<td>分数 / 分 | {{item.point_min}}</td>
-				<td>小僵尸数 | {{item.killed}}</td>
-			</tr>
-			<tr>
-				<td>爆&emsp;&emsp;头 | {{item.shut}}</td>
-				<td>爆&nbsp; 头&nbsp; 率 | {{item.out}}</td>
-			</tr>
-			<tr>
-				<td>游玩次数 | {{item.playtimes}}</td>
-				<td>救&nbsp; 援&nbsp; 关 | {{item.last_one}}</td>
-			</tr>
-		</tbody>
-	</table>
-</div>
-<font color="yellow">
-{% endfor %}
-<h5><center>©爱丽数码</center></br>
-	<center>
-		github.com/Agnes4m/nonebot_plugin_l4d2_server
-	</center>
-</h5>
-</font>
-</body>
+<!DOCTYPE html>
+<head>
+	<link rel="stylesheet" type="text/css" href="vue.css">
+</head>
+</br>
+<body style="background-image: url('back.png'); background-size: cover;">
+	<font color="yellow">
+	{% for item in data %}
+	<h1 ><center>求生药役anne电信服数据</center></h1>
+	<div class="scissors" style="border-top:1px dashed orange;">
+	</div><h3><center>
+		{% for msg_one in item.one_msg %}
+			{{ msg_one }}<br>
+		{% endfor %}</center></h3>
+	</font>
+	<div class="scissors" style="border-top:1px dashed orange;">
+	</div>
+	<div class="myinfo">
+		<table class="transparent-bg">
+			<tbody>
+				<tr>
+					<td rowspan="6">
+						<img src={{item.header}}  width="200" height="200" style="border-radius: 50%;">
+					</td>
+					<td>昵&emsp;&emsp;称 | {{item.name}}</td>
+					<td>Steam id | {{item.Steam_ID}}</td>
+			</tr>
+			<tr>
+				<td>游玩时间 | {{item.play_time}}</td>
+				<td>最后上线 | {{item.last_online}}</td>
+			</tr>
+			<tr>
+				<td>排&emsp;&emsp;行 | {{item.rank}}</td>
+				
+				<td>分&emsp;&emsp;数 | {{item.points}}</td>
+			</tr>
+			<tr>
+				<td>分数 / 分 | {{item.point_min}}</td>
+				<td>小僵尸数 | {{item.killed}}</td>
+			</tr>
+			<tr>
+				<td>爆&emsp;&emsp;头 | {{item.shut}}</td>
+				<td>爆&nbsp; 头&nbsp; 率 | {{item.out}}</td>
+			</tr>
+			<tr>
+				<td>游玩次数 | {{item.playtimes}}</td>
+				<td>救&nbsp; 援&nbsp; 关 | {{item.last_one}}</td>
+			</tr>
+		</tbody>
+	</table>
+</div>
+<font color="yellow">
+{% endfor %}
+<h5><center>©爱丽数码</center></br>
+	<center>
+		github.com/Agnes4m/nonebot_plugin_l4d2_server
+	</center>
+</h5>
+</font>
+</body>
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files 5% similar despite different names*

```diff
@@ -1,135 +1,134 @@
-00000000: 3c73 7667 0d0a 2020 6172 6961 2d68 6964  <svg..  aria-hid
-00000010: 6465 6e3d 2274 7275 6522 0d0a 2020 666f  den="true"..  fo
-00000020: 6375 7361 626c 653d 2266 616c 7365 220d  cusable="false".
-00000030: 0a20 2064 6174 612d 7072 6566 6978 3d22  .  data-prefix="
-00000040: 6661 7322 0d0a 2020 6461 7461 2d69 636f  fas"..  data-ico
-00000050: 6e3d 2266 696e 6765 7270 7269 6e74 220d  n="fingerprint".
-00000060: 0a20 2063 6c61 7373 3d22 7376 672d 696e  .  class="svg-in
-00000070: 6c69 6e65 2d2d 6661 2066 612d 6669 6e67  line--fa fa-fing
-00000080: 6572 7072 696e 7420 6d72 2d32 220d 0a20  erprint mr-2".. 
-00000090: 2072 6f6c 653d 2269 6d67 220d 0a20 2078   role="img"..  x
-000000a0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
-000000b0: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-000000c0: 220d 0a20 2076 6965 7742 6f78 3d22 3020  "..  viewBox="0 
-000000d0: 3020 3531 3220 3531 3222 0d0a 3e0d 0a20  0 512 512"..>.. 
-000000e0: 203c 7061 7468 0d0a 2020 2020 6669 6c6c   <path..    fill
-000000f0: 3d22 6375 7272 656e 7443 6f6c 6f72 220d  ="currentColor".
-00000100: 0a20 2020 2064 3d22 4d32 3536 2e31 3220  .    d="M256.12 
-00000110: 3234 352e 3936 632d 3133 2e32 3520 302d  245.96c-13.25 0-
-00000120: 3234 2031 302e 3734 2d32 3420 3234 2031  24 10.74-24 24 1
-00000130: 2e31 3420 3732 2e32 352d 382e 3134 2031  .14 72.25-8.14 1
-00000140: 3431 2e39 2d32 372e 3720 3231 312e 3535  41.9-27.7 211.55
-00000150: 2d32 2e37 3320 392e 3732 2032 2e31 3520  -2.73 9.72 2.15 
-00000160: 3330 2e34 3920 3233 2e31 3220 3330 2e34  30.49 23.12 30.4
-00000170: 3920 3130 2e34 3820 3020 3230 2e31 312d  9 10.48 0 20.11-
-00000180: 362e 3932 2032 332e 3039 2d31 372e 3532  6.92 23.09-17.52
-00000190: 2031 332e 3533 2d34 372e 3931 2033 312e   13.53-47.91 31.
-000001a0: 3034 2d31 3235 2e34 3120 3239 2e34 382d  04-125.41 29.48-
-000001b0: 3232 342e 3532 2e30 312d 3133 2e32 352d  224.52.01-13.25-
-000001c0: 3130 2e37 332d 3234 2d32 332e 3939 2d32  10.73-24-23.99-2
-000001d0: 347a 6d2d 2e38 362d 3831 2e37 3343 3139  4zm-.86-81.73C19
-000001e0: 3420 3136 342e 3136 2031 3531 2e32 3520  4 164.16 151.25 
-000001f0: 3231 312e 3320 3135 322e 3120 3236 352e  211.3 152.1 265.
-00000200: 3332 632e 3735 2034 372e 3934 2d33 2e37  32c.75 47.94-3.7
-00000210: 3520 3935 2e39 312d 3133 2e33 3720 3134  5 95.91-13.37 14
-00000220: 322e 3535 2d32 2e36 3920 3132 2e39 3820  2.55-2.69 12.98 
-00000230: 352e 3637 2032 352e 3639 2031 382e 3634  5.67 25.69 18.64
-00000240: 2032 382e 3336 2031 332e 3035 2032 2e36   28.36 13.05 2.6
-00000250: 3720 3235 2e36 372d 352e 3636 2032 382e  7 25.67-5.66 28.
-00000260: 3336 2d31 382e 3634 2031 302e 3334 2d35  36-18.64 10.34-5
-00000270: 302e 3039 2031 352e 3137 2d31 3031 2e35  0.09 15.17-101.5
-00000280: 3820 3134 2e33 372d 3135 332e 3032 2d2e  8 14.37-153.02-.
-00000290: 3431 2d32 352e 3935 2031 392e 3932 2d35  41-25.95 19.92-5
-000002a0: 322e 3439 2035 342e 3435 2d35 322e 3334  2.49 54.45-52.34
-000002b0: 2033 312e 3331 2e34 3720 3537 2e31 3520   31.31.47 57.15 
-000002c0: 3235 2e33 3420 3537 2e36 3220 3535 2e34  25.34 57.62 55.4
-000002d0: 372e 3737 2034 382e 3035 2d32 2e38 3120  7.77 48.05-2.81 
-000002e0: 3936 2e33 332d 3130 2e36 3120 3134 332e  96.33-10.61 143.
-000002f0: 3535 2d32 2e31 3720 3133 2e30 3620 362e  55-2.17 13.06 6.
-00000300: 3639 2032 352e 3432 2031 392e 3736 2032  69 25.42 19.76 2
-00000310: 372e 3538 2031 392e 3937 2033 2e33 3320  7.58 19.97 3.33 
-00000320: 3236 2e38 312d 3135 2e31 2032 372e 3538  26.81-15.1 27.58
-00000330: 2d31 392e 3737 2038 2e32 382d 3530 2e30  -19.77 8.28-50.0
-00000340: 3320 3132 2e30 362d 3130 312e 3231 2031  3 12.06-101.21 1
-00000350: 312e 3237 2d31 3532 2e31 312d 2e38 382d  1.27-152.11-.88-
-00000360: 3535 2e38 2d34 372e 3934 2d31 3031 2e38  55.8-47.94-101.8
-00000370: 382d 3130 342e 3931 2d31 3032 2e37 327a  8-104.91-102.72z
-00000380: 6d2d 3131 302e 3639 2d31 392e 3738 632d  m-110.69-19.78c-
-00000390: 3130 2e33 2d38 2e33 342d 3235 2e33 372d  10.3-8.34-25.37-
-000003a0: 362e 382d 3333 2e37 3620 332e 3438 2d32  6.8-33.76 3.48-2
-000003b0: 352e 3632 2033 312e 352d 3339 2e33 3920  5.62 31.5-39.39 
-000003c0: 3731 2e32 382d 3338 2e37 3520 3131 3220  71.28-38.75 112 
-000003d0: 2e35 3920 3337 2e35 382d 322e 3437 2037  .59 37.58-2.47 7
-000003e0: 352e 3237 2d39 2e31 3120 3131 322e 3035  5.27-9.11 112.05
-000003f0: 2d32 2e33 3420 3133 2e30 3520 362e 3331  -2.34 13.05 6.31
-00000400: 2032 352e 3533 2031 392e 3336 2032 372e   25.53 19.36 27.
-00000410: 3839 2032 302e 3131 2033 2e35 2032 372e  89 20.11 3.5 27.
-00000420: 3037 2d31 342e 3831 2032 372e 3839 2d31  07-14.81 27.89-1
-00000430: 392e 3336 2037 2e31 392d 3339 2e38 3420  9.36 7.19-39.84 
-00000440: 3130 2e35 2d38 302e 3636 2039 2e38 362d  10.5-80.66 9.86-
-00000450: 3132 312e 3333 2d2e 3437 2d32 392e 3838  121.33-.47-29.88
-00000460: 2039 2e32 2d35 372e 3838 2032 382d 3830   9.2-57.88 28-80
-00000470: 2e39 3720 382e 3335 2d31 302e 3238 2036  .97 8.35-10.28 6
-00000480: 2e37 392d 3235 2e33 392d 332e 3439 2d33  .79-25.39-3.49-3
-00000490: 332e 3736 7a6d 3130 392e 3437 2d36 322e  3.76zm109.47-62.
-000004a0: 3333 632d 3135 2e34 312d 2e34 312d 3330  33c-15.41-.41-30
-000004b0: 2e38 3720 312e 3434 2d34 352e 3738 2034  .87 1.44-45.78 4
-000004c0: 2e39 372d 3132 2e38 3920 332e 3036 2d32  .97-12.89 3.06-2
-000004d0: 302e 3837 2031 352e 3938 2d31 372e 3833  0.87 15.98-17.83
-000004e0: 2032 382e 3839 2033 2e30 3620 3132 2e38   28.89 3.06 12.8
-000004f0: 3920 3136 2032 302e 3833 2032 382e 3839  9 16 20.83 28.89
-00000500: 2031 372e 3833 2031 312e 3035 2d32 2e36   17.83 11.05-2.6
-00000510: 3120 3232 2e34 372d 332e 3737 2033 342d  1 22.47-3.77 34-
-00000520: 332e 3639 2037 352e 3433 2031 2e31 3320  3.69 75.43 1.13 
-00000530: 3133 372e 3733 2036 312e 3520 3133 382e  137.73 61.5 138.
-00000540: 3838 2031 3334 2e35 382e 3539 2033 372e  88 134.58.59 37.
-00000550: 3838 2d31 2e32 3820 3736 2e31 312d 352e  88-1.28 76.11-5.
-00000560: 3538 2031 3133 2e36 332d 312e 3520 3133  58 113.63-1.5 13
-00000570: 2e31 3720 372e 3935 2032 352e 3038 2032  .17 7.95 25.08 2
-00000580: 312e 3131 2032 362e 3538 2031 362e 3732  1.11 26.58 16.72
-00000590: 2031 2e39 3520 3235 2e35 312d 3131 2e38   1.95 25.51-11.8
-000005a0: 3820 3236 2e35 382d 3231 2e31 3161 3932  8 26.58-21.11a92
-000005b0: 392e 3036 2039 3239 2e30 3620 3020 3020  9.06 929.06 0 0 
-000005c0: 3020 352e 3839 2d31 3139 2e38 3563 2d31  0 5.89-119.85c-1
-000005d0: 2e35 362d 3938 2e37 352d 3835 2e30 372d  .56-98.75-85.07-
-000005e0: 3138 302e 3333 2d31 3836 2e31 362d 3138  180.33-186.16-18
-000005f0: 312e 3833 7a6d 3235 322e 3037 2031 3231  1.83zm252.07 121
-00000600: 2e34 3563 2d32 2e38 362d 3132 2e39 322d  .45c-2.86-12.92-
-00000610: 3135 2e35 312d 3231 2e32 2d32 382e 3631  15.51-21.2-28.61
-00000620: 2d31 382e 3237 2d31 322e 3934 2032 2e38  -18.27-12.94 2.8
-00000630: 362d 3231 2e31 3220 3135 2e36 362d 3138  6-21.12 15.66-18
-00000640: 2e32 3620 3238 2e36 3120 342e 3731 2032  .26 28.61 4.71 2
-00000650: 312e 3431 2034 2e39 3120 3337 2e34 3120  1.41 4.91 37.41 
-00000660: 342e 3720 3631 2e36 2d2e 3131 2031 332e  4.7 61.6-.11 13.
-00000670: 3237 2031 302e 3535 2032 342e 3039 2032  27 10.55 24.09 2
-00000680: 332e 3820 3234 2e32 682e 3263 3133 2e31  3.8 24.2h.2c13.1
-00000690: 3720 3020 3233 2e38 392d 3130 2e36 3120  7 0 23.89-10.61 
-000006a0: 3234 2d32 332e 382e 3138 2d32 322e 3138  24-23.8.18-22.18
-000006b0: 2e34 2d34 342e 3131 2d35 2e38 332d 3732  .4-44.11-5.83-72
-000006c0: 2e33 347a 6d2d 3430 2e31 322d 3930 2e37  .34zm-40.12-90.7
-000006d0: 3243 3431 372e 3239 2034 332e 3436 2033  2C417.29 43.46 3
-000006e0: 3337 2e36 2031 2e32 3920 3235 322e 3831  37.6 1.29 252.81
-000006f0: 2e30 3220 3138 332e 3032 2d2e 3832 2031  .02 183.02-.82 1
-00000700: 3138 2e34 3720 3234 2e39 3120 3730 2e34  18.47 24.91 70.4
-00000710: 3620 3732 2e39 3420 3234 2e30 3920 3131  6 72.94 24.09 11
-00000720: 392e 3337 2d2e 3920 3138 312e 3034 2e31  9.37-.9 181.04.1
-00000730: 3420 3234 362e 3635 6c2d 2e31 3220 3231  4 246.65l-.12 21
-00000740: 2e34 3763 2d2e 3339 2031 332e 3235 2031  .47c-.39 13.25 1
-00000750: 302e 3033 2032 342e 3331 2032 332e 3238  0.03 24.31 23.28
-00000760: 2032 342e 3639 2e32 332e 3032 2e34 382e   24.69.23.02.48.
-00000770: 3032 2e37 322e 3032 2031 322e 3932 2030  02.72.02 12.92 0
-00000780: 2032 332e 3539 2d31 302e 3320 3233 2e39   23.59-10.3 23.9
-00000790: 372d 3233 2e33 6c2e 3136 2d32 332e 3634  7-23.3l.16-23.64
-000007a0: 632d 2e38 332d 3532 2e35 2031 392e 3136  c-.83-52.5 19.16
-000007b0: 2d31 3031 2e38 3620 3536 2e32 382d 3133  -101.86 56.28-13
-000007c0: 3920 3338 2e37 362d 3338 2e38 2039 312e  9 38.76-38.8 91.
-000007d0: 3334 2d35 392e 3637 2031 3437 2e36 382d  34-59.67 147.68-
-000007e0: 3538 2e38 3620 3639 2e34 3520 312e 3033  58.86 69.45 1.03
-000007f0: 2031 3334 2e37 3320 3335 2e35 3620 3137   134.73 35.56 17
-00000800: 342e 3632 2039 322e 3339 2037 2e36 3120  4.62 92.39 7.61 
-00000810: 3130 2e38 3620 3232 2e35 3620 3133 2e34  10.86 22.56 13.4
-00000820: 3520 3333 2e34 3220 352e 3836 2031 302e  5 33.42 5.86 10.
-00000830: 3834 2d37 2e36 3220 3133 2e34 362d 3232  84-7.62 13.46-22
-00000840: 2e35 3920 352e 3834 2d33 332e 3433 7a22  .59 5.84-33.43z"
-00000850: 0d0a 2020 3e3c 2f70 6174 683e 0d0a 3c2f  ..  ></path>..</
-00000860: 7376 673e 0d0a                           svg>..
+00000000: 3c73 7667 0a20 2061 7269 612d 6869 6464  <svg.  aria-hidd
+00000010: 656e 3d22 7472 7565 220a 2020 666f 6375  en="true".  focu
+00000020: 7361 626c 653d 2266 616c 7365 220a 2020  sable="false".  
+00000030: 6461 7461 2d70 7265 6669 783d 2266 6173  data-prefix="fas
+00000040: 220a 2020 6461 7461 2d69 636f 6e3d 2266  ".  data-icon="f
+00000050: 696e 6765 7270 7269 6e74 220a 2020 636c  ingerprint".  cl
+00000060: 6173 733d 2273 7667 2d69 6e6c 696e 652d  ass="svg-inline-
+00000070: 2d66 6120 6661 2d66 696e 6765 7270 7269  -fa fa-fingerpri
+00000080: 6e74 206d 722d 3222 0a20 2072 6f6c 653d  nt mr-2".  role=
+00000090: 2269 6d67 220a 2020 786d 6c6e 733d 2268  "img".  xmlns="h
+000000a0: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+000000b0: 2f32 3030 302f 7376 6722 0a20 2076 6965  /2000/svg".  vie
+000000c0: 7742 6f78 3d22 3020 3020 3531 3220 3531  wBox="0 0 512 51
+000000d0: 3222 0a3e 0a20 203c 7061 7468 0a20 2020  2".>.  <path.   
+000000e0: 2066 696c 6c3d 2263 7572 7265 6e74 436f   fill="currentCo
+000000f0: 6c6f 7222 0a20 2020 2064 3d22 4d32 3536  lor".    d="M256
+00000100: 2e31 3220 3234 352e 3936 632d 3133 2e32  .12 245.96c-13.2
+00000110: 3520 302d 3234 2031 302e 3734 2d32 3420  5 0-24 10.74-24 
+00000120: 3234 2031 2e31 3420 3732 2e32 352d 382e  24 1.14 72.25-8.
+00000130: 3134 2031 3431 2e39 2d32 372e 3720 3231  14 141.9-27.7 21
+00000140: 312e 3535 2d32 2e37 3320 392e 3732 2032  1.55-2.73 9.72 2
+00000150: 2e31 3520 3330 2e34 3920 3233 2e31 3220  .15 30.49 23.12 
+00000160: 3330 2e34 3920 3130 2e34 3820 3020 3230  30.49 10.48 0 20
+00000170: 2e31 312d 362e 3932 2032 332e 3039 2d31  .11-6.92 23.09-1
+00000180: 372e 3532 2031 332e 3533 2d34 372e 3931  7.52 13.53-47.91
+00000190: 2033 312e 3034 2d31 3235 2e34 3120 3239   31.04-125.41 29
+000001a0: 2e34 382d 3232 342e 3532 2e30 312d 3133  .48-224.52.01-13
+000001b0: 2e32 352d 3130 2e37 332d 3234 2d32 332e  .25-10.73-24-23.
+000001c0: 3939 2d32 347a 6d2d 2e38 362d 3831 2e37  99-24zm-.86-81.7
+000001d0: 3343 3139 3420 3136 342e 3136 2031 3531  3C194 164.16 151
+000001e0: 2e32 3520 3231 312e 3320 3135 322e 3120  .25 211.3 152.1 
+000001f0: 3236 352e 3332 632e 3735 2034 372e 3934  265.32c.75 47.94
+00000200: 2d33 2e37 3520 3935 2e39 312d 3133 2e33  -3.75 95.91-13.3
+00000210: 3720 3134 322e 3535 2d32 2e36 3920 3132  7 142.55-2.69 12
+00000220: 2e39 3820 352e 3637 2032 352e 3639 2031  .98 5.67 25.69 1
+00000230: 382e 3634 2032 382e 3336 2031 332e 3035  8.64 28.36 13.05
+00000240: 2032 2e36 3720 3235 2e36 372d 352e 3636   2.67 25.67-5.66
+00000250: 2032 382e 3336 2d31 382e 3634 2031 302e   28.36-18.64 10.
+00000260: 3334 2d35 302e 3039 2031 352e 3137 2d31  34-50.09 15.17-1
+00000270: 3031 2e35 3820 3134 2e33 372d 3135 332e  01.58 14.37-153.
+00000280: 3032 2d2e 3431 2d32 352e 3935 2031 392e  02-.41-25.95 19.
+00000290: 3932 2d35 322e 3439 2035 342e 3435 2d35  92-52.49 54.45-5
+000002a0: 322e 3334 2033 312e 3331 2e34 3720 3537  2.34 31.31.47 57
+000002b0: 2e31 3520 3235 2e33 3420 3537 2e36 3220  .15 25.34 57.62 
+000002c0: 3535 2e34 372e 3737 2034 382e 3035 2d32  55.47.77 48.05-2
+000002d0: 2e38 3120 3936 2e33 332d 3130 2e36 3120  .81 96.33-10.61 
+000002e0: 3134 332e 3535 2d32 2e31 3720 3133 2e30  143.55-2.17 13.0
+000002f0: 3620 362e 3639 2032 352e 3432 2031 392e  6 6.69 25.42 19.
+00000300: 3736 2032 372e 3538 2031 392e 3937 2033  76 27.58 19.97 3
+00000310: 2e33 3320 3236 2e38 312d 3135 2e31 2032  .33 26.81-15.1 2
+00000320: 372e 3538 2d31 392e 3737 2038 2e32 382d  7.58-19.77 8.28-
+00000330: 3530 2e30 3320 3132 2e30 362d 3130 312e  50.03 12.06-101.
+00000340: 3231 2031 312e 3237 2d31 3532 2e31 312d  21 11.27-152.11-
+00000350: 2e38 382d 3535 2e38 2d34 372e 3934 2d31  .88-55.8-47.94-1
+00000360: 3031 2e38 382d 3130 342e 3931 2d31 3032  01.88-104.91-102
+00000370: 2e37 327a 6d2d 3131 302e 3639 2d31 392e  .72zm-110.69-19.
+00000380: 3738 632d 3130 2e33 2d38 2e33 342d 3235  78c-10.3-8.34-25
+00000390: 2e33 372d 362e 382d 3333 2e37 3620 332e  .37-6.8-33.76 3.
+000003a0: 3438 2d32 352e 3632 2033 312e 352d 3339  48-25.62 31.5-39
+000003b0: 2e33 3920 3731 2e32 382d 3338 2e37 3520  .39 71.28-38.75 
+000003c0: 3131 3220 2e35 3920 3337 2e35 382d 322e  112 .59 37.58-2.
+000003d0: 3437 2037 352e 3237 2d39 2e31 3120 3131  47 75.27-9.11 11
+000003e0: 322e 3035 2d32 2e33 3420 3133 2e30 3520  2.05-2.34 13.05 
+000003f0: 362e 3331 2032 352e 3533 2031 392e 3336  6.31 25.53 19.36
+00000400: 2032 372e 3839 2032 302e 3131 2033 2e35   27.89 20.11 3.5
+00000410: 2032 372e 3037 2d31 342e 3831 2032 372e   27.07-14.81 27.
+00000420: 3839 2d31 392e 3336 2037 2e31 392d 3339  89-19.36 7.19-39
+00000430: 2e38 3420 3130 2e35 2d38 302e 3636 2039  .84 10.5-80.66 9
+00000440: 2e38 362d 3132 312e 3333 2d2e 3437 2d32  .86-121.33-.47-2
+00000450: 392e 3838 2039 2e32 2d35 372e 3838 2032  9.88 9.2-57.88 2
+00000460: 382d 3830 2e39 3720 382e 3335 2d31 302e  8-80.97 8.35-10.
+00000470: 3238 2036 2e37 392d 3235 2e33 392d 332e  28 6.79-25.39-3.
+00000480: 3439 2d33 332e 3736 7a6d 3130 392e 3437  49-33.76zm109.47
+00000490: 2d36 322e 3333 632d 3135 2e34 312d 2e34  -62.33c-15.41-.4
+000004a0: 312d 3330 2e38 3720 312e 3434 2d34 352e  1-30.87 1.44-45.
+000004b0: 3738 2034 2e39 372d 3132 2e38 3920 332e  78 4.97-12.89 3.
+000004c0: 3036 2d32 302e 3837 2031 352e 3938 2d31  06-20.87 15.98-1
+000004d0: 372e 3833 2032 382e 3839 2033 2e30 3620  7.83 28.89 3.06 
+000004e0: 3132 2e38 3920 3136 2032 302e 3833 2032  12.89 16 20.83 2
+000004f0: 382e 3839 2031 372e 3833 2031 312e 3035  8.89 17.83 11.05
+00000500: 2d32 2e36 3120 3232 2e34 372d 332e 3737  -2.61 22.47-3.77
+00000510: 2033 342d 332e 3639 2037 352e 3433 2031   34-3.69 75.43 1
+00000520: 2e31 3320 3133 372e 3733 2036 312e 3520  .13 137.73 61.5 
+00000530: 3133 382e 3838 2031 3334 2e35 382e 3539  138.88 134.58.59
+00000540: 2033 372e 3838 2d31 2e32 3820 3736 2e31   37.88-1.28 76.1
+00000550: 312d 352e 3538 2031 3133 2e36 332d 312e  1-5.58 113.63-1.
+00000560: 3520 3133 2e31 3720 372e 3935 2032 352e  5 13.17 7.95 25.
+00000570: 3038 2032 312e 3131 2032 362e 3538 2031  08 21.11 26.58 1
+00000580: 362e 3732 2031 2e39 3520 3235 2e35 312d  6.72 1.95 25.51-
+00000590: 3131 2e38 3820 3236 2e35 382d 3231 2e31  11.88 26.58-21.1
+000005a0: 3161 3932 392e 3036 2039 3239 2e30 3620  1a929.06 929.06 
+000005b0: 3020 3020 3020 352e 3839 2d31 3139 2e38  0 0 0 5.89-119.8
+000005c0: 3563 2d31 2e35 362d 3938 2e37 352d 3835  5c-1.56-98.75-85
+000005d0: 2e30 372d 3138 302e 3333 2d31 3836 2e31  .07-180.33-186.1
+000005e0: 362d 3138 312e 3833 7a6d 3235 322e 3037  6-181.83zm252.07
+000005f0: 2031 3231 2e34 3563 2d32 2e38 362d 3132   121.45c-2.86-12
+00000600: 2e39 322d 3135 2e35 312d 3231 2e32 2d32  .92-15.51-21.2-2
+00000610: 382e 3631 2d31 382e 3237 2d31 322e 3934  8.61-18.27-12.94
+00000620: 2032 2e38 362d 3231 2e31 3220 3135 2e36   2.86-21.12 15.6
+00000630: 362d 3138 2e32 3620 3238 2e36 3120 342e  6-18.26 28.61 4.
+00000640: 3731 2032 312e 3431 2034 2e39 3120 3337  71 21.41 4.91 37
+00000650: 2e34 3120 342e 3720 3631 2e36 2d2e 3131  .41 4.7 61.6-.11
+00000660: 2031 332e 3237 2031 302e 3535 2032 342e   13.27 10.55 24.
+00000670: 3039 2032 332e 3820 3234 2e32 682e 3263  09 23.8 24.2h.2c
+00000680: 3133 2e31 3720 3020 3233 2e38 392d 3130  13.17 0 23.89-10
+00000690: 2e36 3120 3234 2d32 332e 382e 3138 2d32  .61 24-23.8.18-2
+000006a0: 322e 3138 2e34 2d34 342e 3131 2d35 2e38  2.18.4-44.11-5.8
+000006b0: 332d 3732 2e33 347a 6d2d 3430 2e31 322d  3-72.34zm-40.12-
+000006c0: 3930 2e37 3243 3431 372e 3239 2034 332e  90.72C417.29 43.
+000006d0: 3436 2033 3337 2e36 2031 2e32 3920 3235  46 337.6 1.29 25
+000006e0: 322e 3831 2e30 3220 3138 332e 3032 2d2e  2.81.02 183.02-.
+000006f0: 3832 2031 3138 2e34 3720 3234 2e39 3120  82 118.47 24.91 
+00000700: 3730 2e34 3620 3732 2e39 3420 3234 2e30  70.46 72.94 24.0
+00000710: 3920 3131 392e 3337 2d2e 3920 3138 312e  9 119.37-.9 181.
+00000720: 3034 2e31 3420 3234 362e 3635 6c2d 2e31  04.14 246.65l-.1
+00000730: 3220 3231 2e34 3763 2d2e 3339 2031 332e  2 21.47c-.39 13.
+00000740: 3235 2031 302e 3033 2032 342e 3331 2032  25 10.03 24.31 2
+00000750: 332e 3238 2032 342e 3639 2e32 332e 3032  3.28 24.69.23.02
+00000760: 2e34 382e 3032 2e37 322e 3032 2031 322e  .48.02.72.02 12.
+00000770: 3932 2030 2032 332e 3539 2d31 302e 3320  92 0 23.59-10.3 
+00000780: 3233 2e39 372d 3233 2e33 6c2e 3136 2d32  23.97-23.3l.16-2
+00000790: 332e 3634 632d 2e38 332d 3532 2e35 2031  3.64c-.83-52.5 1
+000007a0: 392e 3136 2d31 3031 2e38 3620 3536 2e32  9.16-101.86 56.2
+000007b0: 382d 3133 3920 3338 2e37 362d 3338 2e38  8-139 38.76-38.8
+000007c0: 2039 312e 3334 2d35 392e 3637 2031 3437   91.34-59.67 147
+000007d0: 2e36 382d 3538 2e38 3620 3639 2e34 3520  .68-58.86 69.45 
+000007e0: 312e 3033 2031 3334 2e37 3320 3335 2e35  1.03 134.73 35.5
+000007f0: 3620 3137 342e 3632 2039 322e 3339 2037  6 174.62 92.39 7
+00000800: 2e36 3120 3130 2e38 3620 3232 2e35 3620  .61 10.86 22.56 
+00000810: 3133 2e34 3520 3333 2e34 3220 352e 3836  13.45 33.42 5.86
+00000820: 2031 302e 3834 2d37 2e36 3220 3133 2e34   10.84-7.62 13.4
+00000830: 362d 3232 2e35 3920 352e 3834 2d33 332e  6-22.59 5.84-33.
+00000840: 3433 7a22 0a20 203e 3c2f 7061 7468 3e0a  43z".  ></path>.
+00000850: 3c2f 7376 673e 0a                        </svg>.
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-<html>
-  <head>
-    <style>
-      body {
-        margin: 0px;
-        zoom: 150%;
-      }
-      .image {
-        display: flex;
-        flex-direction: column;
-        overflow: scroll;
-        width: max-content;
-        padding: 20px;
-      }
-      .head {
-        display: flex;
-        flex-direction: row;
-        align-items: center;
-        justify-content: space-between;
-        background-color: #f5f6f7;
-        padding-left: 20px;
-        padding-right: 20px;
-        padding-top: 10px;
-        padding-bottom: 10px;
-        border: 2px solid;
-        border-radius: 50px;
-        border-color: #e5e7eb;
-        font-size: 16px;
-        margin-bottom: 20px;
-      }
-
-      .plugins {
-        display: grid;
-        grid-template-columns: auto auto auto;
-        row-gap: 20px;
-        column-gap: 20px;
-		margin-bottom: 20px;
-      }
-      .plugin {
-        display: flex;
-        padding: 5px;
-        border: 1px solid;
-        border-radius: 5px;
-        border-color: #e5e7eb;
-        box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
-        background-color: #f5f6f7;
-      }
-      .plugin_meta {
-        display: flex;
-        flex-direction: column;
-        padding: 5px;
-        width: 250px;
-        justify-content: space-between;
-      }
-      .plugin_name {
-        font-size: 20px;
-      }
-      .plugin_description {
-        font-size: 15px;
-        color: gray;
-        margin-top: 5px;
-        margin-bottom: 5px;
-      }
-      .plugin_meta_line1 {
-        display: flex;
-        flex-direction: row;
-        align-items: center;
-        justify-content: space-between;
-      }
-      .plugin_meta_line3 {
-        display: flex;
-        flex-direction: row;
-        align-items: center;
-      }
-      .package_name_label{
-        background-image: url(./fingerprint.svg);
-        width: 13px;
-        height: 13px;
-        margin-right: 8px;
-      }
-      .package_name {
-        font-size: 13px;
-        color: gray;
-      }
-      .switch {
-        position: relative;
-        display: inline-block;
-        width: 40px;
-        height: 24px;
-      }
-      .slider {
-        position: absolute;
-        cursor: pointer;
-        top: 0;
-        left: 0;
-        right: 0;
-        bottom: 0;
-        background-color: #ccc;
-      }
-      .slider:before {
-        position: absolute;
-        content: "";
-        height: 16px;
-        width: 16px;
-        left: 4px;
-        bottom: 4px;
-        background-color: white;
-      }
-      .switch input {
-        display: none;
-      }
-      .switch input:checked + .slider {
-        background-color: rgba(86, 40, 238, 0.5);
-      }
-      .switch input:checked + .slider:before {
-        -webkit-transform: translateX(16px);
-        -ms-transform: translateX(16px);
-        transform: translateX(16px);
-      }
-      .slider.round {
-        border-radius: 24px;
-      }
-      .slider.round:before {
-        border-radius: 50%;
-      }
-      .checkbox {
-        visibility: hidden;
-      }
-      .slider.locked {
-        opacity: 0.5;
-      }
-      .switch input + span .lock {
-        width: 8px;
-        height: 7px;
-        background: #99a3ba;
-        position: absolute;
-        left: 8px;
-        bottom: 7px;
-        border-radius: 2px;
-        display: block;
-        z-index: 1;
-        transition: all 0.45s ease;
-      }
-      .switch input + span .lock:before {
-        content: "";
-        width: 2px;
-        height: 2px;
-        border-radius: 1px;
-        background: #fff;
-        position: absolute;
-        display: block;
-        left: 50%;
-        top: 50%;
-        margin: -1px 0 0 -1px;
-      }
-      .switch input + span .lock:after {
-        content: "";
-        border-top-left-radius: 4px;
-        border-top-right-radius: 4px;
-        border: 1px solid #99a3ba;
-        border-bottom: 0;
-        width: 4px;
-        height: 4px;
-        left: 1px;
-        bottom: 6px;
-        position: absolute;
-        z-index: 1;
-        -webkit-transform-origin: 0 100%;
-        transform-origin: 0 100%;
-        transition: all 0.45s ease;
-      }
-      .switch input:checked + span .lock {
-        background: #5628ee;
-        -webkit-transform: translateX(16px);
-        -ms-transform: translateX(16px);
-        transform: translateX(16px);
-      }
-      .lock {
-        visibility: hidden;
-      }
-      .lock.locked {
-        visibility: inherit;
-      }
-    </style>
-  </head>
-  <body>
-    <div class="image">
-      <div class="head">
-        <span><b>已加载服务器</b></span>
-        <span>发送 “<b>服务器昵称/序号</b>” 查看详情</span>
-      </div>
-      <div class="plugins">
-        {% for plugin in plugins %}
-        <div class="plugin">
-          <div class="plugin_meta">
-            <div class="plugin_meta_line1">
-              <div class="plugin_name">{{ plugin.number }}:{{ plugin.name }}</div>
-              <div class="plugin_status">
-                <label class="switch">
-                  <input class="checkbox" type="checkbox" {% if plugin.enabled %} checked {% endif %} />
-                  <span class="slider round {% if plugin.locked %} locked {% endif %}">
-                    <span class="lock {% if plugin.locked %} locked {% endif %}"></span>
-                  </span>
-                </label>
-              </div>
-            </div>
-            <div class="plugin_meta_line2">
-				<font color="blue">{{ plugin.map_ }}</font><br>
-                {% for Player in plugin.Players %}
-                    <font color="green">{{ Player }}</font><br>
-                {% endfor %}
-            </div>
-            <div class="plugin_meta_line3">
-              <svg width="13px" height="13px">
-                <image xlink:href="{{ plugin.system }}" width="13px" height="13px"/>
-              </svg>
-              <div class="package_name">&nbsp{{ plugin.max_players }} </div>
-              <div class="package_name">&nbsp{{ plugin.tick }} </div>
-            </div>
-          </div>
-        </div>
-        {% endfor %}
-      </div>
-	  <div class="head">
-      <span><b>©爱丽数码</b></span>
-      <span>github.com/Agnes4m/nonebot_plugin_l4d2_server</span>
-      </div>
-    </div>
-</html>
-  </body>
-
-
-
+<html>
+  <head>
+    <style>
+      body {
+        margin: 0px;
+        zoom: 150%;
+      }
+      .image {
+        display: flex;
+        flex-direction: column;
+        overflow: scroll;
+        width: max-content;
+        padding: 20px;
+      }
+      .head {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+        justify-content: space-between;
+        background-color: #f5f6f7;
+        padding-left: 20px;
+        padding-right: 20px;
+        padding-top: 10px;
+        padding-bottom: 10px;
+        border: 2px solid;
+        border-radius: 50px;
+        border-color: #e5e7eb;
+        font-size: 16px;
+        margin-bottom: 20px;
+      }
+
+      .plugins {
+        display: grid;
+        grid-template-columns: auto auto auto;
+        row-gap: 20px;
+        column-gap: 20px;
+		margin-bottom: 20px;
+      }
+      .plugin {
+        display: flex;
+        padding: 5px;
+        border: 1px solid;
+        border-radius: 5px;
+        border-color: #e5e7eb;
+        box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
+        background-color: #f5f6f7;
+      }
+      .plugin_meta {
+        display: flex;
+        flex-direction: column;
+        padding: 5px;
+        width: 250px;
+        justify-content: space-between;
+      }
+      .plugin_name {
+        font-size: 20px;
+      }
+      .plugin_description {
+        font-size: 15px;
+        color: gray;
+        margin-top: 5px;
+        margin-bottom: 5px;
+      }
+      .plugin_meta_line1 {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+        justify-content: space-between;
+      }
+      .plugin_meta_line3 {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+      }
+      .package_name_label{
+        background-image: url(./fingerprint.svg);
+        width: 13px;
+        height: 13px;
+        margin-right: 8px;
+      }
+      .package_name {
+        font-size: 13px;
+        color: gray;
+      }
+      .switch {
+        position: relative;
+        display: inline-block;
+        width: 40px;
+        height: 24px;
+      }
+      .slider {
+        position: absolute;
+        cursor: pointer;
+        top: 0;
+        left: 0;
+        right: 0;
+        bottom: 0;
+        background-color: #ccc;
+      }
+      .slider:before {
+        position: absolute;
+        content: "";
+        height: 16px;
+        width: 16px;
+        left: 4px;
+        bottom: 4px;
+        background-color: white;
+      }
+      .switch input {
+        display: none;
+      }
+      .switch input:checked + .slider {
+        background-color: rgba(86, 40, 238, 0.5);
+      }
+      .switch input:checked + .slider:before {
+        -webkit-transform: translateX(16px);
+        -ms-transform: translateX(16px);
+        transform: translateX(16px);
+      }
+      .slider.round {
+        border-radius: 24px;
+      }
+      .slider.round:before {
+        border-radius: 50%;
+      }
+      .checkbox {
+        visibility: hidden;
+      }
+      .slider.locked {
+        opacity: 0.5;
+      }
+      .switch input + span .lock {
+        width: 8px;
+        height: 7px;
+        background: #99a3ba;
+        position: absolute;
+        left: 8px;
+        bottom: 7px;
+        border-radius: 2px;
+        display: block;
+        z-index: 1;
+        transition: all 0.45s ease;
+      }
+      .switch input + span .lock:before {
+        content: "";
+        width: 2px;
+        height: 2px;
+        border-radius: 1px;
+        background: #fff;
+        position: absolute;
+        display: block;
+        left: 50%;
+        top: 50%;
+        margin: -1px 0 0 -1px;
+      }
+      .switch input + span .lock:after {
+        content: "";
+        border-top-left-radius: 4px;
+        border-top-right-radius: 4px;
+        border: 1px solid #99a3ba;
+        border-bottom: 0;
+        width: 4px;
+        height: 4px;
+        left: 1px;
+        bottom: 6px;
+        position: absolute;
+        z-index: 1;
+        -webkit-transform-origin: 0 100%;
+        transform-origin: 0 100%;
+        transition: all 0.45s ease;
+      }
+      .switch input:checked + span .lock {
+        background: #5628ee;
+        -webkit-transform: translateX(16px);
+        -ms-transform: translateX(16px);
+        transform: translateX(16px);
+      }
+      .lock {
+        visibility: hidden;
+      }
+      .lock.locked {
+        visibility: inherit;
+      }
+    </style>
+  </head>
+  <body>
+    <div class="image">
+      <div class="head">
+        <span><b>已加载服务器</b></span>
+        <span>发送 “<b>服务器昵称/序号</b>” 查看详情</span>
+      </div>
+      <div class="plugins">
+        {% for plugin in plugins %}
+        <div class="plugin">
+          <div class="plugin_meta">
+            <div class="plugin_meta_line1">
+              <div class="plugin_name">{{ plugin.number }}:{{ plugin.name }}</div>
+              <div class="plugin_status">
+                <label class="switch">
+                  <input class="checkbox" type="checkbox" {% if plugin.enabled %} checked {% endif %} />
+                  <span class="slider round {% if plugin.locked %} locked {% endif %}">
+                    <span class="lock {% if plugin.locked %} locked {% endif %}"></span>
+                  </span>
+                </label>
+              </div>
+            </div>
+            <div class="plugin_meta_line2">
+				<font color="blue">{{ plugin.map_ }}</font><br>
+                {% for Player in plugin.Players %}
+                    <font color="green">{{ Player }}</font><br>
+                {% endfor %}
+            </div>
+            <div class="plugin_meta_line3">
+              <svg width="13px" height="13px">
+                <image xlink:href="{{ plugin.system }}" width="13px" height="13px"/>
+              </svg>
+              <div class="package_name">&nbsp{{ plugin.max_players }} </div>
+              <div class="package_name">&nbsp{{ plugin.tick }} </div>
+            </div>
+          </div>
+        </div>
+        {% endfor %}
+      </div>
+	  <div class="head">
+      <span><b>©爱丽数码</b></span>
+      <span>github.com/Agnes4m/nonebot_plugin_l4d2_server</span>
+      </div>
+    </div>
+</html>
+  </body>
+
+
+
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,231 +1,231 @@
-<html>
-  <head>
-    <style>
-      body {
-        margin: 0px;
-        zoom: 150%;
-        background-color: #0D1117;
-      }
-      .image {
-        display: flex;
-        flex-direction: column;
-        overflow: scroll;
-        width: max-content;
-        padding: 20px;
-      }
-      .head {
-        display: flex;
-        flex-direction: row;
-        align-items: center;
-        justify-content: space-between;
-        background-color: #161B22;
-        padding-left: 20px;
-        padding-right: 20px;
-        padding-top: 10px;
-        padding-bottom: 10px;
-        border: 2px solid;
-        border-radius: 50px;
-        border-color: #1a1a1a;
-        font-size: 16px;
-        margin-bottom: 20px;
-      }
-
-      .plugins {
-        display: grid;
-        grid-template-columns: auto auto auto;
-        row-gap: 20px;
-        column-gap: 20px;
-		margin-bottom: 20px;
-      }
-      .plugin {
-        display: flex;
-        padding: 5px;
-        border: 1px solid;
-        border-radius: 5px;
-        border-color: #161B22;
-        box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
-        background-color: #1a1a1a;
-      }
-      .plugin_meta {
-        display: flex;
-        flex-direction: column;
-        padding: 5px;
-        width: 250px;
-        justify-content: space-between;
-      }
-      .plugin_name {
-        font-size: 20px;
-      }
-      .plugin_description {
-        font-size: 15px;
-        color: gray;
-        margin-top: 5px;
-        margin-bottom: 5px;
-      }
-      .plugin_meta_line1 {
-        display: flex;
-        flex-direction: row;
-        align-items: center;
-        justify-content: space-between;
-      }
-      .plugin_meta_line3 {
-        display: flex;
-        flex-direction: row;
-        align-items: center;
-      }
-      .package_name_label {
-        background-image: url(./fingerprint.svg);
-        width: 13px;
-        height: 13px;
-        margin-right: 8px;
-      }
-      .package_name {
-        font-size: 13px;
-        color: gray;
-      }
-      .switch {
-        position: relative;
-        display: inline-block;
-        width: 40px;
-        height: 24px;
-      }
-      .slider {
-        position: absolute;
-        cursor: pointer;
-        top: 0;
-        left: 0;
-        right: 0;
-        bottom: 0;
-        background-color: #ccc;
-      }
-      .slider:before {
-        position: absolute;
-        content: "";
-        height: 16px;
-        width: 16px;
-        left: 4px;
-        bottom: 4px;
-        background-color: white;
-      }
-      .switch input {
-        display: none;
-      }
-      .switch input:checked + .slider {
-        background-color: rgba(46, 160, 67);
-      }
-      .switch input:checked + .slider:before {
-        -webkit-transform: translateX(16px);
-        -ms-transform: translateX(16px);
-        transform: translateX(16px);
-      }
-      .slider.round {
-        border-radius: 24px;
-      }
-      .slider.round:before {
-        border-radius: 50%;
-      }
-      .checkbox {
-        visibility: hidden;
-      }
-      .slider.locked {
-        opacity: 0.5;
-      }
-      .switch input + span .lock {
-        width: 8px;
-        height: 7px;
-        background: #99a3ba;
-        position: absolute;
-        left: 8px;
-        bottom: 7px;
-        border-radius: 2px;
-        display: block;
-        z-index: 1;
-        transition: all 0.45s ease;
-      }
-      .switch input + span .lock:before {
-        content: "";
-        width: 2px;
-        height: 2px;
-        border-radius: 1px;
-        background: #fff;
-        position: absolute;
-        display: block;
-        left: 50%;
-        top: 50%;
-        margin: -1px 0 0 -1px;
-      }
-      .switch input + span .lock:after {
-        content: "";
-        border-top-left-radius: 4px;
-        border-top-right-radius: 4px;
-        border: 1px solid #99a3ba;
-        border-bottom: 0;
-        width: 4px;
-        height: 4px;
-        left: 1px;
-        bottom: 6px;
-        position: absolute;
-        z-index: 1;
-        -webkit-transform-origin: 0 100%;
-        transform-origin: 0 100%;
-        transition: all 0.45s ease;
-      }
-      .switch input:checked + span .lock {
-        background: #5628ee;
-        -webkit-transform: translateX(16px);
-        -ms-transform: translateX(16px);
-        transform: translateX(16px);
-      }
-      .lock {
-        visibility: hidden;
-      }
-      .lock.locked {
-        visibility: inherit;
-      }
-    </style>
-  </head>
-  <body>
-    <div class="image">
-      <div class="head">
-        <span><b><font color="Silver">已加载服务器</font></b></span>
-        <span><font color="Silver">发送“<b>服务器昵称/序号</b>”查看详情</font></span>
-      </div>
-      <div class="plugins">
-        {% for plugin in plugins %}
-        <div class="plugin">
-          <div class="plugin_meta">
-            <div class="plugin_meta_line1">
-              <div class="plugin_name"><font color="DeepSkyBlue">{{ plugin.number }}:{{ plugin.name }}</font></div>
-              <div class="plugin_status">
-                <label class="switch">
-                  <input class="checkbox" type="checkbox" {% if plugin.enabled %} checked {% endif %} />
-                  <span class="slider round {% if plugin.locked %} locked {% endif %}">
-                    <span class="lock {% if plugin.locked %} locked {% endif %}"></span>
-                  </span>
-                </label>
-              </div>
-            </div>
-            <div class="plugin_meta_line2">
-				<font color="LightSkyBlue">{{ plugin.map_ }}</font><br>
-                {% for Player in plugin.Players %}
-                    <font color="LightGray">{{ Player }}</font><br>
-                {% endfor %}
-            </div>
-            <div class="plugin_meta_line3">
-              <div class="package_name_label"></div>
-              <div class="package_name"><font color="LightGray">{{ plugin.max_players }}</font></div>
-            </div>
-          </div>
-        </div>
-        {% endfor %}
-      </div>
-	  <div class="head">
-      <span><b><font color="Silver">©爱丽数码</font></b></span>
-      <span><font color="Silver">github*Agnes4m</font></span>
-      </div>
-    </div>
-  </body>
-</html>
-  
-
-/*暗黑风格-ArcPav*/
+<html>
+  <head>
+    <style>
+      body {
+        margin: 0px;
+        zoom: 150%;
+        background-color: #0D1117;
+      }
+      .image {
+        display: flex;
+        flex-direction: column;
+        overflow: scroll;
+        width: max-content;
+        padding: 20px;
+      }
+      .head {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+        justify-content: space-between;
+        background-color: #161B22;
+        padding-left: 20px;
+        padding-right: 20px;
+        padding-top: 10px;
+        padding-bottom: 10px;
+        border: 2px solid;
+        border-radius: 50px;
+        border-color: #1a1a1a;
+        font-size: 16px;
+        margin-bottom: 20px;
+      }
+
+      .plugins {
+        display: grid;
+        grid-template-columns: auto auto auto;
+        row-gap: 20px;
+        column-gap: 20px;
+		margin-bottom: 20px;
+      }
+      .plugin {
+        display: flex;
+        padding: 5px;
+        border: 1px solid;
+        border-radius: 5px;
+        border-color: #161B22;
+        box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
+        background-color: #1a1a1a;
+      }
+      .plugin_meta {
+        display: flex;
+        flex-direction: column;
+        padding: 5px;
+        width: 250px;
+        justify-content: space-between;
+      }
+      .plugin_name {
+        font-size: 20px;
+      }
+      .plugin_description {
+        font-size: 15px;
+        color: gray;
+        margin-top: 5px;
+        margin-bottom: 5px;
+      }
+      .plugin_meta_line1 {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+        justify-content: space-between;
+      }
+      .plugin_meta_line3 {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+      }
+      .package_name_label {
+        background-image: url(./fingerprint.svg);
+        width: 13px;
+        height: 13px;
+        margin-right: 8px;
+      }
+      .package_name {
+        font-size: 13px;
+        color: gray;
+      }
+      .switch {
+        position: relative;
+        display: inline-block;
+        width: 40px;
+        height: 24px;
+      }
+      .slider {
+        position: absolute;
+        cursor: pointer;
+        top: 0;
+        left: 0;
+        right: 0;
+        bottom: 0;
+        background-color: #ccc;
+      }
+      .slider:before {
+        position: absolute;
+        content: "";
+        height: 16px;
+        width: 16px;
+        left: 4px;
+        bottom: 4px;
+        background-color: white;
+      }
+      .switch input {
+        display: none;
+      }
+      .switch input:checked + .slider {
+        background-color: rgba(46, 160, 67);
+      }
+      .switch input:checked + .slider:before {
+        -webkit-transform: translateX(16px);
+        -ms-transform: translateX(16px);
+        transform: translateX(16px);
+      }
+      .slider.round {
+        border-radius: 24px;
+      }
+      .slider.round:before {
+        border-radius: 50%;
+      }
+      .checkbox {
+        visibility: hidden;
+      }
+      .slider.locked {
+        opacity: 0.5;
+      }
+      .switch input + span .lock {
+        width: 8px;
+        height: 7px;
+        background: #99a3ba;
+        position: absolute;
+        left: 8px;
+        bottom: 7px;
+        border-radius: 2px;
+        display: block;
+        z-index: 1;
+        transition: all 0.45s ease;
+      }
+      .switch input + span .lock:before {
+        content: "";
+        width: 2px;
+        height: 2px;
+        border-radius: 1px;
+        background: #fff;
+        position: absolute;
+        display: block;
+        left: 50%;
+        top: 50%;
+        margin: -1px 0 0 -1px;
+      }
+      .switch input + span .lock:after {
+        content: "";
+        border-top-left-radius: 4px;
+        border-top-right-radius: 4px;
+        border: 1px solid #99a3ba;
+        border-bottom: 0;
+        width: 4px;
+        height: 4px;
+        left: 1px;
+        bottom: 6px;
+        position: absolute;
+        z-index: 1;
+        -webkit-transform-origin: 0 100%;
+        transform-origin: 0 100%;
+        transition: all 0.45s ease;
+      }
+      .switch input:checked + span .lock {
+        background: #5628ee;
+        -webkit-transform: translateX(16px);
+        -ms-transform: translateX(16px);
+        transform: translateX(16px);
+      }
+      .lock {
+        visibility: hidden;
+      }
+      .lock.locked {
+        visibility: inherit;
+      }
+    </style>
+  </head>
+  <body>
+    <div class="image">
+      <div class="head">
+        <span><b><font color="Silver">已加载服务器</font></b></span>
+        <span><font color="Silver">发送“<b>服务器昵称/序号</b>”查看详情</font></span>
+      </div>
+      <div class="plugins">
+        {% for plugin in plugins %}
+        <div class="plugin">
+          <div class="plugin_meta">
+            <div class="plugin_meta_line1">
+              <div class="plugin_name"><font color="DeepSkyBlue">{{ plugin.number }}:{{ plugin.name }}</font></div>
+              <div class="plugin_status">
+                <label class="switch">
+                  <input class="checkbox" type="checkbox" {% if plugin.enabled %} checked {% endif %} />
+                  <span class="slider round {% if plugin.locked %} locked {% endif %}">
+                    <span class="lock {% if plugin.locked %} locked {% endif %}"></span>
+                  </span>
+                </label>
+              </div>
+            </div>
+            <div class="plugin_meta_line2">
+				<font color="LightSkyBlue">{{ plugin.map_ }}</font><br>
+                {% for Player in plugin.Players %}
+                    <font color="LightGray">{{ Player }}</font><br>
+                {% endfor %}
+            </div>
+            <div class="plugin_meta_line3">
+              <div class="package_name_label"></div>
+              <div class="package_name"><font color="LightGray">{{ plugin.max_players }}</font></div>
+            </div>
+          </div>
+        </div>
+        {% endfor %}
+      </div>
+	  <div class="head">
+      <span><b><font color="Silver">©爱丽数码</font></b></span>
+      <span><font color="Silver">github*Agnes4m</font></span>
+      </div>
+    </div>
+  </body>
+</html>
+  
+
+/*暗黑风格-ArcPav*/
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-<!DOCTYPE html>
-<html class="pc">
-<head>
-	<link rel="stylesheet" type="text/css" href="vue.css">
-    <title>Server Information</title>
-    <style>
-        table {
-            border-collapse: collapse;
-            width: 100%;
-        }
-        th, td {
-            border: 1px solid #ddd;
-            padding: 8px;
-            text-align: left;
-        }
-        th {
-            background-color: #f2f2f2;
-        }
-    </style>
-</head>
-<body style="background-image: url('back2.jpg'); background-size: 1200px 1800px;">
-<div class="myinfo">
-<table>
-    {% for i in range(0, data|length, 3) %}
-        <tr>
-            {% for j in range(i, i + 3) %}
-                {% if j < data|length %}
-                    <td>
-                         <font color="red">{{ data[j].number }}</font><br>
-                        <font color="yellow">{{ data[j].name }}</font><br>
-                        <font color="gray">{{ data[j].ip }}</font><br>
-                        <font color="blue">{{ data[j].map_ }}</font><br>
-                        {% for Player in data[j].Players %}
-                            <font color="green">{{ Player }}</font><br>
-                        {% endfor %}
-                        <font color="yellow">{{ data[j].max_players }}{{data[j].ping}}</font>
-                    </td>
-                {% endif %}
-            {% endfor %}
-        </tr>
-    {% endfor %}
-</table>
-<h5><center>©爱丽数码</center></br>
-	<center>
-		github.com/Agnes4m/nonebot_plugin_l4d2_server
-	</center>
-</h5>
-</div>
+<!DOCTYPE html>
+<html class="pc">
+<head>
+	<link rel="stylesheet" type="text/css" href="vue.css">
+    <title>Server Information</title>
+    <style>
+        table {
+            border-collapse: collapse;
+            width: 100%;
+        }
+        th, td {
+            border: 1px solid #ddd;
+            padding: 8px;
+            text-align: left;
+        }
+        th {
+            background-color: #f2f2f2;
+        }
+    </style>
+</head>
+<body style="background-image: url('back2.jpg'); background-size: 1200px 1800px;">
+<div class="myinfo">
+<table>
+    {% for i in range(0, data|length, 3) %}
+        <tr>
+            {% for j in range(i, i + 3) %}
+                {% if j < data|length %}
+                    <td>
+                         <font color="red">{{ data[j].number }}</font><br>
+                        <font color="yellow">{{ data[j].name }}</font><br>
+                        <font color="gray">{{ data[j].ip }}</font><br>
+                        <font color="blue">{{ data[j].map_ }}</font><br>
+                        {% for Player in data[j].Players %}
+                            <font color="green">{{ Player }}</font><br>
+                        {% endfor %}
+                        <font color="yellow">{{ data[j].max_players }}{{data[j].ping}}</font>
+                    </td>
+                {% endif %}
+            {% endfor %}
+        </tr>
+    {% endfor %}
+</table>
+<h5><center>©爱丽数码</center></br>
+	<center>
+		github.com/Agnes4m/nonebot_plugin_l4d2_server
+	</center>
+</h5>
+</div>
 </html>
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files 3% similar despite different names*

```diff
@@ -1,345 +1,345 @@
-00000000: 3c73 7667 200d 0a20 2072 6f6c 653d 2269  <svg ..  role="i
-00000010: 6d67 2220 0d0a 2020 7669 6577 426f 783d  mg" ..  viewBox=
-00000020: 2230 2030 2032 3420 3234 2220 0d0a 2020  "0 0 24 24" ..  
-00000030: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
-00000040: 772e 7733 2e6f 7267 2f32 3030 302f 7376  w.w3.org/2000/sv
-00000050: 6722 3e0d 0a20 203c 7469 746c 653e 4c69  g">..  <title>Li
-00000060: 6e75 783c 2f74 6974 6c65 3e0d 0a3e 0d0a  nux</title>..>..
-00000070: 2020 3c70 6174 6820 0d0a 2020 6669 6c6c    <path ..  fill
-00000080: 3d22 6375 7272 656e 7443 6f6c 6f72 220d  ="currentColor".
-00000090: 0a20 2064 3d22 4d31 322e 3530 3420 3063  .  d="M12.504 0c
-000000a0: 2d2e 3135 3520 302d 2e33 3135 2e30 3038  -.155 0-.315.008
-000000b0: 2d2e 3438 2e30 3231 2d34 2e32 3236 2e33  -.48.021-4.226.3
-000000c0: 3333 2d33 2e31 3035 2034 2e38 3037 2d33  33-3.105 4.807-3
-000000d0: 2e31 3720 362e 3239 382d 2e30 3736 2031  .17 6.298-.076 1
-000000e0: 2e30 3932 2d2e 3320 312e 3935 332d 312e  .092-.3 1.953-1.
-000000f0: 3035 2033 2e30 322d 2e38 3835 2031 2e30  05 3.02-.885 1.0
-00000100: 3531 2d32 2e31 3237 2032 2e37 352d 322e  51-2.127 2.75-2.
-00000110: 3731 3620 342e 3532 312d 2e32 3738 2e38  716 4.521-.278.8
-00000120: 3332 2d2e 3431 2031 2e36 3834 2d2e 3238  32-.41 1.684-.28
-00000130: 3720 322e 3438 3961 2e34 3234 2e34 3234  7 2.489a.424.424
-00000140: 2030 2030 302d 2e31 312e 3133 3563 2d2e   0 00-.11.135c-.
-00000150: 3236 2e32 3638 2d2e 3435 2e36 2d2e 3636  26.268-.45.6-.66
-00000160: 332e 3833 392d 2e31 3939 2e31 3939 2d2e  3.839-.199.199-.
-00000170: 3438 352e 3236 372d 2e37 3937 2e34 2d2e  485.267-.797.4-.
-00000180: 3331 332e 3133 362d 2e36 3538 2e32 3639  313.136-.658.269
-00000190: 2d2e 3836 342e 3638 2d2e 3039 2e31 3839  -.864.68-.09.189
-000001a0: 2d2e 3133 362e 3339 342d 2e31 3332 2e36  -.136.394-.132.6
-000001b0: 3032 2030 202e 3139 392e 3032 372e 342e  02 0 .199.027.4.
-000001c0: 3035 352e 3533 362e 3035 382e 3339 392e  055.536.058.399.
-000001d0: 3131 362e 3732 382e 3034 2e39 372d 2e32  116.728.04.97-.2
-000001e0: 3439 2e36 382d 2e32 3820 312e 3134 352d  49.68-.28 1.145-
-000001f0: 2e31 3036 2031 2e34 3834 2e31 3734 2e33  .106 1.484.174.3
-00000200: 3334 2e35 3335 2e34 372e 3934 2e36 3031  34.535.47.94.601
-00000210: 2e38 312e 3220 312e 3931 2e31 3335 2032  .81.2 1.91.135 2
-00000220: 2e37 3734 2e36 2e39 3236 2e34 3636 2031  .774.6.926.466 1
-00000230: 2e38 3636 2e36 3720 322e 3631 362e 3437  .866.67 2.616.47
-00000240: 2e35 3236 2d2e 3131 362e 3937 2d2e 3436  .526-.116.97-.46
-00000250: 3420 312e 3230 382d 2e39 3436 2e35 3837  4 1.208-.946.587
-00000260: 2d2e 3030 3320 312e 3233 2d2e 3236 3920  -.003 1.23-.269 
-00000270: 322e 3236 2d2e 3333 342e 3639 392d 2e30  2.26-.334.699-.0
-00000280: 3538 2031 2e35 3734 2e32 3637 2032 2e35  58 1.574.267 2.5
-00000290: 3737 2e32 2e30 3235 2e31 3334 2e30 3633  77.2.025.134.063
-000002a0: 2e31 3938 2e31 3134 2e33 3333 6c2e 3030  .198.114.333l.00
-000002b0: 332e 3030 3363 2e33 3931 2e37 3738 2031  3.003c.391.778 1
-000002c0: 2e31 3133 2031 2e31 3332 2031 2e38 3834  .113 1.132 1.884
-000002d0: 2031 2e30 3731 2e37 3731 2d2e 3036 2031   1.071.771-.06 1
-000002e0: 2e35 3932 2d2e 3533 3620 322e 3235 372d  .592-.536 2.257-
-000002f0: 312e 3330 362e 3633 312d 2e37 3635 2031  1.306.631-.765 1
-00000300: 2e36 3833 2d31 2e30 3834 2032 2e33 3738  .683-1.084 2.378
-00000310: 2d31 2e35 3033 2e33 3438 2d2e 3139 392e  -1.503.348-.199.
-00000320: 3632 392d 2e34 3639 2e36 3439 2d2e 3835  629-.469.649-.85
-00000330: 332e 3032 332d 2e34 2d2e 322d 2e38 3131  3.023-.4-.2-.811
-00000340: 2d2e 3731 342d 312e 3337 3676 2d2e 3039  -.714-1.376v-.09
-00000350: 376c 2d2e 3030 332d 2e30 3033 632d 2e31  7l-.003-.003c-.1
-00000360: 372d 2e32 2d2e 3235 2d2e 3533 352d 2e33  7-.2-.25-.535-.3
-00000370: 3338 2d2e 3932 362d 2e30 3835 2d2e 3430  38-.926-.085-.40
-00000380: 312d 2e31 3832 2d2e 3738 362d 2e34 3932  1-.182-.786-.492
-00000390: 2d31 2e30 3436 682d 2e30 3033 632d 2e30  -1.046h-.003c-.0
-000003a0: 3539 2d2e 3035 342d 2e31 3233 2d2e 3036  59-.054-.123-.06
-000003b0: 372d 2e31 3838 2d2e 3133 3561 2e33 3537  7-.188-.135a.357
-000003c0: 2e33 3537 2030 2030 302d 2e31 392d 2e30  .357 0 00-.19-.0
-000003d0: 3634 632e 3433 312d 312e 3237 382e 3236  64c.431-1.278.26
-000003e0: 342d 322e 3535 2d2e 3137 332d 332e 3639  4-2.55-.173-3.69
-000003f0: 342d 2e35 3333 2d31 2e34 312d 312e 3436  4-.533-1.41-1.46
-00000400: 352d 322e 3633 382d 322e 3137 352d 332e  5-2.638-2.175-3.
-00000410: 3438 332d 2e37 3936 2d31 2e30 3035 2d31  483-.796-1.005-1
-00000420: 2e35 3736 2d31 2e39 3537 2d31 2e35 362d  .576-1.957-1.56-
-00000430: 332e 3336 382e 3032 362d 322e 3135 322e  3.368.026-2.152.
-00000440: 3233 362d 362e 3133 332d 332e 3534 342d  236-6.133-3.544-
-00000450: 362e 3133 397a 6d2e 3532 3920 332e 3430  6.139zm.529 3.40
-00000460: 3568 2e30 3133 632e 3231 3320 3020 2e33  5h.013c.213 0 .3
-00000470: 3936 2e30 3632 2e35 3834 2e31 3938 2e31  96.062.584.198.1
-00000480: 392e 3133 352e 3333 2e33 3332 2e34 3338  9.135.33.332.438
-00000490: 2e35 3333 2e31 3035 2e32 3539 2e31 3538  .533.105.259.158
-000004a0: 2e34 3539 2e31 3636 2e37 3234 2030 2d2e  .459.166.724 0-.
-000004b0: 3032 2e30 3036 2d2e 3034 2e30 3036 2d2e  02.006-.04.006-.
-000004c0: 3036 762e 3130 3561 2e30 3836 2e30 3836  06v.105a.086.086
-000004d0: 2030 2030 312d 2e30 3034 2d2e 3032 316c   0 01-.004-.021l
-000004e0: 2d2e 3030 342d 2e30 3234 6131 2e38 3037  -.004-.024a1.807
-000004f0: 2031 2e38 3037 2030 2030 312d 2e31 352e   1.807 0 01-.15.
-00000500: 3730 362e 3935 332e 3935 3320 3020 3031  706.953.953 0 01
-00000510: 2d2e 3231 332e 3333 352e 3731 2e37 3120  -.213.335.71.71 
-00000520: 3020 3030 2d2e 3038 382d 2e30 3432 632d  0 00-.088-.042c-
-00000530: 2e31 3034 2d2e 3034 352d 2e31 3938 2d2e  .104-.045-.198-.
-00000540: 3036 342d 2e32 3834 2d2e 3133 3361 312e  064-.284-.133a1.
-00000550: 3331 3220 312e 3331 3220 3020 3030 2d2e  312 1.312 0 00-.
-00000560: 3232 2d2e 3036 3663 2e30 352d 2e30 362e  22-.066c.05-.06.
-00000570: 3134 362d 2e31 3333 2e31 3833 2d2e 3139  146-.133.183-.19
-00000580: 382e 3035 332d 2e31 3238 2e30 3832 2d2e  8.053-.128.082-.
-00000590: 3236 342e 3038 382d 2e34 3032 762d 2e30  264.088-.402v-.0
-000005a0: 3261 312e 3231 2031 2e32 3120 3020 3030  2a1.21 1.21 0 00
-000005b0: 2d2e 3036 312d 2e34 632d 2e30 3435 2d2e  -.061-.4c-.045-.
-000005c0: 3133 342d 2e31 3031 2d2e 322d 2e31 3833  134-.101-.2-.183
-000005d0: 2d2e 3333 332d 2e30 3834 2d2e 3036 362d  -.333-.084-.066-
-000005e0: 2e31 3637 2d2e 3133 322d 2e32 3637 2d2e  .167-.132-.267-.
-000005f0: 3133 3268 2d2e 3031 3663 2d2e 3039 3320  132h-.016c-.093 
-00000600: 302d 2e31 3736 2e30 332d 2e32 3632 2e31  0-.176.03-.262.1
-00000610: 3332 612e 382e 3820 3020 3030 2d2e 3230  32a.8.8 0 00-.20
-00000620: 352e 3333 3420 312e 3138 2031 2e31 3820  5.334 1.18 1.18 
-00000630: 3020 3030 2d2e 3039 2e34 762e 3031 3963  0 00-.09.4v.019c
-00000640: 2e30 3032 2e30 3839 2e30 3038 2e31 3739  .002.089.008.179
-00000650: 2e30 322e 3236 372d 2e31 3933 2d2e 3036  .02.267-.193-.06
-00000660: 372d 2e34 3338 2d2e 3133 352d 2e36 3037  7-.438-.135-.607
-00000670: 2d2e 3230 3261 312e 3633 3520 312e 3633  -.202a1.635 1.63
-00000680: 3520 3020 3031 2d2e 3031 382d 2e32 762d  5 0 01-.018-.2v-
-00000690: 2e30 3261 312e 3737 3220 312e 3737 3220  .02a1.772 1.772 
-000006a0: 3020 3031 2e31 352d 2e37 3638 632e 3038  0 01.15-.768c.08
-000006b0: 322d 2e32 322e 3233 322d 2e34 3036 2e34  2-.22.232-.406.4
-000006c0: 332d 2e35 3333 612e 3938 352e 3938 3520  3-.533a.985.985 
-000006d0: 3020 3031 2e35 3934 2d2e 327a 6d2d 322e  0 01.594-.2zm-2.
-000006e0: 3936 322e 3035 3968 2e30 3336 632e 3134  962.059h.036c.14
-000006f0: 3220 3020 2e32 372e 3034 382e 3339 392e  2 0 .27.048.399.
-00000700: 3133 352e 3134 362e 3132 392e 3236 342e  135.146.129.264.
-00000710: 3238 382e 3334 342e 3436 352e 3039 2e31  288.344.465.09.1
-00000720: 3939 2e31 342e 342e 3135 332e 3636 3776  99.14.4.153.667v
-00000730: 2e30 3034 632e 3030 372e 3133 342e 3030  .004c.007.134.00
-00000740: 362e 322d 2e30 3032 2e32 3636 762e 3038  6.2-.002.266v.08
-00000750: 632d 2e30 332e 3030 372d 2e30 3536 2e30  c-.03.007-.056.0
-00000760: 3138 2d2e 3038 332e 3032 342d 2e31 3532  18-.083.024-.152
-00000770: 2e30 3535 2d2e 3237 342e 3133 352d 2e33  .055-.274.135-.3
-00000780: 3933 2e32 2e30 3132 2d2e 3039 2e30 3133  93.2.012-.09.013
-00000790: 2d2e 3138 2e30 3033 2d2e 3236 3776 2d2e  -.18.003-.267v-.
-000007a0: 3031 3563 2d2e 3031 322d 2e31 3333 2d2e  015c-.012-.133-.
-000007b0: 3034 2d2e 322d 2e30 3832 2d2e 3333 3361  04-.2-.082-.333a
-000007c0: 2e36 3133 2e36 3133 2030 2030 302d 2e31  .613.613 0 00-.1
-000007d0: 3636 2d2e 3236 372e 3234 382e 3234 3820  66-.267.248.248 
-000007e0: 3020 3030 2d2e 3138 332d 2e30 3634 682d  0 00-.183-.064h-
-000007f0: 2e30 3231 632d 2e30 3731 2e30 3036 2d2e  .021c-.071.006-.
-00000800: 3133 2e30 342d 2e31 3836 2e31 3332 612e  13.04-.186.132a.
-00000810: 3535 322e 3535 3220 3020 3030 2d2e 3132  552.552 0 00-.12
-00000820: 2e32 372e 3934 342e 3934 3420 3020 3030  .27.944.944 0 00
-00000830: 2d2e 3032 332e 3333 762e 3031 3563 2e30  -.023.33v.015c.0
-00000840: 3132 2e31 3335 2e30 3337 2e32 2e30 382e  12.135.037.2.08.
-00000850: 3333 342e 3034 362e 3133 342e 3039 382e  334.046.134.098.
-00000860: 322e 3136 362e 3236 382e 3031 2e30 3039  2.166.268.01.009
-00000870: 2e30 322e 3031 382e 3033 342e 3032 342d  .02.018.034.024-
-00000880: 2e30 372e 3035 372d 2e31 3137 2e30 372d  .07.057-.117.07-
-00000890: 2e31 3736 2e31 3336 612e 3330 342e 3330  .176.136a.304.30
-000008a0: 3420 3020 3031 2d2e 3133 312e 3036 3820  4 0 01-.131.068 
-000008b0: 322e 3632 2032 2e36 3220 3020 3031 2d2e  2.62 2.62 0 01-.
-000008c0: 3237 352d 2e34 3032 2031 2e37 3732 2031  275-.402 1.772 1
-000008d0: 2e37 3732 2030 2030 312d 2e31 3535 2d2e  .772 0 01-.155-.
-000008e0: 3636 3720 312e 3735 3920 312e 3735 3920  667 1.759 1.759 
-000008f0: 3020 3031 2e30 382d 2e36 3638 2031 2e34  0 01.08-.668 1.4
-00000900: 3320 312e 3433 2030 2030 312e 3238 332d  3 1.43 0 01.283-
-00000910: 2e35 3335 632e 3132 382d 2e31 3333 2e32  .535c.128-.133.2
-00000920: 362d 2e32 2e34 3138 2d2e 327a 6d31 2e33  6-.2.418-.2zm1.3
-00000930: 3720 312e 3730 3663 2e33 3332 2030 202e  7 1.706c.332 0 .
-00000940: 3733 332e 3036 3520 312e 3231 362e 3339  733.065 1.216.39
-00000950: 392e 3239 332e 322e 3532 332e 3236 3920  9.293.2.523.269 
-00000960: 312e 3035 322e 3436 3868 2e30 3033 632e  1.052.468h.003c.
-00000970: 3235 352e 3133 362e 3430 352e 3236 362e  255.136.405.266.
-00000980: 3437 382e 3339 3976 2d2e 3133 3161 2e35  478.399v-.131a.5
-00000990: 3731 2e35 3731 2030 2030 312e 3031 362e  71.571 0 01.016.
-000009a0: 3437 632d 2e31 3233 2e33 312d 2e35 3136  47c-.123.31-.516
-000009b0: 2e36 3433 2d31 2e30 3633 2e38 3432 762e  .643-1.063.842v.
-000009c0: 3030 3263 2d2e 3236 382e 3133 352d 2e35  002c-.268.135-.5
-000009d0: 3031 2e33 3333 2d2e 3737 352e 3436 352d  01.333-.775.465-
-000009e0: 2e32 3736 2e31 3335 2d2e 3538 382e 3239  .276.135-.588.29
-000009f0: 322d 312e 3031 322e 3236 3761 312e 3133  2-1.012.267a1.13
-00000a00: 3920 312e 3133 3920 3020 3031 2d2e 3434  9 1.139 0 01-.44
-00000a10: 382d 2e30 3637 2033 2e35 3636 2033 2e35  8-.067 3.566 3.5
-00000a20: 3636 2030 2030 312d 2e33 3232 2d2e 3139  66 0 01-.322-.19
-00000a30: 3863 2d2e 3139 352d 2e31 3335 2d2e 3336  8c-.195-.135-.36
-00000a40: 332d 2e33 3332 2d2e 3631 322d 2e34 3635  3-.332-.612-.465
-00000a50: 762d 2e30 3035 682d 2e30 3035 632d 2e34  v-.005h-.005c-.4
-00000a60: 2d2e 3234 362d 2e36 3136 2d2e 3531 322d  -.246-.616-.512-
-00000a70: 2e36 3836 2d2e 3731 2d2e 3037 2d2e 3236  .686-.71-.07-.26
-00000a80: 382d 2e30 3035 2d2e 3437 2e31 3933 2d2e  8-.005-.47.193-.
-00000a90: 362e 3232 342d 2e31 3335 2e33 382d 2e32  6.224-.135.38-.2
-00000aa0: 3731 2e34 3833 2d2e 3333 362e 3130 342d  71.483-.336.104-
-00000ab0: 2e30 3734 2e31 3433 2d2e 3130 322e 3137  .074.143-.102.17
-00000ac0: 362d 2e31 3331 682e 3030 3276 2d2e 3030  6-.131h.002v-.00
-00000ad0: 3363 2e31 3639 2d2e 3230 322e 3433 362d  3c.169-.202.436-
-00000ae0: 2e34 372e 3833 392d 2e36 3031 2e31 3339  .47.839-.601.139
-00000af0: 2d2e 3033 362e 3239 342d 2e30 3635 2e34  -.036.294-.065.4
-00000b00: 3636 2d2e 3036 357a 6d32 2e38 2032 2e31  66-.065zm2.8 2.1
-00000b10: 3432 632e 3335 3820 312e 3431 3720 312e  42c.358 1.417 1.
-00000b20: 3139 3620 332e 3437 3520 312e 3733 3520  196 3.475 1.735 
-00000b30: 342e 3437 332e 3238 362e 3533 342e 3835  4.473.286.534.85
-00000b40: 3520 312e 3635 3920 312e 3130 3220 332e  5 1.659 1.102 3.
-00000b50: 3032 342e 3135 362d 2e30 3035 2e33 332e  024.156-.005.33.
-00000b60: 3031 382e 3531 332e 3036 342e 3634 362d  018.513.064.646-
-00000b70: 312e 3637 312d 2e35 3436 2d33 2e34 3637  1.671-.546-3.467
-00000b80: 2d31 2e30 3839 2d33 2e39 3636 2d2e 3232  -1.089-3.966-.22
-00000b90: 2d2e 322d 2e32 3332 2d2e 3333 352d 2e31  -.2-.232-.335-.1
-00000ba0: 3233 2d2e 3333 352e 3539 2e35 3334 2031  23-.335.59.534 1
-00000bb0: 2e33 3635 2031 2e35 3732 2031 2e36 3436  .365 1.572 1.646
-00000bc0: 2032 2e37 3537 2e31 332e 3533 352e 3136   2.757.13.535.16
-00000bd0: 2031 2e31 3034 2e30 3231 2031 2e36 372e   1.104.021 1.67.
-00000be0: 3036 372e 3032 382e 3133 352e 3036 2e32  067.028.135.06.2
-00000bf0: 3035 2e30 3637 2031 2e30 3332 2e35 3334  05.067 1.032.534
-00000c00: 2031 2e34 3133 2e39 3338 2031 2e32 3320   1.413.938 1.23 
-00000c10: 312e 3533 3776 2d2e 3034 3363 2d2e 3036  1.537v-.043c-.06
-00000c20: 2d2e 3030 332d 2e31 3220 302d 2e31 3820  -.003-.12 0-.18 
-00000c30: 3068 2d2e 3031 3663 2e31 3531 2d2e 3436  0h-.016c.151-.46
-00000c40: 372d 2e31 3832 2d2e 3832 352d 312e 3036  7-.182-.825-1.06
-00000c50: 352d 312e 3232 342d 2e39 3135 2d2e 342d  5-1.224-.915-.4-
-00000c60: 312e 3634 362d 2e33 3336 2d31 2e37 372e  1.646-.336-1.77.
-00000c70: 3436 352d 2e30 3038 2e30 3433 2d2e 3031  465-.008.043-.01
-00000c80: 332e 3036 362d 2e30 3138 2e31 3335 2d2e  3.066-.018.135-.
-00000c90: 3036 382e 3032 332d 2e31 3339 2e30 3533  068.023-.139.053
-00000ca0: 2d2e 3230 392e 3036 342d 2e34 332e 3236  -.209.064-.43.26
-00000cb0: 382d 2e36 3632 2e36 3639 2d2e 3739 3320  8-.662.669-.793 
-00000cc0: 312e 3138 372d 2e31 332e 3533 332d 2e31  1.187-.13.533-.1
-00000cd0: 3720 312e 3135 362d 2e32 3035 2031 2e38  7 1.156-.205 1.8
-00000ce0: 3639 762e 3030 3363 2d2e 3032 2e33 3334  69v.003c-.02.334
-00000cf0: 2d2e 3137 2e38 3338 2d2e 3331 3920 312e  -.17.838-.319 1.
-00000d00: 3335 2d31 2e35 2031 2e30 3732 2d33 2e35  35-1.5 1.072-3.5
-00000d10: 3820 312e 3533 382d 352e 3334 382e 3333  8 1.538-5.348.33
-00000d20: 3461 322e 3634 3520 322e 3634 3520 3020  4a2.645 2.645 0 
-00000d30: 3030 2d2e 3430 322d 2e35 3333 2031 2e34  00-.402-.533 1.4
-00000d40: 3520 312e 3435 2030 2030 302d 2e32 3735  5 1.45 0 00-.275
-00000d50: 2d2e 3333 3363 2e31 3832 2030 202e 3333  -.333c.182 0 .33
-00000d60: 382d 2e30 332e 3436 352d 2e30 3637 612e  8-.03.465-.067a.
-00000d70: 3631 352e 3631 3520 3020 3030 2e33 3134  615.615 0 00.314
-00000d80: 2d2e 3333 3463 2e31 3038 2d2e 3236 3720  -.334c.108-.267 
-00000d90: 302d 2e36 3937 2d2e 3334 352d 312e 3136  0-.697-.345-1.16
-00000da0: 332d 2e33 3435 2d2e 3436 372d 2e39 3331  3-.345-.467-.931
-00000db0: 2d2e 3939 352d 312e 3738 382d 312e 3532  -.995-1.788-1.52
-00000dc0: 312d 2e36 332d 2e34 2d2e 3938 362d 2e38  1-.63-.4-.986-.8
-00000dd0: 372d 312e 3135 2d31 2e33 3936 2d2e 3136  7-1.15-1.396-.16
-00000de0: 352d 2e35 3334 2d2e 3134 332d 312e 3038  5-.534-.143-1.08
-00000df0: 352d 2e30 3135 2d31 2e36 3435 2e32 3435  5-.015-1.645.245
-00000e00: 2d31 2e30 372e 3837 332d 322e 3131 2031  -1.07.873-2.11 1
-00000e10: 2e32 3734 2d32 2e37 3633 2e31 3037 2d2e  .274-2.763.107-.
-00000e20: 3036 352e 3033 372e 3133 352d 2e34 3038  065.037.135-.408
-00000e30: 2e39 3734 2d2e 3339 362e 3735 312d 312e  .974-.396.751-1.
-00000e40: 3134 2032 2e34 3937 2d2e 3132 3220 332e  14 2.497-.122 3.
-00000e50: 3835 3461 382e 3132 3320 382e 3132 3320  854a8.123 8.123 
-00000e60: 3020 3031 2e36 3437 2d32 2e38 3736 632e  0 01.647-2.876c.
-00000e70: 3536 342d 312e 3237 3820 312e 3734 332d  564-1.278 1.743-
-00000e80: 332e 3530 3420 312e 3833 362d 352e 3236  3.504 1.836-5.26
-00000e90: 382e 3034 382e 3033 362e 3231 372e 3133  8.048.036.217.13
-00000ea0: 352e 3238 392e 3230 322e 3231 382e 3133  5.289.202.218.13
-00000eb0: 332e 3338 2e33 3333 2e35 392e 3436 352e  3.38.333.59.465.
-00000ec0: 3231 2e32 3031 2e34 3737 2e33 3335 2e38  21.201.477.335.8
-00000ed0: 3736 2e33 3335 2e30 3339 2e30 3033 2e30  76.335.039.003.0
-00000ee0: 3735 2e30 3036 2e31 312e 3030 362e 3431  75.006.11.006.41
-00000ef0: 3220 3020 2e37 332d 2e31 3334 2e39 3937  2 0 .73-.134.997
-00000f00: 2d2e 3236 382e 3239 2d2e 3133 342e 3532  -.268.29-.134.52
-00000f10: 2d2e 3333 342e 3734 2d2e 3468 2e30 3035  -.334.74-.4h.005
-00000f20: 632e 3436 372d 2e31 3335 2e38 3335 2d2e  c.467-.135.835-.
-00000f30: 3430 3220 312e 3034 342d 2e37 7a6d 322e  402 1.044-.7zm2.
-00000f40: 3138 3520 382e 3935 3863 2e30 3337 2e36  185 8.958c.037.6
-00000f50: 2e33 3433 2031 2e32 3435 2e38 3832 2031  .343 1.245.882 1
-00000f60: 2e33 3737 2e35 3838 2e31 3334 2031 2e34  .377.588.134 1.4
-00000f70: 3334 2d2e 3333 3320 312e 3739 312d 2e37  34-.333 1.791-.7
-00000f80: 3635 6c2e 3231 312d 2e30 3163 2e33 3135  65l.211-.01c.315
-00000f90: 2d2e 3030 372e 3537 372e 3031 2e38 3437  -.007.577.01.847
-00000fa0: 2e32 3638 6c2e 3030 332e 3030 3363 2e32  .268l.003.003c.2
-00000fb0: 3038 2e31 3939 2e33 3035 2e35 332e 3339  08.199.305.53.39
-00000fc0: 312e 3837 362e 3038 352e 342e 3135 342e  1.876.085.4.154.
-00000fd0: 3738 2e34 3039 2031 2e30 3636 2e34 3836  78.409 1.066.486
-00000fe0: 2e35 3237 2e36 3435 2e39 3036 2e36 3336  .527.645.906.636
-00000ff0: 2031 2e31 346c 2e30 3033 2d2e 3030 3776   1.14l.003-.007v
-00001000: 2e30 3138 6c2d 2e30 3033 2d2e 3031 3263  .018l-.003-.012c
-00001010: 2d2e 3031 352e 3236 322d 2e31 3835 2e33  -.015.262-.185.3
-00001020: 3936 2d2e 3439 382e 3539 352d 2e36 332e  96-.498.595-.63.
-00001030: 3430 312d 312e 3734 362e 3731 322d 322e  401-1.746.712-2.
-00001040: 3435 3720 312e 3537 2d2e 3631 382e 3733  457 1.57-.618.73
-00001050: 372d 312e 3337 2031 2e31 342d 322e 3033  7-1.37 1.14-2.03
-00001060: 3620 312e 3139 312d 2e36 3634 2e30 3533  6 1.191-.664.053
-00001070: 2d31 2e32 3337 2d2e 322d 312e 3537 342d  -1.237-.2-1.574-
-00001080: 2e38 3938 6c2d 2e30 3035 2d2e 3030 3363  .898l-.005-.003c
-00001090: 2d2e 3231 2d2e 342d 2e31 322d 312e 3032  -.21-.4-.12-1.02
-000010a0: 352e 3035 362d 312e 3639 2e31 3736 2d2e  5.056-1.69.176-.
-000010b0: 3636 382e 3432 382d 312e 3334 342e 3436  668.428-1.344.46
-000010c0: 332d 312e 3839 372e 3033 372d 2e37 3134  3-1.897.037-.714
-000010d0: 2e30 3736 2d31 2e33 3335 2e31 3935 2d31  .076-1.335.195-1
-000010e0: 2e38 3134 2e31 322d 2e34 3635 2e33 3038  .814.12-.465.308
-000010f0: 2d2e 3739 372e 3634 312d 2e39 3834 6c2e  -.797.641-.984l.
-00001100: 3034 352d 2e30 3232 7a6d 2d31 302e 3831  045-.022zm-10.81
-00001110: 342e 3034 3968 2e30 3163 2e30 3533 2030  4.049h.01c.053 0
-00001120: 202e 3130 352e 3030 352e 3135 372e 3031   .105.005.157.01
-00001130: 342e 3337 362e 3035 352e 3730 362e 3333  4.376.055.706.33
-00001140: 3320 312e 3032 332e 3735 326c 2e39 3120  3 1.023.752l.91 
-00001150: 312e 3636 342e 3030 332e 3030 3363 2e32  1.664.003.003c.2
-00001160: 3433 2e35 3333 2e37 3534 2031 2e30 3634  43.533.754 1.064
-00001170: 2031 2e31 3839 2031 2e36 3337 2e34 3334   1.189 1.637.434
-00001180: 2e35 3938 2e37 3720 312e 3133 312e 3732  .598.77 1.131.72
-00001190: 3920 312e 3537 762e 3030 3663 2d2e 3035  9 1.57v.006c-.05
-000011a0: 372e 3734 342d 2e34 3820 312e 3134 382d  7.744-.48 1.148-
-000011b0: 312e 3132 3520 312e 3239 342d 2e36 3435  1.125 1.294-.645
-000011c0: 2e31 3335 2d31 2e35 322e 3030 322d 322e  .135-1.52.002-2.
-000011d0: 3339 352d 2e34 3634 2d2e 3936 382d 2e35  395-.464-.968-.5
-000011e0: 3336 2d32 2e31 3138 2d2e 3436 392d 322e  36-2.118-.469-2.
-000011f0: 3835 372d 2e36 3032 2d2e 3336 392d 2e30  857-.602-.369-.0
-00001200: 3636 2d2e 3631 2d2e 322d 2e37 3233 2d2e  66-.61-.2-.723-.
-00001210: 342d 2e31 312d 2e32 2d2e 3131 332d 2e36  4-.11-.2-.113-.6
-00001220: 3032 2e31 3233 2d31 2e32 3376 2d2e 3030  02.123-1.23v-.00
-00001230: 346c 2e30 3032 2d2e 3030 3363 2e31 3137  4l.002-.003c.117
-00001240: 2d2e 3333 342e 3033 2d2e 3735 322d 2e30  -.334.03-.752-.0
-00001250: 3237 2d31 2e31 3138 2d2e 3035 352d 2e34  27-1.118-.055-.4
-00001260: 3031 2d2e 3038 332d 2e37 312e 3034 332d  01-.083-.71.043-
-00001270: 2e39 342e 3136 2d2e 3333 342e 3339 362d  .94.16-.334.396-
-00001280: 2e34 2e36 392d 2e35 3333 2e32 3934 2d2e  .4.69-.533.294-.
-00001290: 3133 352e 3634 2d2e 3230 322e 3931 352d  135.64-.202.915-
-000012a0: 2e34 3768 2e30 3032 762d 2e30 3032 632e  .47h.002v-.002c.
-000012b0: 3235 362d 2e32 3638 2e34 3435 2d2e 3630  256-.268.445-.60
-000012c0: 312e 3636 382d 2e38 3338 2e31 392d 2e32  1.668-.838.19-.2
-000012d0: 3031 2e33 382d 2e33 3336 2e36 3633 2d2e  01.38-.336.663-.
-000012e0: 3333 367a 6d37 2e31 3539 2d39 2e30 3734  336zm7.159-9.074
-000012f0: 632d 2e34 3335 2e32 3031 2d2e 3934 352e  c-.435.201-.945.
-00001300: 3533 352d 312e 3438 382e 3533 352d 2e35  535-1.488.535-.5
-00001310: 3432 2030 2d2e 3937 2d2e 3236 372d 312e  42 0-.97-.267-1.
-00001320: 3238 2d2e 3436 362d 2e31 3534 2d2e 3133  28-.466-.154-.13
-00001330: 342d 2e32 382d 2e32 3638 2d2e 3337 332d  4-.28-.268-.373-
-00001340: 2e33 3335 2d2e 3136 342d 2e31 3334 2d2e  .335-.164-.134-.
-00001350: 3134 342d 2e33 3333 2d2e 3037 342d 2e33  144-.333-.074-.3
-00001360: 3333 2e31 3039 2e30 3136 2e31 3239 2e31  33.109.016.129.1
-00001370: 3334 2e31 3939 2e32 2e30 3936 2e30 3636  34.199.2.096.066
-00001380: 2e32 3135 2e32 2e33 362e 3333 332e 3239  .215.2.36.333.29
-00001390: 322e 322e 3638 2e34 3637 2031 2e31 3637  2.2.68.467 1.167
-000013a0: 2e34 3637 2e34 3835 2030 2031 2e30 3533  .467.485 0 1.053
-000013b0: 2d2e 3236 3720 312e 3339 382d 2e34 3636  -.267 1.398-.466
-000013c0: 2e31 3935 2d2e 3133 352e 3434 352d 2e33  .195-.135.445-.3
-000013d0: 3334 2e36 3438 2d2e 3436 372e 3135 362d  34.648-.467.156-
-000013e0: 2e31 3336 2e31 3439 2d2e 3236 372e 3237  .136.149-.267.27
-000013f0: 392d 2e32 3637 2e31 3238 2e30 3136 2e30  9-.267.128.016.0
-00001400: 3334 2e31 3334 2d2e 3134 372e 3333 3261  34.134-.147.332a
-00001410: 382e 3039 3720 382e 3039 3720 3020 3031  8.097 8.097 0 01
-00001420: 2d2e 3639 2e34 3638 7a6d 2d31 2e30 3832  -.69.468zm-1.082
-00001430: 2d31 2e35 3833 5635 2e36 3463 2d2e 3030  -1.583V5.64c-.00
-00001440: 362d 2e30 322e 3031 332d 2e30 3432 2e30  6-.02.013-.042.0
-00001450: 3239 2d2e 3035 2e30 3734 2d2e 3034 332e  29-.05.074-.043.
-00001460: 3138 2d2e 3032 372e 3236 2e30 3034 2e30  18-.027.26.004.0
-00001470: 3633 2030 202e 3136 2e30 3637 2e31 352e  63 0 .16.067.15.
-00001480: 3133 352d 2e30 3036 2e30 3439 2d2e 3038  135-.006.049-.08
-00001490: 352e 3036 362d 2e31 3335 2e30 3636 2d2e  5.066-.135.066-.
-000014a0: 3035 3520 302d 2e30 3932 2d2e 3034 332d  055 0-.092-.043-
-000014b0: 2e31 3431 2d2e 3036 382d 2e30 3532 2d2e  .141-.068-.052-.
-000014c0: 3031 382d 2e31 3436 2d2e 3030 382d 2e31  018-.146-.008-.1
-000014d0: 3633 2d2e 3036 357a 6d2d 2e35 3531 2030  63-.065zm-.551 0
-000014e0: 632d 2e30 322e 3035 382d 2e31 3133 2e30  c-.02.058-.113.0
-000014f0: 3439 2d2e 3136 362e 3036 362d 2e30 3437  49-.166.066-.047
-00001500: 2e30 3235 2d2e 3038 362e 3036 382d 2e31  .025-.086.068-.1
-00001510: 342e 3036 382d 2e30 3520 302d 2e31 332d  4.068-.05 0-.13-
-00001520: 2e30 322d 2e31 3336 2d2e 3036 382d 2e30  .02-.136-.068-.0
-00001530: 312d 2e30 3636 2e30 3838 2d2e 3133 332e  1-.066.088-.133.
-00001540: 3135 2d2e 3133 332e 3038 2d2e 3033 312e  15-.133.08-.031.
-00001550: 3138 342d 2e30 3437 2e32 3539 2d2e 3030  184-.047.259-.00
-00001560: 352e 3031 392e 3030 392e 3033 362e 3033  5.019.009.036.03
-00001570: 2e30 332e 3035 762e 3032 682e 3030 337a  .03.05v.02h.003z
-00001580: 222f 3e0d 0a3c 2f73 7667 3e              "/>..</svg>
+00000000: 3c73 7667 200a 2020 726f 6c65 3d22 696d  <svg .  role="im
+00000010: 6722 200a 2020 7669 6577 426f 783d 2230  g" .  viewBox="0
+00000020: 2030 2032 3420 3234 2220 0a20 2078 6d6c   0 24 24" .  xml
+00000030: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+00000040: 332e 6f72 672f 3230 3030 2f73 7667 223e  3.org/2000/svg">
+00000050: 0a20 203c 7469 746c 653e 4c69 6e75 783c  .  <title>Linux<
+00000060: 2f74 6974 6c65 3e0a 3e0a 2020 3c70 6174  /title>.>.  <pat
+00000070: 6820 0a20 2066 696c 6c3d 2263 7572 7265  h .  fill="curre
+00000080: 6e74 436f 6c6f 7222 0a20 2064 3d22 4d31  ntColor".  d="M1
+00000090: 322e 3530 3420 3063 2d2e 3135 3520 302d  2.504 0c-.155 0-
+000000a0: 2e33 3135 2e30 3038 2d2e 3438 2e30 3231  .315.008-.48.021
+000000b0: 2d34 2e32 3236 2e33 3333 2d33 2e31 3035  -4.226.333-3.105
+000000c0: 2034 2e38 3037 2d33 2e31 3720 362e 3239   4.807-3.17 6.29
+000000d0: 382d 2e30 3736 2031 2e30 3932 2d2e 3320  8-.076 1.092-.3 
+000000e0: 312e 3935 332d 312e 3035 2033 2e30 322d  1.953-1.05 3.02-
+000000f0: 2e38 3835 2031 2e30 3531 2d32 2e31 3237  .885 1.051-2.127
+00000100: 2032 2e37 352d 322e 3731 3620 342e 3532   2.75-2.716 4.52
+00000110: 312d 2e32 3738 2e38 3332 2d2e 3431 2031  1-.278.832-.41 1
+00000120: 2e36 3834 2d2e 3238 3720 322e 3438 3961  .684-.287 2.489a
+00000130: 2e34 3234 2e34 3234 2030 2030 302d 2e31  .424.424 0 00-.1
+00000140: 312e 3133 3563 2d2e 3236 2e32 3638 2d2e  1.135c-.26.268-.
+00000150: 3435 2e36 2d2e 3636 332e 3833 392d 2e31  45.6-.663.839-.1
+00000160: 3939 2e31 3939 2d2e 3438 352e 3236 372d  99.199-.485.267-
+00000170: 2e37 3937 2e34 2d2e 3331 332e 3133 362d  .797.4-.313.136-
+00000180: 2e36 3538 2e32 3639 2d2e 3836 342e 3638  .658.269-.864.68
+00000190: 2d2e 3039 2e31 3839 2d2e 3133 362e 3339  -.09.189-.136.39
+000001a0: 342d 2e31 3332 2e36 3032 2030 202e 3139  4-.132.602 0 .19
+000001b0: 392e 3032 372e 342e 3035 352e 3533 362e  9.027.4.055.536.
+000001c0: 3035 382e 3339 392e 3131 362e 3732 382e  058.399.116.728.
+000001d0: 3034 2e39 372d 2e32 3439 2e36 382d 2e32  04.97-.249.68-.2
+000001e0: 3820 312e 3134 352d 2e31 3036 2031 2e34  8 1.145-.106 1.4
+000001f0: 3834 2e31 3734 2e33 3334 2e35 3335 2e34  84.174.334.535.4
+00000200: 372e 3934 2e36 3031 2e38 312e 3220 312e  7.94.601.81.2 1.
+00000210: 3931 2e31 3335 2032 2e37 3734 2e36 2e39  91.135 2.774.6.9
+00000220: 3236 2e34 3636 2031 2e38 3636 2e36 3720  26.466 1.866.67 
+00000230: 322e 3631 362e 3437 2e35 3236 2d2e 3131  2.616.47.526-.11
+00000240: 362e 3937 2d2e 3436 3420 312e 3230 382d  6.97-.464 1.208-
+00000250: 2e39 3436 2e35 3837 2d2e 3030 3320 312e  .946.587-.003 1.
+00000260: 3233 2d2e 3236 3920 322e 3236 2d2e 3333  23-.269 2.26-.33
+00000270: 342e 3639 392d 2e30 3538 2031 2e35 3734  4.699-.058 1.574
+00000280: 2e32 3637 2032 2e35 3737 2e32 2e30 3235  .267 2.577.2.025
+00000290: 2e31 3334 2e30 3633 2e31 3938 2e31 3134  .134.063.198.114
+000002a0: 2e33 3333 6c2e 3030 332e 3030 3363 2e33  .333l.003.003c.3
+000002b0: 3931 2e37 3738 2031 2e31 3133 2031 2e31  91.778 1.113 1.1
+000002c0: 3332 2031 2e38 3834 2031 2e30 3731 2e37  32 1.884 1.071.7
+000002d0: 3731 2d2e 3036 2031 2e35 3932 2d2e 3533  71-.06 1.592-.53
+000002e0: 3620 322e 3235 372d 312e 3330 362e 3633  6 2.257-1.306.63
+000002f0: 312d 2e37 3635 2031 2e36 3833 2d31 2e30  1-.765 1.683-1.0
+00000300: 3834 2032 2e33 3738 2d31 2e35 3033 2e33  84 2.378-1.503.3
+00000310: 3438 2d2e 3139 392e 3632 392d 2e34 3639  48-.199.629-.469
+00000320: 2e36 3439 2d2e 3835 332e 3032 332d 2e34  .649-.853.023-.4
+00000330: 2d2e 322d 2e38 3131 2d2e 3731 342d 312e  -.2-.811-.714-1.
+00000340: 3337 3676 2d2e 3039 376c 2d2e 3030 332d  376v-.097l-.003-
+00000350: 2e30 3033 632d 2e31 372d 2e32 2d2e 3235  .003c-.17-.2-.25
+00000360: 2d2e 3533 352d 2e33 3338 2d2e 3932 362d  -.535-.338-.926-
+00000370: 2e30 3835 2d2e 3430 312d 2e31 3832 2d2e  .085-.401-.182-.
+00000380: 3738 362d 2e34 3932 2d31 2e30 3436 682d  786-.492-1.046h-
+00000390: 2e30 3033 632d 2e30 3539 2d2e 3035 342d  .003c-.059-.054-
+000003a0: 2e31 3233 2d2e 3036 372d 2e31 3838 2d2e  .123-.067-.188-.
+000003b0: 3133 3561 2e33 3537 2e33 3537 2030 2030  135a.357.357 0 0
+000003c0: 302d 2e31 392d 2e30 3634 632e 3433 312d  0-.19-.064c.431-
+000003d0: 312e 3237 382e 3236 342d 322e 3535 2d2e  1.278.264-2.55-.
+000003e0: 3137 332d 332e 3639 342d 2e35 3333 2d31  173-3.694-.533-1
+000003f0: 2e34 312d 312e 3436 352d 322e 3633 382d  .41-1.465-2.638-
+00000400: 322e 3137 352d 332e 3438 332d 2e37 3936  2.175-3.483-.796
+00000410: 2d31 2e30 3035 2d31 2e35 3736 2d31 2e39  -1.005-1.576-1.9
+00000420: 3537 2d31 2e35 362d 332e 3336 382e 3032  57-1.56-3.368.02
+00000430: 362d 322e 3135 322e 3233 362d 362e 3133  6-2.152.236-6.13
+00000440: 332d 332e 3534 342d 362e 3133 397a 6d2e  3-3.544-6.139zm.
+00000450: 3532 3920 332e 3430 3568 2e30 3133 632e  529 3.405h.013c.
+00000460: 3231 3320 3020 2e33 3936 2e30 3632 2e35  213 0 .396.062.5
+00000470: 3834 2e31 3938 2e31 392e 3133 352e 3333  84.198.19.135.33
+00000480: 2e33 3332 2e34 3338 2e35 3333 2e31 3035  .332.438.533.105
+00000490: 2e32 3539 2e31 3538 2e34 3539 2e31 3636  .259.158.459.166
+000004a0: 2e37 3234 2030 2d2e 3032 2e30 3036 2d2e  .724 0-.02.006-.
+000004b0: 3034 2e30 3036 2d2e 3036 762e 3130 3561  04.006-.06v.105a
+000004c0: 2e30 3836 2e30 3836 2030 2030 312d 2e30  .086.086 0 01-.0
+000004d0: 3034 2d2e 3032 316c 2d2e 3030 342d 2e30  04-.021l-.004-.0
+000004e0: 3234 6131 2e38 3037 2031 2e38 3037 2030  24a1.807 1.807 0
+000004f0: 2030 312d 2e31 352e 3730 362e 3935 332e   01-.15.706.953.
+00000500: 3935 3320 3020 3031 2d2e 3231 332e 3333  953 0 01-.213.33
+00000510: 352e 3731 2e37 3120 3020 3030 2d2e 3038  5.71.71 0 00-.08
+00000520: 382d 2e30 3432 632d 2e31 3034 2d2e 3034  8-.042c-.104-.04
+00000530: 352d 2e31 3938 2d2e 3036 342d 2e32 3834  5-.198-.064-.284
+00000540: 2d2e 3133 3361 312e 3331 3220 312e 3331  -.133a1.312 1.31
+00000550: 3220 3020 3030 2d2e 3232 2d2e 3036 3663  2 0 00-.22-.066c
+00000560: 2e30 352d 2e30 362e 3134 362d 2e31 3333  .05-.06.146-.133
+00000570: 2e31 3833 2d2e 3139 382e 3035 332d 2e31  .183-.198.053-.1
+00000580: 3238 2e30 3832 2d2e 3236 342e 3038 382d  28.082-.264.088-
+00000590: 2e34 3032 762d 2e30 3261 312e 3231 2031  .402v-.02a1.21 1
+000005a0: 2e32 3120 3020 3030 2d2e 3036 312d 2e34  .21 0 00-.061-.4
+000005b0: 632d 2e30 3435 2d2e 3133 342d 2e31 3031  c-.045-.134-.101
+000005c0: 2d2e 322d 2e31 3833 2d2e 3333 332d 2e30  -.2-.183-.333-.0
+000005d0: 3834 2d2e 3036 362d 2e31 3637 2d2e 3133  84-.066-.167-.13
+000005e0: 322d 2e32 3637 2d2e 3133 3268 2d2e 3031  2-.267-.132h-.01
+000005f0: 3663 2d2e 3039 3320 302d 2e31 3736 2e30  6c-.093 0-.176.0
+00000600: 332d 2e32 3632 2e31 3332 612e 382e 3820  3-.262.132a.8.8 
+00000610: 3020 3030 2d2e 3230 352e 3333 3420 312e  0 00-.205.334 1.
+00000620: 3138 2031 2e31 3820 3020 3030 2d2e 3039  18 1.18 0 00-.09
+00000630: 2e34 762e 3031 3963 2e30 3032 2e30 3839  .4v.019c.002.089
+00000640: 2e30 3038 2e31 3739 2e30 322e 3236 372d  .008.179.02.267-
+00000650: 2e31 3933 2d2e 3036 372d 2e34 3338 2d2e  .193-.067-.438-.
+00000660: 3133 352d 2e36 3037 2d2e 3230 3261 312e  135-.607-.202a1.
+00000670: 3633 3520 312e 3633 3520 3020 3031 2d2e  635 1.635 0 01-.
+00000680: 3031 382d 2e32 762d 2e30 3261 312e 3737  018-.2v-.02a1.77
+00000690: 3220 312e 3737 3220 3020 3031 2e31 352d  2 1.772 0 01.15-
+000006a0: 2e37 3638 632e 3038 322d 2e32 322e 3233  .768c.082-.22.23
+000006b0: 322d 2e34 3036 2e34 332d 2e35 3333 612e  2-.406.43-.533a.
+000006c0: 3938 352e 3938 3520 3020 3031 2e35 3934  985.985 0 01.594
+000006d0: 2d2e 327a 6d2d 322e 3936 322e 3035 3968  -.2zm-2.962.059h
+000006e0: 2e30 3336 632e 3134 3220 3020 2e32 372e  .036c.142 0 .27.
+000006f0: 3034 382e 3339 392e 3133 352e 3134 362e  048.399.135.146.
+00000700: 3132 392e 3236 342e 3238 382e 3334 342e  129.264.288.344.
+00000710: 3436 352e 3039 2e31 3939 2e31 342e 342e  465.09.199.14.4.
+00000720: 3135 332e 3636 3776 2e30 3034 632e 3030  153.667v.004c.00
+00000730: 372e 3133 342e 3030 362e 322d 2e30 3032  7.134.006.2-.002
+00000740: 2e32 3636 762e 3038 632d 2e30 332e 3030  .266v.08c-.03.00
+00000750: 372d 2e30 3536 2e30 3138 2d2e 3038 332e  7-.056.018-.083.
+00000760: 3032 342d 2e31 3532 2e30 3535 2d2e 3237  024-.152.055-.27
+00000770: 342e 3133 352d 2e33 3933 2e32 2e30 3132  4.135-.393.2.012
+00000780: 2d2e 3039 2e30 3133 2d2e 3138 2e30 3033  -.09.013-.18.003
+00000790: 2d2e 3236 3776 2d2e 3031 3563 2d2e 3031  -.267v-.015c-.01
+000007a0: 322d 2e31 3333 2d2e 3034 2d2e 322d 2e30  2-.133-.04-.2-.0
+000007b0: 3832 2d2e 3333 3361 2e36 3133 2e36 3133  82-.333a.613.613
+000007c0: 2030 2030 302d 2e31 3636 2d2e 3236 372e   0 00-.166-.267.
+000007d0: 3234 382e 3234 3820 3020 3030 2d2e 3138  248.248 0 00-.18
+000007e0: 332d 2e30 3634 682d 2e30 3231 632d 2e30  3-.064h-.021c-.0
+000007f0: 3731 2e30 3036 2d2e 3133 2e30 342d 2e31  71.006-.13.04-.1
+00000800: 3836 2e31 3332 612e 3535 322e 3535 3220  86.132a.552.552 
+00000810: 3020 3030 2d2e 3132 2e32 372e 3934 342e  0 00-.12.27.944.
+00000820: 3934 3420 3020 3030 2d2e 3032 332e 3333  944 0 00-.023.33
+00000830: 762e 3031 3563 2e30 3132 2e31 3335 2e30  v.015c.012.135.0
+00000840: 3337 2e32 2e30 382e 3333 342e 3034 362e  37.2.08.334.046.
+00000850: 3133 342e 3039 382e 322e 3136 362e 3236  134.098.2.166.26
+00000860: 382e 3031 2e30 3039 2e30 322e 3031 382e  8.01.009.02.018.
+00000870: 3033 342e 3032 342d 2e30 372e 3035 372d  034.024-.07.057-
+00000880: 2e31 3137 2e30 372d 2e31 3736 2e31 3336  .117.07-.176.136
+00000890: 612e 3330 342e 3330 3420 3020 3031 2d2e  a.304.304 0 01-.
+000008a0: 3133 312e 3036 3820 322e 3632 2032 2e36  131.068 2.62 2.6
+000008b0: 3220 3020 3031 2d2e 3237 352d 2e34 3032  2 0 01-.275-.402
+000008c0: 2031 2e37 3732 2031 2e37 3732 2030 2030   1.772 1.772 0 0
+000008d0: 312d 2e31 3535 2d2e 3636 3720 312e 3735  1-.155-.667 1.75
+000008e0: 3920 312e 3735 3920 3020 3031 2e30 382d  9 1.759 0 01.08-
+000008f0: 2e36 3638 2031 2e34 3320 312e 3433 2030  .668 1.43 1.43 0
+00000900: 2030 312e 3238 332d 2e35 3335 632e 3132   01.283-.535c.12
+00000910: 382d 2e31 3333 2e32 362d 2e32 2e34 3138  8-.133.26-.2.418
+00000920: 2d2e 327a 6d31 2e33 3720 312e 3730 3663  -.2zm1.37 1.706c
+00000930: 2e33 3332 2030 202e 3733 332e 3036 3520  .332 0 .733.065 
+00000940: 312e 3231 362e 3339 392e 3239 332e 322e  1.216.399.293.2.
+00000950: 3532 332e 3236 3920 312e 3035 322e 3436  523.269 1.052.46
+00000960: 3868 2e30 3033 632e 3235 352e 3133 362e  8h.003c.255.136.
+00000970: 3430 352e 3236 362e 3437 382e 3339 3976  405.266.478.399v
+00000980: 2d2e 3133 3161 2e35 3731 2e35 3731 2030  -.131a.571.571 0
+00000990: 2030 312e 3031 362e 3437 632d 2e31 3233   01.016.47c-.123
+000009a0: 2e33 312d 2e35 3136 2e36 3433 2d31 2e30  .31-.516.643-1.0
+000009b0: 3633 2e38 3432 762e 3030 3263 2d2e 3236  63.842v.002c-.26
+000009c0: 382e 3133 352d 2e35 3031 2e33 3333 2d2e  8.135-.501.333-.
+000009d0: 3737 352e 3436 352d 2e32 3736 2e31 3335  775.465-.276.135
+000009e0: 2d2e 3538 382e 3239 322d 312e 3031 322e  -.588.292-1.012.
+000009f0: 3236 3761 312e 3133 3920 312e 3133 3920  267a1.139 1.139 
+00000a00: 3020 3031 2d2e 3434 382d 2e30 3637 2033  0 01-.448-.067 3
+00000a10: 2e35 3636 2033 2e35 3636 2030 2030 312d  .566 3.566 0 01-
+00000a20: 2e33 3232 2d2e 3139 3863 2d2e 3139 352d  .322-.198c-.195-
+00000a30: 2e31 3335 2d2e 3336 332d 2e33 3332 2d2e  .135-.363-.332-.
+00000a40: 3631 322d 2e34 3635 762d 2e30 3035 682d  612-.465v-.005h-
+00000a50: 2e30 3035 632d 2e34 2d2e 3234 362d 2e36  .005c-.4-.246-.6
+00000a60: 3136 2d2e 3531 322d 2e36 3836 2d2e 3731  16-.512-.686-.71
+00000a70: 2d2e 3037 2d2e 3236 382d 2e30 3035 2d2e  -.07-.268-.005-.
+00000a80: 3437 2e31 3933 2d2e 362e 3232 342d 2e31  47.193-.6.224-.1
+00000a90: 3335 2e33 382d 2e32 3731 2e34 3833 2d2e  35.38-.271.483-.
+00000aa0: 3333 362e 3130 342d 2e30 3734 2e31 3433  336.104-.074.143
+00000ab0: 2d2e 3130 322e 3137 362d 2e31 3331 682e  -.102.176-.131h.
+00000ac0: 3030 3276 2d2e 3030 3363 2e31 3639 2d2e  002v-.003c.169-.
+00000ad0: 3230 322e 3433 362d 2e34 372e 3833 392d  202.436-.47.839-
+00000ae0: 2e36 3031 2e31 3339 2d2e 3033 362e 3239  .601.139-.036.29
+00000af0: 342d 2e30 3635 2e34 3636 2d2e 3036 357a  4-.065.466-.065z
+00000b00: 6d32 2e38 2032 2e31 3432 632e 3335 3820  m2.8 2.142c.358 
+00000b10: 312e 3431 3720 312e 3139 3620 332e 3437  1.417 1.196 3.47
+00000b20: 3520 312e 3733 3520 342e 3437 332e 3238  5 1.735 4.473.28
+00000b30: 362e 3533 342e 3835 3520 312e 3635 3920  6.534.855 1.659 
+00000b40: 312e 3130 3220 332e 3032 342e 3135 362d  1.102 3.024.156-
+00000b50: 2e30 3035 2e33 332e 3031 382e 3531 332e  .005.33.018.513.
+00000b60: 3036 342e 3634 362d 312e 3637 312d 2e35  064.646-1.671-.5
+00000b70: 3436 2d33 2e34 3637 2d31 2e30 3839 2d33  46-3.467-1.089-3
+00000b80: 2e39 3636 2d2e 3232 2d2e 322d 2e32 3332  .966-.22-.2-.232
+00000b90: 2d2e 3333 352d 2e31 3233 2d2e 3333 352e  -.335-.123-.335.
+00000ba0: 3539 2e35 3334 2031 2e33 3635 2031 2e35  59.534 1.365 1.5
+00000bb0: 3732 2031 2e36 3436 2032 2e37 3537 2e31  72 1.646 2.757.1
+00000bc0: 332e 3533 352e 3136 2031 2e31 3034 2e30  3.535.16 1.104.0
+00000bd0: 3231 2031 2e36 372e 3036 372e 3032 382e  21 1.67.067.028.
+00000be0: 3133 352e 3036 2e32 3035 2e30 3637 2031  135.06.205.067 1
+00000bf0: 2e30 3332 2e35 3334 2031 2e34 3133 2e39  .032.534 1.413.9
+00000c00: 3338 2031 2e32 3320 312e 3533 3776 2d2e  38 1.23 1.537v-.
+00000c10: 3034 3363 2d2e 3036 2d2e 3030 332d 2e31  043c-.06-.003-.1
+00000c20: 3220 302d 2e31 3820 3068 2d2e 3031 3663  2 0-.18 0h-.016c
+00000c30: 2e31 3531 2d2e 3436 372d 2e31 3832 2d2e  .151-.467-.182-.
+00000c40: 3832 352d 312e 3036 352d 312e 3232 342d  825-1.065-1.224-
+00000c50: 2e39 3135 2d2e 342d 312e 3634 362d 2e33  .915-.4-1.646-.3
+00000c60: 3336 2d31 2e37 372e 3436 352d 2e30 3038  36-1.77.465-.008
+00000c70: 2e30 3433 2d2e 3031 332e 3036 362d 2e30  .043-.013.066-.0
+00000c80: 3138 2e31 3335 2d2e 3036 382e 3032 332d  18.135-.068.023-
+00000c90: 2e31 3339 2e30 3533 2d2e 3230 392e 3036  .139.053-.209.06
+00000ca0: 342d 2e34 332e 3236 382d 2e36 3632 2e36  4-.43.268-.662.6
+00000cb0: 3639 2d2e 3739 3320 312e 3138 372d 2e31  69-.793 1.187-.1
+00000cc0: 332e 3533 332d 2e31 3720 312e 3135 362d  3.533-.17 1.156-
+00000cd0: 2e32 3035 2031 2e38 3639 762e 3030 3363  .205 1.869v.003c
+00000ce0: 2d2e 3032 2e33 3334 2d2e 3137 2e38 3338  -.02.334-.17.838
+00000cf0: 2d2e 3331 3920 312e 3335 2d31 2e35 2031  -.319 1.35-1.5 1
+00000d00: 2e30 3732 2d33 2e35 3820 312e 3533 382d  .072-3.58 1.538-
+00000d10: 352e 3334 382e 3333 3461 322e 3634 3520  5.348.334a2.645 
+00000d20: 322e 3634 3520 3020 3030 2d2e 3430 322d  2.645 0 00-.402-
+00000d30: 2e35 3333 2031 2e34 3520 312e 3435 2030  .533 1.45 1.45 0
+00000d40: 2030 302d 2e32 3735 2d2e 3333 3363 2e31   00-.275-.333c.1
+00000d50: 3832 2030 202e 3333 382d 2e30 332e 3436  82 0 .338-.03.46
+00000d60: 352d 2e30 3637 612e 3631 352e 3631 3520  5-.067a.615.615 
+00000d70: 3020 3030 2e33 3134 2d2e 3333 3463 2e31  0 00.314-.334c.1
+00000d80: 3038 2d2e 3236 3720 302d 2e36 3937 2d2e  08-.267 0-.697-.
+00000d90: 3334 352d 312e 3136 332d 2e33 3435 2d2e  345-1.163-.345-.
+00000da0: 3436 372d 2e39 3331 2d2e 3939 352d 312e  467-.931-.995-1.
+00000db0: 3738 382d 312e 3532 312d 2e36 332d 2e34  788-1.521-.63-.4
+00000dc0: 2d2e 3938 362d 2e38 372d 312e 3135 2d31  -.986-.87-1.15-1
+00000dd0: 2e33 3936 2d2e 3136 352d 2e35 3334 2d2e  .396-.165-.534-.
+00000de0: 3134 332d 312e 3038 352d 2e30 3135 2d31  143-1.085-.015-1
+00000df0: 2e36 3435 2e32 3435 2d31 2e30 372e 3837  .645.245-1.07.87
+00000e00: 332d 322e 3131 2031 2e32 3734 2d32 2e37  3-2.11 1.274-2.7
+00000e10: 3633 2e31 3037 2d2e 3036 352e 3033 372e  63.107-.065.037.
+00000e20: 3133 352d 2e34 3038 2e39 3734 2d2e 3339  135-.408.974-.39
+00000e30: 362e 3735 312d 312e 3134 2032 2e34 3937  6.751-1.14 2.497
+00000e40: 2d2e 3132 3220 332e 3835 3461 382e 3132  -.122 3.854a8.12
+00000e50: 3320 382e 3132 3320 3020 3031 2e36 3437  3 8.123 0 01.647
+00000e60: 2d32 2e38 3736 632e 3536 342d 312e 3237  -2.876c.564-1.27
+00000e70: 3820 312e 3734 332d 332e 3530 3420 312e  8 1.743-3.504 1.
+00000e80: 3833 362d 352e 3236 382e 3034 382e 3033  836-5.268.048.03
+00000e90: 362e 3231 372e 3133 352e 3238 392e 3230  6.217.135.289.20
+00000ea0: 322e 3231 382e 3133 332e 3338 2e33 3333  2.218.133.38.333
+00000eb0: 2e35 392e 3436 352e 3231 2e32 3031 2e34  .59.465.21.201.4
+00000ec0: 3737 2e33 3335 2e38 3736 2e33 3335 2e30  77.335.876.335.0
+00000ed0: 3339 2e30 3033 2e30 3735 2e30 3036 2e31  39.003.075.006.1
+00000ee0: 312e 3030 362e 3431 3220 3020 2e37 332d  1.006.412 0 .73-
+00000ef0: 2e31 3334 2e39 3937 2d2e 3236 382e 3239  .134.997-.268.29
+00000f00: 2d2e 3133 342e 3532 2d2e 3333 342e 3734  -.134.52-.334.74
+00000f10: 2d2e 3468 2e30 3035 632e 3436 372d 2e31  -.4h.005c.467-.1
+00000f20: 3335 2e38 3335 2d2e 3430 3220 312e 3034  35.835-.402 1.04
+00000f30: 342d 2e37 7a6d 322e 3138 3520 382e 3935  4-.7zm2.185 8.95
+00000f40: 3863 2e30 3337 2e36 2e33 3433 2031 2e32  8c.037.6.343 1.2
+00000f50: 3435 2e38 3832 2031 2e33 3737 2e35 3838  45.882 1.377.588
+00000f60: 2e31 3334 2031 2e34 3334 2d2e 3333 3320  .134 1.434-.333 
+00000f70: 312e 3739 312d 2e37 3635 6c2e 3231 312d  1.791-.765l.211-
+00000f80: 2e30 3163 2e33 3135 2d2e 3030 372e 3537  .01c.315-.007.57
+00000f90: 372e 3031 2e38 3437 2e32 3638 6c2e 3030  7.01.847.268l.00
+00000fa0: 332e 3030 3363 2e32 3038 2e31 3939 2e33  3.003c.208.199.3
+00000fb0: 3035 2e35 332e 3339 312e 3837 362e 3038  05.53.391.876.08
+00000fc0: 352e 342e 3135 342e 3738 2e34 3039 2031  5.4.154.78.409 1
+00000fd0: 2e30 3636 2e34 3836 2e35 3237 2e36 3435  .066.486.527.645
+00000fe0: 2e39 3036 2e36 3336 2031 2e31 346c 2e30  .906.636 1.14l.0
+00000ff0: 3033 2d2e 3030 3776 2e30 3138 6c2d 2e30  03-.007v.018l-.0
+00001000: 3033 2d2e 3031 3263 2d2e 3031 352e 3236  03-.012c-.015.26
+00001010: 322d 2e31 3835 2e33 3936 2d2e 3439 382e  2-.185.396-.498.
+00001020: 3539 352d 2e36 332e 3430 312d 312e 3734  595-.63.401-1.74
+00001030: 362e 3731 322d 322e 3435 3720 312e 3537  6.712-2.457 1.57
+00001040: 2d2e 3631 382e 3733 372d 312e 3337 2031  -.618.737-1.37 1
+00001050: 2e31 342d 322e 3033 3620 312e 3139 312d  .14-2.036 1.191-
+00001060: 2e36 3634 2e30 3533 2d31 2e32 3337 2d2e  .664.053-1.237-.
+00001070: 322d 312e 3537 342d 2e38 3938 6c2d 2e30  2-1.574-.898l-.0
+00001080: 3035 2d2e 3030 3363 2d2e 3231 2d2e 342d  05-.003c-.21-.4-
+00001090: 2e31 322d 312e 3032 352e 3035 362d 312e  .12-1.025.056-1.
+000010a0: 3639 2e31 3736 2d2e 3636 382e 3432 382d  69.176-.668.428-
+000010b0: 312e 3334 342e 3436 332d 312e 3839 372e  1.344.463-1.897.
+000010c0: 3033 372d 2e37 3134 2e30 3736 2d31 2e33  037-.714.076-1.3
+000010d0: 3335 2e31 3935 2d31 2e38 3134 2e31 322d  35.195-1.814.12-
+000010e0: 2e34 3635 2e33 3038 2d2e 3739 372e 3634  .465.308-.797.64
+000010f0: 312d 2e39 3834 6c2e 3034 352d 2e30 3232  1-.984l.045-.022
+00001100: 7a6d 2d31 302e 3831 342e 3034 3968 2e30  zm-10.814.049h.0
+00001110: 3163 2e30 3533 2030 202e 3130 352e 3030  1c.053 0 .105.00
+00001120: 352e 3135 372e 3031 342e 3337 362e 3035  5.157.014.376.05
+00001130: 352e 3730 362e 3333 3320 312e 3032 332e  5.706.333 1.023.
+00001140: 3735 326c 2e39 3120 312e 3636 342e 3030  752l.91 1.664.00
+00001150: 332e 3030 3363 2e32 3433 2e35 3333 2e37  3.003c.243.533.7
+00001160: 3534 2031 2e30 3634 2031 2e31 3839 2031  54 1.064 1.189 1
+00001170: 2e36 3337 2e34 3334 2e35 3938 2e37 3720  .637.434.598.77 
+00001180: 312e 3133 312e 3732 3920 312e 3537 762e  1.131.729 1.57v.
+00001190: 3030 3663 2d2e 3035 372e 3734 342d 2e34  006c-.057.744-.4
+000011a0: 3820 312e 3134 382d 312e 3132 3520 312e  8 1.148-1.125 1.
+000011b0: 3239 342d 2e36 3435 2e31 3335 2d31 2e35  294-.645.135-1.5
+000011c0: 322e 3030 322d 322e 3339 352d 2e34 3634  2.002-2.395-.464
+000011d0: 2d2e 3936 382d 2e35 3336 2d32 2e31 3138  -.968-.536-2.118
+000011e0: 2d2e 3436 392d 322e 3835 372d 2e36 3032  -.469-2.857-.602
+000011f0: 2d2e 3336 392d 2e30 3636 2d2e 3631 2d2e  -.369-.066-.61-.
+00001200: 322d 2e37 3233 2d2e 342d 2e31 312d 2e32  2-.723-.4-.11-.2
+00001210: 2d2e 3131 332d 2e36 3032 2e31 3233 2d31  -.113-.602.123-1
+00001220: 2e32 3376 2d2e 3030 346c 2e30 3032 2d2e  .23v-.004l.002-.
+00001230: 3030 3363 2e31 3137 2d2e 3333 342e 3033  003c.117-.334.03
+00001240: 2d2e 3735 322d 2e30 3237 2d31 2e31 3138  -.752-.027-1.118
+00001250: 2d2e 3035 352d 2e34 3031 2d2e 3038 332d  -.055-.401-.083-
+00001260: 2e37 312e 3034 332d 2e39 342e 3136 2d2e  .71.043-.94.16-.
+00001270: 3333 342e 3339 362d 2e34 2e36 392d 2e35  334.396-.4.69-.5
+00001280: 3333 2e32 3934 2d2e 3133 352e 3634 2d2e  33.294-.135.64-.
+00001290: 3230 322e 3931 352d 2e34 3768 2e30 3032  202.915-.47h.002
+000012a0: 762d 2e30 3032 632e 3235 362d 2e32 3638  v-.002c.256-.268
+000012b0: 2e34 3435 2d2e 3630 312e 3636 382d 2e38  .445-.601.668-.8
+000012c0: 3338 2e31 392d 2e32 3031 2e33 382d 2e33  38.19-.201.38-.3
+000012d0: 3336 2e36 3633 2d2e 3333 367a 6d37 2e31  36.663-.336zm7.1
+000012e0: 3539 2d39 2e30 3734 632d 2e34 3335 2e32  59-9.074c-.435.2
+000012f0: 3031 2d2e 3934 352e 3533 352d 312e 3438  01-.945.535-1.48
+00001300: 382e 3533 352d 2e35 3432 2030 2d2e 3937  8.535-.542 0-.97
+00001310: 2d2e 3236 372d 312e 3238 2d2e 3436 362d  -.267-1.28-.466-
+00001320: 2e31 3534 2d2e 3133 342d 2e32 382d 2e32  .154-.134-.28-.2
+00001330: 3638 2d2e 3337 332d 2e33 3335 2d2e 3136  68-.373-.335-.16
+00001340: 342d 2e31 3334 2d2e 3134 342d 2e33 3333  4-.134-.144-.333
+00001350: 2d2e 3037 342d 2e33 3333 2e31 3039 2e30  -.074-.333.109.0
+00001360: 3136 2e31 3239 2e31 3334 2e31 3939 2e32  16.129.134.199.2
+00001370: 2e30 3936 2e30 3636 2e32 3135 2e32 2e33  .096.066.215.2.3
+00001380: 362e 3333 332e 3239 322e 322e 3638 2e34  6.333.292.2.68.4
+00001390: 3637 2031 2e31 3637 2e34 3637 2e34 3835  67 1.167.467.485
+000013a0: 2030 2031 2e30 3533 2d2e 3236 3720 312e   0 1.053-.267 1.
+000013b0: 3339 382d 2e34 3636 2e31 3935 2d2e 3133  398-.466.195-.13
+000013c0: 352e 3434 352d 2e33 3334 2e36 3438 2d2e  5.445-.334.648-.
+000013d0: 3436 372e 3135 362d 2e31 3336 2e31 3439  467.156-.136.149
+000013e0: 2d2e 3236 372e 3237 392d 2e32 3637 2e31  -.267.279-.267.1
+000013f0: 3238 2e30 3136 2e30 3334 2e31 3334 2d2e  28.016.034.134-.
+00001400: 3134 372e 3333 3261 382e 3039 3720 382e  147.332a8.097 8.
+00001410: 3039 3720 3020 3031 2d2e 3639 2e34 3638  097 0 01-.69.468
+00001420: 7a6d 2d31 2e30 3832 2d31 2e35 3833 5635  zm-1.082-1.583V5
+00001430: 2e36 3463 2d2e 3030 362d 2e30 322e 3031  .64c-.006-.02.01
+00001440: 332d 2e30 3432 2e30 3239 2d2e 3035 2e30  3-.042.029-.05.0
+00001450: 3734 2d2e 3034 332e 3138 2d2e 3032 372e  74-.043.18-.027.
+00001460: 3236 2e30 3034 2e30 3633 2030 202e 3136  26.004.063 0 .16
+00001470: 2e30 3637 2e31 352e 3133 352d 2e30 3036  .067.15.135-.006
+00001480: 2e30 3439 2d2e 3038 352e 3036 362d 2e31  .049-.085.066-.1
+00001490: 3335 2e30 3636 2d2e 3035 3520 302d 2e30  35.066-.055 0-.0
+000014a0: 3932 2d2e 3034 332d 2e31 3431 2d2e 3036  92-.043-.141-.06
+000014b0: 382d 2e30 3532 2d2e 3031 382d 2e31 3436  8-.052-.018-.146
+000014c0: 2d2e 3030 382d 2e31 3633 2d2e 3036 357a  -.008-.163-.065z
+000014d0: 6d2d 2e35 3531 2030 632d 2e30 322e 3035  m-.551 0c-.02.05
+000014e0: 382d 2e31 3133 2e30 3439 2d2e 3136 362e  8-.113.049-.166.
+000014f0: 3036 362d 2e30 3437 2e30 3235 2d2e 3038  066-.047.025-.08
+00001500: 362e 3036 382d 2e31 342e 3036 382d 2e30  6.068-.14.068-.0
+00001510: 3520 302d 2e31 332d 2e30 322d 2e31 3336  5 0-.13-.02-.136
+00001520: 2d2e 3036 382d 2e30 312d 2e30 3636 2e30  -.068-.01-.066.0
+00001530: 3838 2d2e 3133 332e 3135 2d2e 3133 332e  88-.133.15-.133.
+00001540: 3038 2d2e 3033 312e 3138 342d 2e30 3437  08-.031.184-.047
+00001550: 2e32 3539 2d2e 3030 352e 3031 392e 3030  .259-.005.019.00
+00001560: 392e 3033 362e 3033 2e30 332e 3035 762e  9.036.03.03.05v.
+00001570: 3032 682e 3030 337a 222f 3e0a 3c2f 7376  02h.003z"/>.</sv
+00001580: 673e                                     g>
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,561 +1,546 @@
-00000000: 0d0a 6672 6f6d 206e 6f6e 6562 6f74 2e6c  ..from nonebot.l
-00000010: 6f67 2069 6d70 6f72 7420 6c6f 6767 6572  og import logger
-00000020: 0d0a 0d0a 696d 706f 7274 2070 616e 6461  ....import panda
-00000030: 7320 6173 2070 640d 0a66 726f 6d20 7479  s as pd..from ty
-00000040: 7069 6e67 2069 6d70 6f72 7420 4c69 7374  ping import List
-00000050: 0d0a 0d0a 6672 6f6d 202e 616e 616c 7973  ....from .analys
-00000060: 6973 2069 6d70 6f72 7420 6466 5f74 6f5f  is import df_to_
-00000070: 6775 6f67 7561 6e6c 760d 0a66 726f 6d20  guoguanlv..from 
-00000080: 2e2e 7365 6163 6820 696d 706f 7274 202a  ..seach import *
-00000090: 0d0a 6672 6f6d 202e 2e6c 3464 325f 6461  ..from ..l4d2_da
-000000a0: 7461 2e70 6c61 7965 7273 2069 6d70 6f72  ta.players impor
-000000b0: 7420 4c34 4432 506c 6179 6572 0d0a 6672  t L4D2Player..fr
-000000c0: 6f6d 202e 2e6c 3464 325f 696d 6167 6520  om ..l4d2_image 
-000000d0: 696d 706f 7274 206f 7574 5f70 6e67 0d0a  import out_png..
-000000e0: 2320 6672 6f6d 202e 616e 6e65 5f74 656c  # from .anne_tel
-000000f0: 6563 6f6d 2069 6d70 6f72 7420 414e 4e45  ecom import ANNE
-00000100: 5f41 5049 0d0a 0d0a 0d0a 7320 3d20 4c34  _API......s = L4
-00000110: 4432 506c 6179 6572 2829 0d0a 0d0a 2020  D2Player()....  
-00000120: 2020 0d0a 6173 796e 6320 6465 6620 616e    ..async def an
-00000130: 6e65 5f68 746d 6c28 6e61 6d65 3a73 7472  ne_html(name:str
-00000140: 293a 0d0a 2020 2020 2222 22e6 909c e7b4  ):..    """.....
-00000150: a2e9 878c e68f 90e5 8f96 e78e a9e5 aeb6  ................
-00000160: e4bf a1e6 81af efbc 8ce8 bf94 e59b 9ee5  ................
-00000170: 8897 e8a1 a8e5 ad97 e585 b822 2222 200d  ...........""" .
-00000180: 0a20 2020 2064 6174 615f 7469 746c 6520  .    data_title 
-00000190: 3d20 616e 6e65 5f73 6561 7263 6828 6e61  = anne_search(na
-000001a0: 6d65 290d 0a20 2020 2064 6174 6120 3d20  me)..    data = 
-000001b0: 6461 7461 5f74 6974 6c65 5b30 5d0d 0a20  data_title[0].. 
-000001c0: 2020 2074 6974 6c65 203d 2064 6174 615f     title = data_
-000001d0: 7469 746c 655b 315d 0d0a 2020 2020 6966  title[1]..    if
-000001e0: 206c 656e 2864 6174 6129 203d 3d30 206f   len(data) ==0 o
-000001f0: 7220 6461 7461 5b30 5d20 3d3d 2022 4e6f  r data[0] == "No
-00000200: 2050 6c61 7965 7220 666f 756e 642e 223a   Player found.":
-00000210: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000220: 207b 7d0d 0a20 2020 2064 6174 615f 6c69   {}..    data_li
-00000230: 7374 3a6c 6973 7420 3d20 5b5d 0d0a 2020  st:list = []..  
-00000240: 2020 6c6f 6767 6572 2e69 6e66 6f28 6461    logger.info(da
-00000250: 7461 290d 0a20 2020 2066 6f72 2069 2069  ta)..    for i i
-00000260: 6e20 6461 7461 3a0d 0a20 2020 2020 2020  n data:..       
-00000270: 2069 3a42 6561 7574 6966 756c 536f 7570   i:BeautifulSoup
-00000280: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00000290: 2020 2020 2020 2020 2020 2020 5261 6e6b              Rank
-000002a0: 203d 2069 2e66 696e 6428 2774 6427 2c20   = i.find('td', 
-000002b0: 7b27 6461 7461 2d74 6974 6c65 273a 2027  {'data-title': '
-000002c0: 5261 6e6b 3a27 7d29 2e74 6578 742e 7374  Rank:'}).text.st
-000002d0: 7269 7028 290d 0a20 2020 2020 2020 2020  rip()..         
-000002e0: 2020 2070 6c61 7965 7220 3d20 692e 6669     player = i.fi
-000002f0: 6e64 2827 7464 272c 207b 2764 6174 612d  nd('td', {'data-
-00000300: 7469 746c 6527 3a20 2750 6c61 7965 723a  title': 'Player:
-00000310: 277d 292e 7465 7874 2e73 7472 6970 2829  '}).text.strip()
-00000320: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-00000330: 696e 7473 203d 2069 2e66 696e 6428 2774  ints = i.find('t
-00000340: 6427 2c20 7b27 6461 7461 2d74 6974 6c65  d', {'data-title
-00000350: 273a 2027 506f 696e 7473 3a27 7d29 2e74  ': 'Points:'}).t
-00000360: 6578 742e 7374 7269 7028 290d 0a20 2020  ext.strip()..   
-00000370: 2020 2020 2020 2020 2023 2063 6f75 6e74           # count
-00000380: 7279 203d 2069 2e66 696e 6428 2769 6d67  ry = i.find('img
-00000390: 2729 5b27 616c 7427 5d0d 0a20 2020 2020  ')['alt']..     
-000003a0: 2020 2020 2020 2070 6c61 7974 696d 6520         playtime 
-000003b0: 3d20 692e 6669 6e64 2827 7464 272c 207b  = i.find('td', {
-000003c0: 2764 6174 612d 7469 746c 6527 3a20 2750  'data-title': 'P
-000003d0: 6c61 7974 696d 653a 277d 292e 7465 7874  laytime:'}).text
-000003e0: 2e73 7472 6970 2829 0d0a 2020 2020 2020  .strip()..      
-000003f0: 2020 2020 2020 6c61 7374 5f6f 6e6c 696e        last_onlin
-00000400: 6520 3d20 692e 6669 6e64 2827 7464 272c  e = i.find('td',
-00000410: 207b 2764 6174 612d 7469 746c 6527 3a20   {'data-title': 
-00000420: 274c 6173 7420 4f6e 6c69 6e65 3a27 7d29  'Last Online:'})
-00000430: 2e74 6578 742e 7374 7269 7028 290d 0a20  .text.strip().. 
-00000440: 2020 2020 2020 2065 7863 6570 7420 4174         except At
-00000450: 7472 6962 7574 6545 7272 6f72 3a0d 0a20  tributeError:.. 
-00000460: 2020 2020 2020 2020 2020 2052 616e 6b20             Rank 
-00000470: 3d20 692e 6669 6e64 2827 7464 272c 207b  = i.find('td', {
-00000480: 2764 6174 612d 7469 746c 6527 3a20 27e6  'data-title': '.
-00000490: 8e92 e590 8d3a 277d 292e 7465 7874 2e73  .....:'}).text.s
-000004a0: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
-000004b0: 2020 2020 706c 6179 6572 203d 2069 2e66      player = i.f
-000004c0: 696e 6428 2774 6427 2c20 7b27 6461 7461  ind('td', {'data
-000004d0: 2d74 6974 6c65 273a 2027 e78e a9e5 aeb6  -title': '......
-000004e0: 3a27 7d29 2e74 6578 742e 7374 7269 7028  :'}).text.strip(
-000004f0: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00000500: 6f69 6e74 7320 3d20 692e 6669 6e64 2827  oints = i.find('
-00000510: 7464 272c 207b 2764 6174 612d 7469 746c  td', {'data-titl
-00000520: 6527 3a20 27e5 8886 e695 b03a 277d 292e  e': '......:'}).
-00000530: 7465 7874 2e73 7472 6970 2829 0d0a 2020  text.strip()..  
-00000540: 2020 2020 2020 2020 2020 706c 6179 7469            playti
-00000550: 6d65 203d 2069 2e66 696e 6428 2774 6427  me = i.find('td'
-00000560: 2c20 7b27 6461 7461 2d74 6974 6c65 273a  , {'data-title':
-00000570: 2027 e6b8 b8e7 8ea9 e697 b6e9 97b4 3a27   '............:'
-00000580: 7d29 2e74 6578 742e 7374 7269 7028 290d  }).text.strip().
-00000590: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
-000005a0: 745f 6f6e 6c69 6e65 203d 2069 2e66 696e  t_online = i.fin
-000005b0: 6428 2774 6427 2c20 7b27 6461 7461 2d74  d('td', {'data-t
-000005c0: 6974 6c65 273a 2027 e69c 80e5 908e e4b8  itle': '........
-000005d0: 8ae7 babf e697 b6e9 97b4 3a27 7d29 2e74  ..........:'}).t
-000005e0: 6578 742e 7374 7269 7028 290d 0a20 2020  ext.strip()..   
-000005f0: 2020 2020 206f 6e63 6c69 636b 203d 2069       onclick = i
-00000600: 5b27 6f6e 636c 6963 6b27 5d0d 0a20 2020  ['onclick']..   
-00000610: 2020 2020 2073 7465 616d 6964 203d 206f       steamid = o
-00000620: 6e63 6c69 636b 2e73 706c 6974 2827 3d27  nclick.split('='
-00000630: 295b 325d 2e73 7472 6970 2822 2722 290d  )[2].strip("'").
-00000640: 0a20 2020 2020 2020 2070 6c61 795f 6a73  .        play_js
-00000650: 6f6e 203d 7b0d 0a20 2020 2020 2020 2020  on ={..         
-00000660: 2020 2074 6974 6c65 5b30 5d3a 5261 6e6b     title[0]:Rank
-00000670: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-00000680: 6974 6c65 5b31 5d3a 706c 6179 6572 2c0d  itle[1]:player,.
-00000690: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
-000006a0: 6c65 5b32 5d3a 706f 696e 7473 2c0d 0a20  le[2]:points,.. 
-000006b0: 2020 2020 2020 2020 2020 2023 2074 6974             # tit
-000006c0: 6c65 5b33 5d3a 636f 756e 7472 792c 0d0a  le[3]:country,..
-000006d0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-000006e0: 655b 335d 3a70 6c61 7974 696d 652c 0d0a  e[3]:playtime,..
-000006f0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-00000700: 655b 345d 3a6c 6173 745f 6f6e 6c69 6e65  e[4]:last_online
-00000710: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-00000720: 6974 6c65 5b35 5d3a 7374 6561 6d69 640d  itle[5]:steamid.
-00000730: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
-00000740: 2020 2020 6461 7461 5f6c 6973 742e 6170      data_list.ap
-00000750: 7065 6e64 2870 6c61 795f 6a73 6f6e 290d  pend(play_json).
-00000760: 0a20 2020 206c 6f67 6765 722e 696e 666f  .    logger.info
-00000770: 2822 e690 9ce5 afbb e695 b0e6 8dae 2229  ("............")
-00000780: 0d0a 2020 2020 7265 7475 726e 2064 6174  ..    return dat
-00000790: 615f 6c69 7374 0d0a 0d0a 6465 6620 616e  a_list....def an
-000007a0: 6e65 5f68 746d 6c5f 6d73 6728 6461 7461  ne_html_msg(data
-000007b0: 5f6c 6973 743a 6c69 7374 293a 0d0a 2020  _list:list):..  
-000007c0: 2020 2222 22e4 bb8e e690 9ce7 b4a2 e7bb    """...........
-000007d0: 93e6 9e9c e79a 84e5 ad97 e585 b8e5 8897  ................
-000007e0: e8a1 a8e4 b8ad efbc 8ce8 bf94 e59b 9ee5  ................
-000007f0: 8f91 e980 81e4 bfa1 e681 af22 2222 0d0a  ..........."""..
-00000800: 2020 2020 6d65 7320 3d20 27e6 909c e7b4      mes = '.....
-00000810: a2e5 88b0 e4bb a5e4 b88b e78e a9e5 aeb6  ................
-00000820: e4bf a1e6 81af 270d 0a20 2020 206e 7320  ......'..    ns 
-00000830: 3d20 300d 0a20 2020 200d 0a20 2020 2066  = 0..    ..    f
-00000840: 6f72 206f 6e65 2069 6e20 6461 7461 5f6c  or one in data_l
-00000850: 6973 743a 0d0a 2020 2020 2020 2020 6f6e  ist:..        on
-00000860: 653a 6469 6374 0d0a 2020 2020 2020 2020  e:dict..        
-00000870: 6e73 202b 3d20 310d 0a20 2020 2020 2020  ns += 1..       
-00000880: 2078 203d 2036 0d0a 0d0a 2020 2020 2020   x = 6....      
-00000890: 2020 7469 746c 6573 203d 206c 6973 7428    titles = list(
-000008a0: 6f6e 652e 6b65 7973 2829 290d 0a20 2020  one.keys())..   
-000008b0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-000008c0: 6e67 6528 7829 3a0d 0a20 2020 2020 2020  nge(x):..       
-000008d0: 2020 2020 206d 6573 202b 3d20 275c 6e27       mes += '\n'
-000008e0: 202b 2074 6974 6c65 735b 695d 202b 2027   + titles[i] + '
-000008f0: 3a27 202b 2073 7472 286f 6e65 5b74 6974  :' + str(one[tit
-00000900: 6c65 735b 695d 5d29 0d0a 2020 2020 2020  les[i]])..      
-00000910: 2020 6d65 7320 2b3d 2027 5c6e 2d2d 2d2d    mes += '\n----
-00000920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000930: 270d 0a20 2020 2020 2020 2069 6620 6e73  '..        if ns
-00000940: 3e34 3a0d 0a20 2020 2020 2020 2020 2020  >4:..           
-00000950: 2062 7265 616b 0d0a 2020 2020 7265 7475   break..    retu
-00000960: 726e 206d 6573 0d0a 0d0a 0d0a 2020 0d0a  rn mes......  ..
-00000970: 2020 200d 0a61 7379 6e63 2064 6566 2077     ..async def w
-00000980: 7269 7465 5f70 6c61 7965 7228 6964 2c6d  rite_player(id,m
-00000990: 7367 3a73 7472 2c6e 6963 6b6e 616d 653a  sg:str,nickname:
-000009a0: 7374 7229 3a0d 0a20 2020 2022 2222 e7bb  str):..    """..
-000009b0: 91e5 ae9a e794 a8e6 88b7 2222 220d 0a20  ..........""".. 
-000009c0: 2020 2023 20e5 88a4 e696 ade6 98af 7374     # .........st
-000009d0: 6561 6d0d 0a20 2020 2070 7269 6e74 286d  eam..    print(m
-000009e0: 7367 290d 0a20 2020 2069 6620 6d73 672e  sg)..    if msg.
-000009f0: 7374 6172 7473 7769 7468 2827 5354 4541  startswith('STEA
-00000a00: 4d27 293a 0d0a 2020 2020 2020 2020 2320  M'):..        # 
-00000a10: 7472 793a 0d0a 2020 2020 2020 2020 6461  try:..        da
-00000a20: 7461 5f74 7570 6c65 203d 2073 2e5f 7175  ta_tuple = s._qu
-00000a30: 6572 795f 706c 6179 6572 5f71 7128 6964  ery_player_qq(id
-00000a40: 290d 0a20 2020 2020 2020 2069 6620 6461  )..        if da
-00000a50: 7461 5f74 7570 6c65 2021 3d20 4e6f 6e65  ta_tuple != None
-00000a60: 3a0d 0a20 2020 2020 2020 2020 2020 2071  :..            q
-00000a70: 7120 2c20 6e69 636b 6e61 6d20 2c20 7374  q , nicknam , st
-00000a80: 6561 6d69 6420 3d20 6461 7461 5f74 7570  eamid = data_tup
-00000a90: 6c65 0d0a 2020 2020 2020 2020 656c 7365  le..        else
-00000aa0: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
-00000ab0: 6963 6b6e 616d 203d 204e 6f6e 650d 0a20  icknam = None.. 
-00000ac0: 2020 2020 2020 2061 7761 6974 2073 2e5f         await s._
-00000ad0: 6164 645f 706c 6179 6572 5f61 6c6c 2869  add_player_all(i
-00000ae0: 6420 2c20 6e69 636b 6e61 6d20 2c20 6d73  d , nicknam , ms
-00000af0: 6729 0d0a 2020 2020 2020 2020 2320 6578  g)..        # ex
-00000b00: 6365 7074 2054 7970 6545 7272 6f72 3a0d  cept TypeError:.
-00000b10: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
-00000b20: 7761 6974 2073 2e5f 6164 645f 706c 6179  wait s._add_play
-00000b30: 6572 5f73 7465 616d 6964 2869 6420 2c20  er_steamid(id , 
-00000b40: 6d73 6729 0d0a 2020 2020 2020 2020 6d65  msg)..        me
-00000b50: 7320 3d20 27e7 bb91 e5ae 9ae6 8890 e58a  s = '...........
-00000b60: 9fe5 96b5 7e5c 6e51 513a 2720 2b20 6e69  ....~\nQQ:' + ni
-00000b70: 636b 6e61 6d65 202b 275c 6e27 202b 2027  ckname +'\n' + '
-00000b80: 7374 6561 6d69 643a 272b 6d73 670d 0a20  steamid:'+msg.. 
-00000b90: 2020 2020 2020 2072 6574 7572 6e20 6d65         return me
-00000ba0: 730d 0a20 2020 2065 6c73 653a 0d0a 2020  s..    else:..  
-00000bb0: 2020 2020 2020 2320 7472 793a 0d0a 2020        # try:..  
-00000bc0: 2020 2020 2020 6461 7461 5f74 7570 6c65        data_tuple
-00000bd0: 203d 2073 2e5f 7175 6572 795f 706c 6179   = s._query_play
-00000be0: 6572 5f71 7128 6964 290d 0a20 2020 2020  er_qq(id)..     
-00000bf0: 2020 2069 6620 6461 7461 5f74 7570 6c65     if data_tuple
-00000c00: 2021 3d20 4e6f 6e65 3a0d 0a20 2020 2020   != None:..     
-00000c10: 2020 2020 2020 2069 6420 2c20 6e69 636b         id , nick
-00000c20: 6e61 6d20 2c20 7374 6561 6d69 6420 3d20  nam , steamid = 
-00000c30: 6461 7461 5f74 7570 6c65 0d0a 2020 2020  data_tuple..    
-00000c40: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000c50: 2020 2020 2020 2073 7465 616d 6964 203d         steamid =
-00000c60: 204e 6f6e 650d 0a20 2020 2020 2020 2061   None..        a
-00000c70: 7761 6974 2073 2e5f 6164 645f 706c 6179  wait s._add_play
-00000c80: 6572 5f61 6c6c 2869 6420 2c20 6d73 6720  er_all(id , msg 
-00000c90: 2c20 7374 6561 6d69 6429 0d0a 2020 2020  , steamid)..    
-00000ca0: 2020 2020 2320 6578 6365 7074 2054 7970      # except Typ
-00000cb0: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
-00000cc0: 2023 2020 2020 2061 7761 6974 2073 2e5f   #     await s._
-00000cd0: 6164 645f 706c 6179 6572 5f6e 6963 6b6e  add_player_nickn
-00000ce0: 616d 6528 6964 202c 206d 7367 2029 200d  ame(id , msg ) .
-00000cf0: 0a20 2020 2020 2020 206d 6573 203d 2027  .        mes = '
-00000d00: e7bb 91e5 ae9a e688 90e5 8a9f e596 b57e  ...............~
-00000d10: 5c6e 5151 3a27 202b 206e 6963 6b6e 616d  \nQQ:' + nicknam
-00000d20: 6520 2b27 5c6e 2720 2b20 2773 7465 616d  e +'\n' + 'steam
-00000d30: e698 b5e7 a7b0 3a27 2b6d 7367 0d0a 2020  ......:'+msg..  
-00000d40: 2020 2020 2020 7265 7475 726e 206d 6573        return mes
-00000d50: 0d0a 0d0a 2020 2020 2020 2020 0d0a 0d0a  ....        ....
-00000d60: 2020 2020 2020 2020 0d0a 6465 6620 6465          ..def de
-00000d70: 6c5f 706c 6179 6572 2869 643a 7374 7229  l_player(id:str)
-00000d80: 3a0d 0a20 2020 2022 2222 e588 a0e9 99a4  :..    """......
-00000d90: e7bb 91e5 ae9a e4bf a1e6 81af 2ce8 bf94  ............,...
-00000da0: e59b 9ee6 b688 e681 af22 2222 0d0a 2020  ........."""..  
-00000db0: 2020 6966 206e 6f74 2073 2e5f 7175 6572    if not s._quer
-00000dc0: 795f 706c 6179 6572 5f71 7128 6964 293a  y_player_qq(id):
-00000dd0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000de0: 2027 e4bd a0e8 bf98 e6b2 a1e6 9c89 e7bb   '..............
-00000df0: 91e5 ae9a e8bf 87ef bc8c e8af b7e4 bdbf  ................
-00000e00: e794 a85b e6b1 82e7 949f e7bb 91e5 ae9a  ...[............
-00000e10: 2be6 98b5 e7a7 b02f 7374 6561 6d69 645d  +....../steamid]
-00000e20: 270d 0a20 2020 2069 6620 732e 5f64 656c  '..    if s._del
-00000e30: 6574 655f 706c 6179 6572 3a0d 0a20 2020  ete_player:..   
-00000e40: 2020 2020 2072 6574 7572 6e20 27e5 88a0       return '...
-00000e50: e999 a4e6 8890 e58a 9fe5 96b5 7e27 0d0a  ............~'..
-00000e60: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-00000e70: 0d0a 6173 796e 6320 6465 6620 6964 5f74  ..async def id_t
-00000e80: 6f5f 6d65 7328 6e61 6d65 3a73 7472 293a  o_mes(name:str):
-00000e90: 0d0a 2020 2020 2222 22e6 a0b9 e68d ae6e  ..    """......n
-00000ea0: 616d 65e4 bb8e e695 b0e6 8dae e5ba 932c  ame............,
-00000eb0: e8bf 94e5 9b9e 7374 6561 6d69 64e3 8081  ......steamid...
-00000ec0: e688 96e8 8085 e7a9 bae7 99bd 2222 220d  ............""".
-00000ed0: 0a20 2020 2064 6174 615f 7475 706c 6520  .    data_tuple 
-00000ee0: 3d20 6177 6169 7420 732e 7365 6172 6368  = await s.search
-00000ef0: 5f64 6174 6128 4e6f 6e65 2c6e 616d 652c  _data(None,name,
-00000f00: 4e6f 6e65 290d 0a20 2020 2070 7269 6e74  None)..    print
-00000f10: 2864 6174 615f 7475 706c 6529 0d0a 2020  (data_tuple)..  
-00000f20: 2020 6966 2064 6174 615f 7475 706c 653a    if data_tuple:
-00000f30: 0d0a 2020 2020 2020 2020 7374 6561 6d69  ..        steami
-00000f40: 6420 3d20 6461 7461 5f74 7570 6c65 5b32  d = data_tuple[2
-00000f50: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
-00000f60: 6e20 7374 6561 6d69 640d 0a20 2020 2072  n steamid..    r
-00000f70: 6574 7572 6e20 4e6f 6e65 0d0a 2020 2020  eturn None..    
-00000f80: 0d0a 0d0a 6465 6620 616e 6e65 5f72 616e  ....def anne_ran
-00000f90: 6b5f 6469 6374 286e 616d 653a 7374 7229  k_dict(name:str)
-00000fa0: 3a0d 0a20 2020 2022 2222 e794 a873 7465  :..    """...ste
-00000fb0: 616d 6964 2ce6 9fa5 e8af a6e6 8385 2ce8  amid,.........,.
-00000fc0: be93 e587 bae5 ad97 e585 b822 2222 0d0a  ..........."""..
-00000fd0: 2020 2020 6461 7461 5f64 6963 7420 3d20      data_dict = 
-00000fe0: 7b7d 0d0a 2020 2020 7572 6c20 3d66 2768  {}..    url =f'h
-00000ff0: 7474 7073 3a2f 2f73 622e 7472 7967 656b  ttps://sb.trygek
-00001000: 2e63 6f6d 2f6c 3464 5f73 7461 7473 2f72  .com/l4d_stats/r
-00001010: 616e 6b69 6e67 2f70 6c61 7965 722e 7068  anking/player.ph
-00001020: 703f 7374 6561 6d69 643d 7b6e 616d 657d  p?steamid={name}
-00001030: 270d 0a20 2020 2068 6561 6465 7273 203d  '..    headers =
-00001040: 207b 0d0a 2020 2020 2020 2020 2755 7365   {..        'Use
-00001050: 722d 4167 656e 7427 3a27 4d6f 7a69 6c6c  r-Agent':'Mozill
-00001060: 612f 352e 3020 2857 696e 646f 7773 204e  a/5.0 (Windows N
-00001070: 5420 3130 2e30 3b20 5769 6e36 343b 2078  T 10.0; Win64; x
-00001080: 3634 3b20 7276 3a31 3037 2e30 2920 4765  64; rv:107.0) Ge
-00001090: 636b 6f2f 3230 3130 3031 3031 2046 6972  cko/20100101 Fir
-000010a0: 6566 6f78 2f31 3037 2e30 270d 0a20 2020  efox/107.0'..   
-000010b0: 207d 0d0a 2020 2020 6461 7461 203d 2068   }..    data = h
-000010c0: 7474 7078 2e67 6574 2875 726c 3d75 726c  ttpx.get(url=url
-000010d0: 2c68 6561 6465 7273 3d68 6561 6465 7273  ,headers=headers
-000010e0: 2c74 696d 656f 7574 3d35 290d 0a20 2020  ,timeout=5)..   
-000010f0: 2069 6620 6461 7461 2e73 7461 7475 735f   if data.status_
-00001100: 636f 6465 2021 3d20 3230 303a 0d0a 2020  code != 200:..  
-00001110: 2020 2020 2020 7265 7475 726e 205b 6622        return [f"
-00001120: e69f a5e8 afa2 e994 99e8 afaf efbc 8ce7  ................
-00001130: 8ab6 e680 81e7 a081 7b64 6174 612e 7374  ........{data.st
-00001140: 6174 7573 5f63 6f64 657d 225d 0d0a 2020  atus_code}"]..  
-00001150: 2020 6461 7461 203d 2064 6174 612e 636f    data = data.co
-00001160: 6e74 656e 742e 6465 636f 6465 2827 7574  ntent.decode('ut
-00001170: 662d 3827 290d 0a20 2020 2064 6174 6120  f-8')..    data 
-00001180: 3d20 4265 6175 7469 6675 6c53 6f75 7028  = BeautifulSoup(
-00001190: 6461 7461 2c20 2768 746d 6c2e 7061 7273  data, 'html.pars
-000011a0: 6572 2729 0d0a 2020 2020 6465 7461 696c  er')..    detail
-000011b0: 203d 2064 6174 612e 6669 6e64 5f61 6c6c   = data.find_all
-000011c0: 2827 7461 626c 6527 290d 0a20 2020 206e  ('table')..    n
-000011d0: 203d 2030 0d0a 2020 2020 7768 696c 6520   = 0..    while 
-000011e0: 6e20 3c20 323a 0d0a 2020 2020 2020 2020  n < 2:..        
-000011f0: 6461 7461 5f6c 6973 743a 4c69 7374 5b64  data_list:List[d
-00001200: 6963 745d 203d 205b 5d0d 0a20 2020 2020  ict] = []..     
-00001210: 2020 2064 6574 6169 6c32 203d 2064 6574     detail2 = det
-00001220: 6169 6c5b 6e5d 0d0a 2020 2020 2020 2020  ail[n]..        
-00001230: 7472 203d 2064 6574 6169 6c32 2e66 696e  tr = detail2.fin
-00001240: 645f 616c 6c28 2774 7227 290d 0a20 2020  d_all('tr')..   
-00001250: 2020 2020 2066 6f72 2069 2069 6e20 7472       for i in tr
-00001260: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-00001270: 6974 6c65 203d 2069 2e66 696e 6428 2774  itle = i.find('t
-00001280: 6427 2c20 7b27 636c 6173 7327 3a20 2777  d', {'class': 'w
-00001290: 2d35 3027 7d29 0d0a 2020 2020 2020 2020  -50'})..        
-000012a0: 2020 2020 7661 6c75 6520 3d20 7469 746c      value = titl
-000012b0: 652e 6669 6e64 5f6e 6578 745f 7369 626c  e.find_next_sibl
-000012c0: 696e 6728 2774 6427 290d 0a20 2020 2020  ing('td')..     
-000012d0: 2020 2020 2020 206e 6577 5f64 6963 7420         new_dict 
-000012e0: 3d20 7b74 6974 6c65 2e74 6578 743a 7661  = {title.text:va
-000012f0: 6c75 652e 7465 7874 7d0d 0a20 2020 2020  lue.text}..     
-00001300: 2020 2020 2020 2064 6174 615f 6469 6374         data_dict
-00001310: 2e75 7064 6174 6528 6e65 775f 6469 6374  .update(new_dict
-00001320: 290d 0a20 2020 2020 2020 2064 6174 615f  )..        data_
-00001330: 6c69 7374 2e61 7070 656e 6428 6461 7461  list.append(data
-00001340: 5f64 6963 7429 0d0a 2020 2020 2020 2020  _dict)..        
-00001350: 6e20 2b3d 2031 0d0a 2020 2020 2320 e88e  n += 1..    # ..
-00001360: b7e5 8f96 e5a4 b4e5 838f 0d0a 2020 2020  ............    
-00001370: 656c 656d 656e 743a 7374 7220 3d20 6461  element:str = da
-00001380: 7461 2e66 696e 645f 616c 6c28 6174 7472  ta.find_all(attr
-00001390: 733d 7b22 7374 796c 6522 3a20 2263 7572  s={"style": "cur
-000013a0: 736f 723a 706f 696e 7465 7222 7d29 5b30  sor:pointer"})[0
-000013b0: 5d2e 6765 7428 226f 6e63 6c69 636b 2229  ].get("onclick")
-000013c0: 0d0a 2020 2020 706c 6179 6572 5f75 726c  ..    player_url
-000013d0: 203d 2065 6c65 6d65 6e74 2e73 706c 6974   = element.split
-000013e0: 2822 2722 295b 315d 0d0a 2020 2020 6461  ("'")[1]..    da
-000013f0: 7461 5f6c 6973 745b 305d 2e75 7064 6174  ta_list[0].updat
-00001400: 6528 7b22 e4b8 aae4 baba e8b5 84e6 9699  e({"............
-00001410: 223a 706c 6179 6572 5f75 726c 7d29 0d0a  ":player_url})..
-00001420: 2020 2020 2320 e88e b7e5 8f96 e4b8 80e8      # ..........
-00001430: a880 0d0a 2020 2020 6d65 7373 6167 6520  ....    message 
-00001440: 3d20 6461 7461 2e73 656c 6563 7428 2268  = data.select("h
-00001450: 746d 6c20 626f 6479 2064 6976 2e63 6f6e  tml body div.con
-00001460: 7465 6e74 2e74 6578 742d 6365 6e74 6572  tent.text-center
-00001470: 2e74 6578 742d 6d64 2d6c 6566 7420 6469  .text-md-left di
-00001480: 762e 636f 6e74 6169 6e65 722e 7465 7874  v.container.text
-00001490: 2d6c 6566 7420 6469 762e 636f 6c2d 6d64  -left div.col-md
-000014a0: 2d31 322e 682d 3130 3020 6469 762e 6361  -12.h-100 div.ca
-000014b0: 7264 2d62 6f64 792e 776f 726c 646d 6170  rd-body.worldmap
-000014c0: 2e64 2d66 6c65 782e 666c 6578 2d63 6f6c  .d-flex.flex-col
-000014d0: 756d 6e2e 6a75 7374 6966 792d 636f 6e74  umn.justify-cont
-000014e0: 656e 742d 6365 6e74 6572 2e74 6578 742d  ent-center.text-
-000014f0: 6365 6e74 6572 2073 7061 6e22 290d 0a20  center span").. 
-00001500: 2020 206d 7367 5f6c 6973 7420 3d20 5b5d     msg_list = []
-00001510: 0d0a 2020 2020 666f 7220 6920 696e 206d  ..    for i in m
-00001520: 6573 7361 6765 3a0d 0a20 2020 2020 2020  essage:..       
-00001530: 206d 7367 5f6c 6973 742e 6170 7065 6e64   msg_list.append
-00001540: 2869 2e74 6578 7429 0d0a 2020 2020 6461  (i.text)..    da
-00001550: 7461 5f6c 6973 745b 305d 2e75 7064 6174  ta_list[0].updat
-00001560: 6528 7b22 e4b8 80e8 a880 223a 6d73 675f  e({"......":msg_
-00001570: 6c69 7374 7d29 0d0a 2020 2020 7265 7475  list})..    retu
-00001580: 726e 2064 6174 615f 6c69 7374 0d0a 0d0a  rn data_list....
-00001590: 6465 6620 616e 6e65 5f72 616e 6b5f 6469  def anne_rank_di
-000015a0: 6374 5f6d 7367 2864 6174 615f 6c69 7374  ct_msg(data_list
-000015b0: 293a 0d0a 2020 2020 2222 22e5 ad97 e585  ):..    """.....
-000015c0: b8e8 bdac 6d73 6722 2222 0d0a 2020 2020  ....msg"""..    
-000015d0: 6d73 6720 3d20 2727 0d0a 2020 2020 666f  msg = ''..    fo
-000015e0: 7220 6461 7461 5f64 6963 7420 696e 2064  r data_dict in d
-000015f0: 6174 615f 6c69 7374 3a0d 0a20 2020 2020  ata_list:..     
-00001600: 2020 206d 6573 203d 2027 270d 0a20 2020     mes = ''..   
-00001610: 2020 2020 2066 6f72 2069 2069 6e20 6461       for i in da
-00001620: 7461 5f64 6963 743a 0d0a 2020 2020 2020  ta_dict:..      
-00001630: 2020 2020 2020 6d65 7320 2b3d 275c 6e27        mes +='\n'
-00001640: 2b20 6920 2b20 6461 7461 5f64 6963 745b  + i + data_dict[
-00001650: 695d 0d0a 2020 2020 2020 2020 6d65 7320  i]..        mes 
-00001660: 2b3d 2027 5c6e 2d2d 2d2d 2d2d 2d2d 2d2d  += '\n----------
-00001670: 2d2d 2d2d 2d2d 2d2d 2d2d 270d 0a20 2020  ----------'..   
-00001680: 2020 2020 206d 7367 202b 3d20 6d65 730d       msg += mes.
-00001690: 0a20 2020 2072 6574 7572 6e20 6d73 670d  .    return msg.
-000016a0: 0a0d 0a0d 0a61 7379 6e63 2064 6566 2061  .....async def a
-000016b0: 6e6e 655f 6d65 7373 6761 6528 6e61 6d65  nne_messgae(name
-000016c0: 3a73 7472 2c75 7372 5f69 643a 7374 7229  :str,usr_id:str)
-000016d0: 3a0d 0a20 2020 2022 2222 e88e b7e5 8f96  :..    """......
-000016e0: 616e 6e65 e4bf a1e6 81af e58f afe8 be93  anne............
-000016f0: e587 bae4 bfa1 e681 af22 2222 0d0a 2020  ........."""..  
-00001700: 2020 6966 206e 616d 653a 0d0a 2020 2020    if name:..    
-00001710: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00001720: 22e5 85b3 e994 aee8 af8d e69f a5e8 afa2  "...............
-00001730: 2220 2b20 6e61 6d65 290d 0a20 2020 2020  " + name)..     
-00001740: 2020 2069 6620 6e6f 7420 6e61 6d65 2e73     if not name.s
-00001750: 7461 7274 7377 6974 6828 2753 5445 414d  tartswith('STEAM
-00001760: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-00001770: 2073 7465 616d 6964 203d 2061 7761 6974   steamid = await
-00001780: 2069 645f 746f 5f6d 6573 286e 616d 6529   id_to_mes(name)
-00001790: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000017a0: 206e 6f74 2073 7465 616d 6964 3a0d 0a20   not steamid:.. 
-000017b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000017c0: 6f67 6765 722e 696e 666f 2822 e6b2 a1e6  ogger.info("....
-000017d0: 9c89 e689 bee5 88b0 7171 efbc 8ce4 bdbf  ........qq......
-000017e0: e794 a8e9 bb98 e8ae a4e5 a4b4 e583 8f22  ..............."
-000017f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001800: 2020 206d 6573 7361 6765 203d 2061 7761     message = awa
-00001810: 6974 2061 6e6e 655f 6874 6d6c 286e 616d  it anne_html(nam
-00001820: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00001830: 2020 2020 7573 725f 6964 203d 2022 3131      usr_id = "11
-00001840: 3435 3134 3931 3931 3831 3022 0d0a 2020  45149191810"..  
-00001850: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001860: 206c 656e 286d 6573 7361 6765 2920 3d3d   len(message) ==
-00001870: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00001880: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001890: 27e6 b2a1 e69c 89e5 8fab e8bf 99e4 b8aa  '...............
-000018a0: e590 8de5 ad97 e79a 842e 2e2e 5c6e 270d  ............\n'.
-000018b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000018c0: 2069 6620 6c65 6e28 6d65 7373 6167 6529   if len(message)
-000018d0: 203e 2031 3a0d 0a20 2020 2020 2020 2020   > 1:..         
-000018e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000018f0: 6e20 616e 6e65 5f68 746d 6c5f 6d73 6728  n anne_html_msg(
-00001900: 6d65 7373 6167 6529 0d0a 2020 2020 2020  message)..      
-00001910: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
-00001920: 206d 6573 7361 6765 5b30 5d5b 2773 7465   message[0]['ste
-00001930: 616d 6964 275d 0d0a 2020 2020 2020 2020  amid']..        
-00001940: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00001950: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-00001960: 3d20 7374 6561 6d69 640d 0a20 2020 2020  = steamid..     
-00001970: 2020 2023 2073 7465 616d 6964 0d0a 2020     # steamid..  
-00001980: 2020 2020 2020 6d73 6720 3d20 616e 6e65        msg = anne
-00001990: 5f72 616e 6b5f 6469 6374 286e 616d 6529  _rank_dict(name)
-000019a0: 5b30 5d0d 0a20 2020 2020 2020 2069 6620  [0]..        if 
-000019b0: 7479 7065 286d 7367 2920 3d3d 2064 6963  type(msg) == dic
-000019c0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-000019d0: 6d73 672e 7570 6461 7465 2861 7761 6974  msg.update(await
-000019e0: 2064 665f 746f 5f67 756f 6775 616e 6c76   df_to_guoguanlv
-000019f0: 2861 7761 6974 2061 6e6e 655f 6d61 705f  (await anne_map_
-00001a00: 6d73 6728 6e61 6d65 2929 290d 0a20 2020  msg(name)))..   
-00001a10: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00001a20: 696e 666f 2827 e4bd bfe7 94a8 e59b bee7  info('..........
-00001a30: 8987 2729 0d0a 2020 2020 2020 2020 2020  ..')..          
-00001a40: 2020 6d73 6720 3d20 6177 6169 7420 6f75    msg = await ou
-00001a50: 745f 706e 6728 7573 725f 6964 2c6d 7367  t_png(usr_id,msg
-00001a60: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00001a70: 6e20 6d73 670d 0a20 2020 2065 6c73 653a  n msg..    else:
-00001a80: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001a90: 2020 2020 2020 2031 e380 8171 713e e695         1...qq>..
-00001aa0: b0e6 8dae 3ee6 b2a1 e69c 89e6 95b0 e68d  ....>...........
-00001ab0: aeef bc8c e8bf 94e5 9b9e 0d0a 2020 2020  ............    
-00001ac0: 2020 2020 32e3 8081 7171 3ee6 95b0 e68d      2...qq>.....
-00001ad0: ae3e 7374 6561 6d69 643e e69f a5e8 afa2  .>steamid>......
-00001ae0: 0d0a 2020 2020 2020 2020 33e3 8081 7171  ..        3...qq
-00001af0: 3ee6 95b0 e68d ae3e e698 b5e7 a7b0 3ee6  >......>......>.
-00001b00: 9fa5 e8af a20d 0a20 2020 2020 2020 2022  .......        "
-00001b10: 2222 0d0a 2020 2020 2020 2020 6c6f 6767  ""..        logg
-00001b20: 6572 2e69 6e66 6f28 2271 71e4 bfa1 e681  er.info("qq.....
-00001b30: afe6 9fa5 e8af a222 290d 0a20 2020 2020  .......")..     
-00001b40: 2020 2064 6174 615f 7475 706c 6520 3d20     data_tuple = 
-00001b50: 732e 5f71 7565 7279 5f70 6c61 7965 725f  s._query_player_
-00001b60: 7171 2875 7372 5f69 6429 0d0a 2020 2020  qq(usr_id)..    
-00001b70: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00001b80: 6461 7461 5f74 7570 6c65 290d 0a20 2020  data_tuple)..   
-00001b90: 2020 2020 2069 6620 6461 7461 5f74 7570       if data_tup
-00001ba0: 6c65 3d3d 204e 6f6e 653a 0d0a 2020 2020  le== None:..    
-00001bb0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00001bc0: 22e6 b2a1 e69c 89e7 bb91 e5ae 9ae4 bfa1  "...............
-00001bd0: e681 af2e 2e2e e8af b7e4 bdbf e794 a8e3  ................
-00001be0: 8090 e6b1 82e7 949f e7bb 91e5 ae9a 2078  .............. x
-00001bf0: 7878 e380 915c 6e22 0d0a 2020 2020 2020  xx...\n"..      
-00001c00: 2020 2320 e58f aae6 9c89 e590 8de5 ad97    # ............
-00001c10: efbc 8ce5 8588 e69f a5e8 afa2 e695 b0e6  ................
-00001c20: 8dae e59c a8e5 88a4 e696 ad0d 0a20 2020  .............   
-00001c30: 2020 2020 2065 6c69 6620 6461 7461 5f74       elif data_t
-00001c40: 7570 6c65 5b32 5d3a 0d0a 2020 2020 2020  uple[2]:..      
-00001c50: 2020 2020 2020 6e61 6d65 203d 2064 6174        name = dat
-00001c60: 615f 7475 706c 655b 325d 0d0a 2020 2020  a_tuple[2]..    
-00001c70: 2020 2020 656c 6966 2064 6174 615f 7475      elif data_tu
-00001c80: 706c 655b 315d 3a0d 0a20 2020 2020 2020  ple[1]:..       
-00001c90: 2020 2020 206e 616d 6520 3d20 6177 6169       name = awai
-00001ca0: 7420 6964 5f74 6f5f 6d65 7328 6461 7461  t id_to_mes(data
-00001cb0: 5f74 7570 6c65 5b31 5d29 0d0a 2020 2020  _tuple[1])..    
-00001cc0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00001cd0: 6e66 6f28 6e61 6d65 290d 0a20 2020 2020  nfo(name)..     
-00001ce0: 2020 2020 2020 2069 6620 6e6f 7420 6e61         if not na
-00001cf0: 6d65 3a0d 0a20 2020 2020 2020 2020 2020  me:..           
-00001d00: 2020 2020 206d 6573 7361 6765 203d 2061       message = a
-00001d10: 7761 6974 2061 6e6e 655f 6874 6d6c 2864  wait anne_html(d
-00001d20: 6174 615f 7475 706c 655b 315d 290d 0a20  ata_tuple[1]).. 
-00001d30: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00001d40: 7372 5f69 6420 3d20 2231 3134 3531 3439  sr_id = "1145149
-00001d50: 3139 3138 3130 220d 0a20 2020 2020 2020  191810"..       
-00001d60: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00001d70: 6d65 7373 6167 6529 203d 3d20 303a 0d0a  message) == 0:..
-00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d90: 2020 2020 7265 7475 726e 2027 e6b2 a1e6      return '....
-00001da0: 9c89 e58f abe8 bf99 e4b8 aae5 908d e5ad  ................
-00001db0: 97e7 9a84 2e2e 2e5c 6e27 0d0a 2020 2020  .......\n'..    
-00001dc0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00001dd0: 656e 286d 6573 7361 6765 2920 3e20 313a  en(message) > 1:
-00001de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001df0: 2020 2020 2020 7265 7475 726e 2061 6e6e        return ann
-00001e00: 655f 6874 6d6c 5f6d 7367 286d 6573 7361  e_html_msg(messa
-00001e10: 6765 290d 0a20 2020 2020 2020 2020 2020  ge)..           
-00001e20: 2020 2020 206e 616d 6520 3d20 6d65 7373       name = mess
-00001e30: 6167 655b 305d 5b27 7374 6561 6d69 6427  age[0]['steamid'
-00001e40: 5d0d 0a20 2020 2020 2020 2023 206e 616d  ]..        # nam
-00001e50: 65e6 98af 7374 6561 6d69 640d 0a20 2020  e...steamid..   
-00001e60: 2020 2020 206d 7367 203d 2061 6e6e 655f       msg = anne_
-00001e70: 7261 6e6b 5f64 6963 7428 6e61 6d65 295b  rank_dict(name)[
-00001e80: 305d 0d0a 2020 2020 2020 2020 6966 2074  0]..        if t
-00001e90: 7970 6528 6d73 6729 203d 3d20 6469 6374  ype(msg) == dict
-00001ea0: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
-00001eb0: 7367 2e75 7064 6174 6528 6177 6169 7420  sg.update(await 
-00001ec0: 6466 5f74 6f5f 6775 6f67 7561 6e6c 7628  df_to_guoguanlv(
-00001ed0: 6177 6169 7420 616e 6e65 5f6d 6170 5f6d  await anne_map_m
-00001ee0: 7367 286e 616d 6529 2929 0d0a 2020 2020  sg(name)))..    
-00001ef0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00001f00: 6e66 6f28 27e4 bdbf e794 a8e5 9bbe e789  nfo('...........
-00001f10: 8727 290d 0a20 2020 2020 2020 2020 2020  .')..           
-00001f20: 206d 7367 203d 2061 7761 6974 206f 7574   msg = await out
-00001f30: 5f70 6e67 2875 7372 5f69 642c 6d73 6729  _png(usr_id,msg)
-00001f40: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001f50: 206d 7367 0d0a 2020 2020 0d0a 6173 796e   msg..    ..asyn
-00001f60: 6320 6465 6620 616e 6e65 5f6d 6170 5f6d  c def anne_map_m
-00001f70: 7367 2873 7465 616d 6964 3a73 7472 293a  sg(steamid:str):
-00001f80: 0d0a 2020 2020 2222 2273 7465 616d 6964  ..    """steamid
-00001f90: 2d3e e59c b0e5 9bbe e4bf a1e6 81af 2222  ->............""
-00001fa0: 220d 0a20 2020 2075 726c 203d 2066 2268  "..    url = f"h
-00001fb0: 7474 7073 3a2f 2f73 622e 7472 7967 656b  ttps://sb.trygek
-00001fc0: 2e63 6f6d 2f6c 3464 5f73 7461 7473 2f72  .com/l4d_stats/r
-00001fd0: 616e 6b69 6e67 2f74 696d 6564 6d61 7073  anking/timedmaps
-00001fe0: 2e70 6870 3f73 7465 616d 6964 3d7b 7374  .php?steamid={st
-00001ff0: 6561 6d69 647d 220d 0a20 2020 2068 6561  eamid}"..    hea
-00002000: 6465 7273 203d 207b 0d0a 2020 2020 2020  ders = {..      
-00002010: 2020 2755 7365 722d 4167 656e 7427 3a27    'User-Agent':'
-00002020: 4d6f 7a69 6c6c 612f 352e 3020 2857 696e  Mozilla/5.0 (Win
-00002030: 646f 7773 204e 5420 3130 2e30 3b20 5769  dows NT 10.0; Wi
-00002040: 6e36 343b 2078 3634 3b20 7276 3a31 3037  n64; x64; rv:107
-00002050: 2e30 2920 4765 636b 6f2f 3230 3130 3031  .0) Gecko/201001
-00002060: 3031 2046 6972 6566 6f78 2f31 3037 2e30  01 Firefox/107.0
-00002070: 270d 0a20 2020 207d 0d0a 2020 2020 6461  '..    }..    da
-00002080: 7461 203d 2068 7474 7078 2e67 6574 2875  ta = httpx.get(u
-00002090: 726c 2c68 6561 6465 7273 3d68 6561 6465  rl,headers=heade
-000020a0: 7273 2c74 696d 656f 7574 3d35 292e 636f  rs,timeout=5).co
-000020b0: 6e74 656e 742e 6465 636f 6465 2827 7574  ntent.decode('ut
-000020c0: 662d 3827 290d 0a20 2020 2073 6f75 7020  f-8')..    soup 
-000020d0: 3d20 4265 6175 7469 6675 6c53 6f75 7028  = BeautifulSoup(
-000020e0: 6461 7461 2c20 2768 746d 6c2e 7061 7273  data, 'html.pars
-000020f0: 6572 2729 0d0a 2020 2020 6461 7461 5f6c  er')..    data_l
-00002100: 6973 7420 3d20 5b5d 0d0a 2020 2020 6361  ist = []..    ca
-00002110: 7264 7320 3d20 736f 7570 2e73 656c 6563  rds = soup.selec
-00002120: 7428 2764 6976 2e63 6172 642e 726f 756e  t('div.card.roun
-00002130: 6465 642d 3027 290d 0a20 2020 2066 6f72  ded-0')..    for
-00002140: 2063 6172 6420 696e 2063 6172 6473 3a0d   card in cards:.
-00002150: 0a20 2020 2020 2020 2074 626f 6469 6573  .        tbodies
-00002160: 203d 2063 6172 642e 7365 6c65 6374 2827   = card.select('
-00002170: 7462 6f64 7927 290d 0a20 2020 2020 2020  tbody')..       
-00002180: 2066 6f72 2074 626f 6479 2069 6e20 7462   for tbody in tb
-00002190: 6f64 6965 733a 0d0a 2020 2020 2020 2020  odies:..        
-000021a0: 2020 2020 726f 7773 203d 205b 7464 2e74      rows = [td.t
-000021b0: 6578 742e 7374 7269 7028 2920 666f 7220  ext.strip() for 
-000021c0: 7464 2069 6e20 7462 6f64 792e 6669 6e64  td in tbody.find
-000021d0: 5f61 6c6c 2827 7464 2729 5d0d 0a20 2020  _all('td')]..   
-000021e0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-000021f0: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
-00002200: 6f77 7329 2c20 3929 3a0d 0a20 2020 2020  ows), 9):..     
-00002210: 2020 2020 2020 2020 2020 2072 6f77 203d             row =
-00002220: 2072 6f77 735b 693a 692b 395d 0d0a 2020   rows[i:i+9]..  
-00002230: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00002240: 7461 5f6c 6973 742e 6170 7065 6e64 2872  ta_list.append(r
-00002250: 6f77 290d 0a20 2020 2064 6620 3d20 7064  ow)..    df = pd
-00002260: 2e44 6174 6146 7261 6d65 2864 6174 615f  .DataFrame(data_
-00002270: 6c69 7374 2c20 636f 6c75 6d6e 733d 5b27  list, columns=['
-00002280: e6b8 b8e6 888f e6a8 a1e5 bc8f 272c 2027  ............', '
-00002290: e59c b0e5 9bbe 272c 2027 e99a bee5 baa6  ......', '......
-000022a0: 272c 2027 e5ae 8ce6 8890 e697 b6e9 97b4  ', '............
-000022b0: 272c 2027 e789 b9e6 849f e695 b0e9 878f  ', '............
-000022c0: 272c 2027 e588 b7e6 96b0 e997 b4e9 9a94  ', '............
-000022d0: 272c 2027 42e6 95b0 e4bd bfe7 94a8 272c  ', 'B.........',
-000022e0: 2027 e588 b7e7 89b9 e6a8 a1e5 bc8f 272c   '............',
-000022f0: 2027 416e 6e65 e789 88e6 9cac 275d 290d   'Anne......']).
-00002300: 0a20 2020 2072 6574 7572 6e20 6466       .    return df
+00000000: 0a66 726f 6d20 6e6f 6e65 626f 742e 6c6f  .from nonebot.lo
+00000010: 6720 696d 706f 7274 206c 6f67 6765 720a  g import logger.
+00000020: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
+00000030: 7320 7064 0a66 726f 6d20 7479 7069 6e67  s pd.from typing
+00000040: 2069 6d70 6f72 7420 4c69 7374 0a0a 6672   import List..fr
+00000050: 6f6d 202e 616e 616c 7973 6973 2069 6d70  om .analysis imp
+00000060: 6f72 7420 6466 5f74 6f5f 6775 6f67 7561  ort df_to_guogua
+00000070: 6e6c 760a 6672 6f6d 202e 2e73 6561 6368  nlv.from ..seach
+00000080: 2069 6d70 6f72 7420 2a0a 6672 6f6d 202e   import *.from .
+00000090: 2e6c 3464 325f 6461 7461 2e70 6c61 7965  .l4d2_data.playe
+000000a0: 7273 2069 6d70 6f72 7420 4c34 4432 506c  rs import L4D2Pl
+000000b0: 6179 6572 0a66 726f 6d20 2e2e 6c34 6432  ayer.from ..l4d2
+000000c0: 5f69 6d61 6765 2069 6d70 6f72 7420 6f75  _image import ou
+000000d0: 745f 706e 670a 2320 6672 6f6d 202e 616e  t_png.# from .an
+000000e0: 6e65 5f74 656c 6563 6f6d 2069 6d70 6f72  ne_telecom impor
+000000f0: 7420 414e 4e45 5f41 5049 0a0a 0a73 203d  t ANNE_API...s =
+00000100: 204c 3444 3250 6c61 7965 7228 290a 0a20   L4D2Player().. 
+00000110: 2020 200a 6173 796e 6320 6465 6620 616e     .async def an
+00000120: 6e65 5f68 746d 6c28 6e61 6d65 3a73 7472  ne_html(name:str
+00000130: 293a 0a20 2020 2022 2222 e690 9ce7 b4a2  ):.    """......
+00000140: e987 8ce6 8f90 e58f 96e7 8ea9 e5ae b6e4  ................
+00000150: bfa1 e681 afef bc8c e8bf 94e5 9b9e e588  ................
+00000160: 97e8 a1a8 e5ad 97e5 85b8 2222 2220 0a20  ..........""" . 
+00000170: 2020 2064 6174 615f 7469 746c 6520 3d20     data_title = 
+00000180: 616e 6e65 5f73 6561 7263 6828 6e61 6d65  anne_search(name
+00000190: 290a 2020 2020 6461 7461 203d 2064 6174  ).    data = dat
+000001a0: 615f 7469 746c 655b 305d 0a20 2020 2074  a_title[0].    t
+000001b0: 6974 6c65 203d 2064 6174 615f 7469 746c  itle = data_titl
+000001c0: 655b 315d 0a20 2020 2069 6620 6c65 6e28  e[1].    if len(
+000001d0: 6461 7461 2920 3d3d 3020 6f72 2064 6174  data) ==0 or dat
+000001e0: 615b 305d 203d 3d20 224e 6f20 506c 6179  a[0] == "No Play
+000001f0: 6572 2066 6f75 6e64 2e22 3a0a 2020 2020  er found.":.    
+00000200: 2020 2020 7265 7475 726e 207b 7d0a 2020      return {}.  
+00000210: 2020 6461 7461 5f6c 6973 743a 6c69 7374    data_list:list
+00000220: 203d 205b 5d0a 2020 2020 6c6f 6767 6572   = [].    logger
+00000230: 2e69 6e66 6f28 6461 7461 290a 2020 2020  .info(data).    
+00000240: 666f 7220 6920 696e 2064 6174 613a 0a20  for i in data:. 
+00000250: 2020 2020 2020 2069 3a42 6561 7574 6966         i:Beautif
+00000260: 756c 536f 7570 0a20 2020 2020 2020 2074  ulSoup.        t
+00000270: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00000280: 5261 6e6b 203d 2069 2e66 696e 6428 2774  Rank = i.find('t
+00000290: 6427 2c20 7b27 6461 7461 2d74 6974 6c65  d', {'data-title
+000002a0: 273a 2027 5261 6e6b 3a27 7d29 2e74 6578  ': 'Rank:'}).tex
+000002b0: 742e 7374 7269 7028 290a 2020 2020 2020  t.strip().      
+000002c0: 2020 2020 2020 706c 6179 6572 203d 2069        player = i
+000002d0: 2e66 696e 6428 2774 6427 2c20 7b27 6461  .find('td', {'da
+000002e0: 7461 2d74 6974 6c65 273a 2027 506c 6179  ta-title': 'Play
+000002f0: 6572 3a27 7d29 2e74 6578 742e 7374 7269  er:'}).text.stri
+00000300: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+00000310: 706f 696e 7473 203d 2069 2e66 696e 6428  points = i.find(
+00000320: 2774 6427 2c20 7b27 6461 7461 2d74 6974  'td', {'data-tit
+00000330: 6c65 273a 2027 506f 696e 7473 3a27 7d29  le': 'Points:'})
+00000340: 2e74 6578 742e 7374 7269 7028 290a 2020  .text.strip().  
+00000350: 2020 2020 2020 2020 2020 2320 636f 756e            # coun
+00000360: 7472 7920 3d20 692e 6669 6e64 2827 696d  try = i.find('im
+00000370: 6727 295b 2761 6c74 275d 0a20 2020 2020  g')['alt'].     
+00000380: 2020 2020 2020 2070 6c61 7974 696d 6520         playtime 
+00000390: 3d20 692e 6669 6e64 2827 7464 272c 207b  = i.find('td', {
+000003a0: 2764 6174 612d 7469 746c 6527 3a20 2750  'data-title': 'P
+000003b0: 6c61 7974 696d 653a 277d 292e 7465 7874  laytime:'}).text
+000003c0: 2e73 7472 6970 2829 0a20 2020 2020 2020  .strip().       
+000003d0: 2020 2020 206c 6173 745f 6f6e 6c69 6e65       last_online
+000003e0: 203d 2069 2e66 696e 6428 2774 6427 2c20   = i.find('td', 
+000003f0: 7b27 6461 7461 2d74 6974 6c65 273a 2027  {'data-title': '
+00000400: 4c61 7374 204f 6e6c 696e 653a 277d 292e  Last Online:'}).
+00000410: 7465 7874 2e73 7472 6970 2829 0a20 2020  text.strip().   
+00000420: 2020 2020 2065 7863 6570 7420 4174 7472       except Attr
+00000430: 6962 7574 6545 7272 6f72 3a0a 2020 2020  ibuteError:.    
+00000440: 2020 2020 2020 2020 5261 6e6b 203d 2069          Rank = i
+00000450: 2e66 696e 6428 2774 6427 2c20 7b27 6461  .find('td', {'da
+00000460: 7461 2d74 6974 6c65 273a 2027 e68e 92e5  ta-title': '....
+00000470: 908d 3a27 7d29 2e74 6578 742e 7374 7269  ..:'}).text.stri
+00000480: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+00000490: 706c 6179 6572 203d 2069 2e66 696e 6428  player = i.find(
+000004a0: 2774 6427 2c20 7b27 6461 7461 2d74 6974  'td', {'data-tit
+000004b0: 6c65 273a 2027 e78e a9e5 aeb6 3a27 7d29  le': '......:'})
+000004c0: 2e74 6578 742e 7374 7269 7028 290a 2020  .text.strip().  
+000004d0: 2020 2020 2020 2020 2020 706f 696e 7473            points
+000004e0: 203d 2069 2e66 696e 6428 2774 6427 2c20   = i.find('td', 
+000004f0: 7b27 6461 7461 2d74 6974 6c65 273a 2027  {'data-title': '
+00000500: e588 86e6 95b0 3a27 7d29 2e74 6578 742e  ......:'}).text.
+00000510: 7374 7269 7028 290a 2020 2020 2020 2020  strip().        
+00000520: 2020 2020 706c 6179 7469 6d65 203d 2069      playtime = i
+00000530: 2e66 696e 6428 2774 6427 2c20 7b27 6461  .find('td', {'da
+00000540: 7461 2d74 6974 6c65 273a 2027 e6b8 b8e7  ta-title': '....
+00000550: 8ea9 e697 b6e9 97b4 3a27 7d29 2e74 6578  ........:'}).tex
+00000560: 742e 7374 7269 7028 290a 2020 2020 2020  t.strip().      
+00000570: 2020 2020 2020 6c61 7374 5f6f 6e6c 696e        last_onlin
+00000580: 6520 3d20 692e 6669 6e64 2827 7464 272c  e = i.find('td',
+00000590: 207b 2764 6174 612d 7469 746c 6527 3a20   {'data-title': 
+000005a0: 27e6 9c80 e590 8ee4 b88a e7ba bfe6 97b6  '...............
+000005b0: e997 b43a 277d 292e 7465 7874 2e73 7472  ...:'}).text.str
+000005c0: 6970 2829 0a20 2020 2020 2020 206f 6e63  ip().        onc
+000005d0: 6c69 636b 203d 2069 5b27 6f6e 636c 6963  lick = i['onclic
+000005e0: 6b27 5d0a 2020 2020 2020 2020 7374 6561  k'].        stea
+000005f0: 6d69 6420 3d20 6f6e 636c 6963 6b2e 7370  mid = onclick.sp
+00000600: 6c69 7428 273d 2729 5b32 5d2e 7374 7269  lit('=')[2].stri
+00000610: 7028 2227 2229 0a20 2020 2020 2020 2070  p("'").        p
+00000620: 6c61 795f 6a73 6f6e 203d 7b0a 2020 2020  lay_json ={.    
+00000630: 2020 2020 2020 2020 7469 746c 655b 305d          title[0]
+00000640: 3a52 616e 6b2c 0a20 2020 2020 2020 2020  :Rank,.         
+00000650: 2020 2074 6974 6c65 5b31 5d3a 706c 6179     title[1]:play
+00000660: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00000670: 7469 746c 655b 325d 3a70 6f69 6e74 732c  title[2]:points,
+00000680: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
+00000690: 6974 6c65 5b33 5d3a 636f 756e 7472 792c  itle[3]:country,
+000006a0: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
+000006b0: 6c65 5b33 5d3a 706c 6179 7469 6d65 2c0a  le[3]:playtime,.
+000006c0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+000006d0: 655b 345d 3a6c 6173 745f 6f6e 6c69 6e65  e[4]:last_online
+000006e0: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
+000006f0: 746c 655b 355d 3a73 7465 616d 6964 0a20  tle[5]:steamid. 
+00000700: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00000710: 2064 6174 615f 6c69 7374 2e61 7070 656e   data_list.appen
+00000720: 6428 706c 6179 5f6a 736f 6e29 0a20 2020  d(play_json).   
+00000730: 206c 6f67 6765 722e 696e 666f 2822 e690   logger.info("..
+00000740: 9ce5 afbb e695 b0e6 8dae 2229 0a20 2020  ..........").   
+00000750: 2072 6574 7572 6e20 6461 7461 5f6c 6973   return data_lis
+00000760: 740a 0a64 6566 2061 6e6e 655f 6874 6d6c  t..def anne_html
+00000770: 5f6d 7367 2864 6174 615f 6c69 7374 3a6c  _msg(data_list:l
+00000780: 6973 7429 3a0a 2020 2020 2222 22e4 bb8e  ist):.    """...
+00000790: e690 9ce7 b4a2 e7bb 93e6 9e9c e79a 84e5  ................
+000007a0: ad97 e585 b8e5 8897 e8a1 a8e4 b8ad efbc  ................
+000007b0: 8ce8 bf94 e59b 9ee5 8f91 e980 81e4 bfa1  ................
+000007c0: e681 af22 2222 0a20 2020 206d 6573 203d  ...""".    mes =
+000007d0: 2027 e690 9ce7 b4a2 e588 b0e4 bba5 e4b8   '..............
+000007e0: 8be7 8ea9 e5ae b6e4 bfa1 e681 af27 0a20  .............'. 
+000007f0: 2020 206e 7320 3d20 300a 2020 2020 0a20     ns = 0.    . 
+00000800: 2020 2066 6f72 206f 6e65 2069 6e20 6461     for one in da
+00000810: 7461 5f6c 6973 743a 0a20 2020 2020 2020  ta_list:.       
+00000820: 206f 6e65 3a64 6963 740a 2020 2020 2020   one:dict.      
+00000830: 2020 6e73 202b 3d20 310a 2020 2020 2020    ns += 1.      
+00000840: 2020 7820 3d20 360a 0a20 2020 2020 2020    x = 6..       
+00000850: 2074 6974 6c65 7320 3d20 6c69 7374 286f   titles = list(o
+00000860: 6e65 2e6b 6579 7328 2929 0a20 2020 2020  ne.keys()).     
+00000870: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00000880: 6528 7829 3a0a 2020 2020 2020 2020 2020  e(x):.          
+00000890: 2020 6d65 7320 2b3d 2027 5c6e 2720 2b20    mes += '\n' + 
+000008a0: 7469 746c 6573 5b69 5d20 2b20 273a 2720  titles[i] + ':' 
+000008b0: 2b20 7374 7228 6f6e 655b 7469 746c 6573  + str(one[titles
+000008c0: 5b69 5d5d 290a 2020 2020 2020 2020 6d65  [i]]).        me
+000008d0: 7320 2b3d 2027 5c6e 2d2d 2d2d 2d2d 2d2d  s += '\n--------
+000008e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 270a 2020  ------------'.  
+000008f0: 2020 2020 2020 6966 206e 733e 343a 0a20        if ns>4:. 
+00000900: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00000910: 0a20 2020 2072 6574 7572 6e20 6d65 730a  .    return mes.
+00000920: 0a0a 2020 0a20 2020 0a61 7379 6e63 2064  ..  .   .async d
+00000930: 6566 2077 7269 7465 5f70 6c61 7965 7228  ef write_player(
+00000940: 6964 2c6d 7367 3a73 7472 2c6e 6963 6b6e  id,msg:str,nickn
+00000950: 616d 653a 7374 7229 3a0a 2020 2020 2222  ame:str):.    ""
+00000960: 22e7 bb91 e5ae 9ae7 94a8 e688 b722 2222  "............"""
+00000970: 0a20 2020 2023 20e5 88a4 e696 ade6 98af  .    # .........
+00000980: 7374 6561 6d0a 2020 2020 7072 696e 7428  steam.    print(
+00000990: 6d73 6729 0a20 2020 2069 6620 6d73 672e  msg).    if msg.
+000009a0: 7374 6172 7473 7769 7468 2827 5354 4541  startswith('STEA
+000009b0: 4d27 293a 0a20 2020 2020 2020 2023 2074  M'):.        # t
+000009c0: 7279 3a0a 2020 2020 2020 2020 6461 7461  ry:.        data
+000009d0: 5f74 7570 6c65 203d 2073 2e5f 7175 6572  _tuple = s._quer
+000009e0: 795f 706c 6179 6572 5f71 7128 6964 290a  y_player_qq(id).
+000009f0: 2020 2020 2020 2020 6966 2064 6174 615f          if data_
+00000a00: 7475 706c 6520 213d 204e 6f6e 653a 0a20  tuple != None:. 
+00000a10: 2020 2020 2020 2020 2020 2071 7120 2c20             qq , 
+00000a20: 6e69 636b 6e61 6d20 2c20 7374 6561 6d69  nicknam , steami
+00000a30: 6420 3d20 6461 7461 5f74 7570 6c65 0a20  d = data_tuple. 
+00000a40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00000a50: 2020 2020 2020 2020 206e 6963 6b6e 616d           nicknam
+00000a60: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00000a70: 6177 6169 7420 732e 5f61 6464 5f70 6c61  await s._add_pla
+00000a80: 7965 725f 616c 6c28 6964 202c 206e 6963  yer_all(id , nic
+00000a90: 6b6e 616d 202c 206d 7367 290a 2020 2020  knam , msg).    
+00000aa0: 2020 2020 2320 6578 6365 7074 2054 7970      # except Typ
+00000ab0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00000ac0: 2020 2020 2320 6177 6169 7420 732e 5f61      # await s._a
+00000ad0: 6464 5f70 6c61 7965 725f 7374 6561 6d69  dd_player_steami
+00000ae0: 6428 6964 202c 206d 7367 290a 2020 2020  d(id , msg).    
+00000af0: 2020 2020 6d65 7320 3d20 27e7 bb91 e5ae      mes = '.....
+00000b00: 9ae6 8890 e58a 9fe5 96b5 7e5c 6e51 513a  ..........~\nQQ:
+00000b10: 2720 2b20 6e69 636b 6e61 6d65 202b 275c  ' + nickname +'\
+00000b20: 6e27 202b 2027 7374 6561 6d69 643a 272b  n' + 'steamid:'+
+00000b30: 6d73 670a 2020 2020 2020 2020 7265 7475  msg.        retu
+00000b40: 726e 206d 6573 0a20 2020 2065 6c73 653a  rn mes.    else:
+00000b50: 0a20 2020 2020 2020 2023 2074 7279 3a0a  .        # try:.
+00000b60: 2020 2020 2020 2020 6461 7461 5f74 7570          data_tup
+00000b70: 6c65 203d 2073 2e5f 7175 6572 795f 706c  le = s._query_pl
+00000b80: 6179 6572 5f71 7128 6964 290a 2020 2020  ayer_qq(id).    
+00000b90: 2020 2020 6966 2064 6174 615f 7475 706c      if data_tupl
+00000ba0: 6520 213d 204e 6f6e 653a 0a20 2020 2020  e != None:.     
+00000bb0: 2020 2020 2020 2069 6420 2c20 6e69 636b         id , nick
+00000bc0: 6e61 6d20 2c20 7374 6561 6d69 6420 3d20  nam , steamid = 
+00000bd0: 6461 7461 5f74 7570 6c65 0a20 2020 2020  data_tuple.     
+00000be0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00000bf0: 2020 2020 2073 7465 616d 6964 203d 204e       steamid = N
+00000c00: 6f6e 650a 2020 2020 2020 2020 6177 6169  one.        awai
+00000c10: 7420 732e 5f61 6464 5f70 6c61 7965 725f  t s._add_player_
+00000c20: 616c 6c28 6964 202c 206d 7367 202c 2073  all(id , msg , s
+00000c30: 7465 616d 6964 290a 2020 2020 2020 2020  teamid).        
+00000c40: 2320 6578 6365 7074 2054 7970 6545 7272  # except TypeErr
+00000c50: 6f72 3a0a 2020 2020 2020 2020 2320 2020  or:.        #   
+00000c60: 2020 6177 6169 7420 732e 5f61 6464 5f70    await s._add_p
+00000c70: 6c61 7965 725f 6e69 636b 6e61 6d65 2869  layer_nickname(i
+00000c80: 6420 2c20 6d73 6720 2920 0a20 2020 2020  d , msg ) .     
+00000c90: 2020 206d 6573 203d 2027 e7bb 91e5 ae9a     mes = '......
+00000ca0: e688 90e5 8a9f e596 b57e 5c6e 5151 3a27  .........~\nQQ:'
+00000cb0: 202b 206e 6963 6b6e 616d 6520 2b27 5c6e   + nickname +'\n
+00000cc0: 2720 2b20 2773 7465 616d e698 b5e7 a7b0  ' + 'steam......
+00000cd0: 3a27 2b6d 7367 0a20 2020 2020 2020 2072  :'+msg.        r
+00000ce0: 6574 7572 6e20 6d65 730a 0a20 2020 2020  eturn mes..     
+00000cf0: 2020 200a 0a20 2020 2020 2020 200a 6465     ..        .de
+00000d00: 6620 6465 6c5f 706c 6179 6572 2869 643a  f del_player(id:
+00000d10: 7374 7229 3a0a 2020 2020 2222 22e5 88a0  str):.    """...
+00000d20: e999 a4e7 bb91 e5ae 9ae4 bfa1 e681 af2c  ...............,
+00000d30: e8bf 94e5 9b9e e6b6 88e6 81af 2222 220a  ............""".
+00000d40: 2020 2020 6966 206e 6f74 2073 2e5f 7175      if not s._qu
+00000d50: 6572 795f 706c 6179 6572 5f71 7128 6964  ery_player_qq(id
+00000d60: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00000d70: 6e20 27e4 bda0 e8bf 98e6 b2a1 e69c 89e7  n '.............
+00000d80: bb91 e5ae 9ae8 bf87 efbc 8ce8 afb7 e4bd  ................
+00000d90: bfe7 94a8 5be6 b182 e794 9fe7 bb91 e5ae  ....[...........
+00000da0: 9a2b e698 b5e7 a7b0 2f73 7465 616d 6964  .+....../steamid
+00000db0: 5d27 0a20 2020 2069 6620 732e 5f64 656c  ]'.    if s._del
+00000dc0: 6574 655f 706c 6179 6572 3a0a 2020 2020  ete_player:.    
+00000dd0: 2020 2020 7265 7475 726e 2027 e588 a0e9      return '....
+00000de0: 99a4 e688 90e5 8a9f e596 b57e 270a 2020  ...........~'.  
+00000df0: 2020 2020 2020 0a0a 2020 2020 0a61 7379        ..    .asy
+00000e00: 6e63 2064 6566 2069 645f 746f 5f6d 6573  nc def id_to_mes
+00000e10: 286e 616d 653a 7374 7229 3a0a 2020 2020  (name:str):.    
+00000e20: 2222 22e6 a0b9 e68d ae6e 616d 65e4 bb8e  """......name...
+00000e30: e695 b0e6 8dae e5ba 932c e8bf 94e5 9b9e  .........,......
+00000e40: 7374 6561 6d69 64e3 8081 e688 96e8 8085  steamid.........
+00000e50: e7a9 bae7 99bd 2222 220a 2020 2020 6461  ......""".    da
+00000e60: 7461 5f74 7570 6c65 203d 2061 7761 6974  ta_tuple = await
+00000e70: 2073 2e73 6561 7263 685f 6461 7461 284e   s.search_data(N
+00000e80: 6f6e 652c 6e61 6d65 2c4e 6f6e 6529 0a20  one,name,None). 
+00000e90: 2020 2070 7269 6e74 2864 6174 615f 7475     print(data_tu
+00000ea0: 706c 6529 0a20 2020 2069 6620 6461 7461  ple).    if data
+00000eb0: 5f74 7570 6c65 3a0a 2020 2020 2020 2020  _tuple:.        
+00000ec0: 7374 6561 6d69 6420 3d20 6461 7461 5f74  steamid = data_t
+00000ed0: 7570 6c65 5b32 5d0a 2020 2020 2020 2020  uple[2].        
+00000ee0: 7265 7475 726e 2073 7465 616d 6964 0a20  return steamid. 
+00000ef0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00000f00: 2020 200a 0a64 6566 2061 6e6e 655f 7261     ..def anne_ra
+00000f10: 6e6b 5f64 6963 7428 6e61 6d65 3a73 7472  nk_dict(name:str
+00000f20: 293a 0a20 2020 2022 2222 e794 a873 7465  ):.    """...ste
+00000f30: 616d 6964 2ce6 9fa5 e8af a6e6 8385 2ce8  amid,.........,.
+00000f40: be93 e587 bae5 ad97 e585 b822 2222 0a20  ...........""". 
+00000f50: 2020 2064 6174 615f 6469 6374 203d 207b     data_dict = {
+00000f60: 7d0a 2020 2020 7572 6c20 3d66 2768 7474  }.    url =f'htt
+00000f70: 7073 3a2f 2f73 622e 7472 7967 656b 2e63  ps://sb.trygek.c
+00000f80: 6f6d 2f6c 3464 5f73 7461 7473 2f72 616e  om/l4d_stats/ran
+00000f90: 6b69 6e67 2f70 6c61 7965 722e 7068 703f  king/player.php?
+00000fa0: 7374 6561 6d69 643d 7b6e 616d 657d 270a  steamid={name}'.
+00000fb0: 2020 2020 6865 6164 6572 7320 3d20 7b0a      headers = {.
+00000fc0: 2020 2020 2020 2020 2755 7365 722d 4167          'User-Ag
+00000fd0: 656e 7427 3a27 4d6f 7a69 6c6c 612f 352e  ent':'Mozilla/5.
+00000fe0: 3020 2857 696e 646f 7773 204e 5420 3130  0 (Windows NT 10
+00000ff0: 2e30 3b20 5769 6e36 343b 2078 3634 3b20  .0; Win64; x64; 
+00001000: 7276 3a31 3037 2e30 2920 4765 636b 6f2f  rv:107.0) Gecko/
+00001010: 3230 3130 3031 3031 2046 6972 6566 6f78  20100101 Firefox
+00001020: 2f31 3037 2e30 270a 2020 2020 7d0a 2020  /107.0'.    }.  
+00001030: 2020 6461 7461 203d 2068 7474 7078 2e67    data = httpx.g
+00001040: 6574 2875 726c 3d75 726c 2c68 6561 6465  et(url=url,heade
+00001050: 7273 3d68 6561 6465 7273 2c74 696d 656f  rs=headers,timeo
+00001060: 7574 3d35 290a 2020 2020 6966 2064 6174  ut=5).    if dat
+00001070: 612e 7374 6174 7573 5f63 6f64 6520 213d  a.status_code !=
+00001080: 2032 3030 3a0a 2020 2020 2020 2020 7265   200:.        re
+00001090: 7475 726e 205b 6622 e69f a5e8 afa2 e994  turn [f"........
+000010a0: 99e8 afaf efbc 8ce7 8ab6 e680 81e7 a081  ................
+000010b0: 7b64 6174 612e 7374 6174 7573 5f63 6f64  {data.status_cod
+000010c0: 657d 225d 0a20 2020 2064 6174 6120 3d20  e}"].    data = 
+000010d0: 6461 7461 2e63 6f6e 7465 6e74 2e64 6563  data.content.dec
+000010e0: 6f64 6528 2775 7466 2d38 2729 0a20 2020  ode('utf-8').   
+000010f0: 2064 6174 6120 3d20 4265 6175 7469 6675   data = Beautifu
+00001100: 6c53 6f75 7028 6461 7461 2c20 2768 746d  lSoup(data, 'htm
+00001110: 6c2e 7061 7273 6572 2729 0a20 2020 2064  l.parser').    d
+00001120: 6574 6169 6c20 3d20 6461 7461 2e66 696e  etail = data.fin
+00001130: 645f 616c 6c28 2774 6162 6c65 2729 0a20  d_all('table'). 
+00001140: 2020 206e 203d 2030 0a20 2020 2077 6869     n = 0.    whi
+00001150: 6c65 206e 203c 2032 3a0a 2020 2020 2020  le n < 2:.      
+00001160: 2020 6461 7461 5f6c 6973 743a 4c69 7374    data_list:List
+00001170: 5b64 6963 745d 203d 205b 5d0a 2020 2020  [dict] = [].    
+00001180: 2020 2020 6465 7461 696c 3220 3d20 6465      detail2 = de
+00001190: 7461 696c 5b6e 5d0a 2020 2020 2020 2020  tail[n].        
+000011a0: 7472 203d 2064 6574 6169 6c32 2e66 696e  tr = detail2.fin
+000011b0: 645f 616c 6c28 2774 7227 290a 2020 2020  d_all('tr').    
+000011c0: 2020 2020 666f 7220 6920 696e 2074 723a      for i in tr:
+000011d0: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
+000011e0: 6c65 203d 2069 2e66 696e 6428 2774 6427  le = i.find('td'
+000011f0: 2c20 7b27 636c 6173 7327 3a20 2777 2d35  , {'class': 'w-5
+00001200: 3027 7d29 0a20 2020 2020 2020 2020 2020  0'}).           
+00001210: 2076 616c 7565 203d 2074 6974 6c65 2e66   value = title.f
+00001220: 696e 645f 6e65 7874 5f73 6962 6c69 6e67  ind_next_sibling
+00001230: 2827 7464 2729 0a20 2020 2020 2020 2020  ('td').         
+00001240: 2020 206e 6577 5f64 6963 7420 3d20 7b74     new_dict = {t
+00001250: 6974 6c65 2e74 6578 743a 7661 6c75 652e  itle.text:value.
+00001260: 7465 7874 7d0a 2020 2020 2020 2020 2020  text}.          
+00001270: 2020 6461 7461 5f64 6963 742e 7570 6461    data_dict.upda
+00001280: 7465 286e 6577 5f64 6963 7429 0a20 2020  te(new_dict).   
+00001290: 2020 2020 2064 6174 615f 6c69 7374 2e61       data_list.a
+000012a0: 7070 656e 6428 6461 7461 5f64 6963 7429  ppend(data_dict)
+000012b0: 0a20 2020 2020 2020 206e 202b 3d20 310a  .        n += 1.
+000012c0: 2020 2020 2320 e88e b7e5 8f96 e5a4 b4e5      # ..........
+000012d0: 838f 0a20 2020 2065 6c65 6d65 6e74 3a73  ...    element:s
+000012e0: 7472 203d 2064 6174 612e 6669 6e64 5f61  tr = data.find_a
+000012f0: 6c6c 2861 7474 7273 3d7b 2273 7479 6c65  ll(attrs={"style
+00001300: 223a 2022 6375 7273 6f72 3a70 6f69 6e74  ": "cursor:point
+00001310: 6572 227d 295b 305d 2e67 6574 2822 6f6e  er"})[0].get("on
+00001320: 636c 6963 6b22 290a 2020 2020 706c 6179  click").    play
+00001330: 6572 5f75 726c 203d 2065 6c65 6d65 6e74  er_url = element
+00001340: 2e73 706c 6974 2822 2722 295b 315d 0a20  .split("'")[1]. 
+00001350: 2020 2064 6174 615f 6c69 7374 5b30 5d2e     data_list[0].
+00001360: 7570 6461 7465 287b 22e4 b8aa e4ba bae8  update({".......
+00001370: b584 e696 9922 3a70 6c61 7965 725f 7572  .....":player_ur
+00001380: 6c7d 290a 2020 2020 2320 e88e b7e5 8f96  l}).    # ......
+00001390: e4b8 80e8 a880 0a20 2020 206d 6573 7361  .......    messa
+000013a0: 6765 203d 2064 6174 612e 7365 6c65 6374  ge = data.select
+000013b0: 2822 6874 6d6c 2062 6f64 7920 6469 762e  ("html body div.
+000013c0: 636f 6e74 656e 742e 7465 7874 2d63 656e  content.text-cen
+000013d0: 7465 722e 7465 7874 2d6d 642d 6c65 6674  ter.text-md-left
+000013e0: 2064 6976 2e63 6f6e 7461 696e 6572 2e74   div.container.t
+000013f0: 6578 742d 6c65 6674 2064 6976 2e63 6f6c  ext-left div.col
+00001400: 2d6d 642d 3132 2e68 2d31 3030 2064 6976  -md-12.h-100 div
+00001410: 2e63 6172 642d 626f 6479 2e77 6f72 6c64  .card-body.world
+00001420: 6d61 702e 642d 666c 6578 2e66 6c65 782d  map.d-flex.flex-
+00001430: 636f 6c75 6d6e 2e6a 7573 7469 6679 2d63  column.justify-c
+00001440: 6f6e 7465 6e74 2d63 656e 7465 722e 7465  ontent-center.te
+00001450: 7874 2d63 656e 7465 7220 7370 616e 2229  xt-center span")
+00001460: 0a20 2020 206d 7367 5f6c 6973 7420 3d20  .    msg_list = 
+00001470: 5b5d 0a20 2020 2066 6f72 2069 2069 6e20  [].    for i in 
+00001480: 6d65 7373 6167 653a 0a20 2020 2020 2020  message:.       
+00001490: 206d 7367 5f6c 6973 742e 6170 7065 6e64   msg_list.append
+000014a0: 2869 2e74 6578 7429 0a20 2020 2064 6174  (i.text).    dat
+000014b0: 615f 6c69 7374 5b30 5d2e 7570 6461 7465  a_list[0].update
+000014c0: 287b 22e4 b880 e8a8 8022 3a6d 7367 5f6c  ({"......":msg_l
+000014d0: 6973 747d 290a 2020 2020 7265 7475 726e  ist}).    return
+000014e0: 2064 6174 615f 6c69 7374 0a0a 6465 6620   data_list..def 
+000014f0: 616e 6e65 5f72 616e 6b5f 6469 6374 5f6d  anne_rank_dict_m
+00001500: 7367 2864 6174 615f 6c69 7374 293a 0a20  sg(data_list):. 
+00001510: 2020 2022 2222 e5ad 97e5 85b8 e8bd ac6d     """.........m
+00001520: 7367 2222 220a 2020 2020 6d73 6720 3d20  sg""".    msg = 
+00001530: 2727 0a20 2020 2066 6f72 2064 6174 615f  ''.    for data_
+00001540: 6469 6374 2069 6e20 6461 7461 5f6c 6973  dict in data_lis
+00001550: 743a 0a20 2020 2020 2020 206d 6573 203d  t:.        mes =
+00001560: 2027 270a 2020 2020 2020 2020 666f 7220   ''.        for 
+00001570: 6920 696e 2064 6174 615f 6469 6374 3a0a  i in data_dict:.
+00001580: 2020 2020 2020 2020 2020 2020 6d65 7320              mes 
+00001590: 2b3d 275c 6e27 2b20 6920 2b20 6461 7461  +='\n'+ i + data
+000015a0: 5f64 6963 745b 695d 0a20 2020 2020 2020  _dict[i].       
+000015b0: 206d 6573 202b 3d20 275c 6e2d 2d2d 2d2d   mes += '\n-----
+000015c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d27  ---------------'
+000015d0: 0a20 2020 2020 2020 206d 7367 202b 3d20  .        msg += 
+000015e0: 6d65 730a 2020 2020 7265 7475 726e 206d  mes.    return m
+000015f0: 7367 0a0a 0a61 7379 6e63 2064 6566 2061  sg...async def a
+00001600: 6e6e 655f 6d65 7373 6761 6528 6e61 6d65  nne_messgae(name
+00001610: 3a73 7472 2c75 7372 5f69 643a 7374 7229  :str,usr_id:str)
+00001620: 3a0a 2020 2020 2222 22e8 8eb7 e58f 9661  :.    """......a
+00001630: 6e6e 65e4 bfa1 e681 afe5 8faf e8be 93e5  nne.............
+00001640: 87ba e4bf a1e6 81af 2222 220a 2020 2020  ........""".    
+00001650: 6966 206e 616d 653a 0a20 2020 2020 2020  if name:.       
+00001660: 206c 6f67 6765 722e 696e 666f 2822 e585   logger.info("..
+00001670: b3e9 94ae e8af 8de6 9fa5 e8af a222 202b  ............." +
+00001680: 206e 616d 6529 0a20 2020 2020 2020 2069   name).        i
+00001690: 6620 6e6f 7420 6e61 6d65 2e73 7461 7274  f not name.start
+000016a0: 7377 6974 6828 2753 5445 414d 2729 3a0a  swith('STEAM'):.
+000016b0: 2020 2020 2020 2020 2020 2020 7374 6561              stea
+000016c0: 6d69 6420 3d20 6177 6169 7420 6964 5f74  mid = await id_t
+000016d0: 6f5f 6d65 7328 6e61 6d65 290a 2020 2020  o_mes(name).    
+000016e0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+000016f0: 7465 616d 6964 3a0a 2020 2020 2020 2020  teamid:.        
+00001700: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00001710: 6e66 6f28 22e6 b2a1 e69c 89e6 89be e588  nfo("...........
+00001720: b071 71ef bc8c e4bd bfe7 94a8 e9bb 98e8  .qq.............
+00001730: aea4 e5a4 b4e5 838f 2229 0a20 2020 2020  ........").     
+00001740: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00001750: 6765 203d 2061 7761 6974 2061 6e6e 655f  ge = await anne_
+00001760: 6874 6d6c 286e 616d 6529 0a20 2020 2020  html(name).     
+00001770: 2020 2020 2020 2020 2020 2075 7372 5f69             usr_i
+00001780: 6420 3d20 2231 3134 3531 3439 3139 3138  d = "11451491918
+00001790: 3130 220a 2020 2020 2020 2020 2020 2020  10".            
+000017a0: 2020 2020 6966 206c 656e 286d 6573 7361      if len(messa
+000017b0: 6765 2920 3d3d 2030 3a0a 2020 2020 2020  ge) == 0:.      
+000017c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000017d0: 7475 726e 2027 e6b2 a1e6 9c89 e58f abe8  turn '..........
+000017e0: bf99 e4b8 aae5 908d e5ad 97e7 9a84 2e2e  ................
+000017f0: 2e5c 6e27 0a20 2020 2020 2020 2020 2020  .\n'.           
+00001800: 2020 2020 2069 6620 6c65 6e28 6d65 7373       if len(mess
+00001810: 6167 6529 203e 2031 3a0a 2020 2020 2020  age) > 1:.      
+00001820: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00001830: 7475 726e 2061 6e6e 655f 6874 6d6c 5f6d  turn anne_html_m
+00001840: 7367 286d 6573 7361 6765 290a 2020 2020  sg(message).    
+00001850: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00001860: 203d 206d 6573 7361 6765 5b30 5d5b 2773   = message[0]['s
+00001870: 7465 616d 6964 275d 0a20 2020 2020 2020  teamid'].       
+00001880: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00001890: 2020 2020 2020 2020 2020 206e 616d 6520             name 
+000018a0: 3d20 7374 6561 6d69 640a 2020 2020 2020  = steamid.      
+000018b0: 2020 2320 7374 6561 6d69 640a 2020 2020    # steamid.    
+000018c0: 2020 2020 6d73 6720 3d20 616e 6e65 5f72      msg = anne_r
+000018d0: 616e 6b5f 6469 6374 286e 616d 6529 5b30  ank_dict(name)[0
+000018e0: 5d0a 2020 2020 2020 2020 6966 2074 7970  ].        if typ
+000018f0: 6528 6d73 6729 203d 3d20 6469 6374 3a0a  e(msg) == dict:.
+00001900: 2020 2020 2020 2020 2020 2020 6d73 672e              msg.
+00001910: 7570 6461 7465 2861 7761 6974 2064 665f  update(await df_
+00001920: 746f 5f67 756f 6775 616e 6c76 2861 7761  to_guoguanlv(awa
+00001930: 6974 2061 6e6e 655f 6d61 705f 6d73 6728  it anne_map_msg(
+00001940: 6e61 6d65 2929 290a 2020 2020 2020 2020  name))).        
+00001950: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00001960: 27e4 bdbf e794 a8e5 9bbe e789 8727 290a  '............').
+00001970: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+00001980: 3d20 6177 6169 7420 6f75 745f 706e 6728  = await out_png(
+00001990: 7573 725f 6964 2c6d 7367 290a 2020 2020  usr_id,msg).    
+000019a0: 2020 2020 7265 7475 726e 206d 7367 0a20      return msg. 
+000019b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000019c0: 2022 2222 0a20 2020 2020 2020 2031 e380   """.        1..
+000019d0: 8171 713e e695 b0e6 8dae 3ee6 b2a1 e69c  .qq>......>.....
+000019e0: 89e6 95b0 e68d aeef bc8c e8bf 94e5 9b9e  ................
+000019f0: 0a20 2020 2020 2020 2032 e380 8171 713e  .        2...qq>
+00001a00: e695 b0e6 8dae 3e73 7465 616d 6964 3ee6  ......>steamid>.
+00001a10: 9fa5 e8af a20a 2020 2020 2020 2020 33e3  ......        3.
+00001a20: 8081 7171 3ee6 95b0 e68d ae3e e698 b5e7  ..qq>......>....
+00001a30: a7b0 3ee6 9fa5 e8af a20a 2020 2020 2020  ..>.......      
+00001a40: 2020 2222 220a 2020 2020 2020 2020 6c6f    """.        lo
+00001a50: 6767 6572 2e69 6e66 6f28 2271 71e4 bfa1  gger.info("qq...
+00001a60: e681 afe6 9fa5 e8af a222 290a 2020 2020  .........").    
+00001a70: 2020 2020 6461 7461 5f74 7570 6c65 203d      data_tuple =
+00001a80: 2073 2e5f 7175 6572 795f 706c 6179 6572   s._query_player
+00001a90: 5f71 7128 7573 725f 6964 290a 2020 2020  _qq(usr_id).    
+00001aa0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00001ab0: 6461 7461 5f74 7570 6c65 290a 2020 2020  data_tuple).    
+00001ac0: 2020 2020 6966 2064 6174 615f 7475 706c      if data_tupl
+00001ad0: 653d 3d20 4e6f 6e65 3a0a 2020 2020 2020  e== None:.      
+00001ae0: 2020 2020 2020 7265 7475 726e 2066 22e6        return f".
+00001af0: b2a1 e69c 89e7 bb91 e5ae 9ae4 bfa1 e681  ................
+00001b00: af2e 2e2e e8af b7e4 bdbf e794 a8e3 8090  ................
+00001b10: e6b1 82e7 949f e7bb 91e5 ae9a 2078 7878  ............ xxx
+00001b20: e380 915c 6e22 0a20 2020 2020 2020 2023  ...\n".        #
+00001b30: 20e5 8faa e69c 89e5 908d e5ad 97ef bc8c   ...............
+00001b40: e585 88e6 9fa5 e8af a2e6 95b0 e68d aee5  ................
+00001b50: 9ca8 e588 a4e6 96ad 0a20 2020 2020 2020  .........       
+00001b60: 2065 6c69 6620 6461 7461 5f74 7570 6c65   elif data_tuple
+00001b70: 5b32 5d3a 0a20 2020 2020 2020 2020 2020  [2]:.           
+00001b80: 206e 616d 6520 3d20 6461 7461 5f74 7570   name = data_tup
+00001b90: 6c65 5b32 5d0a 2020 2020 2020 2020 656c  le[2].        el
+00001ba0: 6966 2064 6174 615f 7475 706c 655b 315d  if data_tuple[1]
+00001bb0: 3a0a 2020 2020 2020 2020 2020 2020 6e61  :.            na
+00001bc0: 6d65 203d 2061 7761 6974 2069 645f 746f  me = await id_to
+00001bd0: 5f6d 6573 2864 6174 615f 7475 706c 655b  _mes(data_tuple[
+00001be0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
+00001bf0: 6c6f 6767 6572 2e69 6e66 6f28 6e61 6d65  logger.info(name
+00001c00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00001c10: 206e 6f74 206e 616d 653a 0a20 2020 2020   not name:.     
+00001c20: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00001c30: 6765 203d 2061 7761 6974 2061 6e6e 655f  ge = await anne_
+00001c40: 6874 6d6c 2864 6174 615f 7475 706c 655b  html(data_tuple[
+00001c50: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
+00001c60: 2020 2020 7573 725f 6964 203d 2022 3131      usr_id = "11
+00001c70: 3435 3134 3931 3931 3831 3022 0a20 2020  45149191810".   
+00001c80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00001c90: 6c65 6e28 6d65 7373 6167 6529 203d 3d20  len(message) == 
+00001ca0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00001cb0: 2020 2020 2020 2072 6574 7572 6e20 27e6         return '.
+00001cc0: b2a1 e69c 89e5 8fab e8bf 99e4 b8aa e590  ................
+00001cd0: 8de5 ad97 e79a 842e 2e2e 5c6e 270a 2020  ..........\n'.  
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001cf0: 206c 656e 286d 6573 7361 6765 2920 3e20   len(message) > 
+00001d00: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+00001d10: 2020 2020 2020 2072 6574 7572 6e20 616e         return an
+00001d20: 6e65 5f68 746d 6c5f 6d73 6728 6d65 7373  ne_html_msg(mess
+00001d30: 6167 6529 0a20 2020 2020 2020 2020 2020  age).           
+00001d40: 2020 2020 206e 616d 6520 3d20 6d65 7373       name = mess
+00001d50: 6167 655b 305d 5b27 7374 6561 6d69 6427  age[0]['steamid'
+00001d60: 5d0a 2020 2020 2020 2020 2320 6e61 6d65  ].        # name
+00001d70: e698 af73 7465 616d 6964 0a20 2020 2020  ...steamid.     
+00001d80: 2020 206d 7367 203d 2061 6e6e 655f 7261     msg = anne_ra
+00001d90: 6e6b 5f64 6963 7428 6e61 6d65 295b 305d  nk_dict(name)[0]
+00001da0: 0a20 2020 2020 2020 2069 6620 7479 7065  .        if type
+00001db0: 286d 7367 2920 3d3d 2064 6963 743a 0a20  (msg) == dict:. 
+00001dc0: 2020 2020 2020 2020 2020 206d 7367 2e75             msg.u
+00001dd0: 7064 6174 6528 6177 6169 7420 6466 5f74  pdate(await df_t
+00001de0: 6f5f 6775 6f67 7561 6e6c 7628 6177 6169  o_guoguanlv(awai
+00001df0: 7420 616e 6e65 5f6d 6170 5f6d 7367 286e  t anne_map_msg(n
+00001e00: 616d 6529 2929 0a20 2020 2020 2020 2020  ame))).         
+00001e10: 2020 206c 6f67 6765 722e 696e 666f 2827     logger.info('
+00001e20: e4bd bfe7 94a8 e59b bee7 8987 2729 0a20  ............'). 
+00001e30: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
+00001e40: 2061 7761 6974 206f 7574 5f70 6e67 2875   await out_png(u
+00001e50: 7372 5f69 642c 6d73 6729 0a20 2020 2020  sr_id,msg).     
+00001e60: 2020 2072 6574 7572 6e20 6d73 670a 2020     return msg.  
+00001e70: 2020 0a61 7379 6e63 2064 6566 2061 6e6e    .async def ann
+00001e80: 655f 6d61 705f 6d73 6728 7374 6561 6d69  e_map_msg(steami
+00001e90: 643a 7374 7229 3a0a 2020 2020 2222 2273  d:str):.    """s
+00001ea0: 7465 616d 6964 2d3e e59c b0e5 9bbe e4bf  teamid->........
+00001eb0: a1e6 81af 2222 220a 2020 2020 7572 6c20  ....""".    url 
+00001ec0: 3d20 6622 6874 7470 733a 2f2f 7362 2e74  = f"https://sb.t
+00001ed0: 7279 6765 6b2e 636f 6d2f 6c34 645f 7374  rygek.com/l4d_st
+00001ee0: 6174 732f 7261 6e6b 696e 672f 7469 6d65  ats/ranking/time
+00001ef0: 646d 6170 732e 7068 703f 7374 6561 6d69  dmaps.php?steami
+00001f00: 643d 7b73 7465 616d 6964 7d22 0a20 2020  d={steamid}".   
+00001f10: 2068 6561 6465 7273 203d 207b 0a20 2020   headers = {.   
+00001f20: 2020 2020 2027 5573 6572 2d41 6765 6e74       'User-Agent
+00001f30: 273a 274d 6f7a 696c 6c61 2f35 2e30 2028  ':'Mozilla/5.0 (
+00001f40: 5769 6e64 6f77 7320 4e54 2031 302e 303b  Windows NT 10.0;
+00001f50: 2057 696e 3634 3b20 7836 343b 2072 763a   Win64; x64; rv:
+00001f60: 3130 372e 3029 2047 6563 6b6f 2f32 3031  107.0) Gecko/201
+00001f70: 3030 3130 3120 4669 7265 666f 782f 3130  00101 Firefox/10
+00001f80: 372e 3027 0a20 2020 207d 0a20 2020 2064  7.0'.    }.    d
+00001f90: 6174 6120 3d20 6874 7470 782e 6765 7428  ata = httpx.get(
+00001fa0: 7572 6c2c 6865 6164 6572 733d 6865 6164  url,headers=head
+00001fb0: 6572 732c 7469 6d65 6f75 743d 3529 2e63  ers,timeout=5).c
+00001fc0: 6f6e 7465 6e74 2e64 6563 6f64 6528 2775  ontent.decode('u
+00001fd0: 7466 2d38 2729 0a20 2020 2073 6f75 7020  tf-8').    soup 
+00001fe0: 3d20 4265 6175 7469 6675 6c53 6f75 7028  = BeautifulSoup(
+00001ff0: 6461 7461 2c20 2768 746d 6c2e 7061 7273  data, 'html.pars
+00002000: 6572 2729 0a20 2020 2064 6174 615f 6c69  er').    data_li
+00002010: 7374 203d 205b 5d0a 2020 2020 6361 7264  st = [].    card
+00002020: 7320 3d20 736f 7570 2e73 656c 6563 7428  s = soup.select(
+00002030: 2764 6976 2e63 6172 642e 726f 756e 6465  'div.card.rounde
+00002040: 642d 3027 290a 2020 2020 666f 7220 6361  d-0').    for ca
+00002050: 7264 2069 6e20 6361 7264 733a 0a20 2020  rd in cards:.   
+00002060: 2020 2020 2074 626f 6469 6573 203d 2063       tbodies = c
+00002070: 6172 642e 7365 6c65 6374 2827 7462 6f64  ard.select('tbod
+00002080: 7927 290a 2020 2020 2020 2020 666f 7220  y').        for 
+00002090: 7462 6f64 7920 696e 2074 626f 6469 6573  tbody in tbodies
+000020a0: 3a0a 2020 2020 2020 2020 2020 2020 726f  :.            ro
+000020b0: 7773 203d 205b 7464 2e74 6578 742e 7374  ws = [td.text.st
+000020c0: 7269 7028 2920 666f 7220 7464 2069 6e20  rip() for td in 
+000020d0: 7462 6f64 792e 6669 6e64 5f61 6c6c 2827  tbody.find_all('
+000020e0: 7464 2729 5d0a 2020 2020 2020 2020 2020  td')].          
+000020f0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00002100: 2830 2c20 6c65 6e28 726f 7773 292c 2039  (0, len(rows), 9
+00002110: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00002120: 2020 2072 6f77 203d 2072 6f77 735b 693a     row = rows[i:
+00002130: 692b 395d 0a20 2020 2020 2020 2020 2020  i+9].           
+00002140: 2020 2020 2064 6174 615f 6c69 7374 2e61       data_list.a
+00002150: 7070 656e 6428 726f 7729 0a20 2020 2064  ppend(row).    d
+00002160: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+00002170: 2864 6174 615f 6c69 7374 2c20 636f 6c75  (data_list, colu
+00002180: 6d6e 733d 5b27 e6b8 b8e6 888f e6a8 a1e5  mns=['..........
+00002190: bc8f 272c 2027 e59c b0e5 9bbe 272c 2027  ..', '......', '
+000021a0: e99a bee5 baa6 272c 2027 e5ae 8ce6 8890  ......', '......
+000021b0: e697 b6e9 97b4 272c 2027 e789 b9e6 849f  ......', '......
+000021c0: e695 b0e9 878f 272c 2027 e588 b7e6 96b0  ......', '......
+000021d0: e997 b4e9 9a94 272c 2027 42e6 95b0 e4bd  ......', 'B.....
+000021e0: bfe7 94a8 272c 2027 e588 b7e7 89b9 e6a8  ....', '........
+000021f0: a1e5 bc8f 272c 2027 416e 6e65 e789 88e6  ....', 'Anne....
+00002200: 9cac 275d 290a 2020 2020 7265 7475 726e  ..']).    return
+00002210: 2064 66                                   df
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from .startand import SAVE_MAP,NUMBER_MAP
-import pandas as pd
-
-async def df_to_guoguanlv(df:pd.DataFrame):
-    """分析救援关过图率"""
-    data = df[df['游戏模式'] == 'AnneHappy药役']
-    other = df[df['游戏模式'].isin(['牛牛冲刺', '单人装逼'])]
-    all_map = len(data['地图'])
-    other_map = len(other['地图'])
-    resen = 0
-    last_maps = {}
-    for m in SAVE_MAP:
-        prefix = m.split('m')[0]
-        if prefix in last_maps:
-            last_maps[prefix] = max(last_maps[prefix], m)
-        else:
-            last_maps[prefix] = m
-
-    map_counts = {}
-
-    n = 0
-    for key in last_maps:
-        count = len(data[data['地图'].str.startswith(key)])
-        if count == 0:
-            continue
-        last_map = last_maps[key]
-        map_count = len(data[data['地图'] == last_map])
-        map_counts[key] = map_count*NUMBER_MAP[n] / count
-        quan = count/all_map
-        resen += quan * map_counts[key]
-        n += 1
-
-    # result = []
-    # for i in range(1, 15):
-    #     key = 'c{}'.format(i)
-    #     if key in map_counts:
-    #         result.append('{}:{}%'.format(key, round(map_counts[key] * 100)))
-            
-    # print(result)
-    # result = '救援图过关率: {:.2%}'.format(resen)
-    
-    # 加上特殊关卡
-    try:
-        resen += other_map / (all_map + other_map)
-        result = {"救援关":str('{:.2%}'.format(resen))}
-    except (TypeError,KeyError):
-        result = {"救援关":"错误"}
-    except ZeroDivisionError:
-        result = {"救援关":"0.00%"}
-    except:
-        result = {"救援关":"错误"}
+from .startand import SAVE_MAP,NUMBER_MAP
+import pandas as pd
+
+async def df_to_guoguanlv(df:pd.DataFrame):
+    """分析救援关过图率"""
+    data = df[df['游戏模式'] == 'AnneHappy药役']
+    other = df[df['游戏模式'].isin(['牛牛冲刺', '单人装逼'])]
+    all_map = len(data['地图'])
+    other_map = len(other['地图'])
+    resen = 0
+    last_maps = {}
+    for m in SAVE_MAP:
+        prefix = m.split('m')[0]
+        if prefix in last_maps:
+            last_maps[prefix] = max(last_maps[prefix], m)
+        else:
+            last_maps[prefix] = m
+
+    map_counts = {}
+
+    n = 0
+    for key in last_maps:
+        count = len(data[data['地图'].str.startswith(key)])
+        if count == 0:
+            continue
+        last_map = last_maps[key]
+        map_count = len(data[data['地图'] == last_map])
+        map_counts[key] = map_count*NUMBER_MAP[n] / count
+        quan = count/all_map
+        resen += quan * map_counts[key]
+        n += 1
+
+    # result = []
+    # for i in range(1, 15):
+    #     key = 'c{}'.format(i)
+    #     if key in map_counts:
+    #         result.append('{}:{}%'.format(key, round(map_counts[key] * 100)))
+            
+    # print(result)
+    # result = '救援图过关率: {:.2%}'.format(resen)
+    
+    # 加上特殊关卡
+    try:
+        resen += other_map / (all_map + other_map)
+        result = {"救援关":str('{:.2%}'.format(resen))}
+    except (TypeError,KeyError):
+        result = {"救援关":"错误"}
+    except ZeroDivisionError:
+        result = {"救援关":"0.00%"}
+    except:
+        result = {"救援关":"错误"}
     return result
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# from ..l4d2_image.steam import url_to_byte
-# from bs4 import BeautifulSoup
-# from typing import List
-
-# 暂时废弃
-# class ANNE_API:
-    
-#     async def __init__(
-#         self,
-#         STEAMID:str,
-#         tag:str
-#     ):
-#         self.STEAMID = STEAMID
-#         if tag == '中':
-#             msg1 = await self.anne_msg()
-#         elif tag == '长':
-#             msg1 = await self.anne_msg()
-#             msg1.update(await self.anne_map())
-        
-    
-#     async def anne_msg(self):
-#         """个人资料表"""
-#         data_bytes = await url_to_byte('https://sb.trygek.com/l4d_stats/ranking/player.php?steamid={self.STEAMID}')
-#         data_bs = BeautifulSoup(data_bytes, 'html.parser')
-#         data_fom = data_bs.find_all('table')
-#         n = 0
-#         data_dict = {}
-#         while n < 2:
-#             data_list:List[dict] = []
-#             detail2 = data_fom[n]
-#             tr = detail2.find_all('tr')
-#             for i in tr:
-#                 title = i.find('td', {'class': 'w-50'})
-#                 value = title.find_next_sibling('td')
-#                 new_dict = {title.text:value.text}
-#                 data_dict.update(new_dict)
-#             data_list.append(data_dict)
-#             n += 1
-#         # 获取头像
-#         element:str = data_fom.find_all(attrs={"style": "cursor:pointer"})[0].get("onclick")
-#         player_url = element.split("'")[1]
-#         data_list[0].update({"个人资料":player_url})
-#         # 获取一言
-#         message = data_fom.select("html body div.content.text-center.text-md-left div.container.text-left div.col-md-12.h-100 div.card-body.worldmap.d-flex.flex-column.justify-content-center.text-center span")
-#         msg_list = []
-#         for i in message:
-#             msg_list.append(i.text)
-#         data_list[0].update({"一言":msg_list})
-#         return data_list
-        
-#     async def anne_map(self):
-#         """个人地图表"""
-#         data_dict = {}
-#         data_bytes = await url_to_byte('https://sb.trygek.com/l4d_stats/ranking/timedmaps.php?steamid={self.STEAMID}')
-#         data_bs = BeautifulSoup(data_bytes, 'html.parser')
-#         tbody = data_bs.select('tbody')
-#         for tr in tbody:
-#             tds = tr.select('td')
-#             n = 0
-#             for td in tds:
-#                 n += 1
-#                 title:str = td['data-title'][:-1]
-#                 data_text = td.text
-#                 if title == '特感数量':
-#                     special_amount = data_text
-#                 elif title == '刷新间隔':
-#                     refresh_interval = data_text
-#                 else:
-#                     if title in data_dict:
-#                         data_dict[title].append(data_text)
-#                     else:
-#                         data_dict[title] = [data_text]
-#             if special_amount and refresh_interval:
-#                 data_dict['刷特时间'] = special_amount + refresh_interval
-                
+# from ..l4d2_image.steam import url_to_byte
+# from bs4 import BeautifulSoup
+# from typing import List
+
+# 暂时废弃
+# class ANNE_API:
+    
+#     async def __init__(
+#         self,
+#         STEAMID:str,
+#         tag:str
+#     ):
+#         self.STEAMID = STEAMID
+#         if tag == '中':
+#             msg1 = await self.anne_msg()
+#         elif tag == '长':
+#             msg1 = await self.anne_msg()
+#             msg1.update(await self.anne_map())
+        
+    
+#     async def anne_msg(self):
+#         """个人资料表"""
+#         data_bytes = await url_to_byte('https://sb.trygek.com/l4d_stats/ranking/player.php?steamid={self.STEAMID}')
+#         data_bs = BeautifulSoup(data_bytes, 'html.parser')
+#         data_fom = data_bs.find_all('table')
+#         n = 0
+#         data_dict = {}
+#         while n < 2:
+#             data_list:List[dict] = []
+#             detail2 = data_fom[n]
+#             tr = detail2.find_all('tr')
+#             for i in tr:
+#                 title = i.find('td', {'class': 'w-50'})
+#                 value = title.find_next_sibling('td')
+#                 new_dict = {title.text:value.text}
+#                 data_dict.update(new_dict)
+#             data_list.append(data_dict)
+#             n += 1
+#         # 获取头像
+#         element:str = data_fom.find_all(attrs={"style": "cursor:pointer"})[0].get("onclick")
+#         player_url = element.split("'")[1]
+#         data_list[0].update({"个人资料":player_url})
+#         # 获取一言
+#         message = data_fom.select("html body div.content.text-center.text-md-left div.container.text-left div.col-md-12.h-100 div.card-body.worldmap.d-flex.flex-column.justify-content-center.text-center span")
+#         msg_list = []
+#         for i in message:
+#             msg_list.append(i.text)
+#         data_list[0].update({"一言":msg_list})
+#         return data_list
+        
+#     async def anne_map(self):
+#         """个人地图表"""
+#         data_dict = {}
+#         data_bytes = await url_to_byte('https://sb.trygek.com/l4d_stats/ranking/timedmaps.php?steamid={self.STEAMID}')
+#         data_bs = BeautifulSoup(data_bytes, 'html.parser')
+#         tbody = data_bs.select('tbody')
+#         for tr in tbody:
+#             tds = tr.select('td')
+#             n = 0
+#             for td in tds:
+#                 n += 1
+#                 title:str = td['data-title'][:-1]
+#                 data_text = td.text
+#                 if title == '特感数量':
+#                     special_amount = data_text
+#                 elif title == '刷新间隔':
+#                     refresh_interval = data_text
+#                 else:
+#                     if title in data_dict:
+#                         data_dict[title].append(data_text)
+#                     else:
+#                         data_dict[title] = [data_text]
+#             if special_amount and refresh_interval:
+#                 data_dict['刷特时间'] = special_amount + refresh_interval
+                
 #         return data_dict
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import httpx
-from bs4 import BeautifulSoup
-import json
-from pathlib import Path
-from ..config import TEXT_PATH,anne_url,ANNE_IP,gamemode_list
-from ..l4d2_queries.ohter import ALL_HOST
-
-# 储存anne服务器ip
-
-
-
-
-async def updata_anne_server():
-    """更新anne服务器列表"""
-    data = httpx.get(anne_url).content
-    soup = BeautifulSoup(data, 'html.parser')
-    tbody = soup.find('tbody')
-    n = 0
-    ip_list=[]
-    while n < 50:
-        n += 1
-        tr = tbody.find(id = f'server_{n}')
-        if tr:
-            td = tr.select_one("td:nth-of-type(5)").get_text()
-        else:
-            continue
-        if td:
-            ip_list.append(td)
-    if not ip_list:
-        return None
-    ip_dict = {}
-    n = 0
-    for i in ip_list:
-        n += 1
-        ip_dict.update({f'云{n}':ip_list[n-1]})
-    ANNE_IP.update(ip_dict)
-    with open(Path(TEXT_PATH.parent/'server.json'),'w',encoding='utf-8') as f:
-        json.dump(ANNE_IP, f, indent=4, ensure_ascii=False)
-    return ANNE_IP
-
-async def read_anne_ip():
-    """获取缓存ip"""
-    with open(TEXT_PATH.parent/'server.json','r','utf-8') as f:
-        data = json.load(f)
-        return data
-    
-async def get_anne_ip(text: str) -> str:
-    """从字典里返还消息, 抄(借鉴)的zhenxun-bot"""
-    keys = ANNE_IP.keys()
-    for key in keys:
-        if text == key:
-            return ANNE_IP[key]
-        
-def server_key():
-    """响应的服务器开头"""
-    a = set()
-    try:
-        for tag1,value in ALL_HOST.items():
-            a.add(tag1)
-        a.update(gamemode_list)
-    except AttributeError:
-        a.add('希腊那我从来没有想过这个事情')
-    return a
-            
-            
+import httpx
+from bs4 import BeautifulSoup
+import json
+from pathlib import Path
+from ..config import TEXT_PATH,anne_url,ANNE_IP,gamemode_list
+from ..l4d2_queries.ohter import ALL_HOST
+
+# 储存anne服务器ip
+
+
+
+
+async def updata_anne_server():
+    """更新anne服务器列表"""
+    data = httpx.get(anne_url).content
+    soup = BeautifulSoup(data, 'html.parser')
+    tbody = soup.find('tbody')
+    n = 0
+    ip_list=[]
+    while n < 50:
+        n += 1
+        tr = tbody.find(id = f'server_{n}')
+        if tr:
+            td = tr.select_one("td:nth-of-type(5)").get_text()
+        else:
+            continue
+        if td:
+            ip_list.append(td)
+    if not ip_list:
+        return None
+    ip_dict = {}
+    n = 0
+    for i in ip_list:
+        n += 1
+        ip_dict.update({f'云{n}':ip_list[n-1]})
+    ANNE_IP.update(ip_dict)
+    with open(Path(TEXT_PATH.parent/'server.json'),'w',encoding='utf-8') as f:
+        json.dump(ANNE_IP, f, indent=4, ensure_ascii=False)
+    return ANNE_IP
+
+async def read_anne_ip():
+    """获取缓存ip"""
+    with open(TEXT_PATH.parent/'server.json','r','utf-8') as f:
+        data = json.load(f)
+        return data
+    
+async def get_anne_ip(text: str) -> str:
+    """从字典里返还消息, 抄(借鉴)的zhenxun-bot"""
+    keys = ANNE_IP.keys()
+    for key in keys:
+        if text == key:
+            return ANNE_IP[key]
+        
+def server_key():
+    """响应的服务器开头"""
+    a = set()
+    try:
+        for tag1,value in ALL_HOST.items():
+            a.add(tag1)
+        a.update(gamemode_list)
+    except AttributeError:
+        a.add('希腊那我从来没有想过这个事情')
+    return a
+            
+
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from ..config import (
-    DATASQLITE,
-    table_data,
-    L4d2_players_tag,
-    L4d2_server_tag,
-    L4d2_INTEGER,
-    L4d2_TEXT,
-    L4d2_BOOLEAN,
-    tables_columns
-    )
-import sqlite3
-from nonebot.log import logger
-
-
-
-
-class L4D2DataSqlite:
-    """连接数据库和断开数据库，以及一些检查函数"""
-    def __init__(self):
-        """连接数据库"""
-        self.datasqlite_path = DATASQLITE
-        self.datasqlite_path.mkdir(parents=True, exist_ok=True)
-        self.conn = sqlite3.connect(self.datasqlite_path / 'L4D2.db')
-        self._check_tables_exist()
-        self._check_data_existence()
-        self._check_data_validity()
-        logger.info("已连接求生数据库")
-    
-    def _base_conn(self):
-        return self.conn
-        
-    def _check_tables_exist(self) -> None:
-        """
-        检查表是否存在
-        """  
-        c = self.conn.cursor()
-        for table in table_data:
-            c.execute(f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table}'")
-            if c.fetchone() is None:
-                if table == "L4d2_players":
-                    c.execute(f"CREATE TABLE {table} (qq INTEGER PRIMARY KEY)")
-                elif table == "L4D2_server":
-                    c.execute(f"CREATE TABLE {table} (number INTEGER PRIMARY KEY)")
-                self.conn.commit()
-        
-        
-
-    def _check_data_existence(self) -> None:
-        """
-        检查表头是否存在，如果不存在则新建并填充默认值
-        """
-        c = self.conn.cursor()
-        for table, tag in tables_columns.items():
-            for column in tag:
-                c.execute(f"PRAGMA table_info({table})")
-                if not any(col[1] == column for col in c.fetchall()):
-                    if column in L4d2_BOOLEAN:
-                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} BOOLEAN DEFAULT 0')
-                    elif column in L4d2_INTEGER:
-                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} INTEGER DEFAULT NULL')
-                    else:
-                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} TEXT DEFAULT NULL')
-        self.conn.commit()
-
-    
-    def _check_data_validity(self) -> None:
-        """
-        检查数据库数据的合法性
-        错误数据默认填充NULL或者False
-        """
-        c = self.conn.cursor()
-        for table in table_data:
-            if table == "L4d2_players":
-                columns = L4d2_players_tag
-            elif table == "L4D2_server":
-                columns = L4d2_server_tag
-        for column in columns:
-            if column in L4d2_INTEGER:
-                c.execute(f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'integer'")
-            elif column in L4d2_TEXT:
-                c.execute(f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'text'")
-            elif column in L4d2_BOOLEAN:
-                c.execute(f"UPDATE {table} SET {column} = 'False' WHERE typeof({column}) != 'boolean'")
-        self.conn.commit()
-        
-    def _close(self):
-        """断开连接到数据库"""
-        self.conn.close()
-        logger.info("已断开求生数据库")
-
-
+from ..config import (
+    DATASQLITE,
+    table_data,
+    L4d2_players_tag,
+    L4d2_server_tag,
+    L4d2_INTEGER,
+    L4d2_TEXT,
+    L4d2_BOOLEAN,
+    tables_columns
+    )
+import sqlite3
+from nonebot.log import logger
+
+
+
+
+class L4D2DataSqlite:
+    """连接数据库和断开数据库，以及一些检查函数"""
+    def __init__(self):
+        """连接数据库"""
+        self.datasqlite_path = DATASQLITE
+        self.datasqlite_path.mkdir(parents=True, exist_ok=True)
+        self.conn = sqlite3.connect(self.datasqlite_path / 'L4D2.db')
+        self._check_tables_exist()
+        self._check_data_existence()
+        self._check_data_validity()
+        logger.info("已连接求生数据库")
+    
+    def _base_conn(self):
+        return self.conn
+        
+    def _check_tables_exist(self) -> None:
+        """
+        检查表是否存在
+        """  
+        c = self.conn.cursor()
+        for table in table_data:
+            c.execute(f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table}'")
+            if c.fetchone() is None:
+                if table == "L4d2_players":
+                    c.execute(f"CREATE TABLE {table} (qq INTEGER PRIMARY KEY)")
+                elif table == "L4D2_server":
+                    c.execute(f"CREATE TABLE {table} (number INTEGER PRIMARY KEY)")
+                self.conn.commit()
+        
+        
+
+    def _check_data_existence(self) -> None:
+        """
+        检查表头是否存在，如果不存在则新建并填充默认值
+        """
+        c = self.conn.cursor()
+        for table, tag in tables_columns.items():
+            for column in tag:
+                c.execute(f"PRAGMA table_info({table})")
+                if not any(col[1] == column for col in c.fetchall()):
+                    if column in L4d2_BOOLEAN:
+                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} BOOLEAN DEFAULT 0')
+                    elif column in L4d2_INTEGER:
+                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} INTEGER DEFAULT NULL')
+                    else:
+                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} TEXT DEFAULT NULL')
+        self.conn.commit()
+
+    
+    def _check_data_validity(self) -> None:
+        """
+        检查数据库数据的合法性
+        错误数据默认填充NULL或者False
+        """
+        c = self.conn.cursor()
+        for table in table_data:
+            if table == "L4d2_players":
+                columns = L4d2_players_tag
+            elif table == "L4D2_server":
+                columns = L4d2_server_tag
+        for column in columns:
+            if column in L4d2_INTEGER:
+                c.execute(f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'integer'")
+            elif column in L4d2_TEXT:
+                c.execute(f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'text'")
+            elif column in L4d2_BOOLEAN:
+                c.execute(f"UPDATE {table} SET {column} = 'False' WHERE typeof({column}) != 'boolean'")
+        self.conn.commit()
+        
+    def _close(self):
+        """断开连接到数据库"""
+        self.conn.close()
+        logger.info("已断开求生数据库")
+
+
 sq_L4D2 = L4D2DataSqlite()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from ..config import DATASQLITE
-import sqlite3
-from typing import Union,Tuple
-
-
-class L4D2Player:
-    """数据库L4D2_Player表的操作""" 
-    def __init__(self):
-        """连接数据库"""
-        self.datasqlite_path = DATASQLITE
-        self.conn = sqlite3.connect(self.datasqlite_path / 'L4D2.db')
-        self.c = self.conn.cursor()
-        
-    async def _add_player_nickname(self, qq, nickname):
-        """绑定昵称"""
-        # try:
-        self.c.execute("INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,NULL)", (qq, nickname))
-        self.conn.commit()
-        #     return True
-        # except sqlite3.IntegrityError:
-        #     return False
-
-    async def _add_player_steamid(self, qq, steamid):
-        """绑定steamid"""
-        self.c.execute("INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,NULL,?)", (qq, steamid))
-        self.conn.commit()
-
-              
-    async def _add_player_all(self, qq, nickname,steamid):
-        """用新数据覆盖旧数据"""
-        # try:
-        self.c.execute("INSERT OR REPLACE INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,?)", (qq, nickname,steamid))
-        self.conn.commit()
-        return True
-        # except sqlite3.IntegrityError:
-        #     return False
-        
-    def _delete_player(self, qq):
-        """解除绑定"""
-        self.c.execute(f"DELETE FROM L4d2_players WHERE qq = {qq}")
-        self.conn.commit()
-        return True
-        
-    def _query_player_qq(self, qq) -> Union[tuple,None]:
-        """通过qq获取数据"""
-        self.c.execute(f"SELECT * FROM L4d2_players WHERE qq = '{qq}'")
-        return self.c.fetchone()
-    
-    async def _query_player_nickname(self, nickname:str) -> Union[tuple,None]:
-        """通过nickname获取数据"""
-        self.c.execute(f"SELECT * FROM L4d2_players WHERE nickname = '{nickname}'")
-        return self.c.fetchone()
-
-    async def _query_player_steamid(self, steamid:str):
-        """通过steamid获取数据"""
-        self.c.execute(f"SELECT * FROM L4d2_players WHERE steamid = '{steamid}'")
-        data_tuple = self.c.fetchone()
-        return data_tuple
-    
-    async def search_data(self, qq, nickname, steamid) -> Union[tuple,None]:
-        """
-        输入元组查询，优先qq其次steamid最后nickname，不需要值可以为None
-        输出为元组，如果为空输出None
-        data = (qq , nickname , steamid )
-        """
-        if qq:
-            self.c.execute("SELECT * FROM L4d2_players WHERE qq=?", (qq,))
-            result = self.c.fetchone()
-            if result:
-                return result
-        if steamid:
-            self.c.execute("SELECT * FROM L4d2_players WHERE steamid=?", (steamid,))
-            result = self.c.fetchone()
-            if result:
-                return result
-        if nickname:
-            self.c.execute("SELECT * FROM L4d2_players WHERE nickname=?", (nickname,))
-            result = self.c.fetchone()
-            if result:
-                return result
-        return None
-    
-    def _query_all_player(self) -> Tuple[tuple]:
-        """获取所有玩家信息"""
-        self.c.execute("SELECT * FROM L4d2_players")
-        return self.c.fetchall()
-    
+from ..config import DATASQLITE
+import sqlite3
+from typing import Union,Tuple
+
+
+class L4D2Player:
+    """数据库L4D2_Player表的操作""" 
+    def __init__(self):
+        """连接数据库"""
+        self.datasqlite_path = DATASQLITE
+        self.conn = sqlite3.connect(self.datasqlite_path / 'L4D2.db')
+        self.c = self.conn.cursor()
+        
+    async def _add_player_nickname(self, qq, nickname):
+        """绑定昵称"""
+        # try:
+        self.c.execute("INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,NULL)", (qq, nickname))
+        self.conn.commit()
+        #     return True
+        # except sqlite3.IntegrityError:
+        #     return False
+
+    async def _add_player_steamid(self, qq, steamid):
+        """绑定steamid"""
+        self.c.execute("INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,NULL,?)", (qq, steamid))
+        self.conn.commit()
+
+              
+    async def _add_player_all(self, qq, nickname,steamid):
+        """用新数据覆盖旧数据"""
+        # try:
+        self.c.execute("INSERT OR REPLACE INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,?)", (qq, nickname,steamid))
+        self.conn.commit()
+        return True
+        # except sqlite3.IntegrityError:
+        #     return False
+        
+    def _delete_player(self, qq):
+        """解除绑定"""
+        self.c.execute(f"DELETE FROM L4d2_players WHERE qq = {qq}")
+        self.conn.commit()
+        return True
+        
+    def _query_player_qq(self, qq) -> Union[tuple,None]:
+        """通过qq获取数据"""
+        self.c.execute(f"SELECT * FROM L4d2_players WHERE qq = '{qq}'")
+        return self.c.fetchone()
+    
+    async def _query_player_nickname(self, nickname:str) -> Union[tuple,None]:
+        """通过nickname获取数据"""
+        self.c.execute(f"SELECT * FROM L4d2_players WHERE nickname = '{nickname}'")
+        return self.c.fetchone()
+
+    async def _query_player_steamid(self, steamid:str):
+        """通过steamid获取数据"""
+        self.c.execute(f"SELECT * FROM L4d2_players WHERE steamid = '{steamid}'")
+        data_tuple = self.c.fetchone()
+        return data_tuple
+    
+    async def search_data(self, qq, nickname, steamid) -> Union[tuple,None]:
+        """
+        输入元组查询，优先qq其次steamid最后nickname，不需要值可以为None
+        输出为元组，如果为空输出None
+        data = (qq , nickname , steamid )
+        """
+        if qq:
+            self.c.execute("SELECT * FROM L4d2_players WHERE qq=?", (qq,))
+            result = self.c.fetchone()
+            if result:
+                return result
+        if steamid:
+            self.c.execute("SELECT * FROM L4d2_players WHERE steamid=?", (steamid,))
+            result = self.c.fetchone()
+            if result:
+                return result
+        if nickname:
+            self.c.execute("SELECT * FROM L4d2_players WHERE nickname=?", (nickname,))
+            result = self.c.fetchone()
+            if result:
+                return result
+        return None
+    
+    def _query_all_player(self) -> Tuple[tuple]:
+        """获取所有玩家信息"""
+        self.c.execute("SELECT * FROM L4d2_players")
+        return self.c.fetchall()
+
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from pathlib import Path
-from zipfile import ZipFile
-from time import sleep
-import sys
-import os
-import io
-from typing import List
-
-from ..utils import get_file,get_vpk
-from ..config import systems
-from nonebot.log import logger
-from rarfile import RarFile
-import rarfile
-from pyunpack import Archive
-
-
-
-async def updown_l4d2_vpk(map_paths,name,url):
-    """从url下载压缩包并解压到位置"""
-    original_vpk_files = []
-    original_vpk_files = get_vpk(original_vpk_files,map_paths)
-    down_file = Path(map_paths,name)
-    if await get_file(url,down_file) == None:
-        return None
-    sleep(1)
-    msg = open_packet(name,down_file)
-    logger.info(msg)
-    
-    sleep(1)
-    extracted_vpk_files = []
-    extracted_vpk_files = get_vpk(extracted_vpk_files,map_paths)
-    # 获取新增vpk文件的list
-    vpk_files = list(set(extracted_vpk_files) - set(original_vpk_files))
-    return  vpk_files
-
-def open_packet(name:str,down_file:Path):
-    """解压压缩包"""
-    down_path = os.path.dirname(down_file)
-    logger.info('文件名为：' + name)
-    logger.info(f'系统为{systems}')
-    if systems == 'win':
-        if name.endswith('.zip'):
-            mes = 'zip文件已下载,正在解压'
-            try:
-                with support_gbk(ZipFile(down_file, 'r')) as z:
-                    z.extractall(down_path)
-            except UnicodeEncodeError:
-                with ZipFile(down_file, 'r') as z:
-                    z.extractall(down_path)                
-            os.remove(down_file)
-        elif name.endswith('.7z'):
-            mes ='7z文件已下载,正在解压'
-            Archive(down_file).extractall(down_path)
-            # with SevenZipFile(down_file, 'r') as z:
-            #     z.extractall(down_path)
-            os.remove(down_file)
-        elif name.endswith('rar'):
-            mes = 'rar文件已下载,正在解压'
-            with RarFile(down_file,'r') as z:
-                z.extractall(down_path)
-            os.remove(down_file)
-        elif name.endswith('.vpk'):
-            mes ='vpk文件已下载'
-    else:
-        if name.endswith('.zip'):
-            mes = 'zip文件已下载,正在解压'
-            with support_gbk(ZipFile(down_file, 'r')) as z:
-                z.extractall(down_path)
-            os.remove(down_file)
-        elif name.endswith('.7z'):
-            mes ='7z文件已下载,正在解压'
-            Archive(down_file).extractall(down_path)
-            # with SevenZipFile(down_file, 'r') as z:
-            #     z.extractall(down_path)
-            os.remove(down_file)
-        elif name.endswith('rar'):
-            mes = 'rar文件已下载,正在解压'
-            with rarfile.RarFile(down_file,'r') as z:
-                z.extractall(down_path)
-            os.remove(down_file)
-        else:
-            mes ='vpk文件已下载'        
-    return mes
-
-def support_gbk(zip_file:ZipFile):
-    '''
-    压缩包中文恢复
-    '''
-    if type(zip_file) == ZipFile:
-        name_to_info = zip_file.NameToInfo
-        # copy map first
-        for name, info in name_to_info.copy().items():
-            real_name = name.encode('cp437').decode('gbk')
-            if real_name != name:
-                info.filename = real_name
-                del name_to_info[name]
-                name_to_info[real_name] = info
-    return zip_file
-
-
-
-
-async def all_zip_to_one(data_list:List[bytes]):
-    """多压缩包文件合并"""
-    file_list = []
-    for data in data_list:
-        # 将每个bytes对象解压缩成文件对象
-        # 将文件对象存储在一个列表中
-        file_list.append(io.BytesIO(data))
-
-    # 创建一个新的BytesIO对象
-    data_file = io.BytesIO()
-
-    # 使用zipfile将列表中的文件对象添加到zipfile中
-    with ZipFile(data_file, mode='w') as zf:
-        for i, file in enumerate(file_list):
-            # 将文件名设置为"file{i}.zip"，i为文件在列表中的索引
-            filename = f"file{i}.zip"
-            zf.writestr(filename, file.getvalue())
-
-    # 获取zipfile的bytes对象
-    return data_file.getvalue()
+from pathlib import Path
+from zipfile import ZipFile
+from time import sleep
+import sys
+import os
+import io
+from typing import List
+
+from ..utils import get_file,get_vpk
+from ..config import systems
+from nonebot.log import logger
+from rarfile import RarFile
+import rarfile
+from pyunpack import Archive
+
+
+
+async def updown_l4d2_vpk(map_paths,name,url):
+    """从url下载压缩包并解压到位置"""
+    original_vpk_files = []
+    original_vpk_files = get_vpk(original_vpk_files,map_paths)
+    down_file = Path(map_paths,name)
+    if await get_file(url,down_file) == None:
+        return None
+    sleep(1)
+    msg = open_packet(name,down_file)
+    logger.info(msg)
+    
+    sleep(1)
+    extracted_vpk_files = []
+    extracted_vpk_files = get_vpk(extracted_vpk_files,map_paths)
+    # 获取新增vpk文件的list
+    vpk_files = list(set(extracted_vpk_files) - set(original_vpk_files))
+    return  vpk_files
+
+def open_packet(name:str,down_file:Path):
+    """解压压缩包"""
+    down_path = os.path.dirname(down_file)
+    logger.info('文件名为：' + name)
+    logger.info(f'系统为{systems}')
+    if systems == 'win':
+        if name.endswith('.zip'):
+            mes = 'zip文件已下载,正在解压'
+            try:
+                with support_gbk(ZipFile(down_file, 'r')) as z:
+                    z.extractall(down_path)
+            except UnicodeEncodeError:
+                with ZipFile(down_file, 'r') as z:
+                    z.extractall(down_path)                
+            os.remove(down_file)
+        elif name.endswith('.7z'):
+            mes ='7z文件已下载,正在解压'
+            Archive(down_file).extractall(down_path)
+            # with SevenZipFile(down_file, 'r') as z:
+            #     z.extractall(down_path)
+            os.remove(down_file)
+        elif name.endswith('rar'):
+            mes = 'rar文件已下载,正在解压'
+            with RarFile(down_file,'r') as z:
+                z.extractall(down_path)
+            os.remove(down_file)
+        elif name.endswith('.vpk'):
+            mes ='vpk文件已下载'
+    else:
+        if name.endswith('.zip'):
+            mes = 'zip文件已下载,正在解压'
+            with support_gbk(ZipFile(down_file, 'r')) as z:
+                z.extractall(down_path)
+            os.remove(down_file)
+        elif name.endswith('.7z'):
+            mes ='7z文件已下载,正在解压'
+            Archive(down_file).extractall(down_path)
+            # with SevenZipFile(down_file, 'r') as z:
+            #     z.extractall(down_path)
+            os.remove(down_file)
+        elif name.endswith('rar'):
+            mes = 'rar文件已下载,正在解压'
+            with rarfile.RarFile(down_file,'r') as z:
+                z.extractall(down_path)
+            os.remove(down_file)
+        else:
+            mes ='vpk文件已下载'        
+    return mes
+
+def support_gbk(zip_file:ZipFile):
+    '''
+    压缩包中文恢复
+    '''
+    if type(zip_file) == ZipFile:
+        name_to_info = zip_file.NameToInfo
+        # copy map first
+        for name, info in name_to_info.copy().items():
+            real_name = name.encode('cp437').decode('gbk')
+            if real_name != name:
+                info.filename = real_name
+                del name_to_info[name]
+                name_to_info[real_name] = info
+    return zip_file
+
+
+
+
+async def all_zip_to_one(data_list:List[bytes]):
+    """多压缩包文件合并"""
+    file_list = []
+    for data in data_list:
+        # 将每个bytes对象解压缩成文件对象
+        # 将文件对象存储在一个列表中
+        file_list.append(io.BytesIO(data))
+
+    # 创建一个新的BytesIO对象
+    data_file = io.BytesIO()
+
+    # 使用zipfile将列表中的文件对象添加到zipfile中
+    with ZipFile(data_file, mode='w') as zf:
+        for i, file in enumerate(file_list):
+            # 将文件名设置为"file{i}.zip"，i为文件在列表中的索引
+            filename = f"file{i}.zip"
+            zf.writestr(filename, file.getvalue())
+
+    # 获取zipfile的bytes对象
+    return data_file.getvalue()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import asyncio
-import asyncssh
-
-class AsyncSSHClient:
-    def __init__(self, host, port, username, password=None, private_key=None):
-        self.host = host
-        self.port = port
-        self.username = username
-        self.password = password
-        self.private_key = private_key
-
-    async def connect(self):
-        if self.private_key is not None:
-            try:
-                key = asyncssh.read_private_key(self.private_key)
-            except asyncssh.Error as exc:
-                raise ValueError(f"Unable to read private key: {exc}")
-        else:
-            key = None
-
-        self.conn = await asyncssh.connect(
-            self.host, self.port, 
-            username = self.username, 
-            password=self.password, 
-            client_keys=key
-        )
-
-    async def upload(self, local_path, remote_path):
-        async with self.conn.sftp() as sftp:
-            await sftp.put(local_path, remote_path)
-
-    async def delete(self, remote_path):
-        async with self.conn.sftp() as sftp:
-            await sftp.remove(remote_path)
-
-    async def listdir(self, remote_path):
-        async with self.conn.sftp() as sftp:
-            return await sftp.listdir(remote_path)
-
-    async def close(self):
-        self.conn.close()
-
-async def remote(mode:str,host:str,user:str,password:str,local_path = '',port=22, remote_path = ''):
-    """mode:upload、read、del"""
-    client = AsyncSSHClient(host, port,user, password)
-    await client.connect()
-    if mode == 'upload':
-        await client.upload(local_path, remote_path)
-    elif mode == 'read':
-        file = await client.read(remote_path)
-        return file
-    elif mode == 'del':
-        await client.delete(remote_path)
-
-if __name__ == '__main__':
-    asyncio.run(remote(mode='upload',host='106.13.207.45',user='root',password='Taojie@114514',local_path='E:\\zhang\\文件\\login_info.txt',remote_path='/home/'))
+import asyncio
+import asyncssh
+
+class AsyncSSHClient:
+    def __init__(self, host, port, username, password=None, private_key=None):
+        self.host = host
+        self.port = port
+        self.username = username
+        self.password = password
+        self.private_key = private_key
+
+    async def connect(self):
+        if self.private_key is not None:
+            try:
+                key = asyncssh.read_private_key(self.private_key)
+            except asyncssh.Error as exc:
+                raise ValueError(f"Unable to read private key: {exc}")
+        else:
+            key = None
+
+        self.conn = await asyncssh.connect(
+            self.host, self.port, 
+            username = self.username, 
+            password=self.password, 
+            client_keys=key
+        )
+
+    async def upload(self, local_path, remote_path):
+        async with self.conn.sftp() as sftp:
+            await sftp.put(local_path, remote_path)
+
+    async def delete(self, remote_path):
+        async with self.conn.sftp() as sftp:
+            await sftp.remove(remote_path)
+
+    async def listdir(self, remote_path):
+        async with self.conn.sftp() as sftp:
+            return await sftp.listdir(remote_path)
+
+    async def close(self):
+        self.conn.close()
+
+async def remote(mode:str,host:str,user:str,password:str,local_path = '',port=22, remote_path = ''):
+    """mode:upload、read、del"""
+    client = AsyncSSHClient(host, port,user, password)
+    await client.connect()
+    if mode == 'upload':
+        await client.upload(local_path, remote_path)
+    elif mode == 'read':
+        file = await client.read(remote_path)
+        return file
+    elif mode == 'del':
+        await client.delete(remote_path)
+
+if __name__ == '__main__':
+    asyncio.run(remote(mode='upload',host='106.13.207.45',user='root',password='Taojie@114514',local_path='E:\\zhang\\文件\\login_info.txt',remote_path='/home/'))
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import asyncio
-import paramiko
-
-class SSHClient:
-    def __init__(self, hostname, port, username, password):
-        self._hostname = hostname
-        self._port = port
-        self._username = username
-        self._password = password
-        self._ssh = None
-
-    async def connect(self):
-        self._ssh = paramiko.SSHClient()
-        self._ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-        await asyncio.get_event_loop().run_in_executor(None, self._ssh.connect, self._hostname, self._port, self._username, self._password)
-
-    async def upload(self, local_file_path, remote_file_path):
-        with paramiko.Transport((self._hostname, self._port)) as transport:
-            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
-            sftp = paramiko.SFTPClient.from_transport(transport)
-            await asyncio.get_event_loop().run_in_executor(None, sftp.put, local_file_path, remote_file_path)
-
-
-    async def delete(self, remote_file_path):
-        with paramiko.Transport((self._hostname, self._port)) as transport:
-            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
-            sftp = paramiko.SFTPClient.from_transport(transport)
-            await asyncio.get_event_loop().run_in_executor(None, sftp.remove, remote_file_path)
-
-    async def read(self, remote_dir_path):
-        with paramiko.Transport((self._hostname, self._port)) as transport:
-            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
-            sftp = paramiko.SFTPClient.from_transport(transport)
-            return await asyncio.get_event_loop().run_in_executor(None, sftp.listdir, remote_dir_path)
-
-    async def close(self):
-        if self._ssh is not None:
-            self._ssh.close()
-
-# async def main():
-#     ssh = SSHClient("example.com", 22, "username", "password")
-#     await ssh.connect()
-
-#     await ssh.upload("/path/to/local/file", "/path/to/remote/file")
-#     await ssh.delete("/path/to/remote/file")
-#     files = await ssh.list("/path/to/remote/directory")
-#     print(files)
-
-#     await ssh.close()
-
-# if __name__ == '__main__':
-#     asyncio.run(main())
-
-async def remote(mode:str,host,user,password,local_path = '',port=22, remote_path = ''):
-    """mode:upload、read、del"""
-    client = SSHClient(host, port,user, password)
-    if mode == 'upload':
-        await client.upload(local_path, remote_path)
-    elif mode == 'read':
-        file = await client.read(remote_path)
-        return file
-    elif mode == 'del':
-        await client.delete(remote_path)
+import asyncio
+import paramiko
+
+class SSHClient:
+    def __init__(self, hostname, port, username, password):
+        self._hostname = hostname
+        self._port = port
+        self._username = username
+        self._password = password
+        self._ssh = None
+
+    async def connect(self):
+        self._ssh = paramiko.SSHClient()
+        self._ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+        await asyncio.get_event_loop().run_in_executor(None, self._ssh.connect, self._hostname, self._port, self._username, self._password)
+
+    async def upload(self, local_file_path, remote_file_path):
+        with paramiko.Transport((self._hostname, self._port)) as transport:
+            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
+            sftp = paramiko.SFTPClient.from_transport(transport)
+            await asyncio.get_event_loop().run_in_executor(None, sftp.put, local_file_path, remote_file_path)
+
+
+    async def delete(self, remote_file_path):
+        with paramiko.Transport((self._hostname, self._port)) as transport:
+            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
+            sftp = paramiko.SFTPClient.from_transport(transport)
+            await asyncio.get_event_loop().run_in_executor(None, sftp.remove, remote_file_path)
+
+    async def read(self, remote_dir_path):
+        with paramiko.Transport((self._hostname, self._port)) as transport:
+            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
+            sftp = paramiko.SFTPClient.from_transport(transport)
+            return await asyncio.get_event_loop().run_in_executor(None, sftp.listdir, remote_dir_path)
+
+    async def close(self):
+        if self._ssh is not None:
+            self._ssh.close()
+
+# async def main():
+#     ssh = SSHClient("example.com", 22, "username", "password")
+#     await ssh.connect()
+
+#     await ssh.upload("/path/to/local/file", "/path/to/remote/file")
+#     await ssh.delete("/path/to/remote/file")
+#     files = await ssh.list("/path/to/remote/directory")
+#     print(files)
+
+#     await ssh.close()
+
+# if __name__ == '__main__':
+#     asyncio.run(main())
+
+async def remote(mode:str,host,user,password,local_path = '',port=22, remote_path = ''):
+    """mode:upload、read、del"""
+    client = SSHClient(host, port,user, password)
+    if mode == 'upload':
+        await client.upload(local_path, remote_path)
+    elif mode == 'read':
+        file = await client.read(remote_path)
+        return file
+    elif mode == 'del':
+        await client.delete(remote_path)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-
-from bs4 import BeautifulSoup
-from nonebot.log import logger
-from nonebot_plugin_htmlrender import html_to_pic
-from typing import List,Optional
-# from .htmlimg import dict_to_dict_img
-# from ..l4d2_anne.anne_telecom import ANNE_API
-from ..config import TEXT_PATH
-from .download import get_head_by_user_id_and_save
-from .send_image_tool import convert_img
-import jinja2
-from ..config import l4_config
-template_path = TEXT_PATH/"template"
-
-env = jinja2.Environment(
-    loader=jinja2.FileSystemLoader(template_path), enable_async=True
-)
-
-async def out_png(usr_id,data_dict:dict):
-    """使用html来生成图片"""
-    
-    with open((template_path/"anne.html"),"r", encoding="utf-8") as file:
-        data_html = file.read()
-    # content = template.render_async()
-    soup = BeautifulSoup(data_html, 'html.parser')
-    msg_dict = await dict_to_html(usr_id,data_dict,soup)
-    template = env.get_template('anne.html')
-    html = await template.render_async(data=msg_dict)
-    pic = await html_to_pic(
-                html,
-                wait=0,
-                viewport={"width": 1100, "height": 800},
-                template_path=f"file://{template_path.absolute()}",)
-    print(type(pic))
-    return pic
-
-
-async def dict_to_html(usr_id,DETAIL_MAP:dict,soup:BeautifulSoup):
-    """输入qq、字典，获取新的msg替换html"""
-    DETAIL_right = {}
-    DETAIL_right['name'] = DETAIL_MAP['Steam 名字:']
-    DETAIL_right['Steam_ID'] = DETAIL_MAP['Steam ID:']
-    DETAIL_right['play_time'] = DETAIL_MAP['游玩时间:']
-    DETAIL_right['last_online'] = DETAIL_MAP['最后上线:']
-    DETAIL_right['rank'] = DETAIL_MAP['排行:']
-    DETAIL_right['points'] = DETAIL_MAP['分数:']
-    DETAIL_right['point_min'] = DETAIL_MAP['每分钟获取分数:']
-    DETAIL_right['killed'] = DETAIL_MAP['感染者消灭:']
-    DETAIL_right['shut'] = DETAIL_MAP['爆头:']        
-    DETAIL_right['out'] = DETAIL_MAP['爆头率:']
-    DETAIL_right['playtimes'] = DETAIL_MAP['游玩地图数量:']
-    DETAIL_right['url'] = DETAIL_MAP['个人资料']
-    DETAIL_right['one_msg'] = DETAIL_MAP['一言']
-    DETAIL_right['last_one'] = DETAIL_MAP['救援关']
-    # html_text = soup.prettify()
-    # for key, value in DETAIL_right.items():
-    #     html_text = html_text.replace(key,value)
-    # 头像
-    temp = await get_head_by_user_id_and_save(usr_id)
-    # temp = await get_head_steam_and_save(usr_id,DETAIL_right['url'])
-    res = await convert_img(temp,is_base64=True)
-    DETAIL_right['header'] = f"data:image/png;base64,{res}"
-    data_list:List[dict] = [DETAIL_right]
-    return data_list
-
-
-async def server_ip_pic(msg_list:List[dict]):
-    """
-    输入一个字典列表，输出图片
-    msg_dict:folder/name/map_/players/max_players/Players/[Name]
-    """
-    for server_info in msg_list:
-        server_info['max_players'] = f"{server_info['players']}/{server_info['max_players']}"
-        players_list = []
-        if 'Players' in server_info:
-            sorted_players = sorted(server_info['Players'], key=lambda x: x.get('Score', 0), reverse=True)[:4]
-            for player_info in sorted_players:
-                player_str = f"{player_info['name']} | {player_info['Duration']}"
-                players_list.append(player_str)
-            while len(players_list) < 4:
-                players_list.append("")
-            server_info['Players'] = players_list
-    pic = await get_help_img(msg_list)
-
-    return pic
-
-
-async def get_help_img(plugins: List[dict]) -> Optional[bytes]:
-    try:
-        if l4_config.l4_style == 'black':
-            template = env.get_template("help_dack.html")
-        else:
-            template = env.get_template("help.html")
-        content = await template.render_async(plugins=plugins)
-        return await html_to_pic(
-            content,
-            wait=0,
-            viewport={"width": 100, "height": 100},
-            template_path=f"file://{template_path.absolute()}",
-        )
-    except Exception as e:
-        logger.warning(f"Error in get_help_img: {e}")
-        return None
+
+from bs4 import BeautifulSoup
+from nonebot.log import logger
+from nonebot_plugin_htmlrender import html_to_pic
+from typing import List,Optional
+# from .htmlimg import dict_to_dict_img
+# from ..l4d2_anne.anne_telecom import ANNE_API
+from ..config import TEXT_PATH
+from .download import get_head_by_user_id_and_save
+from .send_image_tool import convert_img
+import jinja2
+from ..config import l4_config
+template_path = TEXT_PATH/"template"
+
+env = jinja2.Environment(
+    loader=jinja2.FileSystemLoader(template_path), enable_async=True
+)
+
+async def out_png(usr_id,data_dict:dict):
+    """使用html来生成图片"""
+    
+    with open((template_path/"anne.html"),"r", encoding="utf-8") as file:
+        data_html = file.read()
+    # content = template.render_async()
+    soup = BeautifulSoup(data_html, 'html.parser')
+    msg_dict = await dict_to_html(usr_id,data_dict,soup)
+    template = env.get_template('anne.html')
+    html = await template.render_async(data=msg_dict)
+    pic = await html_to_pic(
+                html,
+                wait=0,
+                viewport={"width": 1100, "height": 800},
+                template_path=f"file://{template_path.absolute()}",)
+    print(type(pic))
+    return pic
+
+
+async def dict_to_html(usr_id,DETAIL_MAP:dict,soup:BeautifulSoup):
+    """输入qq、字典，获取新的msg替换html"""
+    DETAIL_right = {}
+    DETAIL_right['name'] = DETAIL_MAP['Steam 名字:']
+    DETAIL_right['Steam_ID'] = DETAIL_MAP['Steam ID:']
+    DETAIL_right['play_time'] = DETAIL_MAP['游玩时间:']
+    DETAIL_right['last_online'] = DETAIL_MAP['最后上线:']
+    DETAIL_right['rank'] = DETAIL_MAP['排行:']
+    DETAIL_right['points'] = DETAIL_MAP['分数:']
+    DETAIL_right['point_min'] = DETAIL_MAP['每分钟获取分数:']
+    DETAIL_right['killed'] = DETAIL_MAP['感染者消灭:']
+    DETAIL_right['shut'] = DETAIL_MAP['爆头:']        
+    DETAIL_right['out'] = DETAIL_MAP['爆头率:']
+    DETAIL_right['playtimes'] = DETAIL_MAP['游玩地图数量:']
+    DETAIL_right['url'] = DETAIL_MAP['个人资料']
+    DETAIL_right['one_msg'] = DETAIL_MAP['一言']
+    DETAIL_right['last_one'] = DETAIL_MAP['救援关']
+    # html_text = soup.prettify()
+    # for key, value in DETAIL_right.items():
+    #     html_text = html_text.replace(key,value)
+    # 头像
+    temp = await get_head_by_user_id_and_save(usr_id)
+    # temp = await get_head_steam_and_save(usr_id,DETAIL_right['url'])
+    res = await convert_img(temp,is_base64=True)
+    DETAIL_right['header'] = f"data:image/png;base64,{res}"
+    data_list:List[dict] = [DETAIL_right]
+    return data_list
+
+
+async def server_ip_pic(msg_list:List[dict]):
+    """
+    输入一个字典列表，输出图片
+    msg_dict:folder/name/map_/players/max_players/Players/[Name]
+    """
+    for server_info in msg_list:
+        server_info['max_players'] = f"{server_info['players']}/{server_info['max_players']}"
+        players_list = []
+        if 'Players' in server_info:
+            sorted_players = sorted(server_info['Players'], key=lambda x: x.get('Score', 0), reverse=True)[:4]
+            for player_info in sorted_players:
+                player_str = f"{player_info['name']} | {player_info['Duration']}"
+                players_list.append(player_str)
+            while len(players_list) < 4:
+                players_list.append("")
+            server_info['Players'] = players_list
+    pic = await get_help_img(msg_list)
+
+    return pic
+
+
+async def get_help_img(plugins: List[dict]) -> Optional[bytes]:
+    try:
+        if l4_config.l4_style == 'black':
+            template = env.get_template("help_dack.html")
+        else:
+            template = env.get_template("help.html")
+        content = await template.render_async(plugins=plugins)
+        return await html_to_pic(
+            content,
+            wait=0,
+            viewport={"width": 100, "height": 100},
+            template_path=f"file://{template_path.absolute()}",
+        )
+    except Exception as e:
+        logger.warning(f"Error in get_help_img: {e}")
+        return None
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import httpx
-from nonebot.log import logger
-import asyncio
-import hashlib
-import os
-import random
-from PIL import Image,ImageDraw
-import io
-from ..config import PLAYERSDATA,TEXT_PATH
-# from .steam import web_player
-
-async def download_url(url: str) -> bytes:
-    async with httpx.AsyncClient() as client:
-        for i in range(3):
-            try:
-                resp = await client.get(url, timeout=20)
-                resp.raise_for_status()
-                return resp.content
-            except Exception as e:
-                logger.warning(f"Error downloading {url}, retry {i}/3: {e}")
-                await asyncio.sleep(3)
-    raise Exception(f"{url} 下载失败！")
-
-async def download_head(user_id: str) -> bytes:
-    url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
-    data = await download_url(url)
-    if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
-        url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
-        data = await download_url(url)
-    return data
-
-    
-def square_to_circle(im:Image):
-    """im是正方形，变圆形"""
-    size = im.size
-    mask = Image.new('L', size, 0)
-    draw = ImageDraw.Draw(mask)
-    draw.ellipse((0, 0) + size, fill=255)
-    # 将遮罩层应用到图像上
-    im.putalpha(mask)
-    return im
-
-async def get_head_by_user_id_and_save(user_id):
-    """qq转头像"""
-    user_id = str(user_id)
-    
-    USER_HEAD_PATH = PLAYERSDATA / user_id / 'HEAD.png'
-    DEFAULT_HEADER_PATH = TEXT_PATH / "header"
-    DEFAULT_HEAD_PATH = TEXT_PATH / "head"
-    DEFAULT_HEADER = DEFAULT_HEADER_PATH /random.choice(os.listdir(DEFAULT_HEADER_PATH))
-    DEFAULT_HEAD = DEFAULT_HEAD_PATH /random.choice(os.listdir(DEFAULT_HEAD_PATH))
-    ## im头像 im2头像框 im3合成
-    if os.path.exists(USER_HEAD_PATH):
-        logger.info("使用本地头像")
-        im = Image.open(USER_HEAD_PATH).resize((280, 280)).convert("RGBA")
-    else:
-        if user_id == "1145149191810":
-            logger.info("使用默认头像")
-            im = Image.open(DEFAULT_HEADER).resize((280, 280)).convert("RGBA")
-        else:
-            try:
-                logger.info("正在下载头像")
-                image_bytes = await download_head(user_id)
-                im = Image.open(io.BytesIO(image_bytes)).resize((280, 280)).convert("RGBA")
-                if not os.path.exists(PLAYERSDATA / user_id):#用户文件夹不存在
-                    os.makedirs(PLAYERSDATA / user_id)
-                im.save(USER_HEAD_PATH, "PNG")
-            except:
-                logger.error("获取失败")
-    im2 = Image.open(DEFAULT_HEAD).resize((450,450)).convert("RGBA")
-    im3 = Image.new("RGBA", im2.size, (255,255,255,0))
-    r, g, b, a1 = im.split()
-    r, g, b, a2 = im2.split()
-    im = square_to_circle(im)
-    im3.paste(im,(75,75),mask=a1)
-    im3.paste(im2,mask=a2)
-    return im3
-
-# async def get_head_steam_and_save(user_id:str,urls):
-#     """保存steam头像"""
-#     USER_HEAD_PATH = PLAYERSDATA / str(user_id) / 'HEAD.png'
-#     # DEFAULT_HEAD_PATH = TEXT_PATH / "template/player.jpg"
-#     ## im头像 im2头像框 im3合成
-#     if os.path.exists(USER_HEAD_PATH):
-#         logger.info("使用本地头像")
-#         im = Image.open(USER_HEAD_PATH).resize((280, 280)).convert("RGBA")
-#     else:
-#         # if user_id == "1145149191810":
-#         #     logger.info("使用默认头像")
-#         #     im = Image.open(DEFAULT_HEAD_PATH).resize((300, 300)).convert("RGBA")
-#         # else:
-#             try:
-#                 logger.info("正在下载头像")
-#                 image_bytes = await web_player(urls)
-#                 im = Image.open(io.BytesIO(image_bytes)).resize((280, 280)).convert("RGBA")
-#                 if not os.path.exists(PLAYERSDATA / user_id):#用户文件夹不存在
-#                     os.makedirs(PLAYERSDATA / user_id)
-#                 im.save(USER_HEAD_PATH, "PNG")
-#             except TimeoutError:
-#                 logger.error("获取失败")
-#     return im
+import httpx
+from nonebot.log import logger
+import asyncio
+import hashlib
+import os
+import random
+from PIL import Image,ImageDraw
+import io
+from ..config import PLAYERSDATA,TEXT_PATH
+# from .steam import web_player
+
+async def download_url(url: str) -> bytes:
+    async with httpx.AsyncClient() as client:
+        for i in range(3):
+            try:
+                resp = await client.get(url, timeout=20)
+                resp.raise_for_status()
+                return resp.content
+            except Exception as e:
+                logger.warning(f"Error downloading {url}, retry {i}/3: {e}")
+                await asyncio.sleep(3)
+    raise Exception(f"{url} 下载失败！")
+
+async def download_head(user_id: str) -> bytes:
+    url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
+    data = await download_url(url)
+    if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
+        url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
+        data = await download_url(url)
+    return data
+
+    
+def square_to_circle(im:Image):
+    """im是正方形，变圆形"""
+    size = im.size
+    mask = Image.new('L', size, 0)
+    draw = ImageDraw.Draw(mask)
+    draw.ellipse((0, 0) + size, fill=255)
+    # 将遮罩层应用到图像上
+    im.putalpha(mask)
+    return im
+
+async def get_head_by_user_id_and_save(user_id):
+    """qq转头像"""
+    user_id = str(user_id)
+    
+    USER_HEAD_PATH = PLAYERSDATA / user_id / 'HEAD.png'
+    DEFAULT_HEADER_PATH = TEXT_PATH / "header"
+    DEFAULT_HEAD_PATH = TEXT_PATH / "head"
+    DEFAULT_HEADER = DEFAULT_HEADER_PATH /random.choice(os.listdir(DEFAULT_HEADER_PATH))
+    DEFAULT_HEAD = DEFAULT_HEAD_PATH /random.choice(os.listdir(DEFAULT_HEAD_PATH))
+    ## im头像 im2头像框 im3合成
+    if os.path.exists(USER_HEAD_PATH):
+        logger.info("使用本地头像")
+        im = Image.open(USER_HEAD_PATH).resize((280, 280)).convert("RGBA")
+    else:
+        if user_id == "1145149191810":
+            logger.info("使用默认头像")
+            im = Image.open(DEFAULT_HEADER).resize((280, 280)).convert("RGBA")
+        else:
+            try:
+                logger.info("正在下载头像")
+                image_bytes = await download_head(user_id)
+                im = Image.open(io.BytesIO(image_bytes)).resize((280, 280)).convert("RGBA")
+                if not os.path.exists(PLAYERSDATA / user_id):#用户文件夹不存在
+                    os.makedirs(PLAYERSDATA / user_id)
+                im.save(USER_HEAD_PATH, "PNG")
+            except:
+                logger.error("获取失败")
+    im2 = Image.open(DEFAULT_HEAD).resize((450,450)).convert("RGBA")
+    im3 = Image.new("RGBA", im2.size, (255,255,255,0))
+    r, g, b, a1 = im.split()
+    r, g, b, a2 = im2.split()
+    im = square_to_circle(im)
+    im3.paste(im,(75,75),mask=a1)
+    im3.paste(im2,mask=a2)
+    return im3
+
+# async def get_head_steam_and_save(user_id:str,urls):
+#     """保存steam头像"""
+#     USER_HEAD_PATH = PLAYERSDATA / str(user_id) / 'HEAD.png'
+#     # DEFAULT_HEAD_PATH = TEXT_PATH / "template/player.jpg"
+#     ## im头像 im2头像框 im3合成
+#     if os.path.exists(USER_HEAD_PATH):
+#         logger.info("使用本地头像")
+#         im = Image.open(USER_HEAD_PATH).resize((280, 280)).convert("RGBA")
+#     else:
+#         # if user_id == "1145149191810":
+#         #     logger.info("使用默认头像")
+#         #     im = Image.open(DEFAULT_HEAD_PATH).resize((300, 300)).convert("RGBA")
+#         # else:
+#             try:
+#                 logger.info("正在下载头像")
+#                 image_bytes = await web_player(urls)
+#                 im = Image.open(io.BytesIO(image_bytes)).resize((280, 280)).convert("RGBA")
+#                 if not os.path.exists(PLAYERSDATA / user_id):#用户文件夹不存在
+#                     os.makedirs(PLAYERSDATA / user_id)
+#                 im.save(USER_HEAD_PATH, "PNG")
+#             except TimeoutError:
+#                 logger.error("获取失败")
+#     return im
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from io import BytesIO
-from pathlib import Path
-from typing import Union
-from base64 import b64encode
-
-from PIL import Image
-
-
-async def convert_img(
-    img: Union[Image.Image, str, Path, bytes], is_base64: bool = False
-):
-    """
-    :说明:
-      将PIL.Image对象转换为bytes或者base64格式。
-    :参数:
-      * img (Image): 图片。
-      * is_base64 (bool): 是否转换为base64格式, 不填默认转为bytes。
-    :返回:
-      * res: bytes对象或base64编码图片。
-    """
-    if isinstance(img, Image.Image):
-        img = img.convert('RGBA')
-        result_buffer = BytesIO()
-        img.save(result_buffer, format='PNG', quality=80, subsampling=0)
-        res = result_buffer.getvalue()
-        if is_base64:
-            res = b64encode(res).decode()
-        return res
-    elif isinstance(img, bytes):
-        return b64encode(img).decode()
-    else:
-        return f'[CQ:image,file=file:///{str(img)}]'
+from io import BytesIO
+from pathlib import Path
+from typing import Union
+from base64 import b64encode
+
+from PIL import Image
+
+
+async def convert_img(
+    img: Union[Image.Image, str, Path, bytes], is_base64: bool = False
+):
+    """
+    :说明:
+      将PIL.Image对象转换为bytes或者base64格式。
+    :参数:
+      * img (Image): 图片。
+      * is_base64 (bool): 是否转换为base64格式, 不填默认转为bytes。
+    :返回:
+      * res: bytes对象或base64编码图片。
+    """
+    if isinstance(img, Image.Image):
+        img = img.convert('RGBA')
+        result_buffer = BytesIO()
+        img.save(result_buffer, format='PNG', quality=80, subsampling=0)
+        res = result_buffer.getvalue()
+        if is_base64:
+            res = b64encode(res).decode()
+        return res
+    elif isinstance(img, bytes):
+        return b64encode(img).decode()
+    else:
+        return f'[CQ:image,file=file:///{str(img)}]'
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-
-from PIL import Image
-from nonebot.log import logger
-from io import BytesIO
-# import sys
-# sys.modules["srctools._cy_vtf_readwrite"] = None
-from srctools.vtf import VTF, ImageFormats
-
-async def img_to_vtf(pic_byte:bytes,tag) -> BytesIO:
-    pic = BytesIO(pic_byte)
-    pic = Image.open(pic).convert('RGBA')
-    vtf_io = BytesIO()
-    vtf_ = VTF(1024, 1024, fmt = ImageFormats.DXT5,thumb_fmt = ImageFormats.DXT1,version=(7,2))
-    if tag == '覆盖':
-        logger.info(tag)
-        img2 = Image.new('RGBA',(1024, 1024), (255, 255, 255,0))
-        r, g, b, a = pic.split()
-        img2.paste(pic,mask=a)
-        pic = pic.resize((1024,1024))
-    elif tag == '填充':
-        w, h = pic.size
-        if w > h:
-            ratio = 1024/w
-            new_width = 1024
-            new_height = int(h * ratio)
-        else:
-            ratio = 1024/h
-            new_height = 1024
-            new_width = int(w * ratio)
-        pic = pic.resize((new_width, new_height), Image.ANTIALIAS)
-        background = Image.new('RGBA', (1024, 1024), (255, 255, 255, 0))
-        background.paste(pic, ((1024-new_width)//2, (1024-new_height)//2))
-        pic = background
-    else:
-        logger.info('拉伸')
-        pic = pic.resize((1024,1024))
-    largest_frame = vtf_.get() 
-    largest_frame.copy_from(pic.tobytes(), ImageFormats.RGBA8888)
-    vtf_.save(vtf_io,version=(7,2))
-    return vtf_io
+
+from PIL import Image
+from nonebot.log import logger
+from io import BytesIO
+# import sys
+# sys.modules["srctools._cy_vtf_readwrite"] = None
+from srctools.vtf import VTF, ImageFormats
+
+async def img_to_vtf(pic_byte:bytes,tag) -> BytesIO:
+    pic = BytesIO(pic_byte)
+    pic = Image.open(pic).convert('RGBA')
+    vtf_io = BytesIO()
+    vtf_ = VTF(1024, 1024, fmt = ImageFormats.DXT5,thumb_fmt = ImageFormats.DXT1,version=(7,2))
+    if tag == '覆盖':
+        logger.info(tag)
+        img2 = Image.new('RGBA',(1024, 1024), (255, 255, 255,0))
+        r, g, b, a = pic.split()
+        img2.paste(pic,mask=a)
+        pic = pic.resize((1024,1024))
+    elif tag == '填充':
+        w, h = pic.size
+        if w > h:
+            ratio = 1024/w
+            new_width = 1024
+            new_height = int(h * ratio)
+        else:
+            ratio = 1024/h
+            new_height = 1024
+            new_width = int(w * ratio)
+        pic = pic.resize((new_width, new_height), Image.ANTIALIAS)
+        background = Image.new('RGBA', (1024, 1024), (255, 255, 255, 0))
+        background.paste(pic, ((1024-new_width)//2, (1024-new_height)//2))
+        pic = background
+    else:
+        logger.info('拉伸')
+        pic = pic.resize((1024,1024))
+    largest_frame = vtf_.get() 
+    largest_frame.copy_from(pic.tobytes(), ImageFormats.RGBA8888)
+    vtf_.save(vtf_io,version=(7,2))
+    return vtf_io
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import a2s
-from typing import List
-
-async def queries(ip:str,port:int):
-    port = int(port)
-    msg_dict = await queries_dict(ip,port)
-    message = 'ip:' + msg_dict['ip'] + '\n'
-    message += '名称：' + msg_dict['name'] + '\n'
-    message += f"地图：{msg_dict['map_']}\n"
-    message += f"延迟：{msg_dict['ping']}\n"
-    message += f"玩家：{msg_dict['players']} / {msg_dict['max_players']}\n"
-    return message
-
-async def queries_dict(ip:str,port:int) -> dict:
-    port = int(port)
-    ip = str(ip)
-    msg_dict = {}
-    # message_dict = await l4d(ip,port)
-    msg:a2s.SourceInfo = await a2s.ainfo((ip,port))
-    # message_dict = await l4d2.server(ip,port,times=5)
-    msg_dict['folder'] =  msg.folder
-    msg_dict['name'] =  msg.server_name
-    msg_dict['map_'] =  msg.map_name
-    msg_dict['players'] =  msg.player_count
-    msg_dict['max_players'] =  msg.max_players
-    msg_dict['rank_players'] =  f'{msg.player_count}/{msg.max_players}'
-    msg_dict['ip'] = str(ip) + ':' +str(port)
-    msg_dict['ping'] = f"{msg.ping*1000:.0f}ms"
-    msg_dict['system'] =  f"{msg.platform}.svg"
-    if msg_dict['players'] < msg_dict['max_players']:
-        msg_dict['enabled'] = True
-    else:
-        msg_dict['enabled'] = False
-    return msg_dict
-    
-async def player_queries_anne_dict(ip:str,port:int): 
-    """anne算法返回玩家"""
-    port = int(port)
-    # message_dic = await l4d2.APlayer(ip,port,times=5)
-    message_list:List[a2s.Player] = await a2s.aplayers((ip,port))
-    msg_list = []
-    if message_list != []:
-        for i in message_list:
-            msg_list.append({
-                'name':i.name,
-                'Score':i.score,
-                'Duration':await convert_duration(i.duration)
-            })
-    return msg_list
-
-# async def player_queries_dict(ip:str,port:int): 
-#     """一般算法返回玩家"""
-#     port = int(port)
-#     new_dict = {}
-#     message_dic = await l4d2.APlayer(ip,port,times=5)
-#     if message_dic == {}:
-#         new_dict['header'] = 0
-#     else:
-#         pass
-#         new_list = []
-#         for i in message_dic['Players']:
-#             new_list.append(i['Name'])
-#         new_dict.update({'Players':new_list})
-#     return new_dict
-
-async def player_queries(ip:str,port:int): 
-    port = int(port)
-    message_list = await player_queries_anne_dict(ip,port)
-    return await msg_ip_to_list(message_list)
-
-async def msg_ip_to_list(message_list:list):
-    message = ''
-    n = 0
-    if message_list == []:
-        message += '服务器里，是空空的呢\n'
-    else:
-        max_duration_len = max([len(str(i['Duration'])) for i in message_list])
-        max_score_len = max([len(str(i['Score'])) for i in message_list])
-        for i in message_list:
-            print(i)
-            n += 1 
-            name = i['name']
-            Score = i['Score']
-            if Score == '0':
-                Score = '摸'
-            Duration = i['Duration']
-            soc = "[{:>{}}]".format(Score,max_score_len)
-            dur = "{:^{}}".format(Duration, max_duration_len)
-            message += f'{soc} | {dur} | {name} \n'
-    return message
-
-async def convert_duration(duration: int) -> str:
-    minutes, seconds = divmod(duration, 60)
-    hours, minutes = divmod(minutes, 60)
-    time_str = ""
-    if hours > 0:
-        time_str += f"{int(hours)}h "
-    if minutes > 0 or hours > 0:
-        time_str += f"{int(minutes)}m "
-    time_str += f"{int(seconds)}s"
-    return time_str.strip()
-
-async def server_rule_dict(ip:str,port:int): 
-    port = int(port)
-    ip = str(ip)
-    msg_dict = {}
-    # message_dict = await l4d(ip,port)
-    try:
-        msg:dict = await a2s.arules((ip,port))
-        msg_dict['tick'] = msg['l4d2_tickrate_enabler'] + "tick"
-    except:
-        msg_dict['tick'] = ''
-    return msg_dict
-
+import a2s
+from typing import List
+
+async def queries(ip:str,port:int):
+    port = int(port)
+    msg_dict = await queries_dict(ip,port)
+    message = 'ip:' + msg_dict['ip'] + '\n'
+    message += '名称：' + msg_dict['name'] + '\n'
+    message += f"地图：{msg_dict['map_']}\n"
+    message += f"延迟：{msg_dict['ping']}\n"
+    message += f"玩家：{msg_dict['players']} / {msg_dict['max_players']}\n"
+    return message
+
+async def queries_dict(ip:str,port:int) -> dict:
+    port = int(port)
+    ip = str(ip)
+    msg_dict = {}
+    # message_dict = await l4d(ip,port)
+    msg:a2s.SourceInfo = await a2s.ainfo((ip,port))
+    # message_dict = await l4d2.server(ip,port,times=5)
+    msg_dict['folder'] =  msg.folder
+    msg_dict['name'] =  msg.server_name
+    msg_dict['map_'] =  msg.map_name
+    msg_dict['players'] =  msg.player_count
+    msg_dict['max_players'] =  msg.max_players
+    msg_dict['rank_players'] =  f'{msg.player_count}/{msg.max_players}'
+    msg_dict['ip'] = str(ip) + ':' +str(port)
+    msg_dict['ping'] = f"{msg.ping*1000:.0f}ms"
+    msg_dict['system'] =  f"{msg.platform}.svg"
+    if msg_dict['players'] < msg_dict['max_players']:
+        msg_dict['enabled'] = True
+    else:
+        msg_dict['enabled'] = False
+    return msg_dict
+    
+async def player_queries_anne_dict(ip:str,port:int): 
+    """anne算法返回玩家"""
+    port = int(port)
+    # message_dic = await l4d2.APlayer(ip,port,times=5)
+    message_list:List[a2s.Player] = await a2s.aplayers((ip,port))
+    msg_list = []
+    if message_list != []:
+        for i in message_list:
+            msg_list.append({
+                'name':i.name,
+                'Score':i.score,
+                'Duration':await convert_duration(i.duration)
+            })
+    return msg_list
+
+# async def player_queries_dict(ip:str,port:int): 
+#     """一般算法返回玩家"""
+#     port = int(port)
+#     new_dict = {}
+#     message_dic = await l4d2.APlayer(ip,port,times=5)
+#     if message_dic == {}:
+#         new_dict['header'] = 0
+#     else:
+#         pass
+#         new_list = []
+#         for i in message_dic['Players']:
+#             new_list.append(i['Name'])
+#         new_dict.update({'Players':new_list})
+#     return new_dict
+
+async def player_queries(ip:str,port:int): 
+    port = int(port)
+    message_list = await player_queries_anne_dict(ip,port)
+    return await msg_ip_to_list(message_list)
+
+async def msg_ip_to_list(message_list:list):
+    message = ''
+    n = 0
+    if message_list == []:
+        message += '服务器里，是空空的呢\n'
+    else:
+        max_duration_len = max([len(str(i['Duration'])) for i in message_list])
+        max_score_len = max([len(str(i['Score'])) for i in message_list])
+        for i in message_list:
+            print(i)
+            n += 1 
+            name = i['name']
+            Score = i['Score']
+            if Score == '0':
+                Score = '摸'
+            Duration = i['Duration']
+            soc = "[{:>{}}]".format(Score,max_score_len)
+            dur = "{:^{}}".format(Duration, max_duration_len)
+            message += f'{soc} | {dur} | {name} \n'
+    return message
+
+async def convert_duration(duration: int) -> str:
+    minutes, seconds = divmod(duration, 60)
+    hours, minutes = divmod(minutes, 60)
+    time_str = ""
+    if hours > 0:
+        time_str += f"{int(hours)}h "
+    if minutes > 0 or hours > 0:
+        time_str += f"{int(minutes)}m "
+    time_str += f"{int(seconds)}s"
+    return time_str.strip()
+
+async def server_rule_dict(ip:str,port:int): 
+    port = int(port)
+    ip = str(ip)
+    msg_dict = {}
+    # message_dict = await l4d(ip,port)
+    try:
+        msg:dict = await a2s.arules((ip,port))
+        msg_dict['tick'] = msg['l4d2_tickrate_enabler'] + "tick"
+    except:
+        msg_dict['tick'] = ''
+    return msg_dict
+
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-try:
-        import ujson as json
-except:
-        import json
-from pathlib import Path
-from typing import Dict,List
-import os
-
-BOT_DIR = os.path.dirname(os.path.abspath(__file__))
-filename = 'data/L4D2/l4d2.json'
-global_file = Path(Path(__file__).parent.parent,filename)
-def load_josn():
-        # 本地模块
-        try:
-                LOCAL_HOST:dict = json.load(open(
-                filename, "r", encoding="utf8"))
-        except IOError or FileNotFoundError:
-                os.makedirs(os.path.dirname(filename), exist_ok=True)
-                data = {}
-                with open(filename, "w") as f:
-                        json.dump(data, f)
-                LOCAL_HOST:dict = {}
-        try:
-                # 获取所有json文件的路径
-                json_files = Path('data/L4D2/l4d2').glob('*.json')
-
-                # 将所有json文件中的字典对象合并为一个字典
-                for file_path in json_files:
-                        with open(file_path, 'r', encoding='utf-8') as f:
-                                LOCAL_HOST.update(json.load(f))
-        except:
-                pass
-        return LOCAL_HOST
-
-ALL_HOST:Dict[str, List[dict]] = load_josn()
+try:
+        import ujson as json
+except:
+        import json
+from pathlib import Path
+from typing import Dict,List
+import os
+
+BOT_DIR = os.path.dirname(os.path.abspath(__file__))
+filename = 'data/L4D2/l4d2.json'
+global_file = Path(Path(__file__).parent.parent,filename)
+def load_josn():
+        # 本地模块
+        try:
+                LOCAL_HOST:dict = json.load(open(
+                filename, "r", encoding="utf8"))
+        except IOError or FileNotFoundError:
+                os.makedirs(os.path.dirname(filename), exist_ok=True)
+                data = {}
+                with open(filename, "w") as f:
+                        json.dump(data, f)
+                LOCAL_HOST:dict = {}
+        try:
+                # 获取所有json文件的路径
+                json_files = Path('data/L4D2/l4d2').glob('*.json')
+
+                # 将所有json文件中的字典对象合并为一个字典
+                for file_path in json_files:
+                        with open(file_path, 'r', encoding='utf-8') as f:
+                                LOCAL_HOST.update(json.load(f))
+        except:
+                pass
+        return LOCAL_HOST
+
+ALL_HOST:Dict[str, List[dict]] = load_josn()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import asyncio
-from rcon.source.proto import Packet,Type
-from rcon.source.async_rcon import communicate,close
-
-async def main(host):
-    host = '43.142.178.212'
-    port = 40003
-    password = '1145149191810'
-    encoding = 'utf-8'
-
-    # Connect to RCON server
-
-
-    # Main loop
-    while True:
-        # Read user input
-        command = input('> ')
-        if not command:
-            break
-
-   # 连接服务器
-    reader, writer = await asyncio.open_connection(host, port)
-    login = Packet.make_login(password, encoding=encoding)
-    response = await communicate(reader, writer, login)
-
-    # 等待 SERVERDATA_AUTH_RESPONSE 数据包
-    while response.type != Type.SERVERDATA_AUTH_RESPONSE:
-        response = await Packet.aread(reader)
-
-    if response.id == -1:
-        await close(writer)
-        raise WrongPassword()
-
-    # 循环接收用户输入并发送指令
-    while True:
-        try:
-            command = input('请输入指令：')
-            
-        except EOFError:
-            break
-        
-        if command=='停止':
-            break
-        # 发送指令
-        
-        command = f'say {command}'
-        request = Packet.make_command(command, encoding=encoding)
-        response = await communicate(reader, writer, request)
-
-        # if response.id != request.id:
-        #     raise SessionTimeout()
-
-        print(response.payload.decode(encoding, errors='ignore'))
-
-    # 断开连接
-    await close(writer)
-    
-class WrongPassword(Exception):
-    """Indicates a wrong password."""
-    
-class SessionTimeout(Exception):
+import asyncio
+from rcon.source.proto import Packet,Type
+from rcon.source.async_rcon import communicate,close
+
+async def main(host):
+    host = '43.142.178.212'
+    port = 40003
+    password = '1145149191810'
+    encoding = 'utf-8'
+
+    # Connect to RCON server
+
+
+    # Main loop
+    while True:
+        # Read user input
+        command = input('> ')
+        if not command:
+            break
+
+   # 连接服务器
+    reader, writer = await asyncio.open_connection(host, port)
+    login = Packet.make_login(password, encoding=encoding)
+    response = await communicate(reader, writer, login)
+
+    # 等待 SERVERDATA_AUTH_RESPONSE 数据包
+    while response.type != Type.SERVERDATA_AUTH_RESPONSE:
+        response = await Packet.aread(reader)
+
+    if response.id == -1:
+        await close(writer)
+        raise WrongPassword()
+
+    # 循环接收用户输入并发送指令
+    while True:
+        try:
+            command = input('请输入指令：')
+            
+        except EOFError:
+            break
+        
+        if command=='停止':
+            break
+        # 发送指令
+        
+        command = f'say {command}'
+        request = Packet.make_command(command, encoding=encoding)
+        response = await communicate(reader, writer, request)
+
+        # if response.id != request.id:
+        #     raise SessionTimeout()
+
+        print(response.payload.decode(encoding, errors='ignore'))
+
+    # 断开连接
+    await close(writer)
+    
+class WrongPassword(Exception):
+    """Indicates a wrong password."""
+    
+class SessionTimeout(Exception):
     """Indicates that the session timed out."""
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from rcon.source import rcon
-import asyncio
-from pathlib import Path
-from ..config import l4_config,CHECK_FILE
-# from ..config import l4_rcon,l4_host,l4_port,l4_rcon
-
-
-async def rcon_server(PASSWORD:str,msg:str):
-    # response = await rcon(command=msg, host=l4_host, port=l4_port, passwd=PASSWORD,encoding='utf-8')
-    # return response
-    try:
-        response = await asyncio.wait_for(rcon(command=msg, host=l4_config.l4_ipall[CHECK_FILE]['host'], port = l4_config.l4_ipall[CHECK_FILE]['port'], passwd=PASSWORD), timeout=30)
-        return response
-    except asyncio.TimeoutError:
-        return '超时'
-
-async def read_server_cfg_rcon():
-    """如果没有输入rcon，尝试自动获取"""
-    if not l4_config.l4_ipall[CHECK_FILE]['rcon']:
-        cfg_server = Path(l4_config.l4_ipall[CHECK_FILE]['location'],'left4dead2/cfg/server.cfg')
-        with open(cfg_server,'r')as cfg:
-            content:str = cfg.read()
-            lines = content.split('\n')
-            for line in lines:
-                if line.startswith('rcon_password'):
-                    password = line.split(' ')[-1]
-                    password = password.strip('"')
-                    return password
+from rcon.source import rcon
+import asyncio
+from pathlib import Path
+from ..config import l4_config,CHECK_FILE
+# from ..config import l4_rcon,l4_host,l4_port,l4_rcon
+
+
+async def rcon_server(PASSWORD:str,msg:str):
+    # response = await rcon(command=msg, host=l4_host, port=l4_port, passwd=PASSWORD,encoding='utf-8')
+    # return response
+    try:
+        response = await asyncio.wait_for(rcon(command=msg, host=l4_config.l4_ipall[CHECK_FILE]['host'], port = l4_config.l4_ipall[CHECK_FILE]['port'], passwd=PASSWORD), timeout=30)
+        return response
+    except asyncio.TimeoutError:
+        return '超时'
+
+async def read_server_cfg_rcon():
+    """如果没有输入rcon，尝试自动获取"""
+    if not l4_config.l4_ipall[CHECK_FILE]['rcon']:
+        cfg_server = Path(l4_config.l4_ipall[CHECK_FILE]['location'],'left4dead2/cfg/server.cfg')
+        with open(cfg_server,'r')as cfg:
+            content:str = cfg.read()
+            lines = content.split('\n')
+            for line in lines:
+                if line.startswith('rcon_password'):
+                    password = line.split(' ')[-1]
+                    password = password.strip('"')
+                    return password
     return l4_config.l4_ipall[CHECK_FILE]['rcon']
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,252 +1,234 @@
-import datetime
-from typing import Optional, Union
-
-from fastapi import FastAPI
-from fastapi import Header, HTTPException, Depends
-from fastapi.responses import JSONResponse, HTMLResponse, RedirectResponse
-from jose import jwt
-from nonebot import get_bot, get_app
-
-from pathlib import Path
-
-from nonebot import get_driver, logger
-from ..config import *
-from ..utils import split_maohao
-from ..l4d2_queries.qqgroup import qq_ip_querie
-CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
-
-CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
-
-driver = get_driver()
-
-from .webUI import login_page, admin_app
-
-requestAdaptor = '''
-requestAdaptor(api) {
-    api.headers["token"] = localStorage.getItem("token");
-    return api;
-},
-'''
-responseAdaptor = '''
-responseAdaptor(api, payload, query, request, response) {
-    if (response.data.detail == '登录验证失败或已失效，请重新登录') {
-        window.location.href = '/l4d2/login'
-        window.localStorage.clear()
-        window.sessionStorage.clear()
-        window.alert('登录验证失败或已失效，请重新登录')
-    }
-    return payload
-},
-'''
-
-
-def authentication():
-    def inner(token: Optional[str] = Header(...)):
-        try:
-            payload = jwt.decode(token, config_manager.config.web_secret_key, algorithms='HS256')
-            if not (username := payload.get('username')) or username != config_manager.config.web_username:
-                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-
-    return Depends(inner)
-
-
-COMMAND_START = driver.config.command_start.copy()
-if '' in COMMAND_START:
-    COMMAND_START.remove('')
-
-
-
-
-
-@driver.on_startup
-async def init_web():
-    if not config_manager.config.total_enable:
-        return
-    app: FastAPI = get_app()
-    logger.success('成功加载网页控制台')
-    @app.post('/l4d2/api/login', response_class=JSONResponse)
-    async def login(user: UserModel):
-        if user.username != config_manager.config.web_username or user.password != config_manager.config.web_password:
-            return {
-                'status': -100,
-                'msg':    '登录失败，请确认用户ID和密码无误'
-            }
-        token = jwt.encode({'username': user.username,
-                            'exp':      datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
-                                minutes=30)}, config_manager.config.web_secret_key, algorithm='HS256')
-        return {
-            'status': 0,
-            'msg':    '登录成功',
-            'data':   {
-                'token': token
-            }
-        }
-
-    @app.get('/l4d2/api/get_group_list', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_group_list_api():
-        try:
-            group_list = await get_bot().get_group_list()
-            group_list = [{'label': f'{group["group_name"]}({group["group_id"]})', 'value': group['group_id']} for group
-                          in group_list]
-            return {
-                'status': 0,
-                'msg':    'ok',
-                'data':   {
-                    'group_list': group_list
-                }
-            }
-        except ValueError:
-            return {
-                'status': -100,
-                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
-            }
-
-    @app.post('/l4d2/api/l4d2_global_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def post_l4d2_global_config(data: dict):
-        config_manager.config.update(**data)
-        config_manager.save()
-        return {
-            'status': 0,
-            'msg':    '保存成功'
-        }
-
-    @app.get('/l4d2/api/l4d2_global_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_l4d2_global_config():
-        try:
-            bot = get_bot()
-            groups = await bot.get_group_list()
-            member_list = []
-            for group in groups:
-                members = await bot.get_group_member_list(group_id=group['group_id'])
-                member_list.extend(
-                    [{'label': f'{member["nickname"] or member["card"]}({member["user_id"]})',
-                      'value': member['user_id']}
-                     for
-                     member in members])
-            config = config_manager.config.dict(exclude={'group_config'})
-            config['member_list'] = member_list
-            config['l4_styles'] = ['standard','black']
-
-            return config
-        except ValueError:
-            return {
-                'status': -100,
-                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
-            }
-            
-    @app.get('/l4d2/api/get_query_contexts', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_query_context():
-        try:
-            from ..command import ALL_HOST
-            this_ips = ALL_HOST
-            ip_lists = []
-            for ip_list, v in this_ips.items():
-                for d in v:
-                    host, port = split_maohao(d['ip'])
-                    ip_lists.append((d['id'], ip_list, host, port))
-            data_dict = await qq_ip_querie(ip_lists)
-            if not data_dict:
-                return{
-                'status': -100,
-                'msg':    '返回失败，请确保有可用的服务器ip' 
-                }
-            data_list = data_dict['msg_list']
-            return {
-                'status': 0,
-                'msg': 'ok',
-                'data': {
-                    'items': data_list,
-                    'total': len(data_list),
-                }
-            }
-        except ValueError:
-            return {
-                'status': -100,
-                'msg':    '返回失败，请确保网络连接正常'
-            }
-
-    @app.get('/l4d2/api/get_l4d2_messages', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_l4d2_messages():
-        try:
-            l4_ipall = config_manager.config.l4_ipall
-<<<<<<< Updated upstream
-            server_list = []
-            config = config_manager.config.dict(exclude={'group_config'})
-            server_list.extend(
-                [{'label': f'{item["server_id"] or item["id_rank"]}({item["host"]})',
-                    'value': item['id_rank']}
-                    for item in l4_ipall])
-            config['server_list'] = server_list
-            return config
-=======
-            config = [{'label': item['server_id'] , 'value': item['id_rank']}
-                for item in l4_ipall]
-            return {
-                'status': 0,
-                'msg': 'ok',
-                'data': {'server_list':config}
-            }
->>>>>>> Stashed changes
-        except ValueError:
-            return {
-                'status': -100,
-                'msg':    '返回失败，请确保网络连接正常'
-            }
-    @app.get('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_l4d2_server_config(id_rank :str):
-        try:
-            l4_ipall = config_manager.config.l4_ipall
-            config = {}
-            for item in l4_ipall:
-                if item['id_rank'] == id_rank :
-<<<<<<< Updated upstream
-=======
-                    item['place'] = item['place'] == 'True' or item['place'] == True
->>>>>>> Stashed changes
-                    config = item
-                    break
-            return {
-                'status': 0,
-                'msg': 'ok',
-                'data': config
-            }
-        except ValueError:
-            return {
-                'status': -100,
-                'msg':    '返回失败，请确保网络连接正常'
-            }
-        
-    @app.post('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def post_l4d2_server_config(id_rank :str,data: dict):
-<<<<<<< Updated upstream
-        print(data)
-=======
->>>>>>> Stashed changes
-        for one in config_manager.config.l4_ipall:
-            if one['id_rank']==id_rank:
-                one.update(**data)
-        config_manager.save()
-        return {
-            'status': 0,
-            'msg':    '保存成功'
-        }        
-
-        
-    @app.get('/l4d2', response_class=RedirectResponse)
-    async def redirect_page():
-        return RedirectResponse('/l4d2/login')
-
-    @app.get('/l4d2/login', response_class=HTMLResponse)
-    async def login_page_app():
-        return login_page.render(site_title='登录 | l4d2 后台管理',
-                                 theme='ang')
-
-    @app.get('/l4d2/admin', response_class=HTMLResponse)
-    async def admin_page_app():
-        return admin_app.render(site_title='l4d2-l4d2 后台管理',
-                                theme='ang',
-                                requestAdaptor=requestAdaptor,
-                                responseAdaptor=responseAdaptor)
-
+import datetime
+from typing import Optional, Union
+
+from fastapi import FastAPI
+from fastapi import Header, HTTPException, Depends
+from fastapi.responses import JSONResponse, HTMLResponse, RedirectResponse
+from jose import jwt
+from nonebot import get_bot, get_app
+
+from pathlib import Path
+
+from nonebot import get_driver, logger
+from ..config import *
+from ..utils import split_maohao
+from ..l4d2_queries.qqgroup import qq_ip_querie
+CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
+
+CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
+
+driver = get_driver()
+
+from .webUI import login_page, admin_app
+
+requestAdaptor = '''
+requestAdaptor(api) {
+    api.headers["token"] = localStorage.getItem("token");
+    return api;
+},
+'''
+responseAdaptor = '''
+responseAdaptor(api, payload, query, request, response) {
+    if (response.data.detail == '登录验证失败或已失效，请重新登录') {
+        window.location.href = '/l4d2/login'
+        window.localStorage.clear()
+        window.sessionStorage.clear()
+        window.alert('登录验证失败或已失效，请重新登录')
+    }
+    return payload
+},
+'''
+
+
+def authentication():
+    def inner(token: Optional[str] = Header(...)):
+        try:
+            payload = jwt.decode(token, config_manager.config.web_secret_key, algorithms='HS256')
+            if not (username := payload.get('username')) or username != config_manager.config.web_username:
+                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
+            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+
+    return Depends(inner)
+
+
+COMMAND_START = driver.config.command_start.copy()
+if '' in COMMAND_START:
+    COMMAND_START.remove('')
+
+
+
+
+
+@driver.on_startup
+async def init_web():
+    if not config_manager.config.total_enable:
+        return
+    app: FastAPI = get_app()
+    logger.success('成功加载网页控制台')
+    @app.post('/l4d2/api/login', response_class=JSONResponse)
+    async def login(user: UserModel):
+        if user.username != config_manager.config.web_username or user.password != config_manager.config.web_password:
+            return {
+                'status': -100,
+                'msg':    '登录失败，请确认用户ID和密码无误'
+            }
+        token = jwt.encode({'username': user.username,
+                            'exp':      datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+                                minutes=30)}, config_manager.config.web_secret_key, algorithm='HS256')
+        return {
+            'status': 0,
+            'msg':    '登录成功',
+            'data':   {
+                'token': token
+            }
+        }
+
+    @app.get('/l4d2/api/get_group_list', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_group_list_api():
+        try:
+            group_list = await get_bot().get_group_list()
+            group_list = [{'label': f'{group["group_name"]}({group["group_id"]})', 'value': group['group_id']} for group
+                          in group_list]
+            return {
+                'status': 0,
+                'msg':    'ok',
+                'data':   {
+                    'group_list': group_list
+                }
+            }
+        except ValueError:
+            return {
+                'status': -100,
+                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
+            }
+
+    @app.post('/l4d2/api/l4d2_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def post_l4d2_global_config(data: dict):
+        config_manager.config.update(**data)
+        config_manager.save()
+        return {
+            'status': 0,
+            'msg':    '保存成功'
+        }
+
+    @app.get('/l4d2/api/l4d2_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_l4d2_global_config():
+        try:
+            bot = get_bot()
+            groups = await bot.get_group_list()
+            member_list = []
+            for group in groups:
+                members = await bot.get_group_member_list(group_id=group['group_id'])
+                member_list.extend(
+                    [{'label': f'{member["nickname"] or member["card"]}({member["user_id"]})',
+                      'value': member['user_id']}
+                     for
+                     member in members])
+            config = config_manager.config.dict(exclude={'group_config'})
+            config['member_list'] = member_list
+            config['l4_styles'] = ['standard','black']
+
+            return config
+        except ValueError:
+            return {
+                'status': -100,
+                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
+            }
+            
+    @app.get('/l4d2/api/get_query_contexts', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_query_context():
+        try:
+            from ..command import ALL_HOST
+            this_ips = ALL_HOST
+            ip_lists = []
+            for ip_list, v in this_ips.items():
+                for d in v:
+                    host, port = split_maohao(d['ip'])
+                    ip_lists.append((d['id'], ip_list, host, port))
+            data_dict = await qq_ip_querie(ip_lists)
+            if not data_dict:
+                return{
+                'status': -100,
+                'msg':    '返回失败，请确保有可用的服务器ip' 
+                }
+            data_list = data_dict['msg_list']
+            return {
+                'status': 0,
+                'msg': 'ok',
+                'data': {
+                    'items': data_list,
+                    'total': len(data_list),
+                }
+            }
+        except ValueError:
+            return {
+                'status': -100,
+                'msg':    '返回失败，请确保网络连接正常'
+            }
+
+    @app.get('/l4d2/api/get_l4d2_messages', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_l4d2_messages():
+        try:
+            l4_ipall = config_manager.config.l4_ipall
+            config = [{'label': item['server_id'] , 'value': item['id_rank']}
+                for item in l4_ipall]
+            return {
+                'status': 0,
+                'msg': 'ok',
+                'data': {'server_list':config}
+            }
+        except ValueError:
+            return {
+                'status': -100,
+                'msg':    '返回失败，请确保网络连接正常'
+            }
+    @app.get('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_l4d2_server_config(id_rank :str):
+        try:
+            l4_ipall = config_manager.config.l4_ipall
+            config = {}
+            for item in l4_ipall:
+                if item['id_rank'] == id_rank :
+                    item['place'] = item['place'] == 'True' or item['place'] == True
+                    config = item
+                    break
+            return {
+                'status': 0,
+                'msg': 'ok',
+                'data': config
+            }
+        except ValueError:
+            return {
+                'status': -100,
+                'msg':    '返回失败，请确保网络连接正常'
+            }
+        
+    @app.post('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def post_l4d2_server_config(id_rank :str,data: dict):
+        for one in config_manager.config.l4_ipall:
+            if one['id_rank']==id_rank:
+                one.update(**data)
+        config_manager.save()
+        return {
+            'status': 0,
+            'msg':    '保存成功'
+        }        
+
+        
+    @app.get('/l4d2', response_class=RedirectResponse)
+    async def redirect_page():
+        return RedirectResponse('/l4d2/login')
+
+    @app.get('/l4d2/login', response_class=HTMLResponse)
+    async def login_page_app():
+        return login_page.render(site_title='登录 | l4d2 后台管理',
+                                 theme='ang')
+
+    @app.get('/l4d2/admin', response_class=HTMLResponse)
+    async def admin_page_app():
+        return admin_app.render(site_title='l4d2-l4d2 后台管理',
+                                theme='ang',
+                                requestAdaptor=requestAdaptor,
+                                responseAdaptor=responseAdaptor)
+
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,245 +1,241 @@
-from amis import  ActionType, TableCRUD, TableColumn
-from amis import  PageSchema, Switch, InputNumber, InputTag, Action, App
-from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper
-from amis import LevelEnum, Select,  Alert, Tpl, Flex
-
-
-from ..config import NICKNAME
-
-logo = Html(html='''
-<p align="center">
-    <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server">
-        <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png"
-         width="256" height="256" alt="l4d2-server">
-    </a>
-</p>
-<h1 align="center">Nonebot-Plugin-L4d2-Server 控制台</h1>
-<div align="center">
-    <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/" target="_blank">
-    Github仓库</a>
-</div>
-<br>
-<br>
-''')
-login_api = AmisAPI(
-    url='/l4d2/api/login',
-    method='post',
-    adaptor='''
-        if (payload.status == 0) {
-            localStorage.setItem("token", payload.data.token);
-        }
-        return payload;
-    '''
-)
-
-login_form = Form(api=login_api, title='', body=[
-    InputText(name='username', label='用户名',
-              labelRemark=Remark(shape='circle', content='后台管理用户名，默认为l4d2')),
-    InputPassword(name='password', label='密码',
-                  labelRemark=Remark(shape='circle', content='后台管理密码，默认为admin')),
-], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5), redirect='/l4d2/admin')
-body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form)
-login_page = Page(title='', body=[logo, body])
-
-global_config_form = Form(
-    title='全局配置',
-    name='global_config',
-    initApi='/l4d2/api/l4d2_global_config',
-    api='post:/l4d2/api/l4d2_global_config',
-    body=[
-        Switch(label='控制总开关（摆设）', name='total_enable', value='${total_enable}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle',
-                                  content='关闭后，禁用网页控制台，请参考文档启动方法')),
-        InputText(label='后台管理用户名', name='web_username', value='${web_username}',
-                  labelRemark=Remark(shape='circle',
-                                     content='登录本后台管理所需要的用户名。')),
-        InputPassword(label='后台管理密码', name='web_password', value='${web_password}',
-                      labelRemark=Remark(shape='circle',
-                                         content='登录本后台管理所需要的密码。')),
-        InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于本后台管理加密验证token的密钥。')),
-        InputText(label='查询key', name='l4_key', value='${l4_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于获取拓展功能的key,加q群399365126领取。')),
-        InputText(label='字体', name='l4_font', value='${l4_font}',
-                  labelRemark=Remark(shape='circle',
-                                     content='机器人返回图片中文字的字体。')),
-        Select(label='图片风格', name='l4_style', value='${l4_style}',source='${l4_styles}',
-                  labelRemark=Remark(shape='circle',
-                                     content='仅仅是批量查询的风格')),
-        InputTag(label='查询的远程服务器tag', name='l4_tag', value='${l4_tag}',
-                 enableBatchAdd=True,
-                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle',
-                                    content='在这里加入的用户，才能上传地图')),
-        InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
-                 enableBatchAdd=True,
-                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle',
-                                    content='在这里加入的用户，才能上传地图')),
-
-    ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
-)
-
-upload_map_form = Form(
-    title='全局配置',
-    name='global_config',
-    api='post:/l4d2/api/l4d2_map_config',
-    body=[
-        InputText(label='服务器host', name='web_username', value='${web_username}',
-                  labelRemark=Remark(shape='circle',
-                                     content='127.0.0.1')),
-        InputPassword(label='服务器', name='web_password', value='${web_password}',
-                      labelRemark=Remark(shape='circle',
-                                         content='登录本后台管理所需要的密码。')),
-        InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于本后台管理加密验证token的密钥。')),
-        InputText(label='查询key', name='l4_key', value='${l4_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于获取拓展功能的key。')),
-
-    ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
-)
-
-
-group_select = Select(label='分群配置（暂未完成）', name='group_id', source='${group_list}',
-                      placeholder='选择群')
-group_config_form = Form(
-    title='分群配置（暂未完成）',
-    visibleOn='group_id != null',
-    initApi='/l4d2/api/l4d2_group_config?group_id=${group_id}',
-    api='post:/l4d2/api/l4d2_group_config?group_id=${group_id}',
-    body=[
-        Switch(label='分群开关', name='enable', value='${enable}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle', content='针对该群的群聊学习开关，关闭后，仅该群不会学习和回复。')),
-        InputNumber(label='占位符', name='answer_threshold', value='${answer_threshold}', visibleOn='${enable}',
-                    min=2,
-                    labelRemark=Remark(shape='circle', content='单文本')),
-        InputTag(label='占位符', name='ban_words', value='${ban_words}', enableBatchAdd=True,
-                 placeholder='占位符，词条', visibleOn='${enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle', content='占位符词条')),
-
-    ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             ActionType.Ajax(
-                 label='保存至所有群',
-                 level=LevelEnum.primary,
-                 confirmText='确认将当前配置保存至所有群？',
-                 api='post:/l4d2/api/l4d2_group_config?group_id=all'
-             ),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
-)
-
-server_control = Select(label='服务器设置', name='id_rank', source='${server_list}',
-                      placeholder='选择服务器')
-
-server_ditail= Form(
-    title='',
-    api='post:/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
-    initApi='/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
-<<<<<<< Updated upstream
-    visibleOn='server_id != null',
-=======
-    visibleOn='id_rank != null',
->>>>>>> Stashed changes
-    body=[
-        Switch(label='是否是远程服务器', name='place', value='${place}', onText='是的', offText='不是',
-               labelRemark=Remark(shape='circle',
-                                  content='开启则确认为远程服务器')),
-        InputText(label='服务器名称', name='server_id', value='${server_id}',
-                  labelRemark=Remark(shape='circle',
-                                     content='服务器名字')),
-        InputText(label='服务器ip地址', name='host', value='${host}',
-                  labelRemark=Remark(shape='circle',
-                                     content='服务端所在ip地址,也可以是域名')),
-        InputText(label='所在端口', name='port', value='${port}',
-                      labelRemark=Remark(shape='circle',
-                                         content='服务端所在端口')),
-        InputPassword(label='rcon控制台密码', name='rcon', value='${rcon}',
-                      labelRemark=Remark(shape='circle',
-                                         content='服务端rcon密码')),
-        InputText(label='服务器本地文件位置', name='location', value='${location}',
-                      labelRemark=Remark(shape='circle',
-                                         content='求生服务器所在路径,该路径下有文件srcds_run')),        
-        InputText(label='远程账户', name='account', value='${account}',
-                  visibleOn='${place}',
-                  labelRemark=Remark(shape='circle',
-                                     content='远程服务器的登录账户名')),
-        InputPassword(label='远程密码', name='password', value='${password}',
-                      visibleOn='${place}',
-                  labelRemark=Remark(shape='circle',
-                                     content='远程服务器的登录密码')),
-    ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
-)
-
-query_table = TableCRUD(mode='table',
-                          title='',
-                          syncLocation=False,
-                          api='/l4d2/api/get_query_contexts',
-                          interval=60000,
-                          footable=True,
-                          itemActions=[ActionType.Url(
-                                tooltip='加入游戏',
-                                icon='fa fa-gamepad',
-                                confirmText = "加入steam://connect/"+'${ip}',
-                                url= "steam://connect/"+'${ip}',
-                                # url= "http://"+'${ip}',
-                                blank= True
-                                 ),
-                            ],
-                          columns = [
-                                    TableColumn(label='服主', name='master', searchable=True),
-                                    TableColumn(label='名称', name='name', searchable=True),
-                                    TableColumn(label='地图', name='map_', searchable=True),
-                                    TableColumn(label='玩家', name='rank_players', searchable=True),
-                                    TableColumn(label='延迟', name='ping', searchable=True),
-                                    TableColumn(label='IP 地址', name='ip', searchable=True),
-                                    ])
-
-server_page = PageSchema(url='/messages', icon='fa fa-comment', label='本地服务器管理',
-                          schema=Page(title='本地服务器管理',
-                                      interval=120000,
-                                      initApi='/l4d2/api/get_l4d2_messages',
-                                        body=[
-                              Alert(level=LevelEnum.info,
-                                    className='white-space-pre-wrap',
-                                    body=(f'此数据库记录了{NICKNAME}所在服务器下的求生服务器。\n'
-
-                                          f'· 功能暂未完善')),
-                              server_control,server_ditail]))
-query_page = PageSchema(url='/contexts', icon='fa fa-comments', label='远程服务器查询',
-                          schema=Page(title='远程服务器查询',
-                                      body=[Alert(level=LevelEnum.info,
-                                                  className='white-space-pre-wrap',
-                                                  body=(f'此数据库记录了{NICKNAME}所记录可查询的服务器ip。\n'
-                                                        # '· 点击"回复列表"可以查看该条内容已学习到的可能的回复。\n'
-                                                        # '· 点击"禁用"可以将该学习进行禁用，以后不会再学。\n'
-                                                        f'· 功能暂未完善')),
-                                            query_table]))
-
-database_page = PageSchema(label='数据库', icon='fa fa-database',
-                           children=[server_page, query_page])
-config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-wrench', label='配置',
-                         schema=Page(title='配置', initApi='/l4d2/api/get_group_list',
-                                     body=[global_config_form,group_select, group_config_form]))
-l4d2_page = PageSchema(label='求生之路', icon='fa fa-wechat (alias)', children=[config_page, database_page])
-
-github_logo = Tpl(className='w-full',
-                  tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>')
-header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo])
-
-admin_app = App(brandName='L4d2-Server',
-                logo='https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png',
-                header=header,
-                pages=[{
-                    'children': [config_page, database_page]
-                }],
-                footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>')
+from amis import  ActionType, TableCRUD, TableColumn
+from amis import  PageSchema, Switch, InputNumber, InputTag, Action, App
+from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper
+from amis import LevelEnum, Select,  Alert, Tpl, Flex
+
+
+from ..config import NICKNAME
+
+logo = Html(html='''
+<p align="center">
+    <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server">
+        <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png"
+         width="256" height="256" alt="l4d2-server">
+    </a>
+</p>
+<h1 align="center">Nonebot-Plugin-L4d2-Server 控制台</h1>
+<div align="center">
+    <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/" target="_blank">
+    Github仓库</a>
+</div>
+<br>
+<br>
+''')
+login_api = AmisAPI(
+    url='/l4d2/api/login',
+    method='post',
+    adaptor='''
+        if (payload.status == 0) {
+            localStorage.setItem("token", payload.data.token);
+        }
+        return payload;
+    '''
+)
+
+login_form = Form(api=login_api, title='', body=[
+    InputText(name='username', label='用户名',
+              labelRemark=Remark(shape='circle', content='后台管理用户名，默认为l4d2')),
+    InputPassword(name='password', label='密码',
+                  labelRemark=Remark(shape='circle', content='后台管理密码，默认为admin')),
+], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5), redirect='/l4d2/admin')
+body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form)
+login_page = Page(title='', body=[logo, body])
+
+global_config_form = Form(
+    title='全局配置',
+    name='global_config',
+    initApi='/l4d2/api/l4d2_global_config',
+    api='post:/l4d2/api/l4d2_global_config',
+    body=[
+        Switch(label='控制总开关（摆设）', name='total_enable', value='${total_enable}', onText='开启', offText='关闭',
+               labelRemark=Remark(shape='circle',
+                                  content='关闭后，禁用网页控制台，请参考文档启动方法')),
+        InputText(label='后台管理用户名', name='web_username', value='${web_username}',
+                  labelRemark=Remark(shape='circle',
+                                     content='登录本后台管理所需要的用户名。')),
+        InputPassword(label='后台管理密码', name='web_password', value='${web_password}',
+                      labelRemark=Remark(shape='circle',
+                                         content='登录本后台管理所需要的密码。')),
+        InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
+                  labelRemark=Remark(shape='circle',
+                                     content='用于本后台管理加密验证token的密钥。')),
+        InputText(label='查询key', name='l4_key', value='${l4_key}',
+                  labelRemark=Remark(shape='circle',
+                                     content='用于获取拓展功能的key,加q群399365126领取。')),
+        InputText(label='字体', name='l4_font', value='${l4_font}',
+                  labelRemark=Remark(shape='circle',
+                                     content='机器人返回图片中文字的字体。')),
+        Select(label='图片风格', name='l4_style', value='${l4_style}',source='${l4_styles}',
+                  labelRemark=Remark(shape='circle',
+                                     content='仅仅是批量查询的风格')),
+        InputTag(label='查询的远程服务器tag', name='l4_tag', value='${l4_tag}',
+                 enableBatchAdd=True,
+                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
+                 labelRemark=Remark(shape='circle',
+                                    content='在这里加入的用户，才能上传地图')),
+        InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
+                 enableBatchAdd=True,
+                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
+                 labelRemark=Remark(shape='circle',
+                                    content='在这里加入的用户，才能上传地图')),
+
+    ],
+    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
+             Action(label='重置', level=LevelEnum.warning, type='reset')]
+)
+
+upload_map_form = Form(
+    title='全局配置',
+    name='global_config',
+    api='post:/l4d2/api/l4d2_map_config',
+    body=[
+        InputText(label='服务器host', name='web_username', value='${web_username}',
+                  labelRemark=Remark(shape='circle',
+                                     content='127.0.0.1')),
+        InputPassword(label='服务器', name='web_password', value='${web_password}',
+                      labelRemark=Remark(shape='circle',
+                                         content='登录本后台管理所需要的密码。')),
+        InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
+                  labelRemark=Remark(shape='circle',
+                                     content='用于本后台管理加密验证token的密钥。')),
+        InputText(label='查询key', name='l4_key', value='${l4_key}',
+                  labelRemark=Remark(shape='circle',
+                                     content='用于获取拓展功能的key。')),
+
+    ],
+    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
+             Action(label='重置', level=LevelEnum.warning, type='reset')]
+)
+
+
+group_select = Select(label='分群配置（暂未完成）', name='group_id', source='${group_list}',
+                      placeholder='选择群')
+group_config_form = Form(
+    title='分群配置（暂未完成）',
+    visibleOn='group_id != null',
+    initApi='/l4d2/api/l4d2_group_config?group_id=${group_id}',
+    api='post:/l4d2/api/l4d2_group_config?group_id=${group_id}',
+    body=[
+        Switch(label='分群开关', name='enable', value='${enable}', onText='开启', offText='关闭',
+               labelRemark=Remark(shape='circle', content='针对该群的群聊学习开关，关闭后，仅该群不会学习和回复。')),
+        InputNumber(label='占位符', name='answer_threshold', value='${answer_threshold}', visibleOn='${enable}',
+                    min=2,
+                    labelRemark=Remark(shape='circle', content='单文本')),
+        InputTag(label='占位符', name='ban_words', value='${ban_words}', enableBatchAdd=True,
+                 placeholder='占位符，词条', visibleOn='${enable}', joinValues=False, extractValue=True,
+                 labelRemark=Remark(shape='circle', content='占位符词条')),
+
+    ],
+    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
+             ActionType.Ajax(
+                 label='保存至所有群',
+                 level=LevelEnum.primary,
+                 confirmText='确认将当前配置保存至所有群？',
+                 api='post:/l4d2/api/l4d2_group_config?group_id=all'
+             ),
+             Action(label='重置', level=LevelEnum.warning, type='reset')]
+)
+
+server_control = Select(label='服务器设置', name='id_rank', source='${server_list}',
+                      placeholder='选择服务器')
+
+server_ditail= Form(
+    title='',
+    api='post:/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
+    initApi='/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
+    visibleOn='id_rank != null',
+    body=[
+        Switch(label='是否是远程服务器', name='place', value='${place}', onText='是的', offText='不是',
+               labelRemark=Remark(shape='circle',
+                                  content='开启则确认为远程服务器')),
+        InputText(label='服务器名称', name='server_id', value='${server_id}',
+                  labelRemark=Remark(shape='circle',
+                                     content='服务器名字')),
+        InputText(label='服务器ip地址', name='host', value='${host}',
+                  labelRemark=Remark(shape='circle',
+                                     content='服务端所在ip地址,也可以是域名')),
+        InputText(label='所在端口', name='port', value='${port}',
+                      labelRemark=Remark(shape='circle',
+                                         content='服务端所在端口')),
+        InputPassword(label='rcon控制台密码', name='rcon', value='${rcon}',
+                      labelRemark=Remark(shape='circle',
+                                         content='服务端rcon密码')),
+        InputText(label='服务器本地文件位置', name='location', value='${location}',
+                      labelRemark=Remark(shape='circle',
+                                         content='求生服务器所在路径,该路径下有文件srcds_run')),        
+        InputText(label='远程账户', name='account', value='${account}',
+                  visibleOn='${place}',
+                  labelRemark=Remark(shape='circle',
+                                     content='远程服务器的登录账户名')),
+        InputPassword(label='远程密码', name='password', value='${password}',
+                      visibleOn='${place}',
+                  labelRemark=Remark(shape='circle',
+                                     content='远程服务器的登录密码')),
+    ],
+    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
+             Action(label='重置', level=LevelEnum.warning, type='reset')]
+)
+
+query_table = TableCRUD(mode='table',
+                          title='',
+                          syncLocation=False,
+                          api='/l4d2/api/get_query_contexts',
+                          interval=60000,
+                          footable=True,
+                          itemActions=[ActionType.Url(
+                                tooltip='加入游戏',
+                                icon='fa fa-gamepad',
+                                confirmText = "加入steam://connect/"+'${ip}',
+                                url= "steam://connect/"+'${ip}',
+                                # url= "http://"+'${ip}',
+                                blank= True
+                                 ),
+                            ],
+                          columns = [
+                                    TableColumn(label='服主', name='master', searchable=True),
+                                    TableColumn(label='名称', name='name', searchable=True),
+                                    TableColumn(label='地图', name='map_', searchable=True),
+                                    TableColumn(label='玩家', name='rank_players', searchable=True),
+                                    TableColumn(label='延迟', name='ping', searchable=True),
+                                    TableColumn(label='IP 地址', name='ip', searchable=True),
+                                    ])
+
+server_page = PageSchema(url='/messages', icon='fa fa-comment', label='本地服务器管理',
+                          schema=Page(title='本地服务器管理',
+                                      interval=120000,
+                                      initApi='/l4d2/api/get_l4d2_messages',
+                                        body=[
+                              Alert(level=LevelEnum.info,
+                                    className='white-space-pre-wrap',
+                                    body=(f'此数据库记录了{NICKNAME}所在服务器下的求生服务器。\n'
+
+                                          f'· 功能暂未完善')),
+                              server_control,server_ditail]))
+query_page = PageSchema(url='/contexts', icon='fa fa-comments', label='远程服务器查询',
+                          schema=Page(title='远程服务器查询',
+                                      body=[Alert(level=LevelEnum.info,
+                                                  className='white-space-pre-wrap',
+                                                  body=(f'此数据库记录了{NICKNAME}所记录可查询的服务器ip。\n'
+                                                        # '· 点击"回复列表"可以查看该条内容已学习到的可能的回复。\n'
+                                                        # '· 点击"禁用"可以将该学习进行禁用，以后不会再学。\n'
+                                                        f'· 功能暂未完善')),
+                                            query_table]))
+
+database_page = PageSchema(label='数据库', icon='fa fa-database',
+                           children=[server_page, query_page])
+config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-wrench', label='配置',
+                         schema=Page(title='配置', initApi='/l4d2/api/get_group_list',
+                                     body=[global_config_form,group_select, group_config_form]))
+l4d2_page = PageSchema(label='求生之路', icon='fa fa-wechat (alias)', children=[config_page, database_page])
+
+github_logo = Tpl(className='w-full',
+                  tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>')
+header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo])
+
+admin_app = App(brandName='L4d2-Server',
+                logo='https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png',
+                header=header,
+                pages=[{
+                    'children': [config_page, database_page]
+                }],
+                footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>')
```

#### html2text {}

```diff
@@ -83,19 +83,18 @@
 ( label='ä¿å­è³ææç¾¤', level=LevelEnum.primary,
 confirmText='ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼', api='post:/l4d2/api/
 l4d2_group_config?group_id=all' ), Action(label='éç½®',
 level=LevelEnum.warning, type='reset')] ) server_control = Select
 (label='æå¡å¨è®¾ç½®', name='id_rank', source='${server_list}',
 placeholder='éæ©æå¡å¨') server_ditail= Form( title='', api='post:/l4d2/
 api/l4d2_server_config?id_rank=${id_rank}', initApi='/l4d2/api/
-l4d2_server_config?id_rank=${id_rank}', <<<<<<< Updated upstream
-visibleOn='server_id != null', ======= visibleOn='id_rank != null', >>>>>>>
-Stashed changes body=[ Switch(label='æ¯å¦æ¯è¿ç¨æå¡å¨', name='place',
-value='${place}', onText='æ¯ç', offText='ä¸æ¯', labelRemark=Remark
-(shape='circle', content='å¼å¯åç¡®è®¤ä¸ºè¿ç¨æå¡å¨')), InputText
+l4d2_server_config?id_rank=${id_rank}', visibleOn='id_rank != null', body=
+[ Switch(label='æ¯å¦æ¯è¿ç¨æå¡å¨', name='place', value='${place}',
+onText='æ¯ç', offText='ä¸æ¯', labelRemark=Remark(shape='circle',
+content='å¼å¯åç¡®è®¤ä¸ºè¿ç¨æå¡å¨')), InputText
 (label='æå¡å¨åç§°', name='server_id', value='${server_id}',
 labelRemark=Remark(shape='circle', content='æå¡å¨åå­')), InputText
 (label='æå¡å¨ipå°å', name='host', value='${host}', labelRemark=Remark
 (shape='circle', content='æå¡ç«¯æå¨ipå°å,ä¹å¯ä»¥æ¯åå')),
 InputText(label='æå¨ç«¯å£', name='port', value='${port}',
 labelRemark=Remark(shape='circle', content='æå¡ç«¯æå¨ç«¯å£')),
 InputPassword(label='rconæ§å¶å°å¯ç ', name='rcon', value='${rcon}',
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/message.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# 坐牢
-PRISON = {
-    1:[
-        '⭐低级牢房',
-        '⭐牢动最光荣',
-        '⭐能者多牢',
-        '⭐年年有牢',
-    ],
-    2:[
-        '⭐⭐中级牢房',
-        '⭐⭐牢不可破',
-        '⭐⭐牢不可破联盟',
-        '⭐⭐牢底坐穿联盟',
-        '⭐⭐牢饭恰饱联盟',
-        '⭐⭐个个都是人才说话又好听',
-        '⭐⭐来点狱卒',
-    ],
-    3:[
-        '⭐⭐⭐曼德拉的前半生',
-        '⭐⭐⭐肖申克的救赎',
-        '⭐⭐⭐甲级战犯',
-        '⭐⭐⭐刘培强正在尝试逃离冷冻仓',
-    ]
-}
-
-QUEREN ={
-    1:[
-        '📞📞1Q3速来坐牢',
-        '📞📞📞发起了anne坐牢',
-        '📞📞📞摇人摇人，一个人玩个锤子',
-        '📞📞📞1=3速来坐牢',
-        '📞📞📞差三个速来',
-    ],
-    2:[
-        '📞📞2Q2速来坐牢',
-        '📞📞2=2这牢十分的珍贵，让同志们先做',
-        '📞📞牢房过半，速速人牢',
-        '📞📞2Q2有大佬带逛街速来',
-        '📞📞2=2速来坐牢',
-    ],
-    3:[
-        '📞牢房三缺一，速来',
-        '📞3Q1来个大佬带逛街',
-        '📞3Q1就等你了',
-        '📞别来他们三个还没一个人分高',
-    ],
-    4:[
-        '📞有人旁观，速来',
-        '📞有人越狱，呼叫支援',
-        '📞别让牢房成为寂寞',
-        '📞有人还没进，希望你网络比他好',
-    ]
-}
-KAILAO = [
-    '🏠又来坐牢了？',
-    '🏠已经变成牢房的样子了！',
-    '🏠是谁在呼唤牢房？',
-    '🏠牢房青云阁雅座四位',
+# 坐牢
+PRISON = {
+    1:[
+        '⭐低级牢房',
+        '⭐牢动最光荣',
+        '⭐能者多牢',
+        '⭐年年有牢',
+    ],
+    2:[
+        '⭐⭐中级牢房',
+        '⭐⭐牢不可破',
+        '⭐⭐牢不可破联盟',
+        '⭐⭐牢底坐穿联盟',
+        '⭐⭐牢饭恰饱联盟',
+        '⭐⭐个个都是人才说话又好听',
+        '⭐⭐来点狱卒',
+    ],
+    3:[
+        '⭐⭐⭐曼德拉的前半生',
+        '⭐⭐⭐肖申克的救赎',
+        '⭐⭐⭐甲级战犯',
+        '⭐⭐⭐刘培强正在尝试逃离冷冻仓',
+    ]
+}
+
+QUEREN ={
+    1:[
+        '📞📞1Q3速来坐牢',
+        '📞📞📞发起了anne坐牢',
+        '📞📞📞摇人摇人，一个人玩个锤子',
+        '📞📞📞1=3速来坐牢',
+        '📞📞📞差三个速来',
+    ],
+    2:[
+        '📞📞2Q2速来坐牢',
+        '📞📞2=2这牢十分的珍贵，让同志们先做',
+        '📞📞牢房过半，速速人牢',
+        '📞📞2Q2有大佬带逛街速来',
+        '📞📞2=2速来坐牢',
+    ],
+    3:[
+        '📞牢房三缺一，速来',
+        '📞3Q1来个大佬带逛街',
+        '📞3Q1就等你了',
+        '📞别来他们三个还没一个人分高',
+    ],
+    4:[
+        '📞有人旁观，速来',
+        '📞有人越狱，呼叫支援',
+        '📞别让牢房成为寂寞',
+        '📞有人还没进，希望你网络比他好',
+    ]
+}
+KAILAO = [
+    '🏠又来坐牢了？',
+    '🏠已经变成牢房的样子了！',
+    '🏠是谁在呼唤牢房？',
+    '🏠牢房青云阁雅座四位',
 ]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/seach.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from bs4 import BeautifulSoup
-import httpx
-
-
-def anne_search(name):
-    """输入名字返回列表["""
-    url = 'https://sb.trygek.com/l4d_stats/ranking/search.php'
-    data = {'search': name}
-    headers = {'Content-Type': 'application/x-www-form-urlencoded'}
-    data = httpx.post(url,data = data,headers=headers,timeout=60).content.decode('utf-8')
-    soup = BeautifulSoup(data, 'html.parser')
-    # 获取标题
-    title = []
-    thead = soup.find('thead')
-    for i in thead.find_all('td'):
-        tag = i.text.strip()
-        title.append(tag)
-    title.append('steamid')
-    # 角色信息
-    datas = soup.find('table')
-    datas = datas.find('tbody')
-    datas = datas.find_all('tr')
-    return [datas,title]
-
-def name_steamid_html(name):
-    """您称通过网页来返回求生steamid"""
-    data_title = anne_search(name)
-    data = data_title[0]
-    for i in data:
-        onclick:str = i['onclick']
-        steamid = onclick.split('=')[2].strip("'")
-        return steamid
-
+from bs4 import BeautifulSoup
+import httpx
+
+
+def anne_search(name):
+    """输入名字返回列表["""
+    url = 'https://sb.trygek.com/l4d_stats/ranking/search.php'
+    data = {'search': name}
+    headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+    data = httpx.post(url,data = data,headers=headers,timeout=60).content.decode('utf-8')
+    soup = BeautifulSoup(data, 'html.parser')
+    # 获取标题
+    title = []
+    thead = soup.find('thead')
+    for i in thead.find_all('td'):
+        tag = i.text.strip()
+        title.append(tag)
+    title.append('steamid')
+    # 角色信息
+    datas = soup.find('table')
+    datas = datas.find('tbody')
+    datas = datas.find_all('tr')
+    return [datas,title]
+
+def name_steamid_html(name):
+    """您称通过网页来返回求生steamid"""
+    data_title = anne_search(name)
+    data = data_title[0]
+    for i in data:
+        onclick:str = i['onclick']
+        steamid = onclick.split('=')[2].strip("'")
+        return steamid
+
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/txt_to_img.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from io import BytesIO
-from PIL import Image, ImageDraw, ImageFont
-from nonebot.adapters.onebot.v11 import MessageSegment
-from nonebot_plugin_txt2img import Txt2Img
-from .config import l4_config
-
-l4_font = l4_config.l4_font
-"""直接超的智障回复"""
-def txt_to_img(text: str, font_size=30, font_path=l4_font) -> bytes:
-    text = line_break(text)
-    d_font = ImageFont.truetype(font_path, font_size)
-    lines = text.count('\n')  # 计算行数
-    image = Image.new("L", (LINE_CHAR_COUNT*font_size //
-                      2 + 50, font_size*lines+50), "white")
-    draw_table = ImageDraw.Draw(im=image)
-    draw_table.text(xy=(25, 25), text=text, fill='#000000',
-                    font=d_font, spacing=4)  # spacing调节机制不清楚如何计算
-    new_img = image.convert("RGB")
-    img_byte = BytesIO()
-    new_img.save(img_byte, format='PNG')
-    binary_content = img_byte.getvalue()
-    return binary_content
-
-
-LINE_CHAR_COUNT = 30*2  # 每行字符数：30个中文字符(=60英文字符)
-CHAR_SIZE = 30
-TABLE_WIDTH = 4
-
-
-def line_break(line: str) -> str:
-    ret = ''
-    width = 0
-    for c in line:
-        if len(c.encode('utf8')) == 3:  # 中文
-            if LINE_CHAR_COUNT == width + 1:  # 剩余位置不够一个汉字
-                width = 2
-                ret += '\n' + c
-            else:  # 中文宽度加2，注意换行边界
-                width += 2
-                ret += c
-        else:
-            if c == '\t':
-                space_c = TABLE_WIDTH - width % TABLE_WIDTH  # 已有长度对TABLE_WIDTH取余
-                ret += ' ' * space_c
-                width += space_c
-            elif c == '\n':
-                width = 0
-                ret += c
-            else:
-                width += 1
-                ret += c
-        if width >= LINE_CHAR_COUNT:
-            ret += '\n'
-            width = 0
-    if ret.endswith('\n'):
-        return ret
-    return ret + '\n'
-
-
-def mode_txt_to_img(title:str,text:str,font_size:int = 32,):
-    txt2img = Txt2Img()
-    txt2img.set_font_size(font_size)
-    pic = txt2img.draw(title, text)
-    msg = MessageSegment.image(pic)
+from io import BytesIO
+from PIL import Image, ImageDraw, ImageFont
+from nonebot.adapters.onebot.v11 import MessageSegment
+from nonebot_plugin_txt2img import Txt2Img
+from .config import l4_config
+
+l4_font = l4_config.l4_font
+"""直接超的智障回复"""
+def txt_to_img(text: str, font_size=30, font_path=l4_font) -> bytes:
+    text = line_break(text)
+    d_font = ImageFont.truetype(font_path, font_size)
+    lines = text.count('\n')  # 计算行数
+    image = Image.new("L", (LINE_CHAR_COUNT*font_size //
+                      2 + 50, font_size*lines+50), "white")
+    draw_table = ImageDraw.Draw(im=image)
+    draw_table.text(xy=(25, 25), text=text, fill='#000000',
+                    font=d_font, spacing=4)  # spacing调节机制不清楚如何计算
+    new_img = image.convert("RGB")
+    img_byte = BytesIO()
+    new_img.save(img_byte, format='PNG')
+    binary_content = img_byte.getvalue()
+    return binary_content
+
+
+LINE_CHAR_COUNT = 30*2  # 每行字符数：30个中文字符(=60英文字符)
+CHAR_SIZE = 30
+TABLE_WIDTH = 4
+
+
+def line_break(line: str) -> str:
+    ret = ''
+    width = 0
+    for c in line:
+        if len(c.encode('utf8')) == 3:  # 中文
+            if LINE_CHAR_COUNT == width + 1:  # 剩余位置不够一个汉字
+                width = 2
+                ret += '\n' + c
+            else:  # 中文宽度加2，注意换行边界
+                width += 2
+                ret += c
+        else:
+            if c == '\t':
+                space_c = TABLE_WIDTH - width % TABLE_WIDTH  # 已有长度对TABLE_WIDTH取余
+                ret += ' ' * space_c
+                width += space_c
+            elif c == '\n':
+                width = 0
+                ret += c
+            else:
+                width += 1
+                ret += c
+        if width >= LINE_CHAR_COUNT:
+            ret += '\n'
+            width = 0
+    if ret.endswith('\n'):
+        return ret
+    return ret + '\n'
+
+
+def mode_txt_to_img(title:str,text:str,font_size:int = 32,):
+    txt2img = Txt2Img()
+    txt2img.set_font_size(font_size)
+    pic = txt2img.draw(title, text)
+    msg = MessageSegment.image(pic)
     return msg
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.5.2/nonebot_plugin_l4d2_server/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-
-from nonebot.adapters.onebot.v11 import Bot,MessageEvent,GroupMessageEvent
-from nonebot.log import logger
-import struct
-import httpx
-import os
-from pathlib import Path
-
-from typing import List,Dict,Union
-from .txt_to_img import txt_to_img
-from .config import *
-from .l4d2_anne import write_player,del_player,anne_messgae
-from .l4d2_server.rcon import read_server_cfg_rcon,rcon_server
-from .l4d2_queries import queries,player_queries
-from .l4d2_queries.qqgroup import *
-from .l4d2_server.workshop import workshop_to_dict
-from .l4d2_image.steam import url_to_byte
-import tempfile
-import random
-
-
-
-async def get_file(url: str, down_file: Path):
-    '''
-    下载指定Url到指定位置
-    '''
-    try:
-        if l4_config.l4_only:
-            maps = await url_to_byte(url)
-        else:
-            maps = httpx.get(url).content
-        logger.info('已获取文件，尝试新建文件并写入')
-        with open(down_file, 'wb') as mfile:
-            mfile.write(maps)
-        logger.info('下载成功')
-        return '文件已下载，正在解压'
-    except Exception as e:
-        logger.info(f"文件获取不到/已损坏:原因是{e}")
-        return None
-
-
-def get_vpk(vpk_list: List[str], map_path: Path, file_: str = '.vpk') -> List[str]:
-    '''
-    获取路径下所有vpk文件名，并存入vpk_list列表中
-    '''
-    vpk_list.extend([file for file in os.listdir(str(map_path)) if file.endswith(file_)])
-    return vpk_list
-
-
-
-def mes_list(mes: str, name_list: List[str]) -> str:
-    if name_list:
-        for idx, name in enumerate(name_list):
-            mes += f'\n{idx+1}、{name}'
-    return mes
-
-
-
-
-def del_map(num: int, map_path: Path) -> str:
-    '''
-    删除指定的地图
-    '''
-    map = get_vpk(map_path)
-    map_name = map[num - 1]
-    del_file = map_path / map_name
-    os.remove(del_file)
-    return map_name
-
-
-def rename_map(num: int, rename: str, map_path: Path) -> str:
-    '''
-    改名指定的地图
-    '''
-    map = get_vpk(map_path)
-    map_name = map[num - 1]
-    old_file = map_path / map_name
-    new_file = map_path / rename
-    os.rename(old_file, new_file)
-    logger.info('改名成功')
-    return map_name
-
-
-def text_to_png(msg: str) -> bytes:
-    """文字转png"""
-    return txt_to_img(msg)
-
-
-
-def solve(msg:str):
-    """删除str最后一行"""
-    lines = msg.splitlines()
-    lines.pop()
-    return '\n'.join(lines)
-
-
-async def search_anne(name:str,usr_id:str):
-    """获取anne成绩"""
-    return await anne_messgae(name,usr_id)
-    
-
-async def bind_steam(id:str,msg:str,nickname:str):
-    """绑定qq-steam"""
-    return await write_player(id,msg,nickname)
-
-def name_exist(id:str):
-    """删除绑定信息"""
-    return del_player(id)
-
-async def get_message_at(data: str) -> list:
-    data = json.loads(data)
-    return [int(msg['data']['qq']) for msg in data['message'] if msg['type'] == 'at']
-
-    
-
-def at_to_usrid(at):
-    return at[0] if at else None
-
-
-async def rcon_command(rcon, cmd):
-    return await rcon_server(rcon, cmd.strip())
-
-async def command_server(msg: str):
-    rcon = await read_server_cfg_rcon()
-    msg = await rcon_command(rcon, msg)
-    if not msg:
-        msg = '你可能发送了一个无用指令，或者换图导致服务器无响应'
-    elif msg.startswith('Unknown command'):
-        msg = '无效指令：' + msg.replace('Unknown command', '').strip()
-    return msg.strip().replace('\n', '')
-
-
-
-
-async def queries_server(msg:list) -> str:
-    """查询ip返回信息"""
-    ip = msg[0]
-    port = msg[1]
-    msgs = ''
-    try:
-        msgs = await  queries(ip,port)
-        msgs += await player_queries(ip,port)
-    except (struct.error,TimeoutError):
-        pass
-    # except Exception:
-        # msgs = '有无法识别的用户名'
-        # return msgs
-    return msgs
-
-async def add_ip(group_id,host,port):
-    """先查找是否存在，如果不存在则创建"""
-    return await bind_group_ip(group_id,host,port)
-
-async def del_ip(group_id,number):
-    """删除群ip"""
-    return await del_group_ip(group_id,number)
-
-async def show_ip(group_id):
-    """先查找群ip，再根据群ip返回"""
-    data_list = await get_qqgroup_ip_msg(group_id)
-    logger.info(data_list)
-    if len(data_list) == 0 :
-        return "本群没有订阅"
-    msg = await qq_ip_queries_pic(data_list)
-    return  msg
-
-async def get_number_url(number):
-    'connect AGNES.DIGITAL.LINE.PM:40001'
-    ip = await get_server_ip(number)
-    if not ip:
-        return '该序号不存在'
-    url = f'connect {ip}'
-    return url
-
-async def workshop_msg(msg:str):
-    """url变成id，拼接post请求"""
-    if msg.startswith('https://steamcommunity.com/sharedfiles/filedetails/?id'):
-        try:
-            msg = msg.split('&')[0]
-        except:
-            pass
-        msg = msg.replace('https://steamcommunity.com/sharedfiles/filedetails/?id=','')
-    if msg.isdigit():
-        data:Union[dict,List[dict]] = await workshop_to_dict(msg)
-        return data
-    else:
-        return None
-    
-async def save_file(file:bytes,path_name):
-    """保存文件"""
-    with open(path_name,'w') as files:
-        files.write(file)
-        
-async def get_anne_server_ip(ip):
-    """输出查询ip和ping"""
-    host,port = split_maohao(ip)
-    data = await queries_server([host,port])
-    lines = data.splitlines()
-    msg = '\n'.join(lines[1:])
-    msg += '\nconnect ' + ip
-    return msg
-
-async def upload_file(bot: Bot, event: MessageEvent, file_data: bytes, filename: str):
-    """上传临时文件"""
-    if systems == "win" or "other":
-        with tempfile.TemporaryDirectory() as temp_dir:
-            with open(Path(temp_dir) / filename, "wb") as f:
-                f.write(file_data)
-            if isinstance(event, GroupMessageEvent):
-                await bot.call_api(
-                    "upload_group_file", group_id=event.group_id, file=f.name, name=filename
-                )
-            else:
-                await bot.call_api(
-                    "upload_private_file", user_id=event.user_id, file=f.name, name=filename
-                )
-        os.remove(Path().joinpath(filename))
-    elif systems == "linux":
-        with tempfile.NamedTemporaryFile("wb+") as f:
-            f.write(file_data)
-            if isinstance(event, GroupMessageEvent):
-                await bot.call_api(
-                    "upload_group_file", group_id=event.group_id, file=f.name, name=filename
-                )
-            else:
-                await bot.call_api(
-                    "upload_private_file", user_id=event.user_id, file=f.name, name=filename
-                )
-
-
-async def json_server_to_tag_dict(key:str,msg:str):
-    """
-    l4d2字典转tag的dict结果
-     - 1、先匹配腐竹
-     - 2、再匹配模式、没有参数则从直接匹配最上面的
-     - 3、匹配数字（几服），没有参数则从结果里随机返回一个
-    """
-    data_dict = {}
-    data_list = []
-    msg = msg.replace(' ','')
-    # 腐竹循环
-    for tag,value in ALL_HOST.items():
-        value:List[dict]  
-        if tag == key:
-            data_dict.update({'server':tag})
-            if not msg:
-                # 腐竹
-                data_dict.update(random.choice(value))
-            elif msg.isdigit():
-                logger.info("腐竹 + 序号")
-                for server in value:
-                    if msg == str(server['id']):
-                        data_dict.update(server)
-                        break
-            else:
-                logger.info("腐竹 + 模式 + 序号")
-                for server in value:
-                    if msg.startswith(server['version']):
-                        data_list.append(server)
-                        msg_id = msg[len(server['version']):]
-                        if msg_id == str(server['id']):
-                            data_dict.update(server)
-                            break
-                else:
-                    # 腐竹 + 模式
-                    data_dict.update(random.choice(data_list))
-
-    logger.info(data_dict)
-    return data_dict
-
-
-
+
+from nonebot.adapters.onebot.v11 import Bot,MessageEvent,GroupMessageEvent
+from nonebot.log import logger
+import struct
+import httpx
+import os
+from pathlib import Path
+
+from typing import List,Dict,Union
+from .txt_to_img import txt_to_img
+from .config import *
+from .l4d2_anne import write_player,del_player,anne_messgae
+from .l4d2_server.rcon import read_server_cfg_rcon,rcon_server
+from .l4d2_queries import queries,player_queries
+from .l4d2_queries.qqgroup import *
+from .l4d2_server.workshop import workshop_to_dict
+from .l4d2_image.steam import url_to_byte
+import tempfile
+import random
+
+
+
+async def get_file(url: str, down_file: Path):
+    '''
+    下载指定Url到指定位置
+    '''
+    try:
+        if l4_config.l4_only:
+            maps = await url_to_byte(url)
+        else:
+            maps = httpx.get(url).content
+        logger.info('已获取文件，尝试新建文件并写入')
+        with open(down_file, 'wb') as mfile:
+            mfile.write(maps)
+        logger.info('下载成功')
+        return '文件已下载，正在解压'
+    except Exception as e:
+        logger.info(f"文件获取不到/已损坏:原因是{e}")
+        return None
+
+
+def get_vpk(vpk_list: List[str], map_path: Path, file_: str = '.vpk') -> List[str]:
+    '''
+    获取路径下所有vpk文件名，并存入vpk_list列表中
+    '''
+    vpk_list.extend([file for file in os.listdir(str(map_path)) if file.endswith(file_)])
+    return vpk_list
+
+
+
+def mes_list(mes: str, name_list: List[str]) -> str:
+    if name_list:
+        for idx, name in enumerate(name_list):
+            mes += f'\n{idx+1}、{name}'
+    return mes
+
+
+
+
+def del_map(num: int, map_path: Path) -> str:
+    '''
+    删除指定的地图
+    '''
+    map = get_vpk(map_path)
+    map_name = map[num - 1]
+    del_file = map_path / map_name
+    os.remove(del_file)
+    return map_name
+
+
+def rename_map(num: int, rename: str, map_path: Path) -> str:
+    '''
+    改名指定的地图
+    '''
+    map = get_vpk(map_path)
+    map_name = map[num - 1]
+    old_file = map_path / map_name
+    new_file = map_path / rename
+    os.rename(old_file, new_file)
+    logger.info('改名成功')
+    return map_name
+
+
+def text_to_png(msg: str) -> bytes:
+    """文字转png"""
+    return txt_to_img(msg)
+
+
+
+def solve(msg:str):
+    """删除str最后一行"""
+    lines = msg.splitlines()
+    lines.pop()
+    return '\n'.join(lines)
+
+
+async def search_anne(name:str,usr_id:str):
+    """获取anne成绩"""
+    return await anne_messgae(name,usr_id)
+    
+
+async def bind_steam(id:str,msg:str,nickname:str):
+    """绑定qq-steam"""
+    return await write_player(id,msg,nickname)
+
+def name_exist(id:str):
+    """删除绑定信息"""
+    return del_player(id)
+
+async def get_message_at(data: str) -> list:
+    data = json.loads(data)
+    return [int(msg['data']['qq']) for msg in data['message'] if msg['type'] == 'at']
+
+    
+
+def at_to_usrid(at):
+    return at[0] if at else None
+
+
+async def rcon_command(rcon, cmd):
+    return await rcon_server(rcon, cmd.strip())
+
+async def command_server(msg: str):
+    rcon = await read_server_cfg_rcon()
+    msg = await rcon_command(rcon, msg)
+    if not msg:
+        msg = '你可能发送了一个无用指令，或者换图导致服务器无响应'
+    elif msg.startswith('Unknown command'):
+        msg = '无效指令：' + msg.replace('Unknown command', '').strip()
+    return msg.strip().replace('\n', '')
+
+
+
+
+async def queries_server(msg:list) -> str:
+    """查询ip返回信息"""
+    ip = msg[0]
+    port = msg[1]
+    msgs = ''
+    try:
+        msgs = await  queries(ip,port)
+        msgs += await player_queries(ip,port)
+    except (struct.error,TimeoutError):
+        pass
+    # except Exception:
+        # msgs = '有无法识别的用户名'
+        # return msgs
+    return msgs
+
+async def add_ip(group_id,host,port):
+    """先查找是否存在，如果不存在则创建"""
+    return await bind_group_ip(group_id,host,port)
+
+async def del_ip(group_id,number):
+    """删除群ip"""
+    return await del_group_ip(group_id,number)
+
+async def show_ip(group_id):
+    """先查找群ip，再根据群ip返回"""
+    data_list = await get_qqgroup_ip_msg(group_id)
+    logger.info(data_list)
+    if len(data_list) == 0 :
+        return "本群没有订阅"
+    msg = await qq_ip_queries_pic(data_list)
+    return  msg
+
+async def get_number_url(number):
+    'connect AGNES.DIGITAL.LINE.PM:40001'
+    ip = await get_server_ip(number)
+    if not ip:
+        return '该序号不存在'
+    url = f'connect {ip}'
+    return url
+
+async def workshop_msg(msg:str):
+    """url变成id，拼接post请求"""
+    if msg.startswith('https://steamcommunity.com/sharedfiles/filedetails/?id'):
+        try:
+            msg = msg.split('&')[0]
+        except:
+            pass
+        msg = msg.replace('https://steamcommunity.com/sharedfiles/filedetails/?id=','')
+    if msg.isdigit():
+        data:Union[dict,List[dict]] = await workshop_to_dict(msg)
+        return data
+    else:
+        return None
+    
+async def save_file(file:bytes,path_name):
+    """保存文件"""
+    with open(path_name,'w') as files:
+        files.write(file)
+        
+async def get_anne_server_ip(ip):
+    """输出查询ip和ping"""
+    host,port = split_maohao(ip)
+    data = await queries_server([host,port])
+    lines = data.splitlines()
+    msg = '\n'.join(lines[1:])
+    msg += '\nconnect ' + ip
+    return msg
+
+async def upload_file(bot: Bot, event: MessageEvent, file_data: bytes, filename: str):
+    """上传临时文件"""
+    if systems == "win" or "other":
+        with tempfile.TemporaryDirectory() as temp_dir:
+            with open(Path(temp_dir) / filename, "wb") as f:
+                f.write(file_data)
+            if isinstance(event, GroupMessageEvent):
+                await bot.call_api(
+                    "upload_group_file", group_id=event.group_id, file=f.name, name=filename
+                )
+            else:
+                await bot.call_api(
+                    "upload_private_file", user_id=event.user_id, file=f.name, name=filename
+                )
+        os.remove(Path().joinpath(filename))
+    elif systems == "linux":
+        with tempfile.NamedTemporaryFile("wb+") as f:
+            f.write(file_data)
+            if isinstance(event, GroupMessageEvent):
+                await bot.call_api(
+                    "upload_group_file", group_id=event.group_id, file=f.name, name=filename
+                )
+            else:
+                await bot.call_api(
+                    "upload_private_file", user_id=event.user_id, file=f.name, name=filename
+                )
+
+
+async def json_server_to_tag_dict(key:str,msg:str):
+    """
+    l4d2字典转tag的dict结果
+     - 1、先匹配腐竹
+     - 2、再匹配模式、没有参数则从直接匹配最上面的
+     - 3、匹配数字（几服），没有参数则从结果里随机返回一个
+    """
+    data_dict = {}
+    data_list = []
+    msg = msg.replace(' ','')
+    # 腐竹循环
+    for tag,value in ALL_HOST.items():
+        value:List[dict]  
+        if tag == key:
+            data_dict.update({'server':tag})
+            if not msg:
+                # 腐竹
+                data_dict.update(random.choice(value))
+            elif msg.isdigit():
+                logger.info("腐竹 + 序号")
+                for server in value:
+                    if msg == str(server['id']):
+                        data_dict.update(server)
+                        break
+            else:
+                logger.info("腐竹 + 模式 + 序号")
+                for server in value:
+                    if msg.startswith(server['version']):
+                        data_list.append(server)
+                        msg_id = msg[len(server['version']):]
+                        if msg_id == str(server['id']):
+                            data_dict.update(server)
+                            break
+                else:
+                    # 腐竹 + 模式
+                    data_dict.update(random.choice(data_list))
+
+    logger.info(data_dict)
+    return data_dict
+
+
+
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/README.md` & `nonebot_plugin_l4d2_server-0.5.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,360 +1,365 @@
-<div align="center">
-  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
-  <br>
-  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot_plugin_l4d2_server
-
-_✨Nonebot & Left 4 Dead 2 server操作✨_
-<div align = "center">
-        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
-</div><br>
-<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
-        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">
-</a>
-<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">
-        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">
-</a>
-<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
-        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
-        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
-    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
-</a>
-    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
-    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
-
-</div>
-
-
-
-## 主要功能
-
-- 求生服务器-本地多路径操作（传地图）
-- 批量查询指定ip服务器状态和玩家
-- 创意工坊下载和喷漆制作
-- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
-
-
-## 数据结构
-
-bot所在文件夹下
-```txt
-举例：
-└── data
-    └── L4D2
-        ├── l4d2.yml
-        ├── l4d2.json
-        ├── sql
-        │   └── L4D2.db
-        ├── image
-        │   └── players
-        │       └── ...
-        └── l4d2
-            ├── 关键词1.json
-            ├── 关键词2.json
-            └── ...
-...
-```
-
-新增一个json文件，格式如下,文件名与需要响应的指令一致
-`l4d2.json`和`关键词1.json`都可以加载
-
-        {
-        "呆呆": [
-                {
-                "id": 1,
-                "version": "战役",
-                "ip": "43.248.188.17:27031"
-                },
-                {
-                "id": 2,
-                "version": "战役",
-                "ip": "43.248.188.17:27032"
-                }
-        ]
-        }
-
-## 🌐 默认服务器
-
-由于不可抗力原因，暂时不使用在线的方式获取ip，有需求可以自行添加
-以下仅供参考本人使用的查询服务器
-
-| 指令 | 服务器 | op | 数量 |
-|:-----:|:----:|:----:|:----:|
-| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 5
-| 云 | anne电信服云服 | 东 | 19
-| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
-| 橘 | 橘希实香的小窝 | 橘希实香 | 21
-| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
-| 音理 | 星空列车与白的旅行 | 音理 | 3
-| 尤 | 尤尤 | 晓音 | 3
-| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
-| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 2
-| Air | Air | Air | 15
-| 3ks | 为人民服务 | DK | 14
-| 驴头 | 驴头服 | lvt | 4
-| 尸鬼 | 尸鬼狂潮 | ❀几❀ | 7
-
-## 🔖 更新日志
-
-<details>
-<summary>展开/收起</summary>
-
-### 0.5.1--2022.5.01
-
-- 解决了main和dev分支的一个严重bug（也许没解决
-- 本地化，更好的添加,删除远程分支
-- 服务器忘了备份，尽力抢救了数据了
-
-### 0.5.0--2022.4.28
-
-- 重构config，并弃用env设置
-- 使用网页控制台来控制配置
-- 新增了很多不会报错的bug
-
-### 0.4.9--2022.4
-
-- 修复h11版本错误的bug
-- 重写了config，下个版本正式使用yaml替代env设置
-- 新增远程连接测试代码
-
-### 0.4.8--2022.4.16
-
-- 新增重载ip
-- 修复了一些windows启动下奇奇怪怪的bug
-
-### 0.4.7--2022.4.13
-
-- 新增模式查询
-- 列表推导替换套娃循环
-
-### 0.4.6--2022.4.9
-
-- 显示无效服
-- 优化服务器排序算法（list.sort()天下第一）
-- 默认关闭web端
-
-### 0.4.5--2022.4.9
-
-- 修bug（恼）
-
-### 0.4.2--2022.4.9
-
-- 修复响应开头匹配出现的重大bug
-- 启用web端
-- web使用yaml管理，未来可能删除env配置
-
-### 0.4.1--2022.3
-
-- 修复rar压缩包命名错误
-- 更新了tag的参数读取方式
-- 确定了传文件私聊比群聊快速
-- 修复了电信服计算错误
-
-### 0.4.0--2022.3.27
-
-- 新增web控制台
-- 修复传图超时参数错误
-- 重写求生ip获取方法 ~ 数据库苦手 ~
-- 重写文档
-- 不再内置ip（毕竟ipv4都暴露太危险了）
-
-### 0.3.7--2022.3
-
-- 新增三方下载网盘
-- 修复windows上传临时文件错误
-- 优化查服流程
-- 优化anne服随机功能
-
-### 0.3.6--2022.3.10
-
-- 暂时关闭web端，后续修改
-- 优化图片显示
-- 修复了海量bug
-- 新增三方图查询
-
-### 0.3.5--2022.3.6
-
-- 新增ping查询（在ip里包括）
-- 新增api查询（未完成）
-- 修复了电信服查询绑定名字无法查询的错误
-- 新增了救援率的显示
-- 新增web端（未完成）
-
-### 0.3.4--2022.3.1
-
-- 新增本地插件smx查询
-- 增加了三个内置群服
-- 修改了图片的UI,变好看了
-- 删减了部分图片和字体，使得轻量化
-- 修复了海量bug
-- 修复了python3.8中typing错误
-
-### 0.3.3--2022.2.26
-
-- 重写协议，使用a2s库，同时解决win端不同报错无法输出
-- 重~抄~写服务器查询UI,解决了不好看的问题
-- 从win测试，解决了一些win特有的bug
-- 重写服务器查询~还得是json~
-- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问
-- 新增批量查询服务器，不带参数则返回图片
-
-### 0.3.1--2022.2.22
-
-- 修复了路径识别为str对象的错误
-- 修复了初始化找不到文件的错误
-- 修复了路径拼接错误
-- 在win端成功测试，修复压缩包bug
-- 新增开关协程异步env设置
-- 测试rcon建立通讯
-- 实现切换路径查看地图和使用rcon指令
-
-### 0.3.0--2022.2.18
-
-- 修改了新的env配置，使得支持本地多服务器操作
-- 彻底解决了压缩包解压linux端的问题
-- 解决了win端默认gbk解码的错误
-- 解决rcon指令字体报错
-
-### 0.2.5--2022.2.10
-
-- 修复了依赖不足的bug
-- 更新了电信服战绩个人图片UI
-- 更新了批量服务器查看的UI
-- 修改了传文件为协程异步
-- 优化了部分rcon指令
-- ~tnd7z怎么不去死啊~使用pyunpack库解压7z
-
-### 0.2.4--2022.2.8
-
-- 使用poetry修复了pip安装文件缺失的bug
-
-### 0.2.3--2022.2.7
-
-- 新增坐牢和开牢
-- 修改了获取资源为异步协程却阻碍其他指令的bug
-- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）
-- 喷剂制作开摆了，推测需要c/c++环境
-- 修改抽取文案
-- 新增查询服务器状态时返回connect ip
-- 修复了服务器查询无响应的时候，因为报错无回复信息的bug
-- 个人信息重置测试代码，下个版本更新
-- 新增求生更新添加和删除
-
-### 0.2.2--2022.2.1
-
-- 新增探监
-- 新增喷漆制作
-- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）
-- 修改了部分对话响应
-
-### 0.2.1--2022.1.25
-
-- 新增电信服获取（东哥的肯定）
-- 优化图片UI
-- 新增云服快捷查询
-- 修复了因为没用玩家，导致的服务器状态查询错误
-- 新增电信服ip爬取（仅仅作为单次更新ip列表）
-
-### 0.2.0--2022.1.21
-
-- 新增创意工坊查询
-- 优化查询图片UI
-- 新增创意工坊文件下载
-- 修复了因为电信服官网前端修改导致查询失败的BUG
-
-### 0.1.7--2022.1.19
-
-- 新增群ip订阅，批量查询
-- 新增图片显示ip状态
-- 修复了因为玩家名字特殊字符导致的utf-8解码错误
-- 更新自己的第三方库VSQ==0.0.6
-
-### 0.1.6--2022.1.15
-
-- 新增ip查询服务器提供玩家数量和名字
-- 增加协程函数修复因为加载顺序导致的错误
-- 更新自己的第三方库VSQ==0.0.4
-
-### 0.1.5--2022.1.15
-
-- 新增服务器控制台指令，新增依赖rcon
-- 重新了数据库，不再使用json而是使用sql3
-- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示
-
-### 0.1.4--2022.1.9
-
-- 新增求生anne详情（看排名）
-- 所有的请求改为httpx
-- 更新了anne信息图片
-- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)
-
-### 0.1.3--2022.1.7
-
-- 新增绑定昵称和steamid
-- 新增可以艾特人查询anne成绩
-- 新增解绑信息
-
-### 0.1.2--2022.1.6
-
-- 新增支持图片输出
-- 新增查询anne服数据
-
-### 0.1.1--2022.1.5
-
-- 新增删除地图
-- 新增地图改名
-- 新增支持图片输出
-
-### 0.1.0--2022.1.4
-
-- 集中修复了Bug
-
-### 0.0.9--2022.1.4
-
-- 新增上传地图后，检测对比回复新地图名字
-- 修复中文名乱码问题
-
-### 0.0.8--2022.1.4
-
-- 支持vpk格式地图
-- 支持查看所有vpk格式文件
-
-### 0.0.6--2022.1.3
-
-- 修复了7z压缩包的方式，优化代码
-
-### 0.0.1--2022.1.3
-
-- 插件初次发布，可私聊添加地图
-
-</details>
-
-## 🙈 其他
-
-- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
-- 如果本插件对你有帮助，不要忘了点个Star~
-- 本项目仅供学习使用，请勿用于商业用途
-- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
-
-## 🌐 感谢
-
-- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架
-- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考
-- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)
-- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
-  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
-- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
-- [日向麻麻](https://github.com/Special-Week)- 代码优化参考
-- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考
-- 呆呆- 提供三方地图的详细数据
+<div align="center">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_l4d2_server
+
+_✨Nonebot & Left 4 Dead 2 server操作✨_
+<div align = "center">
+        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
+</div><br>
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">
+</a>
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
+        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
+    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
+</a>
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
+
+</div>
+
+## 顶置公告
+
+0.5.0破坏式更新，不再使用env配置，采用web控制台管理
+
+同时不再支持远程查询，改为只允许本地查询
+
+## 主要功能
+
+- 求生服务器-本地多路径操作（传地图）
+- 批量查询指定ip服务器状态和玩家
+- 创意工坊下载和喷漆制作
+- web控制台
+- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
+
+
+## 数据结构
+
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
+
+新增一个json文件，格式如下,文件名与需要响应的指令一致
+`l4d2.json`和`关键词1.json`都可以加载
+
+        {
+        "呆呆": [
+                {
+                "id": 1,
+                "version": "战役",
+                "ip": "43.248.188.17:27031"
+                },
+                {
+                "id": 2,
+                "version": "战役",
+                "ip": "43.248.188.17:27032"
+                }
+        ]
+        }
+
+## 🌐 默认服务器
+
+由于不可抗力原因，暂时不使用在线的方式获取ip，有需求可以自行添加
+以下仅供参考本人使用的查询服务器
+
+| 指令 | 服务器 | op | 数量 |
+|:-----:|:----:|:----:|:----:|
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 5
+| 云 | anne电信服云服 | 东 | 19
+| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
+| 橘 | 橘希实香的小窝 | 橘希实香 | 21
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
+| 音理 | 星空列车与白的旅行 | 音理 | 3
+| 尤 | 尤尤 | 晓音 | 3
+| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
+| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 2
+| Air | Air | Air | 15
+| 3ks | 为人民服务 | DK | 14
+| 驴头 | 驴头服 | lvt | 4
+| 尸鬼 | 尸鬼狂潮 | ❀几❀ | 7
+
+## 🔖 更新日志
+
+<details>
+<summary>展开/收起</summary>
+
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
+### 0.4.9--2022.4
+
+- 修复h11版本错误的bug
+- 重写了config，下个版本正式使用yaml替代env设置
+- 新增远程连接测试代码
+
+### 0.4.8--2022.4.16
+
+- 新增重载ip
+- 修复了一些windows启动下奇奇怪怪的bug
+
+### 0.4.7--2022.4.13
+
+- 新增模式查询
+- 列表推导替换套娃循环
+
+### 0.4.6--2022.4.9
+
+- 显示无效服
+- 优化服务器排序算法（list.sort()天下第一）
+- 默认关闭web端
+
+### 0.4.5--2022.4.9
+
+- 修bug（恼）
+
+### 0.4.2--2022.4.9
+
+- 修复响应开头匹配出现的重大bug
+- 启用web端
+- web使用yaml管理，未来可能删除env配置
+
+### 0.4.1--2022.3
+
+- 修复rar压缩包命名错误
+- 更新了tag的参数读取方式
+- 确定了传文件私聊比群聊快速
+- 修复了电信服计算错误
+
+### 0.4.0--2022.3.27
+
+- 新增web控制台
+- 修复传图超时参数错误
+- 重写求生ip获取方法 ~ 数据库苦手 ~
+- 重写文档
+- 不再内置ip（毕竟ipv4都暴露太危险了）
+
+### 0.3.7--2022.3
+
+- 新增三方下载网盘
+- 修复windows上传临时文件错误
+- 优化查服流程
+- 优化anne服随机功能
+
+### 0.3.6--2022.3.10
+
+- 暂时关闭web端，后续修改
+- 优化图片显示
+- 修复了海量bug
+- 新增三方图查询
+
+### 0.3.5--2022.3.6
+
+- 新增ping查询（在ip里包括）
+- 新增api查询（未完成）
+- 修复了电信服查询绑定名字无法查询的错误
+- 新增了救援率的显示
+- 新增web端（未完成）
+
+### 0.3.4--2022.3.1
+
+- 新增本地插件smx查询
+- 增加了三个内置群服
+- 修改了图片的UI,变好看了
+- 删减了部分图片和字体，使得轻量化
+- 修复了海量bug
+- 修复了python3.8中typing错误
+
+### 0.3.3--2022.2.26
+
+- 重写协议，使用a2s库，同时解决win端不同报错无法输出
+- 重~抄~写服务器查询UI,解决了不好看的问题
+- 从win测试，解决了一些win特有的bug
+- 重写服务器查询~还得是json~
+- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问
+- 新增批量查询服务器，不带参数则返回图片
+
+### 0.3.1--2022.2.22
+
+- 修复了路径识别为str对象的错误
+- 修复了初始化找不到文件的错误
+- 修复了路径拼接错误
+- 在win端成功测试，修复压缩包bug
+- 新增开关协程异步env设置
+- 测试rcon建立通讯
+- 实现切换路径查看地图和使用rcon指令
+
+### 0.3.0--2022.2.18
+
+- 修改了新的env配置，使得支持本地多服务器操作
+- 彻底解决了压缩包解压linux端的问题
+- 解决了win端默认gbk解码的错误
+- 解决rcon指令字体报错
+
+### 0.2.5--2022.2.10
+
+- 修复了依赖不足的bug
+- 更新了电信服战绩个人图片UI
+- 更新了批量服务器查看的UI
+- 修改了传文件为协程异步
+- 优化了部分rcon指令
+- ~tnd7z怎么不去死啊~使用pyunpack库解压7z
+
+### 0.2.4--2022.2.8
+
+- 使用poetry修复了pip安装文件缺失的bug
+
+### 0.2.3--2022.2.7
+
+- 新增坐牢和开牢
+- 修改了获取资源为异步协程却阻碍其他指令的bug
+- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）
+- 喷剂制作开摆了，推测需要c/c++环境
+- 修改抽取文案
+- 新增查询服务器状态时返回connect ip
+- 修复了服务器查询无响应的时候，因为报错无回复信息的bug
+- 个人信息重置测试代码，下个版本更新
+- 新增求生更新添加和删除
+
+### 0.2.2--2022.2.1
+
+- 新增探监
+- 新增喷漆制作
+- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）
+- 修改了部分对话响应
+
+### 0.2.1--2022.1.25
+
+- 新增电信服获取（东哥的肯定）
+- 优化图片UI
+- 新增云服快捷查询
+- 修复了因为没用玩家，导致的服务器状态查询错误
+- 新增电信服ip爬取（仅仅作为单次更新ip列表）
+
+### 0.2.0--2022.1.21
+
+- 新增创意工坊查询
+- 优化查询图片UI
+- 新增创意工坊文件下载
+- 修复了因为电信服官网前端修改导致查询失败的BUG
+
+### 0.1.7--2022.1.19
+
+- 新增群ip订阅，批量查询
+- 新增图片显示ip状态
+- 修复了因为玩家名字特殊字符导致的utf-8解码错误
+- 更新自己的第三方库VSQ==0.0.6
+
+### 0.1.6--2022.1.15
+
+- 新增ip查询服务器提供玩家数量和名字
+- 增加协程函数修复因为加载顺序导致的错误
+- 更新自己的第三方库VSQ==0.0.4
+
+### 0.1.5--2022.1.15
+
+- 新增服务器控制台指令，新增依赖rcon
+- 重新了数据库，不再使用json而是使用sql3
+- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示
+
+### 0.1.4--2022.1.9
+
+- 新增求生anne详情（看排名）
+- 所有的请求改为httpx
+- 更新了anne信息图片
+- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)
+
+### 0.1.3--2022.1.7
+
+- 新增绑定昵称和steamid
+- 新增可以艾特人查询anne成绩
+- 新增解绑信息
+
+### 0.1.2--2022.1.6
+
+- 新增支持图片输出
+- 新增查询anne服数据
+
+### 0.1.1--2022.1.5
+
+- 新增删除地图
+- 新增地图改名
+- 新增支持图片输出
+
+### 0.1.0--2022.1.4
+
+- 集中修复了Bug
+
+### 0.0.9--2022.1.4
+
+- 新增上传地图后，检测对比回复新地图名字
+- 修复中文名乱码问题
+
+### 0.0.8--2022.1.4
+
+- 支持vpk格式地图
+- 支持查看所有vpk格式文件
+
+### 0.0.6--2022.1.3
+
+- 修复了7z压缩包的方式，优化代码
+
+### 0.0.1--2022.1.3
+
+- 插件初次发布，可私聊添加地图
+
+</details>
+
+## 🙈 其他
+
+- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
+- 如果本插件对你有帮助，不要忘了点个Star~
+- 本项目仅供学习使用，请勿用于商业用途
+- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
+
+## 🌐 感谢
+
+- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架
+- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考
+- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)
+- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
+  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
+- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
+- [日向麻麻](https://github.com/Special-Week)- 代码优化参考
+- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考
+- 呆呆- 提供三方地图的详细数据
 - ArcPav -积极反馈bug，提供改进思路
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
    # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
-## ä¸»è¦åè½ - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
+## é¡¶ç½®å¬å
+0.5.0ç ´åå¼æ´æ°ï¼ä¸åä½¿ç¨envéç½®ï¼éç¨webæ§å¶å°ç®¡ç
+åæ¶ä¸åæ¯æè¿ç¨æ¥è¯¢ï¼æ¹ä¸ºåªåè®¸æ¬å°æ¥è¯¢ ## ä¸»è¦åè½ -
+æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
-åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
-fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt ä¸¾ä¾ï¼
-âââ data âââ L4D2 âââ l4d2.yml âââ l4d2.json âââ
-sql â âââ L4D2.db âââ image â âââ players â âââ
-... âââ l4d2 âââ å³é®è¯1.json âââ å³é®è¯2.json
-âââ ... ... ```
+åæå·¥åä¸è½½åå·æ¼å¶ä½ - webæ§å¶å° - [æ±ççµä¿¡æanne](https:
+//github.com/fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/
+l4d_stats/ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt
+ä¸¾ä¾ï¼ âââ data âââ L4D2 âââ l4d2.yml âââ l4d2.json
+âââ sql â âââ L4D2.db âââ image â âââ players â
+âââ ... âââ l4d2 âââ å³é®è¯1.json âââ
+å³é®è¯2.json âââ ... ... ```
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 `l4d2.json`å`å³é®è¯1.json`é½å¯ä»¥å è½½ { "åå": [ { "id": 1,
 "version": "æå½¹", "ip": "43.248.188.17:27031" }, { "id": 2, "version":
 "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð é»è®¤æå¡å¨
 ç±äºä¸å¯æååå ï¼ææ¶ä¸ä½¿ç¨å¨çº¿çæ¹å¼è·åipï¼æéæ±å¯ä»¥èªè¡æ·»å 
 ä»¥ä¸ä»ä¾åèæ¬äººä½¿ç¨çæ¥è¯¢æå¡å¨ | æä»¤ | æå¡å¨ | op |
 æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  | ç±ä¸½æ°ç æ³è¦æ¶©æ¶© |
```

### Comparing `nonebot_plugin_l4d2_server-0.5.1/setup.py` & `nonebot_plugin_l4d2_server-0.5.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,413 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-l4d2-server
+Version: 0.5.2
+Summary: L4D2 server related operations plugin for NoneBot2
+Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+License: GPLv3
+Keywords: steam,game,l4d2,nonebot2,plugin
+Author: Agnes_Digital
+Author-email: Z735803792@163.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: amis-python (>=1.0.6,<2.0.0)
+Requires-Dist: asyncio (>=3.4.3)
+Requires-Dist: beautifulsoup4 (>=4.8.0)
+Requires-Dist: h11 (>=0.14.0,<0.15.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: jieba (>=0.42.1,<0.43.0)
+Requires-Dist: jinja2 (>=3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
+Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
+Requires-Dist: nonebot_plugin_txt2img (>=0.3.0)
+Requires-Dist: pandas (>=1.5.2)
+Requires-Dist: patool (>=1.12,<2.0)
+Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Requires-Dist: python-a2s (>=1.3.0,<2.0.0)
+Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: pyunpack (>=0.3.0,<0.4.0)
+Requires-Dist: rarfile (>=4.0,<5.0)
+Requires-Dist: rcon (>=2.1.0,<3.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: srctools (>=2.3.9,<3.0.0)
+Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_l4d2_server',
- 'nonebot_plugin_l4d2_server.l4d2_anne',
- 'nonebot_plugin_l4d2_server.l4d2_data',
- 'nonebot_plugin_l4d2_server.l4d2_file',
- 'nonebot_plugin_l4d2_server.l4d2_image',
- 'nonebot_plugin_l4d2_server.l4d2_queries',
- 'nonebot_plugin_l4d2_server.l4d2_server',
- 'nonebot_plugin_l4d2_server.l4d2_web']
-
-package_data = \
-{'': ['*'],
- 'nonebot_plugin_l4d2_server': ['data/L4D2/image/head/*',
-                                'data/L4D2/image/header/*',
-                                'data/L4D2/image/template/*']}
-
-install_requires = \
-['aiohttp>=3.8.3,<4.0.0',
- 'amis-python>=1.0.6,<2.0.0',
- 'asyncio>=3.4.3',
- 'beautifulsoup4>=4.8.0',
- 'h11>=0.14.0,<0.15.0',
- 'httpx>=0.23.3,<0.24.0',
- 'jieba>=0.42.1,<0.43.0',
- 'jinja2>=3.0.0',
- 'nonebot-adapter-onebot>=2.1.5',
- 'nonebot2>=2.0.0rc4,<3.0.0',
- 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
- 'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0',
- 'nonebot_plugin_txt2img>=0.3.0',
- 'pandas>=1.5.2',
- 'patool>=1.12,<2.0',
- 'pillow>=9.3.0,<10.0.0',
- 'python-a2s>=1.3.0,<2.0.0',
- 'python-jose>=3.3.0,<4.0.0',
- 'pyunpack>=0.3.0,<0.4.0',
- 'rarfile>=4.0,<5.0',
- 'rcon>=2.1.0,<3.0.0',
- 'ruamel.yaml>=0.17.21,<0.18.0',
- 'srctools>=2.3.9,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-l4d2-server',
-    'version': '0.5.1',
-    'description': 'L4D2 server related operations plugin for NoneBot2',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n\n</div>\n\n\n\n## 主要功能\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n## 数据结构\n\nbot所在文件夹下\n```txt\n举例：\n└── data\n    └── L4D2\n        ├── l4d2.yml\n        ├── l4d2.json\n        ├── sql\n        │   └── L4D2.db\n        ├── image\n        │   └── players\n        │       └── ...\n        └── l4d2\n            ├── 关键词1.json\n            ├── 关键词2.json\n            └── ...\n...\n```\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n`l4d2.json`和`关键词1.json`都可以加载\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                },\n                {\n                "id": 2,\n                "version": "战役",\n                "ip": "43.248.188.17:27032"\n                }\n        ]\n        }\n\n## 🌐 默认服务器\n\n由于不可抗力原因，暂时不使用在线的方式获取ip，有需求可以自行添加\n以下仅供参考本人使用的查询服务器\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 5\n| 云 | anne电信服云服 | 东 | 19\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15\n| 橘 | 橘希实香的小窝 | 橘希实香 | 21\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 2\n| Air | Air | Air | 15\n| 3ks | 为人民服务 | DK | 14\n| 驴头 | 驴头服 | lvt | 4\n| 尸鬼 | 尸鬼狂潮 | ❀几❀ | 7\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.5.1--2022.5.01\n\n- 解决了main和dev分支的一个严重bug（也许没解决\n- 本地化，更好的添加,删除远程分支\n- 服务器忘了备份，尽力抢救了数据了\n\n### 0.5.0--2022.4.28\n\n- 重构config，并弃用env设置\n- 使用网页控制台来控制配置\n- 新增了很多不会报错的bug\n\n### 0.4.9--2022.4\n\n- 修复h11版本错误的bug\n- 重写了config，下个版本正式使用yaml替代env设置\n- 新增远程连接测试代码\n\n### 0.4.8--2022.4.16\n\n- 新增重载ip\n- 修复了一些windows启动下奇奇怪怪的bug\n\n### 0.4.7--2022.4.13\n\n- 新增模式查询\n- 列表推导替换套娃循环\n\n### 0.4.6--2022.4.9\n\n- 显示无效服\n- 优化服务器排序算法（list.sort()天下第一）\n- 默认关闭web端\n\n### 0.4.5--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n- 修复响应开头匹配出现的重大bug\n- 启用web端\n- web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n- 修复rar压缩包命名错误\n- 更新了tag的参数读取方式\n- 确定了传文件私聊比群聊快速\n- 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n- 新增web控制台\n- 修复传图超时参数错误\n- 重写求生ip获取方法 ~ 数据库苦手 ~\n- 重写文档\n- 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n- 新增三方下载网盘\n- 修复windows上传临时文件错误\n- 优化查服流程\n- 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n- 暂时关闭web端，后续修改\n- 优化图片显示\n- 修复了海量bug\n- 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n- 新增ping查询（在ip里包括）\n- 新增api查询（未完成）\n- 修复了电信服查询绑定名字无法查询的错误\n- 新增了救援率的显示\n- 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n- 新增本地插件smx查询\n- 增加了三个内置群服\n- 修改了图片的UI,变好看了\n- 删减了部分图片和字体，使得轻量化\n- 修复了海量bug\n- 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n- 重写协议，使用a2s库，同时解决win端不同报错无法输出\n- 重~抄~写服务器查询UI,解决了不好看的问题\n- 从win测试，解决了一些win特有的bug\n- 重写服务器查询~还得是json~\n- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n- 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n- 修复了路径识别为str对象的错误\n- 修复了初始化找不到文件的错误\n- 修复了路径拼接错误\n- 在win端成功测试，修复压缩包bug\n- 新增开关协程异步env设置\n- 测试rcon建立通讯\n- 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n- 修改了新的env配置，使得支持本地多服务器操作\n- 彻底解决了压缩包解压linux端的问题\n- 解决了win端默认gbk解码的错误\n- 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n- 修复了依赖不足的bug\n- 更新了电信服战绩个人图片UI\n- 更新了批量服务器查看的UI\n- 修改了传文件为协程异步\n- 优化了部分rcon指令\n- ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n- 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n- 新增坐牢和开牢\n- 修改了获取资源为异步协程却阻碍其他指令的bug\n- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n- 喷剂制作开摆了，推测需要c/c++环境\n- 修改抽取文案\n- 新增查询服务器状态时返回connect ip\n- 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n- 个人信息重置测试代码，下个版本更新\n- 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n- 新增探监\n- 新增喷漆制作\n- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n- 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n- 新增电信服获取（东哥的肯定）\n- 优化图片UI\n- 新增云服快捷查询\n- 修复了因为没用玩家，导致的服务器状态查询错误\n- 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n- 新增创意工坊查询\n- 优化查询图片UI\n- 新增创意工坊文件下载\n- 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n- 新增群ip订阅，批量查询\n- 新增图片显示ip状态\n- 修复了因为玩家名字特殊字符导致的utf-8解码错误\n- 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n- 新增ip查询服务器提供玩家数量和名字\n- 增加协程函数修复因为加载顺序导致的错误\n- 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n- 如果本插件对你有帮助，不要忘了点个Star~\n- 本项目仅供学习使用，请勿用于商业用途\n- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n\n## 🌐 感谢\n\n- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考\n- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)\n- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考\n- [日向麻麻](https://github.com/Special-Week)- 代码优化参考\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考\n- 呆呆- 提供三方地图的详细数据\n- ArcPav -积极反馈bug，提供改进思路',
-    'author': 'Agnes_Digital',
-    'author_email': 'Z735803792@163.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+<div align="center">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
 
+<div align="center">
 
-setup(**setup_kwargs)
+# nonebot_plugin_l4d2_server
+
+_✨Nonebot & Left 4 Dead 2 server操作✨_
+<div align = "center">
+        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
+</div><br>
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">
+</a>
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
+        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
+    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
+</a>
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
+
+</div>
+
+## 顶置公告
+
+0.5.0破坏式更新，不再使用env配置，采用web控制台管理
+
+同时不再支持远程查询，改为只允许本地查询
+
+## 主要功能
+
+- 求生服务器-本地多路径操作（传地图）
+- 批量查询指定ip服务器状态和玩家
+- 创意工坊下载和喷漆制作
+- web控制台
+- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
+
+
+## 数据结构
+
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
+
+新增一个json文件，格式如下,文件名与需要响应的指令一致
+`l4d2.json`和`关键词1.json`都可以加载
+
+        {
+        "呆呆": [
+                {
+                "id": 1,
+                "version": "战役",
+                "ip": "43.248.188.17:27031"
+                },
+                {
+                "id": 2,
+                "version": "战役",
+                "ip": "43.248.188.17:27032"
+                }
+        ]
+        }
+
+## 🌐 默认服务器
+
+由于不可抗力原因，暂时不使用在线的方式获取ip，有需求可以自行添加
+以下仅供参考本人使用的查询服务器
+
+| 指令 | 服务器 | op | 数量 |
+|:-----:|:----:|:----:|:----:|
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 5
+| 云 | anne电信服云服 | 东 | 19
+| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
+| 橘 | 橘希实香的小窝 | 橘希实香 | 21
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
+| 音理 | 星空列车与白的旅行 | 音理 | 3
+| 尤 | 尤尤 | 晓音 | 3
+| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
+| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 2
+| Air | Air | Air | 15
+| 3ks | 为人民服务 | DK | 14
+| 驴头 | 驴头服 | lvt | 4
+| 尸鬼 | 尸鬼狂潮 | ❀几❀ | 7
+
+## 🔖 更新日志
+
+<details>
+<summary>展开/收起</summary>
+
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
+### 0.4.9--2022.4
+
+- 修复h11版本错误的bug
+- 重写了config，下个版本正式使用yaml替代env设置
+- 新增远程连接测试代码
+
+### 0.4.8--2022.4.16
+
+- 新增重载ip
+- 修复了一些windows启动下奇奇怪怪的bug
+
+### 0.4.7--2022.4.13
+
+- 新增模式查询
+- 列表推导替换套娃循环
+
+### 0.4.6--2022.4.9
+
+- 显示无效服
+- 优化服务器排序算法（list.sort()天下第一）
+- 默认关闭web端
+
+### 0.4.5--2022.4.9
+
+- 修bug（恼）
+
+### 0.4.2--2022.4.9
+
+- 修复响应开头匹配出现的重大bug
+- 启用web端
+- web使用yaml管理，未来可能删除env配置
+
+### 0.4.1--2022.3
+
+- 修复rar压缩包命名错误
+- 更新了tag的参数读取方式
+- 确定了传文件私聊比群聊快速
+- 修复了电信服计算错误
+
+### 0.4.0--2022.3.27
+
+- 新增web控制台
+- 修复传图超时参数错误
+- 重写求生ip获取方法 ~ 数据库苦手 ~
+- 重写文档
+- 不再内置ip（毕竟ipv4都暴露太危险了）
+
+### 0.3.7--2022.3
+
+- 新增三方下载网盘
+- 修复windows上传临时文件错误
+- 优化查服流程
+- 优化anne服随机功能
+
+### 0.3.6--2022.3.10
+
+- 暂时关闭web端，后续修改
+- 优化图片显示
+- 修复了海量bug
+- 新增三方图查询
+
+### 0.3.5--2022.3.6
+
+- 新增ping查询（在ip里包括）
+- 新增api查询（未完成）
+- 修复了电信服查询绑定名字无法查询的错误
+- 新增了救援率的显示
+- 新增web端（未完成）
+
+### 0.3.4--2022.3.1
+
+- 新增本地插件smx查询
+- 增加了三个内置群服
+- 修改了图片的UI,变好看了
+- 删减了部分图片和字体，使得轻量化
+- 修复了海量bug
+- 修复了python3.8中typing错误
+
+### 0.3.3--2022.2.26
+
+- 重写协议，使用a2s库，同时解决win端不同报错无法输出
+- 重~抄~写服务器查询UI,解决了不好看的问题
+- 从win测试，解决了一些win特有的bug
+- 重写服务器查询~还得是json~
+- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问
+- 新增批量查询服务器，不带参数则返回图片
+
+### 0.3.1--2022.2.22
+
+- 修复了路径识别为str对象的错误
+- 修复了初始化找不到文件的错误
+- 修复了路径拼接错误
+- 在win端成功测试，修复压缩包bug
+- 新增开关协程异步env设置
+- 测试rcon建立通讯
+- 实现切换路径查看地图和使用rcon指令
+
+### 0.3.0--2022.2.18
+
+- 修改了新的env配置，使得支持本地多服务器操作
+- 彻底解决了压缩包解压linux端的问题
+- 解决了win端默认gbk解码的错误
+- 解决rcon指令字体报错
+
+### 0.2.5--2022.2.10
+
+- 修复了依赖不足的bug
+- 更新了电信服战绩个人图片UI
+- 更新了批量服务器查看的UI
+- 修改了传文件为协程异步
+- 优化了部分rcon指令
+- ~tnd7z怎么不去死啊~使用pyunpack库解压7z
+
+### 0.2.4--2022.2.8
+
+- 使用poetry修复了pip安装文件缺失的bug
+
+### 0.2.3--2022.2.7
+
+- 新增坐牢和开牢
+- 修改了获取资源为异步协程却阻碍其他指令的bug
+- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）
+- 喷剂制作开摆了，推测需要c/c++环境
+- 修改抽取文案
+- 新增查询服务器状态时返回connect ip
+- 修复了服务器查询无响应的时候，因为报错无回复信息的bug
+- 个人信息重置测试代码，下个版本更新
+- 新增求生更新添加和删除
+
+### 0.2.2--2022.2.1
+
+- 新增探监
+- 新增喷漆制作
+- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）
+- 修改了部分对话响应
+
+### 0.2.1--2022.1.25
+
+- 新增电信服获取（东哥的肯定）
+- 优化图片UI
+- 新增云服快捷查询
+- 修复了因为没用玩家，导致的服务器状态查询错误
+- 新增电信服ip爬取（仅仅作为单次更新ip列表）
+
+### 0.2.0--2022.1.21
+
+- 新增创意工坊查询
+- 优化查询图片UI
+- 新增创意工坊文件下载
+- 修复了因为电信服官网前端修改导致查询失败的BUG
+
+### 0.1.7--2022.1.19
+
+- 新增群ip订阅，批量查询
+- 新增图片显示ip状态
+- 修复了因为玩家名字特殊字符导致的utf-8解码错误
+- 更新自己的第三方库VSQ==0.0.6
+
+### 0.1.6--2022.1.15
+
+- 新增ip查询服务器提供玩家数量和名字
+- 增加协程函数修复因为加载顺序导致的错误
+- 更新自己的第三方库VSQ==0.0.4
+
+### 0.1.5--2022.1.15
+
+- 新增服务器控制台指令，新增依赖rcon
+- 重新了数据库，不再使用json而是使用sql3
+- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示
+
+### 0.1.4--2022.1.9
+
+- 新增求生anne详情（看排名）
+- 所有的请求改为httpx
+- 更新了anne信息图片
+- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)
+
+### 0.1.3--2022.1.7
+
+- 新增绑定昵称和steamid
+- 新增可以艾特人查询anne成绩
+- 新增解绑信息
+
+### 0.1.2--2022.1.6
+
+- 新增支持图片输出
+- 新增查询anne服数据
+
+### 0.1.1--2022.1.5
+
+- 新增删除地图
+- 新增地图改名
+- 新增支持图片输出
+
+### 0.1.0--2022.1.4
+
+- 集中修复了Bug
+
+### 0.0.9--2022.1.4
+
+- 新增上传地图后，检测对比回复新地图名字
+- 修复中文名乱码问题
+
+### 0.0.8--2022.1.4
+
+- 支持vpk格式地图
+- 支持查看所有vpk格式文件
+
+### 0.0.6--2022.1.3
+
+- 修复了7z压缩包的方式，优化代码
+
+### 0.0.1--2022.1.3
+
+- 插件初次发布，可私聊添加地图
+
+</details>
+
+## 🙈 其他
+
+- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
+- 如果本插件对你有帮助，不要忘了点个Star~
+- 本项目仅供学习使用，请勿用于商业用途
+- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
+
+## 🌐 感谢
+
+- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架
+- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考
+- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)
+- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
+  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
+- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
+- [日向麻麻](https://github.com/Special-Week)- 代码优化参考
+- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考
+- 呆呆- 提供三方地图的详细数据
+- ArcPav -积极反馈bug，提供改进思路
```

#### html2text {}

```diff
@@ -1,173 +1,167 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_l4d2_server', 'nonebot_plugin_l4d2_server.l4d2_anne',
-'nonebot_plugin_l4d2_server.l4d2_data', 'nonebot_plugin_l4d2_server.l4d2_file',
-'nonebot_plugin_l4d2_server.l4d2_image',
-'nonebot_plugin_l4d2_server.l4d2_queries',
-'nonebot_plugin_l4d2_server.l4d2_server',
-'nonebot_plugin_l4d2_server.l4d2_web'] package_data = \ {'': ['*'],
-'nonebot_plugin_l4d2_server': ['data/L4D2/image/head/*', 'data/L4D2/image/
-header/*', 'data/L4D2/image/template/*']} install_requires = \
-['aiohttp>=3.8.3,<4.0.0', 'amis-python>=1.0.6,<2.0.0', 'asyncio>=3.4.3',
-'beautifulsoup4>=4.8.0', 'h11>=0.14.0,<0.15.0', 'httpx>=0.23.3,<0.24.0',
-'jieba>=0.42.1,<0.43.0', 'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5',
-'nonebot2>=2.0.0rc4,<3.0.0', 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
-'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0', 'nonebot_plugin_txt2img>=0.3.0',
-'pandas>=1.5.2', 'patool>=1.12,<2.0', 'pillow>=9.3.0,<10.0.0', 'python-
-a2s>=1.3.0,<2.0.0', 'python-jose>=3.3.0,<4.0.0', 'pyunpack>=0.3.0,<0.4.0',
-'rarfile>=4.0,<5.0', 'rcon>=2.1.0,<3.0.0', 'ruamel.yaml>=0.17.21,<0.18.0',
-'srctools>=2.3.9,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-l4d2-
-server', 'version': '0.5.1', 'description': 'L4D2 server related operations
-plugin for NoneBot2', 'long_description': '
-                           \n [AgnesDigitalLogo]\n
-                                      \n
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.2 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
+github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
+steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
+Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
+Proprietary License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Requires-Dist: aiohttp
+(>=3.8.3,<4.0.0) Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist:
+asyncio (>=3.4.3) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist: h11
+(>=0.14.0,<0.15.0) Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: jieba
+(>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-
+Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
+nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
+patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Requires-Dist:
+python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0)
+Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml
+(>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0) Project-URL:
+Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server Description-
+Content-Type: text/markdown
+                              [AgnesDigitalLogo]
                               [NoneBotPluginText]
-                                      \n
-\n\n
-        \n\n# nonebot_plugin_l4d2_server\n\n_â¨Nonebot & Left 4 Dead 2
-                              serveræä½â¨_\n
-            \n ææ¡£   Â·  \n æä»¤åè¡¨   Â·  \n å¸¸è§é®é¢\n
+   # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
+                ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
-    \n\n_[GitHub_stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n\n_
-           [pypi]\n\n\n_[pypi_download]\n\n [python]\n [NoneBot]\n\n
-\n\n\n\n## ä¸»è¦åè½\n\n- æ±çæå¡å¨-
-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼\n-
-æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶\n-
-åæå·¥åä¸è½½åå·æ¼å¶ä½\n- [æ±ççµä¿¡æanne](https://github.com/
-fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php)\n\n\n##
-æ°æ®ç»æ\n\nbotæå¨æä»¶å¤¹ä¸\n```txt\nä¸¾ä¾ï¼\nâââ data\n
-âââ L4D2\n âââ l4d2.yml\n âââ l4d2.json\n âââ sql\n â
-âââ L4D2.db\n âââ image\n â âââ players\n â âââ
-...\n âââ l4d2\n âââ å³é®è¯1.json\n âââ å³é®è¯2.json\n
-âââ
-...\n...\n```\n\næ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´\n`l4d2.json`å`å³é®è¯1.json`é½å¯ä»¥å è½½\n\n
-{\n "åå": [\n {\n "id": 1,\n "version": "æå½¹",\n "ip": "43.248.188.17:
-27031"\n },\n {\n "id": 2,\n "version": "æå½¹",\n "ip": "43.248.188.17:
-27032"\n }\n ]\n }\n\n## ð
-é»è®¤æå¡å¨\n\nç±äºä¸å¯æååå ï¼ææ¶ä¸ä½¿ç¨å¨çº¿çæ¹å¼è·åipï¼æéæ±å¯ä»¥èªè¡æ·»å \nä»¥ä¸ä»ä¾åèæ¬äººä½¿ç¨çæ¥è¯¢æå¡å¨\n\n|
-æä»¤ | æå¡å¨ | op | æ°é |\n|:-----:|:----:|:----:|:----:|\n| æ°ç  |
-ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 5\n| äº | anneçµä¿¡æäºæ | ä¸
-| 19\n| åå | ååçå°çª | æè«å¤§é­ç | 15\n| æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 21\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
-| 21\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
-æé³ | 3\n| é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3\n| ææ |
-ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 2\n| Air | Air | Air |
-15\n| 3ks | ä¸ºäººæ°æå¡ | DK | 14\n| é©´å¤´ | é©´å¤´æ | lvt | 4\n| å°¸é¬¼
-| å°¸é¬¼çæ½® | âå â | 7\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
-æ¶èµ·\n\n### 0.5.1--2022.5.01\n\n-
-è§£å³äºmainådevåæ¯çä¸ä¸ªä¸¥ébugï¼ä¹è®¸æ²¡è§£å³\n-
-æ¬å°åï¼æ´å¥½çæ·»å ,å é¤è¿ç¨åæ¯\n-
-æå¡å¨å¿äºå¤ä»½ï¼å°½åæ¢æäºæ°æ®äº\n\n### 0.5.0--2022.4.28\n\n-
-éæconfigï¼å¹¶å¼ç¨envè®¾ç½®\n- ä½¿ç¨ç½é¡µæ§å¶å°æ¥æ§å¶éç½®\n-
-æ°å¢äºå¾å¤ä¸ä¼æ¥éçbug\n\n### 0.4.9--2022.4\n\n-
-ä¿®å¤h11çæ¬éè¯¯çbug\n-
-éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½®\n-
-æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç \n\n### 0.4.8--2022.4.16\n\n- æ°å¢éè½½ip\n-
-ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug\n\n### 0.4.7--2022.4.13\n\n-
-æ°å¢æ¨¡å¼æ¥è¯¢\n- åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯\n\n### 0.4.6--
-2022.4.9\n\n- æ¾ç¤ºæ ææ\n- ä¼åæå¡å¨æåºç®æ³ï¼list.sort
-()å¤©ä¸ç¬¬ä¸ï¼\n- é»è®¤å³é­webç«¯\n\n### 0.4.5--2022.4.9\n\n-
-ä¿®bugï¼æ¼ï¼\n\n### 0.4.2--2022.4.9\n\n-
-ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n- å¯ç¨webç«¯\n-
-webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½®\n\n### 0.4.1--2022.3\n\n-
-ä¿®å¤raråç¼©åå½åéè¯¯\n- æ´æ°äºtagçåæ°è¯»åæ¹å¼\n-
-ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é\n-
-ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯\n\n### 0.4.0--2022.3.27\n\n-
-æ°å¢webæ§å¶å°\n- ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯\n-
-éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~\n- éåææ¡£\n-
-ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼\n\n### 0.3.7--2022.3\n\n-
-æ°å¢ä¸æ¹ä¸è½½ç½ç\n- ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯\n-
-ä¼åæ¥ææµç¨\n- ä¼åanneæéæºåè½\n\n### 0.3.6--2022.3.10\n\n-
-ææ¶å³é­webç«¯ï¼åç»­ä¿®æ¹\n- ä¼åå¾çæ¾ç¤º\n-
-ä¿®å¤äºæµ·ébug\n- æ°å¢ä¸æ¹å¾æ¥è¯¢\n\n### 0.3.5--2022.3.6\n\n-
-æ°å¢pingæ¥è¯¢ï¼å¨ipéåæ¬ï¼\n- æ°å¢apiæ¥è¯¢ï¼æªå®æï¼\n-
-ä¿®å¤äºçµä¿¡ææ¥è¯¢ç»å®åå­æ æ³æ¥è¯¢çéè¯¯\n-
-æ°å¢äºææ´ççæ¾ç¤º\n- æ°å¢webç«¯ï¼æªå®æï¼\n\n### 0.3.4--
-2022.3.1\n\n- æ°å¢æ¬å°æä»¶smxæ¥è¯¢\n- å¢å äºä¸ä¸ªåç½®ç¾¤æ\n-
-ä¿®æ¹äºå¾ççUI,åå¥½çäº\n-
-å åäºé¨åå¾çåå­ä½ï¼ä½¿å¾è½»éå\n- ä¿®å¤äºæµ·ébug\n-
-ä¿®å¤äºpython3.8ä¸­typingéè¯¯\n\n### 0.3.3--2022.2.26\n\n-
-éååè®®ï¼ä½¿ç¨a2såºï¼åæ¶è§£å³winç«¯ä¸åæ¥éæ æ³è¾åº\n-
-é~æ~åæå¡å¨æ¥è¯¢UI,è§£å³äºä¸å¥½ççé®é¢\n-
-ä»winæµè¯ï¼è§£å³äºä¸äºwinç¹æçbug\n-
-éåæå¡å¨æ¥è¯¢~è¿å¾æ¯json~\n-
+[GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
+                                   [NoneBot]
+## é¡¶ç½®å¬å
+0.5.0ç ´åå¼æ´æ°ï¼ä¸åä½¿ç¨envéç½®ï¼éç¨webæ§å¶å°ç®¡ç
+åæ¶ä¸åæ¯æè¿ç¨æ¥è¯¢ï¼æ¹ä¸ºåªåè®¸æ¬å°æ¥è¯¢ ## ä¸»è¦åè½ -
+æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
+æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
+åæå·¥åä¸è½½åå·æ¼å¶ä½ - webæ§å¶å° - [æ±ççµä¿¡æanne](https:
+//github.com/fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/
+l4d_stats/ranking/index.php) ## æ°æ®ç»æ botæå¨æä»¶å¤¹ä¸ ```txt
+ä¸¾ä¾ï¼ âââ data âââ L4D2 âââ l4d2.yml âââ l4d2.json
+âââ sql â âââ L4D2.db âââ image â âââ players â
+âââ ... âââ l4d2 âââ å³é®è¯1.json âââ
+å³é®è¯2.json âââ ... ... ```
+æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
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
+éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½® -
+æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç  ### 0.4.8--2022.4.16 - æ°å¢éè½½ip -
+ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug ### 0.4.7--2022.4.13 -
+æ°å¢æ¨¡å¼æ¥è¯¢ - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯ ### 0.4.6--2022.4.9 -
+æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort()å¤©ä¸ç¬¬ä¸ï¼ -
+é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼ ### 0.4.2--2022.4.9 -
+ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
+webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
+ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
+ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
+0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
+éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~ - éåææ¡£ -
+ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼ ### 0.3.7--2022.3 -
+æ°å¢ä¸æ¹ä¸è½½ç½ç - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯ -
+ä¼åæ¥ææµç¨ - ä¼åanneæéæºåè½ ### 0.3.6--2022.3.10 -
+ææ¶å³é­webç«¯ï¼åç»­ä¿®æ¹ - ä¼åå¾çæ¾ç¤º - ä¿®å¤äºæµ·ébug -
+æ°å¢ä¸æ¹å¾æ¥è¯¢ ### 0.3.5--2022.3.6 -
+æ°å¢pingæ¥è¯¢ï¼å¨ipéåæ¬ï¼ - æ°å¢apiæ¥è¯¢ï¼æªå®æï¼ -
+ä¿®å¤äºçµä¿¡ææ¥è¯¢ç»å®åå­æ æ³æ¥è¯¢çéè¯¯ -
+æ°å¢äºææ´ççæ¾ç¤º - æ°å¢webç«¯ï¼æªå®æï¼ ### 0.3.4--2022.3.1 -
+æ°å¢æ¬å°æä»¶smxæ¥è¯¢ - å¢å äºä¸ä¸ªåç½®ç¾¤æ -
+ä¿®æ¹äºå¾ççUI,åå¥½çäº -
+å åäºé¨åå¾çåå­ä½ï¼ä½¿å¾è½»éå - ä¿®å¤äºæµ·ébug -
+ä¿®å¤äºpython3.8ä¸­typingéè¯¯ ### 0.3.3--2022.2.26 -
+éååè®®ï¼ä½¿ç¨a2såºï¼åæ¶è§£å³winç«¯ä¸åæ¥éæ æ³è¾åº -
+é~æ~åæå¡å¨æ¥è¯¢UI,è§£å³äºä¸å¥½ççé®é¢ -
+ä»winæµè¯ï¼è§£å³äºä¸äºwinç¹æçbug -
+éåæå¡å¨æ¥è¯¢~è¿å¾æ¯json~ -
 åç½®æå¡å¨æ¥è¯¢ç³»ç»ï¼å¯ä»¥éè¿[æå¡å¨ç®ç§°]+[number]/
-[æ¨¡å¼]æ¥è®¿é®\n-
-æ°å¢æ¹éæ¥è¯¢æå¡å¨ï¼ä¸å¸¦åæ°åè¿åå¾ç\n\n### 0.3.1--
-2022.2.22\n\n- ä¿®å¤äºè·¯å¾è¯å«ä¸ºstrå¯¹è±¡çéè¯¯\n-
-ä¿®å¤äºåå§åæ¾ä¸å°æä»¶çéè¯¯\n- ä¿®å¤äºè·¯å¾æ¼æ¥éè¯¯\n-
-å¨winç«¯æåæµè¯ï¼ä¿®å¤åç¼©åbug\n-
-æ°å¢å¼å³åç¨å¼æ­¥envè®¾ç½®\n- æµè¯rconå»ºç«éè®¯\n-
-å®ç°åæ¢è·¯å¾æ¥çå°å¾åä½¿ç¨rconæä»¤\n\n### 0.3.0--2022.2.18\n\n-
-ä¿®æ¹äºæ°çenvéç½®ï¼ä½¿å¾æ¯ææ¬å°å¤æå¡å¨æä½\n-
-å½»åºè§£å³äºåç¼©åè§£ålinuxç«¯çé®é¢\n-
-è§£å³äºwinç«¯é»è®¤gbkè§£ç çéè¯¯\n- è§£å³rconæä»¤å­ä½æ¥é\n\n###
-0.2.5--2022.2.10\n\n- ä¿®å¤äºä¾èµä¸è¶³çbug\n-
-æ´æ°äºçµä¿¡ææç»©ä¸ªäººå¾çUI\n-
-æ´æ°äºæ¹éæå¡å¨æ¥ççUI\n- ä¿®æ¹äºä¼ æä»¶ä¸ºåç¨å¼æ­¥\n-
-ä¼åäºé¨årconæä»¤\n-
-~tnd7zæä¹ä¸å»æ­»å~ä½¿ç¨pyunpackåºè§£å7z\n\n### 0.2.4--2022.2.8\n\n-
-ä½¿ç¨poetryä¿®å¤äºpipå®è£æä»¶ç¼ºå¤±çbug\n\n### 0.2.3--2022.2.7\n\n-
-æ°å¢åç¢åå¼ç¢\n-
-ä¿®æ¹äºè·åèµæºä¸ºå¼æ­¥åç¨å´é»ç¢å¶ä»æä»¤çbug\n-
-æ°å¢jsonç»è®¡é¨åå·²ç¥æå¡å¨ï¼æªæ¥åºè¯¥ç¬ç«æåºæç»­æ´æ°ï¼å¦æææ¨çéå¬å¼æè®°å½è¯·èç³»æå é¤ï¼\n-
-å·åå¶ä½å¼æäºï¼æ¨æµéè¦c/c++ç¯å¢\n- ä¿®æ¹æ½åææ¡\n-
-æ°å¢æ¥è¯¢æå¡å¨ç¶ææ¶è¿åconnect ip\n-
-ä¿®å¤äºæå¡å¨æ¥è¯¢æ ååºçæ¶åï¼å ä¸ºæ¥éæ åå¤ä¿¡æ¯çbug\n-
-ä¸ªäººä¿¡æ¯éç½®æµè¯ä»£ç ï¼ä¸ä¸ªçæ¬æ´æ°\n-
-æ°å¢æ±çæ´æ°æ·»å åå é¤\n\n### 0.2.2--2022.2.1\n\n- æ°å¢æ¢ç\n-
-æ°å¢å·æ¼å¶ä½\n-
-ä¿®å¤äºé­æ¹æå¡å¨å¯¼è´è§£åéè¯¯çbugï¼å°±æ¯ç´æ¥å¿½ç¥äºï¼\n-
-ä¿®æ¹äºé¨åå¯¹è¯ååº\n\n### 0.2.1--2022.1.25\n\n-
-æ°å¢çµä¿¡æè·åï¼ä¸å¥çè¯å®ï¼\n- ä¼åå¾çUI\n-
-æ°å¢äºæå¿«æ·æ¥è¯¢\n-
-ä¿®å¤äºå ä¸ºæ²¡ç¨ç©å®¶ï¼å¯¼è´çæå¡å¨ç¶ææ¥è¯¢éè¯¯\n-
-æ°å¢çµä¿¡æipç¬åï¼ä»ä»ä½ä¸ºåæ¬¡æ´æ°ipåè¡¨ï¼\n\n### 0.2.0--
-2022.1.21\n\n- æ°å¢åæå·¥åæ¥è¯¢\n- ä¼åæ¥è¯¢å¾çUI\n-
-æ°å¢åæå·¥åæä»¶ä¸è½½\n-
-ä¿®å¤äºå ä¸ºçµä¿¡æå®ç½åç«¯ä¿®æ¹å¯¼è´æ¥è¯¢å¤±è´¥çBUG\n\n###
-0.1.7--2022.1.19\n\n- æ°å¢ç¾¤ipè®¢éï¼æ¹éæ¥è¯¢\n-
-æ°å¢å¾çæ¾ç¤ºipç¶æ\n-
-ä¿®å¤äºå ä¸ºç©å®¶åå­ç¹æ®å­ç¬¦å¯¼è´çutf-8è§£ç éè¯¯\n-
-æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n-
-æ°å¢ipæ¥è¯¢æå¡å¨æä¾ç©å®¶æ°éååå­\n-
-å¢å åç¨å½æ°ä¿®å¤å ä¸ºå è½½é¡ºåºå¯¼è´çéè¯¯\n-
-æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n-
-æ°å¢æå¡å¨æ§å¶å°æä»¤ï¼æ°å¢ä¾èµrcon\n-
-éæ°äºæ°æ®åºï¼ä¸åä½¿ç¨jsonèæ¯ä½¿ç¨sql3\n-
-æ¹åäºæ±çanneä¿¡æ¯æ¾ç¤ºæ¹å¼ï¼å¦æåä¸ªæ°æ®ä»¥å¾çæ¾ç¤ºï¼å¦æå¤ä¸ªæ°æ®ä»¥æå­æ¾ç¤º\n\n###
-0.1.4--2022.1.9\n\n- æ°å¢æ±çanneè¯¦æï¼çæåï¼\n-
-ææçè¯·æ±æ¹ä¸ºhttpx\n- æ´æ°äºanneä¿¡æ¯å¾ç\n-
-å¯éä½¿ç¨æ¨¡æè°·æ­æµè§å¨æ¥è·åanneæ´å¤æ°æ®ï¼~æç¹å±äºï¼å¸æå¤§ä½¬ææ~)\n\n###
-0.1.3--2022.1.7\n\n- æ°å¢ç»å®æµç§°åsteamid\n-
-æ°å¢å¯ä»¥è¾ç¹äººæ¥è¯¢anneæç»©\n- æ°å¢è§£ç»ä¿¡æ¯\n\n### 0.1.2--
-2022.1.6\n\n- æ°å¢æ¯æå¾çè¾åº\n- æ°å¢æ¥è¯¢anneææ°æ®\n\n###
-0.1.1--2022.1.5\n\n- æ°å¢å é¤å°å¾\n- æ°å¢å°å¾æ¹å\n-
-æ°å¢æ¯æå¾çè¾åº\n\n### 0.1.0--2022.1.4\n\n- éä¸­ä¿®å¤äºBug\n\n###
-0.0.9--2022.1.4\n\n-
-æ°å¢ä¸ä¼ å°å¾åï¼æ£æµå¯¹æ¯åå¤æ°å°å¾åå­\n-
-ä¿®å¤ä¸­æåä¹±ç é®é¢\n\n### 0.0.8--2022.1.4\n\n-
-æ¯ævpkæ ¼å¼å°å¾\n- æ¯ææ¥çæævpkæ ¼å¼æä»¶\n\n### 0.0.6--
-2022.1.3\n\n- ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç \n\n### 0.0.1--
-2022.1.3\n\n- æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾\n\n\n\n## ð
-å¶ä»\n\n-
+[æ¨¡å¼]æ¥è®¿é® - æ°å¢æ¹éæ¥è¯¢æå¡å¨ï¼ä¸å¸¦åæ°åè¿åå¾ç
+### 0.3.1--2022.2.22 - ä¿®å¤äºè·¯å¾è¯å«ä¸ºstrå¯¹è±¡çéè¯¯ -
+ä¿®å¤äºåå§åæ¾ä¸å°æä»¶çéè¯¯ - ä¿®å¤äºè·¯å¾æ¼æ¥éè¯¯ -
+å¨winç«¯æåæµè¯ï¼ä¿®å¤åç¼©åbug - æ°å¢å¼å³åç¨å¼æ­¥envè®¾ç½®
+- æµè¯rconå»ºç«éè®¯ - å®ç°åæ¢è·¯å¾æ¥çå°å¾åä½¿ç¨rconæä»¤
+### 0.3.0--2022.2.18 -
+ä¿®æ¹äºæ°çenvéç½®ï¼ä½¿å¾æ¯ææ¬å°å¤æå¡å¨æä½ -
+å½»åºè§£å³äºåç¼©åè§£ålinuxç«¯çé®é¢ -
+è§£å³äºwinç«¯é»è®¤gbkè§£ç çéè¯¯ - è§£å³rconæä»¤å­ä½æ¥é ###
+0.2.5--2022.2.10 - ä¿®å¤äºä¾èµä¸è¶³çbug -
+æ´æ°äºçµä¿¡ææç»©ä¸ªäººå¾çUI - æ´æ°äºæ¹éæå¡å¨æ¥ççUI -
+ä¿®æ¹äºä¼ æä»¶ä¸ºåç¨å¼æ­¥ - ä¼åäºé¨årconæä»¤ -
+~tnd7zæä¹ä¸å»æ­»å~ä½¿ç¨pyunpackåºè§£å7z ### 0.2.4--2022.2.8 -
+ä½¿ç¨poetryä¿®å¤äºpipå®è£æä»¶ç¼ºå¤±çbug ### 0.2.3--2022.2.7 -
+æ°å¢åç¢åå¼ç¢ -
+ä¿®æ¹äºè·åèµæºä¸ºå¼æ­¥åç¨å´é»ç¢å¶ä»æä»¤çbug -
+æ°å¢jsonç»è®¡é¨åå·²ç¥æå¡å¨ï¼æªæ¥åºè¯¥ç¬ç«æåºæç»­æ´æ°ï¼å¦æææ¨çéå¬å¼æè®°å½è¯·èç³»æå é¤ï¼
+- å·åå¶ä½å¼æäºï¼æ¨æµéè¦c/c++ç¯å¢ - ä¿®æ¹æ½åææ¡ -
+æ°å¢æ¥è¯¢æå¡å¨ç¶ææ¶è¿åconnect ip -
+ä¿®å¤äºæå¡å¨æ¥è¯¢æ ååºçæ¶åï¼å ä¸ºæ¥éæ åå¤ä¿¡æ¯çbug
+- ä¸ªäººä¿¡æ¯éç½®æµè¯ä»£ç ï¼ä¸ä¸ªçæ¬æ´æ° -
+æ°å¢æ±çæ´æ°æ·»å åå é¤ ### 0.2.2--2022.2.1 - æ°å¢æ¢ç -
+æ°å¢å·æ¼å¶ä½ -
+ä¿®å¤äºé­æ¹æå¡å¨å¯¼è´è§£åéè¯¯çbugï¼å°±æ¯ç´æ¥å¿½ç¥äºï¼ -
+ä¿®æ¹äºé¨åå¯¹è¯ååº ### 0.2.1--2022.1.25 -
+æ°å¢çµä¿¡æè·åï¼ä¸å¥çè¯å®ï¼ - ä¼åå¾çUI -
+æ°å¢äºæå¿«æ·æ¥è¯¢ -
+ä¿®å¤äºå ä¸ºæ²¡ç¨ç©å®¶ï¼å¯¼è´çæå¡å¨ç¶ææ¥è¯¢éè¯¯ -
+æ°å¢çµä¿¡æipç¬åï¼ä»ä»ä½ä¸ºåæ¬¡æ´æ°ipåè¡¨ï¼ ### 0.2.0--
+2022.1.21 - æ°å¢åæå·¥åæ¥è¯¢ - ä¼åæ¥è¯¢å¾çUI -
+æ°å¢åæå·¥åæä»¶ä¸è½½ -
+ä¿®å¤äºå ä¸ºçµä¿¡æå®ç½åç«¯ä¿®æ¹å¯¼è´æ¥è¯¢å¤±è´¥çBUG ### 0.1.7--
+2022.1.19 - æ°å¢ç¾¤ipè®¢éï¼æ¹éæ¥è¯¢ - æ°å¢å¾çæ¾ç¤ºipç¶æ -
+ä¿®å¤äºå ä¸ºç©å®¶åå­ç¹æ®å­ç¬¦å¯¼è´çutf-8è§£ç éè¯¯ -
+æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.6 ### 0.1.6--2022.1.15 -
+æ°å¢ipæ¥è¯¢æå¡å¨æä¾ç©å®¶æ°éååå­ -
+å¢å åç¨å½æ°ä¿®å¤å ä¸ºå è½½é¡ºåºå¯¼è´çéè¯¯ -
+æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.4 ### 0.1.5--2022.1.15 -
+æ°å¢æå¡å¨æ§å¶å°æä»¤ï¼æ°å¢ä¾èµrcon -
+éæ°äºæ°æ®åºï¼ä¸åä½¿ç¨jsonèæ¯ä½¿ç¨sql3 -
+æ¹åäºæ±çanneä¿¡æ¯æ¾ç¤ºæ¹å¼ï¼å¦æåä¸ªæ°æ®ä»¥å¾çæ¾ç¤ºï¼å¦æå¤ä¸ªæ°æ®ä»¥æå­æ¾ç¤º
+### 0.1.4--2022.1.9 - æ°å¢æ±çanneè¯¦æï¼çæåï¼ -
+ææçè¯·æ±æ¹ä¸ºhttpx - æ´æ°äºanneä¿¡æ¯å¾ç -
+å¯éä½¿ç¨æ¨¡æè°·æ­æµè§å¨æ¥è·åanneæ´å¤æ°æ®ï¼~æç¹å±äºï¼å¸æå¤§ä½¬ææ~)
+### 0.1.3--2022.1.7 - æ°å¢ç»å®æµç§°åsteamid -
+æ°å¢å¯ä»¥è¾ç¹äººæ¥è¯¢anneæç»© - æ°å¢è§£ç»ä¿¡æ¯ ### 0.1.2--2022.1.6
+- æ°å¢æ¯æå¾çè¾åº - æ°å¢æ¥è¯¢anneææ°æ® ### 0.1.1--2022.1.5 -
+æ°å¢å é¤å°å¾ - æ°å¢å°å¾æ¹å - æ°å¢æ¯æå¾çè¾åº ### 0.1.0--
+2022.1.4 - éä¸­ä¿®å¤äºBug ### 0.0.9--2022.1.4 -
+æ°å¢ä¸ä¼ å°å¾åï¼æ£æµå¯¹æ¯åå¤æ°å°å¾åå­ -
+ä¿®å¤ä¸­æåä¹±ç é®é¢ ### 0.0.8--2022.1.4 - æ¯ævpkæ ¼å¼å°å¾ -
+æ¯ææ¥çæævpkæ ¼å¼æä»¶ ### 0.0.6--2022.1.3 -
+ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç  ### 0.0.1--2022.1.3 -
+æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» -
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
-& Pr\n- å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n-
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n- [GPL-3.0 License]
+& Pr - å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ -
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [GPL-3.0 License]
 (https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m)\n\n## ð æè°¢\n\n- [nonebot2](https:
-//github.com/nonebot/nonebot2)- èå¤©æºå¨äººçåºç¡æ¡æ¶\n- [ä¿®ä»]
-(https://github.com/s52047qwas/nonebot_plugin_xiuxian)- æ°æ®åºåè\n- ~~
+[@Agnes4m](https://github.com/Agnes4m) ## ð æè°¢ - [nonebot2](https://
+github.com/nonebot/nonebot2)- èå¤©æºå¨äººçåºç¡æ¡æ¶ - [ä¿®ä»](https:/
+/github.com/s52047qwas/nonebot_plugin_xiuxian)- æ°æ®åºåè - ~~
 [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://github.com/Agnes4m/VSQ)~~
-(å·²å¼ç¨)\n- [@MeetWq](https://github.com/MeetWq)-
-éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³\n - [å¯ç±å°Q](https://github.com/
-MeetWq/mybot)- æå¡å¨å¾çåè\n- [ç¾¤èå­¦ä¹ ](https://github.com/
-CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè\n-
-[æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè\n- [gsuid]
-(https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè\n-
-åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®\n- ArcPav -
-ç§¯æåé¦bugï¼æä¾æ¹è¿æè·¯', 'author': 'Agnes_Digital',
-'author_email': 'Z735803792@163.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq)-
+éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
+MeetWq/mybot)- æå¡å¨å¾çåè - [ç¾¤èå­¦ä¹ ](https://github.com/
+CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè -
+[æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè - [gsuid]
+(https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè -
+åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ® - ArcPav -
+ç§¯æåé¦bugï¼æä¾æ¹è¿æè·¯
```

