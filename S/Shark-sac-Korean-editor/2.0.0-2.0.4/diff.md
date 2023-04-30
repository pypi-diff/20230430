# Comparing `tmp/Shark sac Korean editor-2.0.0.tar.gz` & `tmp/Shark sac Korean editor-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shark sac Korean editor-2.0.0.tar", last modified: Thu Apr 27 13:12:00 2023, max compression
+gzip compressed data, was "Shark sac Korean editor-2.0.4.tar", last modified: Sun Apr 30 10:52:01 2023, max compression
```

## Comparing `Shark sac Korean editor-2.0.0.tar` & `Shark sac Korean editor-2.0.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.494131 Shark sac Korean editor-2.0.0/
--rw-rw-rw-   0        0        0      731 2023-04-27 13:12:00.493158 Shark sac Korean editor-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.423501 Shark sac Korean editor-2.0.0/Shark_sac_Korean_editor.egg-info/
--rw-rw-rw-   0        0        0      731 2023-04-27 13:12:00.000000 Shark sac Korean editor-2.0.0/Shark_sac_Korean_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-04-27 13:12:00.000000 Shark sac Korean editor-2.0.0/Shark_sac_Korean_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 13:12:00.000000 Shark sac Korean editor-2.0.0/Shark_sac_Korean_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 13:12:00.000000 Shark sac Korean editor-2.0.0/Shark_sac_Korean_editor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.438799 Shark sac Korean editor-2.0.0/modkr/
--rw-rw-rw-   0        0        0      281 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/__init__.py
--rw-rw-rw-   0        0        0     9489 2023-04-26 11:23:23.000000 Shark sac Korean editor-2.0.0/modkr/__main__.py
--rw-rw-rw-   0        0        0    10240 2023-04-26 10:58:08.000000 Shark sac Korean editor-2.0.0/modkr/adb_handler.py
--rw-rw-rw-   0        0        0    13764 2023-04-26 10:44:46.000000 Shark sac Korean editor-2.0.0/modkr/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-04-26 08:21:08.000000 Shark sac Korean editor-2.0.0/modkr/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.440774 Shark sac Korean editor-2.0.0/modkr/edits/
--rw-rw-rw-   0        0        0       67 2023-04-26 08:19:36.000000 Shark sac Korean editor-2.0.0/modkr/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.446616 Shark sac Korean editor-2.0.0/modkr/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8976 2023-04-27 12:50:49.000000 Shark sac Korean editor-2.0.0/modkr/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-04-26 08:20:39.000000 Shark sac Korean editor-2.0.0/modkr/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     4041 2023-04-27 11:46:25.000000 Shark sac Korean editor-2.0.0/modkr/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16755 2023-04-27 11:45:13.000000 Shark sac Korean editor-2.0.0/modkr/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.454421 Shark sac Korean editor-2.0.0/modkr/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8994 2023-04-27 02:57:22.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11240 2023-04-27 03:01:29.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3262 2023-04-26 08:44:31.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1083 2023-04-27 03:03:55.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2883 2023-04-27 03:19:09.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1277 2023-04-27 03:06:18.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     8065 2023-04-27 02:58:27.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4607 2023-04-27 02:48:44.000000 Shark sac Korean editor-2.0.0/modkr/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.458786 Shark sac Korean editor-2.0.0/modkr/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      333 2023-04-26 10:32:02.000000 Shark sac Korean editor-2.0.0/modkr/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2835 2023-04-26 08:38:24.000000 Shark sac Korean editor-2.0.0/modkr/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3399 2023-04-26 08:41:50.000000 Shark sac Korean editor-2.0.0/modkr/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4130 2023-04-26 08:40:01.000000 Shark sac Korean editor-2.0.0/modkr/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.473915 Shark sac Korean editor-2.0.0/modkr/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/aku.py
--rw-rw-rw-   0        0        0      516 2023-04-26 09:33:48.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      869 2023-04-26 09:29:09.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      650 2023-04-26 10:31:23.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6389 2023-04-26 09:30:45.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     2062 2023-04-26 09:29:36.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1056 2023-04-26 09:28:52.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 09:34:32.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4451 2023-04-27 03:25:53.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2361 2023-04-26 09:35:46.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3106 2023-04-27 03:25:08.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1227 2023-04-26 09:29:23.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8576 2023-04-27 03:28:15.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1082 2023-04-26 09:16:16.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      799 2023-04-26 09:17:54.000000 Shark sac Korean editor-2.0.0/modkr/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.486344 Shark sac Korean editor-2.0.0/modkr/edits/other/
--rw-rw-rw-   0        0        0      276 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3913 2023-04-26 10:25:28.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1124 2023-04-26 10:23:52.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2236 2023-04-26 09:44:49.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      698 2023-04-26 09:46:24.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3510 2023-04-26 10:22:39.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7140 2023-04-26 10:03:11.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4384 2023-04-26 10:17:15.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/missions.py
--rw-rw-rw-   0        0        0     1016 2023-04-26 10:13:14.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1657 2023-04-26 10:18:48.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1426 2023-04-26 10:16:14.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      356 2023-04-26 10:30:56.000000 Shark sac Korean editor-2.0.0/modkr/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-27 13:12:00.492185 Shark sac Korean editor-2.0.0/modkr/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1308 2023-04-26 11:02:30.000000 Shark sac Korean editor-2.0.0/modkr/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2795 2023-04-26 11:01:45.000000 Shark sac Korean editor-2.0.0/modkr/edits/save_management/load.py
--rw-rw-rw-   0        0        0      661 2023-04-26 10:58:58.000000 Shark sac Korean editor-2.0.0/modkr/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1900 2023-04-25 09:48:00.000000 Shark sac Korean editor-2.0.0/modkr/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    13745 2023-04-27 03:16:46.000000 Shark sac Korean editor-2.0.0/modkr/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-04-26 08:26:01.000000 Shark sac Korean editor-2.0.0/modkr/game_data_getter.py
--rw-rw-rw-   0        0        0    22979 2023-04-26 10:56:29.000000 Shark sac Korean editor-2.0.0/modkr/helper.py
--rw-rw-rw-   0        0        0     7075 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/item.py
--rw-rw-rw-   0        0        0     3505 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/managed_item.py
--rw-rw-rw-   0        0        0    66980 2023-04-25 17:12:37.000000 Shark sac Korean editor-2.0.0/modkr/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/patcher.py
--rw-rw-rw-   0        0        0     2450 2023-04-26 10:55:23.000000 Shark sac Korean editor-2.0.0/modkr/root_handler.py
--rw-rw-rw-   0        0        0    53823 2023-04-26 08:24:37.000000 Shark sac Korean editor-2.0.0/modkr/serialise_save.py
--rw-rw-rw-   0        0        0    25211 2023-04-26 10:54:03.000000 Shark sac Korean editor-2.0.0/modkr/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/tracker.py
--rw-rw-rw-   0        0        0     3544 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/updater.py
--rw-rw-rw-   0        0        0     8297 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.0/modkr/user_input_handler.py
--rw-rw-rw-   0        0        0       42 2023-04-27 13:12:00.494131 Shark sac Korean editor-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-04-27 13:06:28.000000 Shark sac Korean editor-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.441468 Shark sac Korean editor-2.0.4/
+-rw-rw-rw-   0        0        0      731 2023-04-30 10:52:01.440494 Shark sac Korean editor-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.370000 Shark sac Korean editor-2.0.4/Shark_sac_Korean_editor.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-04-30 10:52:01.000000 Shark sac Korean editor-2.0.4/Shark_sac_Korean_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-30 10:52:01.000000 Shark sac Korean editor-2.0.4/Shark_sac_Korean_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 10:52:01.000000 Shark sac Korean editor-2.0.4/Shark_sac_Korean_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 10:52:01.000000 Shark sac Korean editor-2.0.4/Shark_sac_Korean_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.386853 Shark sac Korean editor-2.0.4/modkr/
+-rw-rw-rw-   0        0        0      281 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/__init__.py
+-rw-rw-rw-   0        0        0     9549 2023-04-30 07:48:02.000000 Shark sac Korean editor-2.0.4/modkr/__main__.py
+-rw-rw-rw-   0        0        0    10240 2023-04-26 10:58:08.000000 Shark sac Korean editor-2.0.4/modkr/adb_handler.py
+-rw-rw-rw-   0        0        0    13764 2023-04-26 10:44:46.000000 Shark sac Korean editor-2.0.4/modkr/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-04-26 08:21:08.000000 Shark sac Korean editor-2.0.4/modkr/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.387828 Shark sac Korean editor-2.0.4/modkr/edits/
+-rw-rw-rw-   0        0        0       67 2023-04-26 08:19:36.000000 Shark sac Korean editor-2.0.4/modkr/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.394017 Shark sac Korean editor-2.0.4/modkr/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8976 2023-04-27 12:50:49.000000 Shark sac Korean editor-2.0.4/modkr/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-04-26 08:20:39.000000 Shark sac Korean editor-2.0.4/modkr/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     4041 2023-04-27 11:46:25.000000 Shark sac Korean editor-2.0.4/modkr/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16755 2023-04-27 11:45:13.000000 Shark sac Korean editor-2.0.4/modkr/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.402703 Shark sac Korean editor-2.0.4/modkr/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8994 2023-04-27 02:57:22.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11449 2023-04-30 07:58:40.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3262 2023-04-26 08:44:31.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1083 2023-04-27 03:03:55.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2883 2023-04-27 03:19:09.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1277 2023-04-27 03:06:18.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     8065 2023-04-27 02:58:27.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1900 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4634 2023-04-30 08:11:09.000000 Shark sac Korean editor-2.0.4/modkr/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.407076 Shark sac Korean editor-2.0.4/modkr/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-04-26 10:32:02.000000 Shark sac Korean editor-2.0.4/modkr/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2835 2023-04-26 08:38:24.000000 Shark sac Korean editor-2.0.4/modkr/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3399 2023-04-26 08:41:50.000000 Shark sac Korean editor-2.0.4/modkr/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4130 2023-04-26 08:40:01.000000 Shark sac Korean editor-2.0.4/modkr/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.421720 Shark sac Korean editor-2.0.4/modkr/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-04-30 08:16:08.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      516 2023-04-26 09:33:48.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      869 2023-04-26 09:29:09.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      650 2023-04-26 10:31:23.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6389 2023-04-26 09:30:45.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     2062 2023-04-26 09:29:36.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1056 2023-04-26 09:28:52.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1481 2023-04-30 09:04:42.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4451 2023-04-27 03:25:53.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2361 2023-04-26 09:35:46.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3106 2023-04-27 03:25:08.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1227 2023-04-26 09:29:23.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8576 2023-04-27 03:28:15.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1082 2023-04-26 09:16:16.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      802 2023-04-30 08:25:27.000000 Shark sac Korean editor-2.0.4/modkr/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.433933 Shark sac Korean editor-2.0.4/modkr/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3913 2023-04-26 10:25:28.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1124 2023-04-26 10:23:52.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2236 2023-04-26 09:44:49.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      698 2023-04-26 09:46:24.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3510 2023-04-26 10:22:39.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7140 2023-04-26 10:03:11.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4384 2023-04-26 10:17:15.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/missions.py
+-rw-rw-rw-   0        0        0     1016 2023-04-26 10:13:14.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1657 2023-04-26 10:18:48.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1426 2023-04-26 10:16:14.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      356 2023-04-26 10:30:56.000000 Shark sac Korean editor-2.0.4/modkr/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:52:01.440494 Shark sac Korean editor-2.0.4/modkr/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1308 2023-04-26 11:02:30.000000 Shark sac Korean editor-2.0.4/modkr/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2795 2023-04-26 11:01:45.000000 Shark sac Korean editor-2.0.4/modkr/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      661 2023-04-26 10:58:58.000000 Shark sac Korean editor-2.0.4/modkr/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1906 2023-04-30 08:09:14.000000 Shark sac Korean editor-2.0.4/modkr/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    13855 2023-04-30 09:03:37.000000 Shark sac Korean editor-2.0.4/modkr/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-04-26 08:26:01.000000 Shark sac Korean editor-2.0.4/modkr/game_data_getter.py
+-rw-rw-rw-   0        0        0    23001 2023-04-30 08:04:44.000000 Shark sac Korean editor-2.0.4/modkr/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/item.py
+-rw-rw-rw-   0        0        0     3505 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/managed_item.py
+-rw-rw-rw-   0        0        0    66980 2023-04-25 17:12:37.000000 Shark sac Korean editor-2.0.4/modkr/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-04-30 07:47:55.000000 Shark sac Korean editor-2.0.4/modkr/patcher.py
+-rw-rw-rw-   0        0        0     2450 2023-04-26 10:55:23.000000 Shark sac Korean editor-2.0.4/modkr/root_handler.py
+-rw-rw-rw-   0        0        0    53823 2023-04-26 08:24:37.000000 Shark sac Korean editor-2.0.4/modkr/serialise_save.py
+-rw-rw-rw-   0        0        0    25211 2023-04-26 10:54:03.000000 Shark sac Korean editor-2.0.4/modkr/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/tracker.py
+-rw-rw-rw-   0        0        0     3544 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.4/modkr/user_input_handler.py
+-rw-rw-rw-   0        0        0       42 2023-04-30 10:52:01.441468 Shark sac Korean editor-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-04-30 10:51:17.000000 Shark sac Korean editor-2.0.4/setup.py
```

### Comparing `Shark sac Korean editor-2.0.0/PKG-INFO` & `Shark sac Korean editor-2.0.4/Shark_sac_Korean_editor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Shark sac Korean editor
-Version: 2.0.0
+Name: Shark-sac-Korean-editor
+Version: 2.0.4
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-2.0.0/Shark_sac_Korean_editor.egg-info/PKG-INFO` & `Shark sac Korean editor-2.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Shark-sac-Korean-editor
-Version: 2.0.0
+Name: Shark sac Korean editor
+Version: 2.0.4
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-2.0.0/Shark_sac_Korean_editor.egg-info/SOURCES.txt` & `Shark sac Korean editor-2.0.4/Shark_sac_Korean_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/__main__.py` & `Shark sac Korean editor-2.0.4/modkr/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         helper.colored_text(
             base=helper.RED,
             new=helper.WHITE,
         )
     print()
     helper.colored_text(
         f"{locale_manager.search_key('thanks_title')}\n"
+        + f"{locale_manager.search_key('thanks_title2')}\n"
         + f"{locale_manager.search_key('lethal_thanks')}\n"
         + f"{locale_manager.search_key('beeven_cse_thanks')}\n"
         + f"{locale_manager.search_key('support_thanks')}\n"
         + locale_manager.search_key("discord_thanks"),
         base=helper.GREEN,
         new=helper.WHITE,
     )
```

### Comparing `Shark sac Korean editor-2.0.0/modkr/adb_handler.py` & `Shark sac Korean editor-2.0.4/modkr/adb_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/config_manager.py` & `Shark sac Korean editor-2.0.4/modkr/config_manager.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/csv_handler.py` & `Shark sac Korean editor-2.0.4/modkr/csv_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/basic/basic_items.py` & `Shark sac Korean editor-2.0.4/modkr/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/basic/catfruit.py` & `Shark sac Korean editor-2.0.4/modkr/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/basic/catseyes.py` & `Shark sac Korean editor-2.0.4/modkr/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/basic/ototo_base_mats.py` & `Shark sac Korean editor-2.0.4/modkr/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/basic/talent_orbs.py` & `Shark sac Korean editor-2.0.4/modkr/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/basic/talent_orbs_new.py` & `Shark sac Korean editor-2.0.4/modkr/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/cat_helper.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/cat_id_selector.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/cat_id_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,34 +75,34 @@
 
 
 def select_cats_range(save_stats: dict[str, Any]) -> list[int]:
     """Select cats in a range"""
 
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "Enter cat ids (Look up cro battle cats to find ids)(You can enter &all& to get all, a range e.g &1&-&50&, or ids separate by spaces e.g &5 4 7&):"
+            "고양이 ID를 입력하십시오(ID를 찾으려면 &냥코id사이트.kro.kr 에서 를 조회하십시오)(모든 범위를 얻으려면 &all&을 입력할 수 있습니다(예: &1&-&50& 또는 공백으로 구분된 ID(예: &5 4 7&)).:"
         ),
         length=len(save_stats["cats"]),
     )
     return ids
 
 
 def select_cats_gatya_banner(save_stats: dict[str, Any]) -> list[int]:
     """Select cats for a specific gacha banner"""
     is_jp = helper.is_jp(save_stats)
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "GatyaDataSetR1.csv", is_jp
     )
     if file_data is None:
-        helper.colored_text("Failed to get gatya banners")
+        helper.colored_text("개다레 배너를 가져오지 못했습니다.")
         return []
     data = helper.parse_int_list_list(csv_handler.parse_csv(file_data.decode("utf-8")))
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "Enter gacha banner id (Look up the gacha banners you want, then click on the image at the top, and look for the last digits of the file name (e.g royal fest = 602))(You can enter &all& to get all, a range e.g &1&-&50&, or ids separate by spaces e.g &5 4 7&):"
+            "가챠배너 아이디 입력 (원하는 가챠배너 조회 후 상단의 이미지 클릭 후 파일명 마지막 자리 찾기 (예. royal fest = 602))(&all& 입력하시면 모두 받으실 수 있습니다. 범위(예: &1&-&50&) 또는 공백으로 구분된 ID(예: &5 4 7&):"
         ),
         length=len(data),
     )
     data = treasures.remove_negative_1(data)
     cat_ids: list[int] = []
     for c_id in ids:
         cat_ids.extend(data[c_id])
@@ -138,17 +138,17 @@
     cat_ids: list[int] = []
     cat_ids_str: list[str] = []
     cat_names: list[str] = []
     for cat_name, cat_id, _ in found_names:
         cat_ids.append(cat_id)
         cat_name = cat_name.replace("&", "\\&")
         cat_names.append(cat_name)
-        cat_ids_str.append(f"Cat id: &{cat_id}&")
+        cat_ids_str.append(f"고양이id: &{cat_id}&")
 
-    print("선택할 고양이의 인덱스 선택 (cat id 자체가 아님):")
+    print("선택할 고양이의 인덱스 선택 (고양이 id 자체가 아님):")
     indexes = user_input_handler.select_not_inc(
         cat_names, mode="select", extra_data=cat_ids_str
     )
     selected_ids: list[int] = []
     for index in indexes:
         try:
             selected_ids.append(cat_ids[index])
@@ -275,21 +275,21 @@
         return None
     file_path_dir = os.path.dirname(helper.get_file(path))
     helper.create_dirs(file_path_dir)
     if len(helper.find_files_in_dir(file_path_dir, "Unit_Explanation")) < len(
         save_stats["cats"]
     ):
         helper.colored_text(
-            "Downloading cat names for the first time... (This may take some time, but next time it will be much faster)",
+            "처음으로 고양이 이름을 다운로드하는 중... (시간이 좀 걸릴 수 있지만 다음에는 훨씬 더 빠를 것입니다)",
             helper.GREEN,
         )
         funcs: list[Process] = []
         version = game_data_getter.get_latest_version(is_jp)
         if version is None:
-            helper.colored_text("Failed to get cat names", helper.RED)
+            helper.colored_text("고양이 이름을 가져오지 못했습니다.", helper.RED)
             return None
         all_file_names: list[str] = []
         for cat_id, _ in enumerate(save_stats["cats"]):
             file_name = f"Unit_Explanation{cat_id+1}_{helper.get_lang(is_jp)}.csv"
             all_file_names.append(file_name)
         file_names_split = helper.chunks(all_file_names, 10)
         for file_names in file_names_split:
```

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/chara_drop.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/clear_cat_guide.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/evolve_cats.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/get_remove_cats.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/talents.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/upgrade_blue.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/cats/upgrade_cats.py` & `Shark sac Korean editor-2.0.4/modkr/edits/cats/upgrade_cats.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     first = True
     base_lvl = None
     plus_lvl = None
     for cat_id in ids:
         if not individual and first:
             levels = get_plus_base(
                 user_input_handler.colored_input(
-                    '냥코 캐릭터 기본 수준 다음에 "&+&" 다음에 플러스 수준을 입력합니다(예: 5&+&12). 기본 레벨을 무시하려면 &+&12 를 입력 하시구 플러스 레벨을 무시하려면 &+5&를 입력하십시오.:\n'
+                    '냥코 캐릭터 기본 수준 다음에 "&+&" 다음에 플러스 수준을 입력합니다(예: 5&+&12). 기본 레벨을 무시하려면 &+&12 를 입력 하시구 플러스 레벨을 무시하려면 &5+&를 입력하십시오. 올강레벨(예제:30+70):\n'
                 )
             )
             base_lvl = levels[0]
             plus_lvl = levels[1]
             first = False
         elif individual:
             helper.colored_text(
```

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/gamototo/gamatoto_xp.py` & `Shark sac Korean editor-2.0.4/modkr/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/gamototo/helpers.py` & `Shark sac Korean editor-2.0.4/modkr/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/gamototo/ototo_cat_cannon.py` & `Shark sac Korean editor-2.0.4/modkr/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/allow_filibuster_clearing.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/allow_filibuster_clearing.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/behemoth_culling.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/clear_tutorial.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/enigma_stages.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/event_stages.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/gauntlet.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/itf_timed_scores.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/legend_quest.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/legend_quest.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,9 +26,9 @@
             stage_data["Value"]["clear_amount"][0][0][i] = 0
             stage_data["Value"]["tries"][0][0][i] = 0
     
     if stage_data["Value"]["clear_progress"][0][0] == total:
         stage_data["Value"]["unlock_next"][0][1] = lengths["stars"] - 1
 
     save_stats["legend_quest"] = stage_data
-    helper.colored_text("Successfully set legend quest stages")
+    helper.colored_text("레전드 퀘스트 스테이지 설정 성공")
     return save_stats
```

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/main_story.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/outbreaks.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/story_level_id_selector.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/towers.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/treasures.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/uncanny.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/levels/unlock_aku_realm.py` & `Shark sac Korean editor-2.0.4/modkr/edits/levels/unlock_aku_realm.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
         save_stats["event_stages"] = event_stages.set_stage_data(
             save_stats["event_stages"],
             stage_id + offset,
             1,
             save_stats["event_stages"]["Lengths"],
             True,
         )
-    helper.colored_text("&Aku 영역이 성공적으로 잠금 해제되었습니다..")
+    helper.colored_text("&마계 영역이 성공적으로 잠금 해제되었습니다..")
     return save_stats
```

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/cat_shrine.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/claim_user_rank_rewards.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/create_new_account.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/fix_elsewhere.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/fix_time_issues.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/get_gold_pass.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/meow_medals.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/missions.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/play_time.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/scheme_item.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/trade_progress.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/other/unlock_enemy_guide.py` & `Shark sac Korean editor-2.0.4/modkr/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/save_management/convert.py` & `Shark sac Korean editor-2.0.4/modkr/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/save_management/load.py` & `Shark sac Korean editor-2.0.4/modkr/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/save_management/other.py` & `Shark sac Korean editor-2.0.4/modkr/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/save_management/save.py` & `Shark sac Korean editor-2.0.4/modkr/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/edits/save_management/server_upload.py` & `Shark sac Korean editor-2.0.4/modkr/edits/save_management/server_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,11 +44,11 @@
             "Error uploading save data\nPlease report this in #bug-reports"
         )
     if len(upload_data["transferCode"]) < 5:
         helper.colored_text(
             "Error uploading save data\nPlease report this in #bug-reports"
         )
     else:
-        helper.colored_text(f"전송 코드 : &{upload_data['transferCode']}&")
-        helper.colored_text(f"확인 코드 : &{upload_data['pin']}&")
+        helper.colored_text(f"이어하기 코드 : &{upload_data['transferCode']}&")
+        helper.colored_text(f"인증 코드 : &{upload_data['pin']}&")
 
     return save_stats
```

### Comparing `Shark sac Korean editor-2.0.0/modkr/feature_handler.py` & `Shark sac Korean editor-2.0.4/modkr/feature_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,22 +110,22 @@
         "보물": {
             "보물 그룹 (예: 에너지 드링크, 아쿠아 크리스탈 등)": levels.treasures.treasure_groups,
             "개별적으로 특정 단계 및 특정 챕터": levels.treasures.specific_stages,
             "특정 스테이지와 챕터를 한 번에": levels.treasures.specific_stages_all_chapters,
         },
         "좀비 스테이지 / 바이러스": levels.outbreaks.edit_outbreaks,
         "이벤트 스테이지": levels.event_stages.event_stages,
-        "전설의 이야기": levels.event_stages.stories_of_legend,
-        "섬뜩한 레전드리": levels.uncanny.edit_uncanny,
-        "아쿠 렐름/게이트 클리어링": levels.aku.edit_aku,
-        "악마 영역/게이트 잠금 해제": levels.unlock_aku_realm.unlock_aku_realm,
-        "건틀릿": levels.gauntlet.edit_gauntlet,
-        "콜라보 건틀릿": levels.gauntlet.edit_collab_gauntlet,
+        "레전드리 스토리": levels.event_stages.stories_of_legend,
+        "신레전드리 스토리": levels.uncanny.edit_uncanny,
+        "마계편 스테이지/게이트 클리어": levels.aku.edit_aku,
+        "마계편 스테이지/게이트 잠금 해제": levels.unlock_aku_realm.unlock_aku_realm,
+        "건틀릿[한국냥코사용불가]": levels.gauntlet.edit_gauntlet,
+        "콜라보 건틀릿[한국냥코사용불가]": levels.gauntlet.edit_collab_gauntlet,
         "타워": levels.towers.edit_tower,
-        "베히모스 컬링": levels.behemoth_culling.edit_behemoth_culling,
+        "레전드리스토리[빅 하앜마양 강림 클리어]": levels.behemoth_culling.edit_behemoth_culling,
         "미래편 시간 초과 점수": levels.itf_timed_scores.timed_scores,
         "도전 전투 점수": basic.basic_items.edit_challenge_battle,
         "튜토리얼 클리어": levels.clear_tutorial.clear_tutorial,
         "랭킹 점수(입문자의 전당)": basic.basic_items.edit_dojo_score,
         "수수께끼 단계 추가": levels.enigma_stages.edit_enigma_stages,
         "필리버스터 단계 재청산 허용": levels.allow_filibuster_clearing.allow_filibuster_clearing,
         "레전드 퀘스트": levels.legend_quest.edit_legend_quest,
```

### Comparing `Shark sac Korean editor-2.0.0/modkr/game_data_getter.py` & `Shark sac Korean editor-2.0.4/modkr/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/helper.py` & `Shark sac Korean editor-2.0.4/modkr/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,15 @@
 
 def ask_save_changes():
     """
     Ask if the user wants to save the changes
     """
     save = (
         user_input_handler.colored_input(
-            "You have unsaved changes. Would you like to save them? (&y&/&n&):"
+            "저장되지 않은 변경사항이 있습니다. 저장하시겠습니까? (&y&/&n&):"
         )
         == "y"
     )
     if save:
         current_path = get_save_path()
         temp_file_path = os.path.join(
             config_manager.get_app_data_folder(), "SAVE_DATA_temp"
@@ -830,15 +830,15 @@
 
 
 def ask_cc():
     """Ask the user for their country code"""
     default_gv = config_manager.get_config_value("DEFAULT_COUNTRY_CODE")
     if default_gv:
         if len(default_gv) == 2:
-            colored_text(f"Using default country code: &{default_gv}&")
+            colored_text(f"기본 국가 코드 사용: &{default_gv}&")
             return default_gv
 
     country_code = user_input_handler.colored_input(
         "국가 코드를 입력하세요(&en&, &jp&, &kr&, &tw&):"
     )
     return country_code
```

### Comparing `Shark sac Korean editor-2.0.0/modkr/item.py` & `Shark sac Korean editor-2.0.4/modkr/item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/locale_handler.py` & `Shark sac Korean editor-2.0.4/modkr/locale_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/managed_item.py` & `Shark sac Korean editor-2.0.4/modkr/managed_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/parse_save.py` & `Shark sac Korean editor-2.0.4/modkr/parse_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/patcher.py` & `Shark sac Korean editor-2.0.4/modkr/patcher.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/root_handler.py` & `Shark sac Korean editor-2.0.4/modkr/root_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/serialise_save.py` & `Shark sac Korean editor-2.0.4/modkr/serialise_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/server_handler.py` & `Shark sac Korean editor-2.0.4/modkr/server_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/tracker.py` & `Shark sac Korean editor-2.0.4/modkr/tracker.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/updater.py` & `Shark sac Korean editor-2.0.4/modkr/updater.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/modkr/user_input_handler.py` & `Shark sac Korean editor-2.0.4/modkr/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.0/setup.py` & `Shark sac Korean editor-2.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 basedir = path.abspath(path.dirname(__file__))
 with open(path.join(basedir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read().replace('\r\n', '\n')
 
 setup(
     name='Shark sac Korean editor',
-    version='2.0.0',
+    version='2.0.4',
     description='냥코에디터 한글화',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='익명',
     author_email='',
     url='https://github.com/sharkwodm/koreditor',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
```

