# Comparing `tmp/space-invaders-0.3.0.tar.gz` & `tmp/space-invaders-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.3.0.tar", last modified: Sun Apr 30 16:15:49 2023, max compression
+gzip compressed data, was "space-invaders-0.3.2.tar", last modified: Sun Apr 30 17:24:08 2023, max compression
```

## Comparing `space-invaders-0.3.0.tar` & `space-invaders-0.3.2.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.148253 space-invaders-0.3.0/
--rw-rw-rw-   0        0        0      295 2023-04-29 00:00:41.000000 space-invaders-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2339 2023-04-30 16:15:49.148253 space-invaders-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-30 16:15:49.148253 space-invaders-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-04-30 16:15:27.000000 space-invaders-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.107167 space-invaders-0.3.0/space_invaders/
-drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.120240 space-invaders-0.3.0/space_invaders/Fonts/
--rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.3.0/space_invaders/Fonts/AGENCYB.TTF
--rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.3.0/space_invaders/Fonts/AGENCYR.TTF
--rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.3.0/space_invaders/Fonts/Alien Invader Italic.ttf
--rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.3.0/space_invaders/Fonts/Alien Invader.ttf
--rw-rw-rw-   0        0        0     2116 2023-04-29 01:33:08.000000 space-invaders-0.3.0/space_invaders/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.131746 space-invaders-0.3.0/space_invaders/Sounds/
--rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.3.0/space_invaders/Sounds/122255__jivatma07__level_complete.wav
--rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.3.0/space_invaders/Sounds/156895__halgrimm__a-shot.wav
--rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.3.0/space_invaders/Sounds/18380__inferno__hvrl.wav
--rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.3.0/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
--rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.3.0/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav
--rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.3.0/space_invaders/Sounds/353775__samueloak89__next-scene.mp3
--rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.3.0/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
--rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.3.0/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav
--rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.3.0/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
--rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.3.0/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav
--rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.3.0/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
-drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.143253 space-invaders-0.3.0/space_invaders/Sprites/
--rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.3.0/space_invaders/Sprites/background.png
--rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.3.0/space_invaders/Sprites/default_enemy_gun.png
--rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.3.0/space_invaders/Sprites/default_enemy_projectile.png
--rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.3.0/space_invaders/Sprites/default_enemy_ship.png
--rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.3.0/space_invaders/Sprites/default_gun.png
--rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.3.0/space_invaders/Sprites/default_gun_pickup.png
--rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.3.0/space_invaders/Sprites/default_projectile.png
--rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.3.0/space_invaders/Sprites/default_ship.png
--rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.3.0/space_invaders/Sprites/explosion.png
--rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.3.0/space_invaders/Sprites/fire_rate_booster.png
--rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.3.0/space_invaders/Sprites/life.png
--rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.3.0/space_invaders/Sprites/medium_heal.png
--rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.3.0/space_invaders/Sprites/minigun.png
--rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.3.0/space_invaders/Sprites/minigun_pickup.png
--rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.3.0/space_invaders/Sprites/minigun_projectile.png
--rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.3.0/space_invaders/Sprites/repair.png
--rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.3.0/space_invaders/Sprites/rocket_gun.png
--rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.3.0/space_invaders/Sprites/rocket_gun_pickup.png
--rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.3.0/space_invaders/Sprites/rocket_projectile.png
--rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.3.0/space_invaders/Sprites/ship_explosion.png
--rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.3.0/space_invaders/Sprites/small_heal.png
-drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.144253 space-invaders-0.3.0/space_invaders/TestResults/
--rw-rw-rw-   0        0        0      157 2023-04-28 10:17:05.000000 space-invaders-0.3.0/space_invaders/TestResults/flake8.txt
--rw-rw-rw-   0        0        0      146 2023-04-28 10:06:54.000000 space-invaders-0.3.0/space_invaders/TestResults/pycodestyle.txt
--rw-rw-rw-   0        0        0      452 2023-04-30 00:05:08.000000 space-invaders-0.3.0/space_invaders/__entrypoint__.py
--rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.3.0/space_invaders/__init__.py
--rw-rw-rw-   0        0        0     4768 2023-04-30 15:23:37.000000 space-invaders-0.3.0/space_invaders/config.py
--rw-rw-rw-   0        0        0     6813 2023-04-30 15:23:37.000000 space-invaders-0.3.0/space_invaders/entity.py
--rw-rw-rw-   0        0        0    21244 2023-04-30 14:20:42.000000 space-invaders-0.3.0/space_invaders/level.py
--rw-rw-rw-   0        0        0    18069 2023-04-30 16:08:55.000000 space-invaders-0.3.0/space_invaders/main.py
--rw-rw-rw-   0        0        0     5857 2023-04-30 15:23:37.000000 space-invaders-0.3.0/space_invaders/pickup.py
--rw-rw-rw-   0        0        0    18491 2023-04-30 15:36:04.000000 space-invaders-0.3.0/space_invaders/spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.147254 space-invaders-0.3.0/space_invaders/tests/
--rw-rw-rw-   0        0        0        0 2023-04-29 14:49:16.000000 space-invaders-0.3.0/space_invaders/tests/__init__.py
--rw-rw-rw-   0        0        0     3467 2023-04-29 14:27:17.000000 space-invaders-0.3.0/space_invaders/tests/test_entity.py
--rw-rw-rw-   0        0        0     2704 2023-04-29 17:32:02.000000 space-invaders-0.3.0/space_invaders/tests/test_level.py
--rw-rw-rw-   0        0        0     2031 2023-04-29 19:47:22.000000 space-invaders-0.3.0/space_invaders/tests/test_main.py
--rw-rw-rw-   0        0        0     1494 2023-04-29 15:11:06.000000 space-invaders-0.3.0/space_invaders/tests/test_pickup.py
--rw-rw-rw-   0        0        0     3513 2023-04-30 15:23:37.000000 space-invaders-0.3.0/space_invaders/tests/test_spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.117240 space-invaders-0.3.0/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     2339 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2481 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 17:24:08.073749 space-invaders-0.3.2/
+-rw-rw-rw-   0        0        0      333 2023-04-30 16:24:01.000000 space-invaders-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3314 2023-04-30 17:24:08.072748 space-invaders-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-30 17:24:08.073749 space-invaders-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-04-30 17:23:52.000000 space-invaders-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:24:08.013621 space-invaders-0.3.2/space_invaders/
+drwxrwxrwx   0        0        0        0 2023-04-30 17:24:08.027600 space-invaders-0.3.2/space_invaders/Fonts/
+-rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.3.2/space_invaders/Fonts/AGENCYB.TTF
+-rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.3.2/space_invaders/Fonts/AGENCYR.TTF
+-rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.3.2/space_invaders/Fonts/Alien Invader Italic.ttf
+-rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.3.2/space_invaders/Fonts/Alien Invader.ttf
+-rw-rw-rw-   0        0        0     3065 2023-04-30 17:23:23.000000 space-invaders-0.3.2/space_invaders/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 17:24:08.039641 space-invaders-0.3.2/space_invaders/Sounds/
+-rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.3.2/space_invaders/Sounds/122255__jivatma07__level_complete.wav
+-rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.3.2/space_invaders/Sounds/156895__halgrimm__a-shot.wav
+-rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.3.2/space_invaders/Sounds/18380__inferno__hvrl.wav
+-rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.3.2/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
+-rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.3.2/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav
+-rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.3.2/space_invaders/Sounds/353775__samueloak89__next-scene.mp3
+-rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.3.2/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
+-rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.3.2/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav
+-rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.3.2/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
+-rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.3.2/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav
+-rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.3.2/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
+drwxrwxrwx   0        0        0        0 2023-04-30 17:24:08.051785 space-invaders-0.3.2/space_invaders/Sprites/
+-rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.3.2/space_invaders/Sprites/background.png
+-rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.3.2/space_invaders/Sprites/default_enemy_gun.png
+-rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.3.2/space_invaders/Sprites/default_enemy_projectile.png
+-rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.3.2/space_invaders/Sprites/default_enemy_ship.png
+-rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.3.2/space_invaders/Sprites/default_gun.png
+-rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.3.2/space_invaders/Sprites/default_gun_pickup.png
+-rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.3.2/space_invaders/Sprites/default_projectile.png
+-rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.3.2/space_invaders/Sprites/default_ship.png
+-rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.3.2/space_invaders/Sprites/explosion.png
+-rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.3.2/space_invaders/Sprites/fire_rate_booster.png
+-rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.3.2/space_invaders/Sprites/life.png
+-rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.3.2/space_invaders/Sprites/medium_heal.png
+-rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.3.2/space_invaders/Sprites/minigun.png
+-rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.3.2/space_invaders/Sprites/minigun_pickup.png
+-rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.3.2/space_invaders/Sprites/minigun_projectile.png
+-rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.3.2/space_invaders/Sprites/repair.png
+-rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.3.2/space_invaders/Sprites/rocket_gun.png
+-rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.3.2/space_invaders/Sprites/rocket_gun_pickup.png
+-rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.3.2/space_invaders/Sprites/rocket_projectile.png
+-rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.3.2/space_invaders/Sprites/ship_explosion.png
+-rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.3.2/space_invaders/Sprites/small_heal.png
+drwxrwxrwx   0        0        0        0 2023-04-30 17:24:08.052784 space-invaders-0.3.2/space_invaders/TestResults/
+-rw-rw-rw-   0        0        0      177 2023-04-30 16:25:35.000000 space-invaders-0.3.2/space_invaders/TestResults/flake8.txt
+-rw-rw-rw-   0        0        0      164 2023-04-30 16:25:56.000000 space-invaders-0.3.2/space_invaders/TestResults/pycodestyle.txt
+-rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.3.2/space_invaders/__init__.py
+-rw-rw-rw-   0        0        0     4768 2023-04-30 15:23:37.000000 space-invaders-0.3.2/space_invaders/config.py
+-rw-rw-rw-   0        0        0     6813 2023-04-30 15:23:37.000000 space-invaders-0.3.2/space_invaders/entity.py
+-rw-rw-rw-   0        0        0    21244 2023-04-30 14:20:42.000000 space-invaders-0.3.2/space_invaders/level.py
+-rw-rw-rw-   0        0        0    18069 2023-04-30 16:08:55.000000 space-invaders-0.3.2/space_invaders/main.py
+-rw-rw-rw-   0        0        0     5857 2023-04-30 15:23:37.000000 space-invaders-0.3.2/space_invaders/pickup.py
+-rw-rw-rw-   0        0        0      452 2023-04-30 00:05:08.000000 space-invaders-0.3.2/space_invaders/run_game.py
+-rw-rw-rw-   0        0        0    18493 2023-04-30 16:25:23.000000 space-invaders-0.3.2/space_invaders/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:24:08.071747 space-invaders-0.3.2/space_invaders/tests/
+-rw-rw-rw-   0        0        0     3142 2023-04-29 19:50:35.000000 space-invaders-0.3.2/space_invaders/tests/INFO.md
+-rw-rw-rw-   0        0        0        0 2023-04-29 14:49:16.000000 space-invaders-0.3.2/space_invaders/tests/__init__.py
+-rw-rw-rw-   0        0        0     3467 2023-04-29 14:27:17.000000 space-invaders-0.3.2/space_invaders/tests/test_entity.py
+-rw-rw-rw-   0        0        0     2704 2023-04-29 17:32:02.000000 space-invaders-0.3.2/space_invaders/tests/test_level.py
+-rw-rw-rw-   0        0        0     2031 2023-04-29 19:47:22.000000 space-invaders-0.3.2/space_invaders/tests/test_main.py
+-rw-rw-rw-   0        0        0     1494 2023-04-29 15:11:06.000000 space-invaders-0.3.2/space_invaders/tests/test_pickup.py
+-rw-rw-rw-   0        0        0     3513 2023-04-30 15:23:37.000000 space-invaders-0.3.2/space_invaders/tests/test_spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:24:08.024600 space-invaders-0.3.2/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     3314 2023-04-30 17:24:07.000000 space-invaders-0.3.2/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2023-04-30 17:24:07.000000 space-invaders-0.3.2/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 17:24:07.000000 space-invaders-0.3.2/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-30 17:24:07.000000 space-invaders-0.3.2/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-30 17:24:07.000000 space-invaders-0.3.2/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-30 17:24:07.000000 space-invaders-0.3.2/space_invaders.egg-info/top_level.txt
```

### Comparing `space-invaders-0.3.0/space_invaders/Fonts/AGENCYB.TTF` & `space-invaders-0.3.2/space_invaders/Fonts/AGENCYB.TTF`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Fonts/AGENCYR.TTF` & `space-invaders-0.3.2/space_invaders/Fonts/AGENCYR.TTF`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Fonts/Alien Invader Italic.ttf` & `space-invaders-0.3.2/space_invaders/Fonts/Alien Invader Italic.ttf`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Fonts/Alien Invader.ttf` & `space-invaders-0.3.2/space_invaders/Fonts/Alien Invader.ttf`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/122255__jivatma07__level_complete.wav` & `space-invaders-0.3.2/space_invaders/Sounds/122255__jivatma07__level_complete.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/156895__halgrimm__a-shot.wav` & `space-invaders-0.3.2/space_invaders/Sounds/156895__halgrimm__a-shot.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/18380__inferno__hvrl.wav` & `space-invaders-0.3.2/space_invaders/Sounds/18380__inferno__hvrl.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav` & `space-invaders-0.3.2/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav` & `space-invaders-0.3.2/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/353775__samueloak89__next-scene.mp3` & `space-invaders-0.3.2/space_invaders/Sounds/353775__samueloak89__next-scene.mp3`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg` & `space-invaders-0.3.2/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav` & `space-invaders-0.3.2/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav` & `space-invaders-0.3.2/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav` & `space-invaders-0.3.2/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav` & `space-invaders-0.3.2/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/background.png` & `space-invaders-0.3.2/space_invaders/Sprites/background.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/default_enemy_gun.png` & `space-invaders-0.3.2/space_invaders/Sprites/default_enemy_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/default_enemy_projectile.png` & `space-invaders-0.3.2/space_invaders/Sprites/default_enemy_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/default_enemy_ship.png` & `space-invaders-0.3.2/space_invaders/Sprites/default_enemy_ship.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/default_gun.png` & `space-invaders-0.3.2/space_invaders/Sprites/default_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/default_gun_pickup.png` & `space-invaders-0.3.2/space_invaders/Sprites/default_gun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/default_projectile.png` & `space-invaders-0.3.2/space_invaders/Sprites/default_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/default_ship.png` & `space-invaders-0.3.2/space_invaders/Sprites/default_ship.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/explosion.png` & `space-invaders-0.3.2/space_invaders/Sprites/explosion.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/fire_rate_booster.png` & `space-invaders-0.3.2/space_invaders/Sprites/fire_rate_booster.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/life.png` & `space-invaders-0.3.2/space_invaders/Sprites/life.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/medium_heal.png` & `space-invaders-0.3.2/space_invaders/Sprites/medium_heal.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/minigun.png` & `space-invaders-0.3.2/space_invaders/Sprites/minigun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/minigun_pickup.png` & `space-invaders-0.3.2/space_invaders/Sprites/minigun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/minigun_projectile.png` & `space-invaders-0.3.2/space_invaders/Sprites/minigun_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/repair.png` & `space-invaders-0.3.2/space_invaders/Sprites/repair.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/rocket_gun.png` & `space-invaders-0.3.2/space_invaders/Sprites/rocket_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/rocket_gun_pickup.png` & `space-invaders-0.3.2/space_invaders/Sprites/rocket_gun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/rocket_projectile.png` & `space-invaders-0.3.2/space_invaders/Sprites/rocket_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/ship_explosion.png` & `space-invaders-0.3.2/space_invaders/Sprites/ship_explosion.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/Sprites/small_heal.png` & `space-invaders-0.3.2/space_invaders/Sprites/small_heal.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/config.py` & `space-invaders-0.3.2/space_invaders/config.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/entity.py` & `space-invaders-0.3.2/space_invaders/entity.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/level.py` & `space-invaders-0.3.2/space_invaders/level.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/main.py` & `space-invaders-0.3.2/space_invaders/main.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/pickup.py` & `space-invaders-0.3.2/space_invaders/pickup.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/spaceship.py` & `space-invaders-0.3.2/space_invaders/spaceship.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,27 +62,27 @@
         """
         Sets the position of the ship to the given vector
         @param vec the new position (center)
         """
         self._image_rect.center = vec
         for i, vertex in enumerate(self._collider_relative_vertices):
             self._collider[i] = (vertex[0] + vec[0],
-                                vertex[1] + vec[1])
+                                 vertex[1] + vec[1])
         for gun in self._guns:
             gun.set_position(vec)
 
     def move(self, vec):
         """
         Moves the ship by the given vector
         @param vec the move
         """
         self._image_rect.move_ip(vec[0], vec[1])
         for i, vertex in enumerate(self._collider_relative_vertices):
             self._collider[i] = (self._image_rect.center[0] + vertex[0],
-                                self._image_rect.center[1] + vertex[1])
+                                 self._image_rect.center[1] + vertex[1])
         for gun in self._guns:
             gun.move(vec)
 
     def next_gun(self):
         """Cycles the selected gun to be the next available one"""
         self._active_gun += 1
         self._active_gun %= len(self._guns)
```

### Comparing `space-invaders-0.3.0/space_invaders/tests/test_entity.py` & `space-invaders-0.3.2/space_invaders/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/tests/test_level.py` & `space-invaders-0.3.2/space_invaders/tests/test_level.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/tests/test_main.py` & `space-invaders-0.3.2/space_invaders/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/tests/test_pickup.py` & `space-invaders-0.3.2/space_invaders/tests/test_pickup.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders/tests/test_spaceship.py` & `space-invaders-0.3.2/space_invaders/tests/test_spaceship.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.3.0/space_invaders.egg-info/SOURCES.txt` & `space-invaders-0.3.2/space_invaders.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 MANIFEST.in
 setup.py
 space_invaders/README.md
-space_invaders/__entrypoint__.py
 space_invaders/__init__.py
 space_invaders/config.py
 space_invaders/entity.py
 space_invaders/level.py
 space_invaders/main.py
 space_invaders/pickup.py
+space_invaders/run_game.py
 space_invaders/spaceship.py
 space_invaders.egg-info/PKG-INFO
 space_invaders.egg-info/SOURCES.txt
 space_invaders.egg-info/dependency_links.txt
 space_invaders.egg-info/entry_points.txt
 space_invaders.egg-info/requires.txt
 space_invaders.egg-info/top_level.txt
@@ -49,13 +49,14 @@
 space_invaders/Sprites/rocket_gun.png
 space_invaders/Sprites/rocket_gun_pickup.png
 space_invaders/Sprites/rocket_projectile.png
 space_invaders/Sprites/ship_explosion.png
 space_invaders/Sprites/small_heal.png
 space_invaders/TestResults/flake8.txt
 space_invaders/TestResults/pycodestyle.txt
+space_invaders/tests/INFO.md
 space_invaders/tests/__init__.py
 space_invaders/tests/test_entity.py
 space_invaders/tests/test_level.py
 space_invaders/tests/test_main.py
 space_invaders/tests/test_pickup.py
 space_invaders/tests/test_spaceship.py
```

