# Comparing `tmp/Shark sac Korean editor-2.0.2.tar.gz` & `tmp/Shark sac Korean editor-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shark sac Korean editor-2.0.2.tar", last modified: Sun Apr 30 10:45:45 2023, max compression
+gzip compressed data, was "Shark sac Korean editor-2.0.3.tar", last modified: Sun Apr 30 10:48:35 2023, max compression
```

## Comparing `Shark sac Korean editor-2.0.2.tar` & `Shark sac Korean editor-2.0.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.853406 Shark sac Korean editor-2.0.2/
--rw-rw-rw-   0        0        0      731 2023-04-30 10:45:45.852431 Shark sac Korean editor-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.763867 Shark sac Korean editor-2.0.2/Shark_sac_Korean_editor.egg-info/
--rw-rw-rw-   0        0        0      731 2023-04-30 10:45:45.000000 Shark sac Korean editor-2.0.2/Shark_sac_Korean_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-04-30 10:45:45.000000 Shark sac Korean editor-2.0.2/Shark_sac_Korean_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 10:45:45.000000 Shark sac Korean editor-2.0.2/Shark_sac_Korean_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 10:45:45.000000 Shark sac Korean editor-2.0.2/Shark_sac_Korean_editor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.786170 Shark sac Korean editor-2.0.2/modkr/
--rw-rw-rw-   0        0        0      281 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/__init__.py
--rw-rw-rw-   0        0        0     9549 2023-04-30 07:48:02.000000 Shark sac Korean editor-2.0.2/modkr/__main__.py
--rw-rw-rw-   0        0        0    10240 2023-04-26 10:58:08.000000 Shark sac Korean editor-2.0.2/modkr/adb_handler.py
--rw-rw-rw-   0        0        0    13764 2023-04-26 10:44:46.000000 Shark sac Korean editor-2.0.2/modkr/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-04-26 08:21:08.000000 Shark sac Korean editor-2.0.2/modkr/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.787164 Shark sac Korean editor-2.0.2/modkr/edits/
--rw-rw-rw-   0        0        0       67 2023-04-26 08:19:36.000000 Shark sac Korean editor-2.0.2/modkr/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.794954 Shark sac Korean editor-2.0.2/modkr/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8976 2023-04-27 12:50:49.000000 Shark sac Korean editor-2.0.2/modkr/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-04-26 08:20:39.000000 Shark sac Korean editor-2.0.2/modkr/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     4041 2023-04-27 11:46:25.000000 Shark sac Korean editor-2.0.2/modkr/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16755 2023-04-27 11:45:13.000000 Shark sac Korean editor-2.0.2/modkr/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.806134 Shark sac Korean editor-2.0.2/modkr/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8994 2023-04-27 02:57:22.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11449 2023-04-30 07:58:40.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3262 2023-04-26 08:44:31.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1083 2023-04-27 03:03:55.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2883 2023-04-27 03:19:09.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1277 2023-04-27 03:06:18.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     8065 2023-04-27 02:58:27.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4634 2023-04-30 08:11:09.000000 Shark sac Korean editor-2.0.2/modkr/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.811415 Shark sac Korean editor-2.0.2/modkr/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      333 2023-04-26 10:32:02.000000 Shark sac Korean editor-2.0.2/modkr/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2835 2023-04-26 08:38:24.000000 Shark sac Korean editor-2.0.2/modkr/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3399 2023-04-26 08:41:50.000000 Shark sac Korean editor-2.0.2/modkr/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4130 2023-04-26 08:40:01.000000 Shark sac Korean editor-2.0.2/modkr/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.830060 Shark sac Korean editor-2.0.2/modkr/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1057 2023-04-30 08:16:08.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/aku.py
--rw-rw-rw-   0        0        0      516 2023-04-26 09:33:48.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      869 2023-04-26 09:29:09.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      650 2023-04-26 10:31:23.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6389 2023-04-26 09:30:45.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     2062 2023-04-26 09:29:36.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1056 2023-04-26 09:28:52.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1481 2023-04-30 09:04:42.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4451 2023-04-27 03:25:53.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2361 2023-04-26 09:35:46.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3106 2023-04-27 03:25:08.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1227 2023-04-26 09:29:23.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8576 2023-04-27 03:28:15.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1082 2023-04-26 09:16:16.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      802 2023-04-30 08:25:27.000000 Shark sac Korean editor-2.0.2/modkr/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.846088 Shark sac Korean editor-2.0.2/modkr/edits/other/
--rw-rw-rw-   0        0        0      276 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3913 2023-04-26 10:25:28.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1124 2023-04-26 10:23:52.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2236 2023-04-26 09:44:49.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      698 2023-04-26 09:46:24.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3510 2023-04-26 10:22:39.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7140 2023-04-26 10:03:11.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4384 2023-04-26 10:17:15.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/missions.py
--rw-rw-rw-   0        0        0     1016 2023-04-26 10:13:14.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1657 2023-04-26 10:18:48.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1426 2023-04-26 10:16:14.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      356 2023-04-26 10:30:56.000000 Shark sac Korean editor-2.0.2/modkr/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:45:45.851460 Shark sac Korean editor-2.0.2/modkr/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1308 2023-04-26 11:02:30.000000 Shark sac Korean editor-2.0.2/modkr/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2795 2023-04-26 11:01:45.000000 Shark sac Korean editor-2.0.2/modkr/edits/save_management/load.py
--rw-rw-rw-   0        0        0      661 2023-04-26 10:58:58.000000 Shark sac Korean editor-2.0.2/modkr/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1906 2023-04-30 08:09:14.000000 Shark sac Korean editor-2.0.2/modkr/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    13855 2023-04-30 09:03:37.000000 Shark sac Korean editor-2.0.2/modkr/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-04-26 08:26:01.000000 Shark sac Korean editor-2.0.2/modkr/game_data_getter.py
--rw-rw-rw-   0        0        0    23001 2023-04-30 08:04:44.000000 Shark sac Korean editor-2.0.2/modkr/helper.py
--rw-rw-rw-   0        0        0     7075 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/item.py
--rw-rw-rw-   0        0        0     3505 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/managed_item.py
--rw-rw-rw-   0        0        0    66980 2023-04-25 17:12:37.000000 Shark sac Korean editor-2.0.2/modkr/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-04-30 07:47:55.000000 Shark sac Korean editor-2.0.2/modkr/patcher.py
--rw-rw-rw-   0        0        0     2450 2023-04-26 10:55:23.000000 Shark sac Korean editor-2.0.2/modkr/root_handler.py
--rw-rw-rw-   0        0        0    53823 2023-04-26 08:24:37.000000 Shark sac Korean editor-2.0.2/modkr/serialise_save.py
--rw-rw-rw-   0        0        0    25211 2023-04-26 10:54:03.000000 Shark sac Korean editor-2.0.2/modkr/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/tracker.py
--rw-rw-rw-   0        0        0     3544 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/updater.py
--rw-rw-rw-   0        0        0     8297 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.2/modkr/user_input_handler.py
--rw-rw-rw-   0        0        0       42 2023-04-30 10:45:45.853406 Shark sac Korean editor-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-04-30 10:45:28.000000 Shark sac Korean editor-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.550018 Shark sac Korean editor-2.0.3/
+-rw-rw-rw-   0        0        0      731 2023-04-30 10:48:35.549045 Shark sac Korean editor-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.460358 Shark sac Korean editor-2.0.3/Shark_sac_Korean_editor.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-04-30 10:48:35.000000 Shark sac Korean editor-2.0.3/Shark_sac_Korean_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-30 10:48:35.000000 Shark sac Korean editor-2.0.3/Shark_sac_Korean_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 10:48:35.000000 Shark sac Korean editor-2.0.3/Shark_sac_Korean_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 10:48:35.000000 Shark sac Korean editor-2.0.3/Shark_sac_Korean_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.479332 Shark sac Korean editor-2.0.3/modkr/
+-rw-rw-rw-   0        0        0      281 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/__init__.py
+-rw-rw-rw-   0        0        0     9549 2023-04-30 07:48:02.000000 Shark sac Korean editor-2.0.3/modkr/__main__.py
+-rw-rw-rw-   0        0        0    10240 2023-04-26 10:58:08.000000 Shark sac Korean editor-2.0.3/modkr/adb_handler.py
+-rw-rw-rw-   0        0        0    13764 2023-04-26 10:44:46.000000 Shark sac Korean editor-2.0.3/modkr/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-04-26 08:21:08.000000 Shark sac Korean editor-2.0.3/modkr/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.480306 Shark sac Korean editor-2.0.3/modkr/edits/
+-rw-rw-rw-   0        0        0       67 2023-04-26 08:19:36.000000 Shark sac Korean editor-2.0.3/modkr/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.486699 Shark sac Korean editor-2.0.3/modkr/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8976 2023-04-27 12:50:49.000000 Shark sac Korean editor-2.0.3/modkr/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-04-26 08:20:39.000000 Shark sac Korean editor-2.0.3/modkr/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     4041 2023-04-27 11:46:25.000000 Shark sac Korean editor-2.0.3/modkr/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16755 2023-04-27 11:45:13.000000 Shark sac Korean editor-2.0.3/modkr/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.495872 Shark sac Korean editor-2.0.3/modkr/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8994 2023-04-27 02:57:22.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11449 2023-04-30 07:58:40.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3262 2023-04-26 08:44:31.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1083 2023-04-27 03:03:55.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2883 2023-04-27 03:19:09.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1277 2023-04-27 03:06:18.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     8065 2023-04-27 02:58:27.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1900 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4634 2023-04-30 08:11:09.000000 Shark sac Korean editor-2.0.3/modkr/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.500763 Shark sac Korean editor-2.0.3/modkr/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-04-26 10:32:02.000000 Shark sac Korean editor-2.0.3/modkr/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2835 2023-04-26 08:38:24.000000 Shark sac Korean editor-2.0.3/modkr/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3399 2023-04-26 08:41:50.000000 Shark sac Korean editor-2.0.3/modkr/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4130 2023-04-26 08:40:01.000000 Shark sac Korean editor-2.0.3/modkr/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.516925 Shark sac Korean editor-2.0.3/modkr/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-04-30 08:16:08.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      516 2023-04-26 09:33:48.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      869 2023-04-26 09:29:09.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      650 2023-04-26 10:31:23.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6389 2023-04-26 09:30:45.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     2062 2023-04-26 09:29:36.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1056 2023-04-26 09:28:52.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1481 2023-04-30 09:04:42.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4451 2023-04-27 03:25:53.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2361 2023-04-26 09:35:46.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3106 2023-04-27 03:25:08.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1227 2023-04-26 09:29:23.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8576 2023-04-27 03:28:15.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1082 2023-04-26 09:16:16.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      802 2023-04-30 08:25:27.000000 Shark sac Korean editor-2.0.3/modkr/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.532544 Shark sac Korean editor-2.0.3/modkr/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3913 2023-04-26 10:25:28.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1124 2023-04-26 10:23:52.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2236 2023-04-26 09:44:49.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      698 2023-04-26 09:46:24.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3510 2023-04-26 10:22:39.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7140 2023-04-26 10:03:11.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4384 2023-04-26 10:17:15.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/missions.py
+-rw-rw-rw-   0        0        0     1016 2023-04-26 10:13:14.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1657 2023-04-26 10:18:48.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1426 2023-04-26 10:16:14.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      356 2023-04-26 10:30:56.000000 Shark sac Korean editor-2.0.3/modkr/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-30 10:48:35.542953 Shark sac Korean editor-2.0.3/modkr/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1308 2023-04-26 11:02:30.000000 Shark sac Korean editor-2.0.3/modkr/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2795 2023-04-26 11:01:45.000000 Shark sac Korean editor-2.0.3/modkr/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      661 2023-04-26 10:58:58.000000 Shark sac Korean editor-2.0.3/modkr/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1906 2023-04-30 08:09:14.000000 Shark sac Korean editor-2.0.3/modkr/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    13855 2023-04-30 09:03:37.000000 Shark sac Korean editor-2.0.3/modkr/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-04-26 08:26:01.000000 Shark sac Korean editor-2.0.3/modkr/game_data_getter.py
+-rw-rw-rw-   0        0        0    23001 2023-04-30 08:04:44.000000 Shark sac Korean editor-2.0.3/modkr/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/item.py
+-rw-rw-rw-   0        0        0     3505 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/managed_item.py
+-rw-rw-rw-   0        0        0    66980 2023-04-25 17:12:37.000000 Shark sac Korean editor-2.0.3/modkr/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-04-30 07:47:55.000000 Shark sac Korean editor-2.0.3/modkr/patcher.py
+-rw-rw-rw-   0        0        0     2450 2023-04-26 10:55:23.000000 Shark sac Korean editor-2.0.3/modkr/root_handler.py
+-rw-rw-rw-   0        0        0    53823 2023-04-26 08:24:37.000000 Shark sac Korean editor-2.0.3/modkr/serialise_save.py
+-rw-rw-rw-   0        0        0    25211 2023-04-26 10:54:03.000000 Shark sac Korean editor-2.0.3/modkr/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/tracker.py
+-rw-rw-rw-   0        0        0     3544 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.3/modkr/user_input_handler.py
+-rw-rw-rw-   0        0        0       42 2023-04-30 10:48:35.550018 Shark sac Korean editor-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-04-30 10:48:20.000000 Shark sac Korean editor-2.0.3/setup.py
```

### Comparing `Shark sac Korean editor-2.0.2/PKG-INFO` & `Shark sac Korean editor-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shark sac Korean editor
-Version: 2.0.2
+Version: 2.0.3
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-2.0.2/Shark_sac_Korean_editor.egg-info/PKG-INFO` & `Shark sac Korean editor-2.0.3/Shark_sac_Korean_editor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shark-sac-Korean-editor
-Version: 2.0.2
+Version: 2.0.3
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-2.0.2/Shark_sac_Korean_editor.egg-info/SOURCES.txt` & `Shark sac Korean editor-2.0.3/Shark_sac_Korean_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/__main__.py` & `Shark sac Korean editor-2.0.3/modkr/__main__.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/adb_handler.py` & `Shark sac Korean editor-2.0.3/modkr/adb_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/config_manager.py` & `Shark sac Korean editor-2.0.3/modkr/config_manager.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/csv_handler.py` & `Shark sac Korean editor-2.0.3/modkr/csv_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/basic/basic_items.py` & `Shark sac Korean editor-2.0.3/modkr/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/basic/catfruit.py` & `Shark sac Korean editor-2.0.3/modkr/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/basic/catseyes.py` & `Shark sac Korean editor-2.0.3/modkr/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/basic/ototo_base_mats.py` & `Shark sac Korean editor-2.0.3/modkr/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/basic/talent_orbs.py` & `Shark sac Korean editor-2.0.3/modkr/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/basic/talent_orbs_new.py` & `Shark sac Korean editor-2.0.3/modkr/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/cat_helper.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/cat_id_selector.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/chara_drop.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/clear_cat_guide.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/evolve_cats.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/get_remove_cats.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/talents.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/upgrade_blue.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/cats/upgrade_cats.py` & `Shark sac Korean editor-2.0.3/modkr/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/gamototo/gamatoto_xp.py` & `Shark sac Korean editor-2.0.3/modkr/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/gamototo/helpers.py` & `Shark sac Korean editor-2.0.3/modkr/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/gamototo/ototo_cat_cannon.py` & `Shark sac Korean editor-2.0.3/modkr/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/aku.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/allow_filibuster_clearing.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/allow_filibuster_clearing.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/behemoth_culling.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/clear_tutorial.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/enigma_stages.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/event_stages.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/gauntlet.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/itf_timed_scores.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/legend_quest.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/main_story.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/outbreaks.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/story_level_id_selector.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/towers.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/treasures.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/uncanny.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/levels/unlock_aku_realm.py` & `Shark sac Korean editor-2.0.3/modkr/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/cat_shrine.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/claim_user_rank_rewards.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/create_new_account.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/fix_elsewhere.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/fix_time_issues.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/get_gold_pass.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/meow_medals.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/missions.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/play_time.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/scheme_item.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/trade_progress.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/other/unlock_enemy_guide.py` & `Shark sac Korean editor-2.0.3/modkr/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/save_management/convert.py` & `Shark sac Korean editor-2.0.3/modkr/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/save_management/load.py` & `Shark sac Korean editor-2.0.3/modkr/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/save_management/other.py` & `Shark sac Korean editor-2.0.3/modkr/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/save_management/save.py` & `Shark sac Korean editor-2.0.3/modkr/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/edits/save_management/server_upload.py` & `Shark sac Korean editor-2.0.3/modkr/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/feature_handler.py` & `Shark sac Korean editor-2.0.3/modkr/feature_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/game_data_getter.py` & `Shark sac Korean editor-2.0.3/modkr/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/helper.py` & `Shark sac Korean editor-2.0.3/modkr/helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/item.py` & `Shark sac Korean editor-2.0.3/modkr/item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/locale_handler.py` & `Shark sac Korean editor-2.0.3/modkr/locale_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/managed_item.py` & `Shark sac Korean editor-2.0.3/modkr/managed_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/parse_save.py` & `Shark sac Korean editor-2.0.3/modkr/parse_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/patcher.py` & `Shark sac Korean editor-2.0.3/modkr/patcher.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/root_handler.py` & `Shark sac Korean editor-2.0.3/modkr/root_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/serialise_save.py` & `Shark sac Korean editor-2.0.3/modkr/serialise_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/server_handler.py` & `Shark sac Korean editor-2.0.3/modkr/server_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/tracker.py` & `Shark sac Korean editor-2.0.3/modkr/tracker.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/updater.py` & `Shark sac Korean editor-2.0.3/modkr/updater.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/modkr/user_input_handler.py` & `Shark sac Korean editor-2.0.3/modkr/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-2.0.2/setup.py` & `Shark sac Korean editor-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 basedir = path.abspath(path.dirname(__file__))
 with open(path.join(basedir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read().replace('\r\n', '\n')
 
 setup(
     name='Shark sac Korean editor',
-    version='2.0.2',
+    version='2.0.3',
     description='냥코에디터 한글화',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='익명',
     author_email='',
     url='https://github.com/sharkwodm/koreditor',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
```

