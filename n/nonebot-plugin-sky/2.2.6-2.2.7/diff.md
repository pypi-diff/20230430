# Comparing `tmp/nonebot-plugin-sky-2.2.6.tar.gz` & `tmp/nonebot-plugin-sky-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sky-2.2.6.tar", last modified: Wed Apr 26 07:19:48 2023, max compression
+gzip compressed data, was "nonebot-plugin-sky-2.2.7.tar", last modified: Sun Apr 30 05:21:33 2023, max compression
```

## Comparing `nonebot-plugin-sky-2.2.6.tar` & `nonebot-plugin-sky-2.2.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.493358 nonebot-plugin-sky-2.2.6/
--rw-rw-rw-   0        0        0    35823 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/LICENSE
--rw-rw-rw-   0        0        0    15893 2023-04-26 07:19:48.492361 nonebot-plugin-sky-2.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    15369 2023-04-26 07:02:50.000000 nonebot-plugin-sky-2.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.402601 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/
--rw-rw-rw-   0        0        0     6153 2023-04-13 02:27:05.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.418558 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/__init__.py
--rw-rw-rw-   0        0        0     5707 2023-03-02 08:15:25.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/command.py
--rw-rw-rw-   0        0        0     1810 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/helper_at_all.py
--rw-rw-rw-   0        0        0     1261 2023-02-24 05:45:59.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/load_config.py
--rw-rw-rw-   0        0        0     1747 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/msg_forward.py
--rw-rw-rw-   0        0        0     1560 2023-02-24 02:36:59.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/travelling_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.423545 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/
--rw-rw-rw-   0        0        0     1160 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/light_beauty.py
--rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/light_cute.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.430526 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.434540 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/__init__.py
--rw-rw-rw-   0        0        0     2547 2023-04-04 06:39:21.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/international.py
--rw-rw-rw-   0        0        0     3077 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/national.py
--rw-rw-rw-   0        0        0   459817 2023-04-26 06:51:25.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/get_id.png
--rw-rw-rw-   0        0        0      637 2023-03-02 07:17:23.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/public_notice.py
--rw-rw-rw-   0        0        0    13536 2023-04-26 07:15:44.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/query_tools.py
--rw-rw-rw-   0        0        0     1080 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/queue.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.438530 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
--rw-rw-rw-   0        0        0     3041 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/international.py
--rw-rw-rw-   0        0        0     2996 2023-04-12 10:08:03.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/national.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.444490 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.466431 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/
--rw-rw-rw-   0        0        0    16051 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/eating.jpg
--rw-rw-rw-   0        0        0    89789 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_braid.gif
--rw-rw-rw-   0        0        0    79644 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_bun.gif
--rw-rw-rw-   0        0        0    72146 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_cat.gif
--rw-rw-rw-   0        0        0    87935 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_fox.gif
--rw-rw-rw-   0        0        0    80542 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
--rw-rw-rw-   0        0        0    95522 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/go.jpg
--rw-rw-rw-   0        0        0      274 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/menu.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.469450 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/menu_image/
--rw-rw-rw-   0        0        0   824527 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/menu_image/menu.png
--rw-rw-rw-   0        0        0       95 2023-02-20 02:53:16.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/pusher.py
--rw-rw-rw-   0        0        0     3791 2023-03-02 09:17:27.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.490366 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/
--rw-rw-rw-   0        0        0     2280 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/__init__.py
--rw-rw-rw-   0        0        0      405 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/bot_loader.py
--rw-rw-rw-   0        0        0      607 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/chain_reply.py
--rw-rw-rw-   0        0        0     5061 2023-04-26 07:02:50.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/check_update.py
--rw-rw-rw-   0        0        0     6369 2023-03-23 08:02:10.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/data_pack.py
--rw-rw-rw-   0        0        0      391 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/date_util.py
--rw-rw-rw-   0        0        0      746 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/json_cards.py
--rw-rw-rw-   0        0        0     1264 2023-04-04 07:30:19.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/notice_board.py
-drwxrwxrwx   0        0        0        0 2023-04-26 07:19:48.408586 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/
--rw-rw-rw-   0        0        0    15893 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1984 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-26 07:19:48.000000 nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 07:19:48.493358 nonebot-plugin-sky-2.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1450 2023-04-26 07:19:24.000000 nonebot-plugin-sky-2.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:33.583501 nonebot-plugin-sky-2.2.7/
+-rw-rw-rw-   0        0        0    35823 2022-11-03 06:35:38.000000 nonebot-plugin-sky-2.2.7/LICENSE
+-rw-rw-rw-   0        0        0    16034 2023-04-30 05:21:33.558566 nonebot-plugin-sky-2.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    15510 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.373413 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/
+-rw-rw-rw-   0        0        0     6169 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.498080 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/
+-rw-rw-rw-   0        0        0        0 2023-03-01 11:49:56.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/__init__.py
+-rw-rw-rw-   0        0        0     5707 2023-03-07 11:28:55.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/command.py
+-rw-rw-rw-   0        0        0     1810 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/helper_at_all.py
+-rw-rw-rw-   0        0        0     1261 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/load_config.py
+-rw-rw-rw-   0        0        0     1747 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/msg_forward.py
+-rw-rw-rw-   0        0        0     1560 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/travelling_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.612774 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/
+-rw-rw-rw-   0        0        0     1160 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/light_beauty.py
+-rw-rw-rw-   0        0        0        0 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/light_cute.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.684580 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/
+-rw-rw-rw-   0        0        0        0 2023-03-01 11:48:13.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.744420 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/
+-rw-rw-rw-   0        0        0        0 2023-03-01 11:48:13.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2547 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/international.py
+-rw-rw-rw-   0        0        0     3077 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/national.py
+-rw-rw-rw-   0        0        0   459817 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/get_id.png
+-rw-rw-rw-   0        0        0      637 2023-03-07 11:28:55.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/public_notice.py
+-rw-rw-rw-   0        0        0    13461 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/query_tools.py
+-rw-rw-rw-   0        0        0     1080 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/queue.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.796281 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/
+-rw-rw-rw-   0        0        0        0 2023-03-01 12:32:18.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
+-rw-rw-rw-   0        0        0     3041 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/international.py
+-rw-rw-rw-   0        0        0     2996 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/national.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:32.592151 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/
+-rw-rw-rw-   0        0        0        0 2023-03-01 11:50:17.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:33.396004 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/
+-rw-rw-rw-   0        0        0    16051 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/eating.jpg
+-rw-rw-rw-   0        0        0    89789 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_braid.gif
+-rw-rw-rw-   0        0        0    79644 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_bun.gif
+-rw-rw-rw-   0        0        0    72146 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_cat.gif
+-rw-rw-rw-   0        0        0    87935 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_fox.gif
+-rw-rw-rw-   0        0        0    80542 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
+-rw-rw-rw-   0        0        0    95522 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/go.jpg
+-rw-rw-rw-   0        0        0      274 2023-01-02 06:48:03.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/menu.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:33.414951 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/menu_image/
+-rw-rw-rw-   0        0        0   824527 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/menu_image/menu.png
+-rw-rw-rw-   0        0        0       95 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/pusher.py
+-rw-rw-rw-   0        0        0     3791 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:33.545601 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/
+-rw-rw-rw-   0        0        0     2280 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/__init__.py
+-rw-rw-rw-   0        0        0      405 2022-12-22 07:28:55.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/bot_loader.py
+-rw-rw-rw-   0        0        0      607 2023-03-01 12:37:46.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/chain_reply.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/check_update.py
+-rw-rw-rw-   0        0        0     6369 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/data_pack.py
+-rw-rw-rw-   0        0        0      391 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/date_util.py
+-rw-rw-rw-   0        0        0      746 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/json_cards.py
+-rw-rw-rw-   0        0        0     1264 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/notice_board.py
+drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.382390 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/
+-rw-rw-rw-   0        0        0    16034 2023-04-30 05:21:30.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-04-30 05:21:31.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 05:21:30.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-04-30 05:21:30.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-30 05:21:30.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 05:21:33.583501 nonebot-plugin-sky-2.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1450 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/setup.py
```

### Comparing `nonebot-plugin-sky-2.2.6/LICENSE` & `nonebot-plugin-sky-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/PKG-INFO` & `nonebot-plugin-sky-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.6
+Version: 2.2.7
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -286,14 +286,20 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.30 v2.2.7
+
+1.在这个版本之后所有querytools命令均废弃不再生效。
+
+2.更新季节时间（暂时不是很准确
+
 2023.4.25 v2.2.6
 
 1.修复获取uid帮助图片无法发送的问题
 
 2.当处于季节真空期时查询季蜡、蜡烛数返回相应提示
 
 2023.4.12 v2.2.5.post2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.6 Summary: nonebot2
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.7 Summary: nonebot2
 plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
 pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
@@ -111,15 +111,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.25 v2.2.6
+â¨æ´æ°æ¥å¿â¨ 2023.4.30 v2.2.7
+1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
+2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
 3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
```

### Comparing `nonebot-plugin-sky-2.2.6/README.md` & `nonebot-plugin-sky-2.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,20 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.30 v2.2.7
+
+1.在这个版本之后所有querytools命令均废弃不再生效。
+
+2.更新季节时间（暂时不是很准确
+
 2023.4.25 v2.2.6
 
 1.修复获取uid帮助图片无法发送的问题
 
 2.当处于季节真空期时查询季蜡、蜡烛数返回相应提示
 
 2023.4.12 v2.2.5.post2
```

#### html2text {}

```diff
@@ -104,15 +104,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.25 v2.2.6
+â¨æ´æ°æ¥å¿â¨ 2023.4.30 v2.2.7
+1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
+2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
 3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
```

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/__init__.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         seconds = remain_time.seconds % 3600 % 60
         # 发送剩余时间
         return f'距离{season_name}结束还有{days}天{hours}小时{minutes}分钟{seconds}秒'
 
 
 @RemainCN.handle()
 async def remain_cn():
-    results = remain("追忆季", 2023, 4, 20, 00, 00, 00)
+    results = remain("夜行季国服", 2023, 7, 19, 00, 00, 00)
     await RemainIN.send(results)
 
 
 @RemainIN.handle()
 async def remain_in():
-    results = remain("缅怀季", 2023, 4, 3, 15, 00, 00)
+    results = remain("夜行季国际服", 2023, 6, 25, 15, 00, 00)
     await RemainIN.send(results)
```

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/command.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/command.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/helper_at_all.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/helper_at_all.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/load_config.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/msg_forward.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/msg_forward.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/config/travelling_cache.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/travelling_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/guild/__init__.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/international.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/daily_tasks/national.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/get_id.png` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/get_id.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/public_notice.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/public_notice.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/query_tools.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/query_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,25 +330,22 @@
                 To_Get_Uid
             )
         query = Sprite()
 
         try:
             season = await query.get_season_candles(sky_id)
             white = await query.get_candles(sky_id)
-
+            season_left = ''
             if '这边查询一下' not in season and '这边查询一下' not in white:
                 pass
             else:
                 time.sleep(1)
                 season = await query.get_season_candles(sky_id)
                 white = await query.get_candles(sky_id)
-            try:
-                season_left = re.findall('剩余：(\d+)+?', season)[0]
-            except Exception as e:
-                e.__str__()
+            if '真空期' in season:
                 season_left = 0
             white_left = re.findall('剩余：(\d+)+?', white)[0]
             await CandlesView.send(
                 f'蜡烛总览：\n●普通蜡烛：{white_left}\n●季节蜡烛：{season_left}'
             )
         except Exception as e:
             str(e)
@@ -389,14 +386,14 @@
                 NO_BIND_MSG +
                 To_Get_Uid
             )
         results = await query.get_activities(sky_id)
         await Activities.send(results)
 
 
-__all__ = (
-    "save_id_handler",
-    "sky_id_handler",
-    "white_candles_handler",
-    "season_candles_handler",
-    "weather_handle"
-)
+# __all__ = (
+#     "save_id_handler",
+#     "sky_id_handler",
+#     "white_candles_handler",
+#     "season_candles_handler",
+#     "weather_handle"
+# )
```

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/queue.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/queue.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/international.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/sky/travelling_spirit/national.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/eating.jpg` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/eating.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_braid.gif` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_braid.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_bun.gif` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_bun.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_cat.gif` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_fox.gif` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_fox.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/helper_image/go.jpg` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/go.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/menu_image/menu.png` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/menu_image/menu.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/tools/scheduler.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/__init__.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/chain_reply.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/chain_reply.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/check_update.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/check_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 
 from nonebot import on_command, logger
 from ..config.command import get_cmd_alias
 
 logging.captureWarnings(True)  # 去掉建议使用SSL验证的显示
 
-Version = '2.2.6'  # 全局插件版本信息  （不用加v！）
+Version = '2.2.7'  # 全局插件版本信息  （不用加v！）
 
 
 async def get_datapack_ver():
     """
     检查本地数据包版本
     """
     try:
```

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/data_pack.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/data_pack.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/json_cards.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/json_cards.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky/utils_/notice_board.py` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/notice_board.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/PKG-INFO` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.6
+Version: 2.2.7
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -286,14 +286,20 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.30 v2.2.7
+
+1.在这个版本之后所有querytools命令均废弃不再生效。
+
+2.更新季节时间（暂时不是很准确
+
 2023.4.25 v2.2.6
 
 1.修复获取uid帮助图片无法发送的问题
 
 2.当处于季节真空期时查询季蜡、蜡烛数返回相应提示
 
 2023.4.12 v2.2.5.post2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.6 Summary: nonebot2
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.7 Summary: nonebot2
 plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
 pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
@@ -111,15 +111,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.25 v2.2.6
+â¨æ´æ°æ¥å¿â¨ 2023.4.30 v2.2.7
+1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
+2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
 3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
```

### Comparing `nonebot-plugin-sky-2.2.6/nonebot_plugin_sky.egg-info/SOURCES.txt` & `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.6/setup.py` & `nonebot-plugin-sky-2.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 Files = get_files(r'nonebot_plugin_sky/tools/helper_image')
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
 setuptools.setup(
     name='nonebot-plugin-sky',
-    version='v2.2.6',
+    version='v2.2.7',
     author='Kaguya233qwq',
     author_email='1435608435@qq.com',
     keywords=["pip", "nonebot2", "nonebot", "sky光遇", "光遇"],
     url='https://github.com/Kaguya233qwq/nonebot_plugin_sky',
     description='''nonebot2 plugin sky''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

