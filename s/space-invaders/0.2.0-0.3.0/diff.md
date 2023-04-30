# Comparing `tmp/space-invaders-0.2.0.tar.gz` & `tmp/space-invaders-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space-invaders-0.2.0.tar", last modified: Sat Apr 29 19:55:48 2023, max compression
+gzip compressed data, was "space-invaders-0.3.0.tar", last modified: Sun Apr 30 16:15:49 2023, max compression
```

## Comparing `space-invaders-0.2.0.tar` & `space-invaders-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.883988 space-invaders-0.2.0/
--rw-rw-rw-   0        0        0      295 2023-04-29 00:00:41.000000 space-invaders-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2339 2023-04-29 19:55:48.882988 space-invaders-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-29 19:55:48.883988 space-invaders-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-04-29 19:55:41.000000 space-invaders-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.840769 space-invaders-0.2.0/space_invaders/
-drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.851783 space-invaders-0.2.0/space_invaders/Fonts/
--rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.2.0/space_invaders/Fonts/AGENCYB.TTF
--rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.2.0/space_invaders/Fonts/AGENCYR.TTF
--rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.2.0/space_invaders/Fonts/Alien Invader Italic.ttf
--rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.2.0/space_invaders/Fonts/Alien Invader.ttf
--rw-rw-rw-   0        0        0     2116 2023-04-29 01:33:08.000000 space-invaders-0.2.0/space_invaders/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.864823 space-invaders-0.2.0/space_invaders/Sounds/
--rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.2.0/space_invaders/Sounds/122255__jivatma07__level_complete.wav
--rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.2.0/space_invaders/Sounds/156895__halgrimm__a-shot.wav
--rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.2.0/space_invaders/Sounds/18380__inferno__hvrl.wav
--rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.2.0/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
--rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.2.0/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav
--rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.2.0/space_invaders/Sounds/353775__samueloak89__next-scene.mp3
--rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.2.0/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
--rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.2.0/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav
--rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.2.0/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
--rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.2.0/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav
--rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.2.0/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
-drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.878988 space-invaders-0.2.0/space_invaders/Sprites/
--rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.2.0/space_invaders/Sprites/background.png
--rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.2.0/space_invaders/Sprites/default_enemy_gun.png
--rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.2.0/space_invaders/Sprites/default_enemy_projectile.png
--rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.2.0/space_invaders/Sprites/default_enemy_ship.png
--rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.2.0/space_invaders/Sprites/default_gun.png
--rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.2.0/space_invaders/Sprites/default_gun_pickup.png
--rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.2.0/space_invaders/Sprites/default_projectile.png
--rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.2.0/space_invaders/Sprites/default_ship.png
--rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.2.0/space_invaders/Sprites/explosion.png
--rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.2.0/space_invaders/Sprites/fire_rate_booster.png
--rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.2.0/space_invaders/Sprites/life.png
--rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.2.0/space_invaders/Sprites/medium_heal.png
--rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.2.0/space_invaders/Sprites/minigun.png
--rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.2.0/space_invaders/Sprites/minigun_pickup.png
--rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.2.0/space_invaders/Sprites/minigun_projectile.png
--rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.2.0/space_invaders/Sprites/repair.png
--rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.2.0/space_invaders/Sprites/rocket_gun.png
--rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.2.0/space_invaders/Sprites/rocket_gun_pickup.png
--rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.2.0/space_invaders/Sprites/rocket_projectile.png
--rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.2.0/space_invaders/Sprites/ship_explosion.png
--rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.2.0/space_invaders/Sprites/small_heal.png
-drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.879988 space-invaders-0.2.0/space_invaders/TestResults/
--rw-rw-rw-   0        0        0      157 2023-04-28 10:17:05.000000 space-invaders-0.2.0/space_invaders/TestResults/flake8.txt
--rw-rw-rw-   0        0        0      146 2023-04-28 10:06:54.000000 space-invaders-0.2.0/space_invaders/TestResults/pycodestyle.txt
--rw-rw-rw-   0        0        0      225 2023-04-29 19:24:05.000000 space-invaders-0.2.0/space_invaders/__entrypoint__.py
--rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.2.0/space_invaders/__init__.py
--rw-rw-rw-   0        0        0     4006 2023-04-29 19:22:53.000000 space-invaders-0.2.0/space_invaders/config.py
--rw-rw-rw-   0        0        0     3516 2023-04-29 19:47:34.000000 space-invaders-0.2.0/space_invaders/entity.py
--rw-rw-rw-   0        0        0    17495 2023-04-29 17:30:28.000000 space-invaders-0.2.0/space_invaders/level.py
--rw-rw-rw-   0        0        0    16049 2023-04-29 19:33:35.000000 space-invaders-0.2.0/space_invaders/main.py
--rw-rw-rw-   0        0        0     3296 2023-04-29 19:33:02.000000 space-invaders-0.2.0/space_invaders/pickup.py
--rw-rw-rw-   0        0        0    11389 2023-04-29 14:27:17.000000 space-invaders-0.2.0/space_invaders/spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.882988 space-invaders-0.2.0/space_invaders/tests/
--rw-rw-rw-   0        0        0        0 2023-04-29 14:49:16.000000 space-invaders-0.2.0/space_invaders/tests/__init__.py
--rw-rw-rw-   0        0        0     3467 2023-04-29 14:27:17.000000 space-invaders-0.2.0/space_invaders/tests/test_entity.py
--rw-rw-rw-   0        0        0     2704 2023-04-29 17:32:02.000000 space-invaders-0.2.0/space_invaders/tests/test_level.py
--rw-rw-rw-   0        0        0     2031 2023-04-29 19:47:22.000000 space-invaders-0.2.0/space_invaders/tests/test_main.py
--rw-rw-rw-   0        0        0     1494 2023-04-29 15:11:06.000000 space-invaders-0.2.0/space_invaders/tests/test_pickup.py
--rw-rw-rw-   0        0        0     3512 2023-04-29 14:40:40.000000 space-invaders-0.2.0/space_invaders/tests/test_spaceship.py
-drwxrwxrwx   0        0        0        0 2023-04-29 19:55:48.849784 space-invaders-0.2.0/space_invaders.egg-info/
--rw-rw-rw-   0        0        0     2339 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2481 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 19:55:48.000000 space-invaders-0.2.0/space_invaders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.148253 space-invaders-0.3.0/
+-rw-rw-rw-   0        0        0      295 2023-04-29 00:00:41.000000 space-invaders-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2339 2023-04-30 16:15:49.148253 space-invaders-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-30 16:15:49.148253 space-invaders-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      618 2023-04-30 16:15:27.000000 space-invaders-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.107167 space-invaders-0.3.0/space_invaders/
+drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.120240 space-invaders-0.3.0/space_invaders/Fonts/
+-rw-rw-rw-   0        0        0    60656 2023-01-01 13:11:56.000000 space-invaders-0.3.0/space_invaders/Fonts/AGENCYB.TTF
+-rw-rw-rw-   0        0        0    58920 2023-01-01 13:11:56.000000 space-invaders-0.3.0/space_invaders/Fonts/AGENCYR.TTF
+-rw-rw-rw-   0        0        0    17652 2023-04-21 15:04:24.000000 space-invaders-0.3.0/space_invaders/Fonts/Alien Invader Italic.ttf
+-rw-rw-rw-   0        0        0    16580 2023-04-21 15:04:24.000000 space-invaders-0.3.0/space_invaders/Fonts/Alien Invader.ttf
+-rw-rw-rw-   0        0        0     2116 2023-04-29 01:33:08.000000 space-invaders-0.3.0/space_invaders/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.131746 space-invaders-0.3.0/space_invaders/Sounds/
+-rw-rw-rw-   0        0        0   195360 2023-04-24 10:56:13.000000 space-invaders-0.3.0/space_invaders/Sounds/122255__jivatma07__level_complete.wav
+-rw-rw-rw-   0        0        0   123868 2023-04-24 10:52:01.000000 space-invaders-0.3.0/space_invaders/Sounds/156895__halgrimm__a-shot.wav
+-rw-rw-rw-   0        0        0    49408 2023-04-24 10:52:53.000000 space-invaders-0.3.0/space_invaders/Sounds/18380__inferno__hvrl.wav
+-rw-rw-rw-   0        0        0  1130484 2023-04-24 10:55:11.000000 space-invaders-0.3.0/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav
+-rw-rw-rw-   0        0        0  6578108 2023-04-24 11:58:55.000000 space-invaders-0.3.0/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav
+-rw-rw-rw-   0        0        0   260856 2023-04-27 21:51:59.000000 space-invaders-0.3.0/space_invaders/Sounds/353775__samueloak89__next-scene.mp3
+-rw-rw-rw-   0        0        0     5175 2023-04-24 10:57:09.000000 space-invaders-0.3.0/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg
+-rw-rw-rw-   0        0        0   530986 2023-04-24 10:59:10.000000 space-invaders-0.3.0/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav
+-rw-rw-rw-   0        0        0   203136 2023-04-24 10:50:18.000000 space-invaders-0.3.0/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav
+-rw-rw-rw-   0        0        0    11760 2023-04-24 10:57:50.000000 space-invaders-0.3.0/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav
+-rw-rw-rw-   0        0        0    16008 2023-04-24 11:00:03.000000 space-invaders-0.3.0/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav
+drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.143253 space-invaders-0.3.0/space_invaders/Sprites/
+-rw-rw-rw-   0        0        0   214392 2023-04-19 23:29:22.000000 space-invaders-0.3.0/space_invaders/Sprites/background.png
+-rw-rw-rw-   0        0        0     2411 2023-04-20 21:12:59.000000 space-invaders-0.3.0/space_invaders/Sprites/default_enemy_gun.png
+-rw-rw-rw-   0        0        0     2672 2023-04-20 21:18:40.000000 space-invaders-0.3.0/space_invaders/Sprites/default_enemy_projectile.png
+-rw-rw-rw-   0        0        0    39680 2023-04-20 21:02:57.000000 space-invaders-0.3.0/space_invaders/Sprites/default_enemy_ship.png
+-rw-rw-rw-   0        0        0    10597 2023-04-19 23:20:42.000000 space-invaders-0.3.0/space_invaders/Sprites/default_gun.png
+-rw-rw-rw-   0        0        0    11317 2023-04-21 22:50:44.000000 space-invaders-0.3.0/space_invaders/Sprites/default_gun_pickup.png
+-rw-rw-rw-   0        0        0     5646 2023-04-19 23:15:52.000000 space-invaders-0.3.0/space_invaders/Sprites/default_projectile.png
+-rw-rw-rw-   0        0        0    29304 2023-04-19 23:20:05.000000 space-invaders-0.3.0/space_invaders/Sprites/default_ship.png
+-rw-rw-rw-   0        0        0     6218 2023-04-24 13:05:19.000000 space-invaders-0.3.0/space_invaders/Sprites/explosion.png
+-rw-rw-rw-   0        0        0    12092 2023-04-21 19:12:55.000000 space-invaders-0.3.0/space_invaders/Sprites/fire_rate_booster.png
+-rw-rw-rw-   0        0        0    10240 2023-04-21 18:58:11.000000 space-invaders-0.3.0/space_invaders/Sprites/life.png
+-rw-rw-rw-   0        0        0     9636 2023-04-21 18:22:32.000000 space-invaders-0.3.0/space_invaders/Sprites/medium_heal.png
+-rw-rw-rw-   0        0        0     7158 2023-04-21 19:34:58.000000 space-invaders-0.3.0/space_invaders/Sprites/minigun.png
+-rw-rw-rw-   0        0        0    12568 2023-04-21 22:47:28.000000 space-invaders-0.3.0/space_invaders/Sprites/minigun_pickup.png
+-rw-rw-rw-   0        0        0     2071 2023-04-21 17:44:27.000000 space-invaders-0.3.0/space_invaders/Sprites/minigun_projectile.png
+-rw-rw-rw-   0        0        0     7934 2023-04-21 18:11:41.000000 space-invaders-0.3.0/space_invaders/Sprites/repair.png
+-rw-rw-rw-   0        0        0     7072 2023-04-21 19:50:03.000000 space-invaders-0.3.0/space_invaders/Sprites/rocket_gun.png
+-rw-rw-rw-   0        0        0    12603 2023-04-21 19:51:49.000000 space-invaders-0.3.0/space_invaders/Sprites/rocket_gun_pickup.png
+-rw-rw-rw-   0        0        0     2843 2023-04-21 20:09:41.000000 space-invaders-0.3.0/space_invaders/Sprites/rocket_projectile.png
+-rw-rw-rw-   0        0        0    51289 2023-04-27 16:34:25.000000 space-invaders-0.3.0/space_invaders/Sprites/ship_explosion.png
+-rw-rw-rw-   0        0        0     6111 2023-04-21 18:21:08.000000 space-invaders-0.3.0/space_invaders/Sprites/small_heal.png
+drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.144253 space-invaders-0.3.0/space_invaders/TestResults/
+-rw-rw-rw-   0        0        0      157 2023-04-28 10:17:05.000000 space-invaders-0.3.0/space_invaders/TestResults/flake8.txt
+-rw-rw-rw-   0        0        0      146 2023-04-28 10:06:54.000000 space-invaders-0.3.0/space_invaders/TestResults/pycodestyle.txt
+-rw-rw-rw-   0        0        0      452 2023-04-30 00:05:08.000000 space-invaders-0.3.0/space_invaders/__entrypoint__.py
+-rw-rw-rw-   0        0        0       72 2023-04-28 23:10:31.000000 space-invaders-0.3.0/space_invaders/__init__.py
+-rw-rw-rw-   0        0        0     4768 2023-04-30 15:23:37.000000 space-invaders-0.3.0/space_invaders/config.py
+-rw-rw-rw-   0        0        0     6813 2023-04-30 15:23:37.000000 space-invaders-0.3.0/space_invaders/entity.py
+-rw-rw-rw-   0        0        0    21244 2023-04-30 14:20:42.000000 space-invaders-0.3.0/space_invaders/level.py
+-rw-rw-rw-   0        0        0    18069 2023-04-30 16:08:55.000000 space-invaders-0.3.0/space_invaders/main.py
+-rw-rw-rw-   0        0        0     5857 2023-04-30 15:23:37.000000 space-invaders-0.3.0/space_invaders/pickup.py
+-rw-rw-rw-   0        0        0    18491 2023-04-30 15:36:04.000000 space-invaders-0.3.0/space_invaders/spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.147254 space-invaders-0.3.0/space_invaders/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-29 14:49:16.000000 space-invaders-0.3.0/space_invaders/tests/__init__.py
+-rw-rw-rw-   0        0        0     3467 2023-04-29 14:27:17.000000 space-invaders-0.3.0/space_invaders/tests/test_entity.py
+-rw-rw-rw-   0        0        0     2704 2023-04-29 17:32:02.000000 space-invaders-0.3.0/space_invaders/tests/test_level.py
+-rw-rw-rw-   0        0        0     2031 2023-04-29 19:47:22.000000 space-invaders-0.3.0/space_invaders/tests/test_main.py
+-rw-rw-rw-   0        0        0     1494 2023-04-29 15:11:06.000000 space-invaders-0.3.0/space_invaders/tests/test_pickup.py
+-rw-rw-rw-   0        0        0     3513 2023-04-30 15:23:37.000000 space-invaders-0.3.0/space_invaders/tests/test_spaceship.py
+drwxrwxrwx   0        0        0        0 2023-04-30 16:15:49.117240 space-invaders-0.3.0/space_invaders.egg-info/
+-rw-rw-rw-   0        0        0     2339 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2481 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-30 16:15:49.000000 space-invaders-0.3.0/space_invaders.egg-info/top_level.txt
```

### Comparing `space-invaders-0.2.0/PKG-INFO` & `space-invaders-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.2.0
+Version: 0.3.0
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.2.0/setup.py` & `space-invaders-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='space-invaders',
-    version='0.2.0',
+    version='0.3.0',
     packages=find_packages(),
     install_requires=[
         'pygame',
         'shapely'
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `space-invaders-0.2.0/space_invaders/Fonts/AGENCYB.TTF` & `space-invaders-0.3.0/space_invaders/Fonts/AGENCYB.TTF`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Fonts/AGENCYR.TTF` & `space-invaders-0.3.0/space_invaders/Fonts/AGENCYR.TTF`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Fonts/Alien Invader Italic.ttf` & `space-invaders-0.3.0/space_invaders/Fonts/Alien Invader Italic.ttf`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Fonts/Alien Invader.ttf` & `space-invaders-0.3.0/space_invaders/Fonts/Alien Invader.ttf`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/README.md` & `space-invaders-0.3.0/space_invaders/README.md`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/122255__jivatma07__level_complete.wav` & `space-invaders-0.3.0/space_invaders/Sounds/122255__jivatma07__level_complete.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/156895__halgrimm__a-shot.wav` & `space-invaders-0.3.0/space_invaders/Sounds/156895__halgrimm__a-shot.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/18380__inferno__hvrl.wav` & `space-invaders-0.3.0/space_invaders/Sounds/18380__inferno__hvrl.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav` & `space-invaders-0.3.0/space_invaders/Sounds/277403__landlucky__game-over-sfx-and-voice.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav` & `space-invaders-0.3.0/space_invaders/Sounds/340452__zagi2__dondolan2-loop.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/353775__samueloak89__next-scene.mp3` & `space-invaders-0.3.0/space_invaders/Sounds/353775__samueloak89__next-scene.mp3`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg` & `space-invaders-0.3.0/space_invaders/Sounds/427409__artembasov__ab_beep_or_blaster_shot.ogg`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav` & `space-invaders-0.3.0/space_invaders/Sounds/565481__jakegwizdak__small-explosion.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav` & `space-invaders-0.3.0/space_invaders/Sounds/615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav` & `space-invaders-0.3.0/space_invaders/Sounds/648200__strangehorizon__glitch_blip.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav` & `space-invaders-0.3.0/space_invaders/Sounds/678384__jocabundus__item-pickup-v1.wav`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/background.png` & `space-invaders-0.3.0/space_invaders/Sprites/background.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/default_enemy_gun.png` & `space-invaders-0.3.0/space_invaders/Sprites/default_enemy_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/default_enemy_projectile.png` & `space-invaders-0.3.0/space_invaders/Sprites/default_enemy_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/default_enemy_ship.png` & `space-invaders-0.3.0/space_invaders/Sprites/default_enemy_ship.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/default_gun.png` & `space-invaders-0.3.0/space_invaders/Sprites/default_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/default_gun_pickup.png` & `space-invaders-0.3.0/space_invaders/Sprites/default_gun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/default_projectile.png` & `space-invaders-0.3.0/space_invaders/Sprites/default_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/default_ship.png` & `space-invaders-0.3.0/space_invaders/Sprites/default_ship.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/explosion.png` & `space-invaders-0.3.0/space_invaders/Sprites/explosion.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/fire_rate_booster.png` & `space-invaders-0.3.0/space_invaders/Sprites/fire_rate_booster.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/life.png` & `space-invaders-0.3.0/space_invaders/Sprites/life.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/medium_heal.png` & `space-invaders-0.3.0/space_invaders/Sprites/medium_heal.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/minigun.png` & `space-invaders-0.3.0/space_invaders/Sprites/minigun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/minigun_pickup.png` & `space-invaders-0.3.0/space_invaders/Sprites/minigun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/minigun_projectile.png` & `space-invaders-0.3.0/space_invaders/Sprites/minigun_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/repair.png` & `space-invaders-0.3.0/space_invaders/Sprites/repair.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/rocket_gun.png` & `space-invaders-0.3.0/space_invaders/Sprites/rocket_gun.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/rocket_gun_pickup.png` & `space-invaders-0.3.0/space_invaders/Sprites/rocket_gun_pickup.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/rocket_projectile.png` & `space-invaders-0.3.0/space_invaders/Sprites/rocket_projectile.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/ship_explosion.png` & `space-invaders-0.3.0/space_invaders/Sprites/ship_explosion.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/Sprites/small_heal.png` & `space-invaders-0.3.0/space_invaders/Sprites/small_heal.png`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/config.py` & `space-invaders-0.3.0/space_invaders/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import pygame
 import os
 
+"""
+This is the configuration file, containing most of the globally used constants
+Also a couple of globally used functions
+"""
 
 PATH = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_path(*args):
+    """
+    The method returns the given relative path converted into absolute path, based on where the project is installed
+    It is required since the running environment may be elsewhere
+    @param args the split relative path.
+    @return: the absolute path
+    """
     return os.path.join(PATH, *args)
 
 
 CHANNEL_COUNT = 30
 SOUND_MAIN_THEME_DATA = (get_path("Sounds", "340452__zagi2__dondolan2-loop.wav"), 0.5, 0)
 SOUND_DEFAULT_GUN_DATA = (get_path("Sounds", "615809__flyingsaucerinvasion__sci-fi-laser-blaster-shot-3.wav"), 0.15, 0)
 SOUND_MINIGUN_DATA = (get_path("Sounds", "156895__halgrimm__a-shot.wav"), 0.9, 0)
@@ -22,14 +32,19 @@
 SOUND_PICKUP_DATA = (get_path("Sounds", "678384__jocabundus__item-pickup-v1.wav"), 0.7, 0)
 SOUND_CREDITS_DATA = (get_path("Sounds", "353775__samueloak89__next-scene.mp3"), 0.7, 0)
 
 MUSICS = (SOUND_MAIN_THEME_DATA, SOUND_CREDITS_DATA)
 
 
 def play_sound(sound_data, loops):
+    """
+    Plays a sound or music based on the given sound_data, and loops it 'loops' times
+    @param sound_data the sound_data tuple that is selected from the constants defined in config
+    @param loops the number of loops
+    """
     if sound_data in MUSICS:
         pygame.mixer_music.load(sound_data[0], "muzsika")
         pygame.mixer_music.set_volume(sound_data[1])
         pygame.mixer_music.fadeout(sound_data[2])
         pygame.mixer_music.play(loops=loops)
         return
 
@@ -54,22 +69,26 @@
 RESET_SWITCH_DELAY = 200
 PICKUP_SPEED = 5
 PICKUP_SPAWN_INTERVAL = (4, 8)
 score = 0
 
 LAUNCH_GAME = False
 
-SHOW_HIT_BOXES = False
+SHOW_COLLIDERS = False
 WINDOW_WIDTH = 1400
 WINDOW_HEIGHT = 950
 CAPTION = "Space Invaders"
 BACKGROUND_IMAGE = get_path("Sprites", "background.png")
 
 
 def get_credits_text():
+    """
+    Returns the credits string, with the updated score value
+    @return: the credits string
+    """
     return f"""CONGRATULATIONS!
 YOU HAVE SUCCESSFULLY BEATEN THE GAME!
 FINAL SCORE:  {score}
 
 
 
 SOUNDS
```

### Comparing `space-invaders-0.2.0/space_invaders/main.py` & `space-invaders-0.3.0/space_invaders/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,43 +4,50 @@
 from shapely.geometry import Polygon
 from space_invaders.entity import Entity
 from space_invaders.pickup import PICKUP_LIFE, PICKUP_MINIGUN, PICKUP_REPAIR, PICKUP_ROCKET_GUN, PICKUP_SMALL_HEAL, \
     PICKUP_MEDIUM_HEAL, PICKUP_FIRE_RATE_BOOSTER, Pickup, RESET_FIRE_RATE, PICKUP_DEFAULT_GUN
 from space_invaders.spaceship import ROCKET_GUN, MINIGUN
 from space_invaders.config import WINDOW_WIDTH, WINDOW_HEIGHT, play_sound, PICKUP_SPEED, PICKUP_SPAWN_INTERVAL, \
     SOUND_CREDITS_DATA, SOUND_EXPLOSION_DATA, SOUND_MAIN_THEME_DATA, SOUND_DEFEAT_DATA, SOUND_VICTORY_DATA, \
-    SOUND_ENEMY_HIT_DATA, SOUND_PLAYER_HIT_DATA, SHOW_HIT_BOXES, get_credits_text, EXPLOSION_DURATION, \
+    SOUND_ENEMY_HIT_DATA, SOUND_PLAYER_HIT_DATA, SHOW_COLLIDERS, get_credits_text, EXPLOSION_DURATION, \
     RESET_SWITCH_DELAY, FONT_CREDITS_TEXT_DATA, FONT_CREDITS_TITLE_DATA, FONT86_DATA, FONT15_DATA, FONT152_DATA, \
     FONT25_DATA, FONT36_DATA, CHANNEL_COUNT, CAPTION, BACKGROUND_IMAGE, SOUND_PICKUP_DATA, LAUNCH_GAME
 import space_invaders.config as config
 import space_invaders.level as level
 
 
 def update_pickups():
+    """
+    Moves each pickup downwards, checks if any of them collides with the player.
+    If there is collision, it plays a sound and applies the effect of the pickup
+    """
     global pickups, window, player
-    player_poly = Polygon(player.hit_box)
+    player_poly = Polygon(player.collider)
 
     for pickup in pickups:
         if pickup.position[1] > WINDOW_HEIGHT + 55:
             pickups.remove(pickup)
         else:
-            pickup_poly = Polygon([pickup.hit_box.topleft, pickup.hit_box.topright,
-                                   pickup.hit_box.bottomright, pickup.hit_box.bottomleft])
+            pickup_poly = Polygon([pickup.collider.topleft, pickup.collider.topright,
+                                   pickup.collider.bottomright, pickup.collider.bottomleft])
             if pickup_poly.intersects(player_poly):
                 play_sound(SOUND_PICKUP_DATA, 0)
                 pickup.action(player, *pickup.args)
                 pickups.remove(pickup)
             else:
                 pickup.move((0, PICKUP_SPEED))
                 pickup.render(window)
-                if SHOW_HIT_BOXES:
-                    pygame.draw.rect(window, (255, 0, 255), pickup.hit_box, 1)
+                if SHOW_COLLIDERS:
+                    pygame.draw.rect(window, (255, 0, 255), pickup.collider, 1)
 
 
 def spawn_pickup():
+    """
+    Spawns a random pickup at a random position, adds it to the global pickups array
+    """
     global pickups, current_level
 
     rnd = random.randint(0, 100)
     if rnd > 96:
         pickup_type = PICKUP_LIFE
     elif rnd > 87:
         pickup_type = PICKUP_REPAIR
@@ -58,29 +65,39 @@
     spawn_location = (random.randint(50, WINDOW_WIDTH-50), -60)
     spawned_pickup = pickup_type.new_pickup()
     spawned_pickup.position = spawn_location
     pickups.append(spawned_pickup)
 
 
 def spawn_at_random_interval():
+    """Sets a timer with random delay for the SPAWN PICKUP event"""
     pygame.time.set_timer(SPAWN_PICKUP, random.randint(int(PICKUP_SPAWN_INTERVAL[0]*1000),
                                                        int(PICKUP_SPAWN_INTERVAL[1]*1000)))
 
 
 def get_pickup_image_by_gun(gun):
+    """
+    @param gun a Gun object
+    @return: a pygame Surface image based on the type of the given gun
+    """
     match gun.type:
         case "rocket":
             return PICKUP_ROCKET_GUN.image
         case "minigun":
             return PICKUP_MINIGUN.image
         case _:
             return PICKUP_DEFAULT_GUN.image
 
 
 def display_hud():
+    """
+    Displays each enemy's health, then the player's health, lives.
+    Draws the fire rate booster's symbol if the player's fire rate is boosted
+    And shows the player's current score
+    """
     global player, enemies, window
 
     # Enemy healths
     for enemy_ in enemies:
         position = (enemy_.image_rect.center[0], enemy_.image_rect.center[1] - 18)
         shift = 37
         scale = 15
@@ -129,14 +146,18 @@
     score_text = FONT36.render(str(config.score), True, (255, 255, 0))
     score_text_shadow = FONT36.render(str(config.score), True, (50, 50, 0))
     window.blit(score_text_shadow, (15, WINDOW_HEIGHT - 45))
     window.blit(score_text, (10, WINDOW_HEIGHT - 50))
 
 
 def display_credits():
+    """
+    Displays the credits of the project, makes it possible fast-forward with SPACE, W, S keys
+    At the end of the credits, the application is closed
+    """
     global window
     pygame.mixer_music.stop()
     play_sound(SOUND_CREDITS_DATA, -1)
     shift = 0
     while shift < int(WINDOW_HEIGHT * 3.05):
         for _event in pygame.event.get():
             if _event.type == pygame.QUIT:
@@ -167,14 +188,19 @@
 
     pygame.time.wait(500)
     pygame.quit()
     exit()
 
 
 def level_over():
+    """
+    Handles the end of the current level
+    Loads the first level if the player died
+    Otherwise it loads the next level if it exists, if it doesn't, the display_credits is called
+    """
     global LEVELS, LEVEL_OVER, level_index
 
     if player.alive():
         play_sound(SOUND_VICTORY_DATA, 0)
         text_color = (50, 200, 50)
         shadow_color = (20, 100, 20)
         config.score += 1000
@@ -213,27 +239,39 @@
     else:
         entities.remove(player)
         level_index = 0
         load_level(LEVELS[0])
 
 
 def check_entity_collision(player_entity, enemy_entities):
-    player_poly = Polygon(player_entity.hit_box)
+    """
+    Checks if the player collides with any of the enemy entities, if yes they both take damage equal to the other's hp
+
+    @param player_entity the player
+    @param enemy_entities the array of enemies that are checked
+    """
+    player_poly = Polygon(player_entity.collider)
 
     for _enemy in enemy_entities:
-        enemy_poly = Polygon(_enemy.hit_box)
+        enemy_poly = Polygon(_enemy.collider)
         if player_poly.intersects(enemy_poly):
             play_sound(SOUND_ENEMY_HIT_DATA, 0)
             play_sound(SOUND_PLAYER_HIT_DATA, 0)
             enemy_hp = _enemy.hp
             _enemy.take_damage(player_entity.hp)
             player_entity.take_damage(enemy_hp)
 
 
 def handle_player_input(player_entity: Entity, max_x, max_y):
+    """
+    Handles the player's input
+    @param player_entity the player's entity
+    @param max_x the maximum x position that is allowed
+    @param max_y the maximum y position that is allowed
+    """
     global CAN_SWITCH_GUN, RESET_CAN_SWITCH
     pressed_keys = pygame.key.get_pressed()
     vec = [0, 0]
 
     # setting up the movement vector
     if pressed_keys[K_w]:
         vec[1] -= 0.65
@@ -263,14 +301,20 @@
         player_entity.next_gun()
         pygame.time.set_timer(RESET_CAN_SWITCH, RESET_SWITCH_DELAY)
     if pressed_keys[K_SPACE]:
         player_entity.shoot()
 
 
 def load_level(_level):
+    """
+    Loads the next level, resets the global arrays to be empty
+    If the player is still alive from the last level it is copied to the new level and his position is set to the
+    new level's spawn position, also the player's hp is recharged.
+    After loading the level, the level's title and text is displayed
+    """
     global current_level, player, entities, enemies, pickups, explosions
     entities = []
     enemies = []
     pickups = []
     explosions = []
     level.initialize_global_arrays(entities, enemies)
 
@@ -298,15 +342,19 @@
 
     pygame.display.update()
     pygame.time.wait(2000)
 
     return player, current_level
 
 
+"""
+The main game loop tat pulls everything together
+"""
 if LAUNCH_GAME:
+    # INITIALIZATIONS
     pygame.init()
     pygame.mixer.init()
     pygame.mixer.set_num_channels(CHANNEL_COUNT)
     LEVEL_OVER = False
     CAN_SWITCH_GUN = True
     RESET_CAN_SWITCH = USEREVENT + 2
     SPAWN_PICKUP = USEREVENT + 3
@@ -328,17 +376,20 @@
 
     clock = pygame.time.Clock()
     play_sound(SOUND_MAIN_THEME_DATA, -1)
 
     # Declaration of global arrays
     entities = enemies = pickups = explosions = []
 
+    # Loading the first level, and its player
     current_level = player = None
     player, current_level = load_level(LEVELS[0])
+
     if player is not None and current_level is not None:
+        # Queues a new pickup spawn
         spawn_at_random_interval()
 
         while True:
             if LEVEL_OVER:
                 level_over()
 
             for event in pygame.event.get():
@@ -372,15 +423,15 @@
 
                         enemies.remove(enemy)
                         entities.remove(enemy)
 
             # render everything
             window.blit(background_img, (0, 0))
             for entity in entities:
-                entity.render(window, SHOW_HIT_BOXES)
+                entity.render(window, SHOW_COLLIDERS)
             update_pickups()
             for explosion in explosions:
                 if explosion[2] == 0:
                     explosions.remove(explosion)
                 else:
                     explosion_image = explosion[0]
                     explosion_image = pygame.transform.scale(explosion_image, (explosion_image.get_size()[0] * 1.15,
```

### Comparing `space-invaders-0.2.0/space_invaders/tests/test_entity.py` & `space-invaders-0.3.0/space_invaders/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/tests/test_level.py` & `space-invaders-0.3.0/space_invaders/tests/test_level.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/tests/test_main.py` & `space-invaders-0.3.0/space_invaders/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/tests/test_pickup.py` & `space-invaders-0.3.0/space_invaders/tests/test_pickup.py`

 * *Files identical despite different names*

### Comparing `space-invaders-0.2.0/space_invaders/tests/test_spaceship.py` & `space-invaders-0.3.0/space_invaders/tests/test_spaceship.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,11 +58,11 @@
 
         prev_pos = proj.image_rect.center
         for i in range(12):
             proj.move_forward(False)
             self.assertEqual(proj.image_rect.center[0], prev_pos[0], "x coordinate not set properly in set position")
             self.assertEqual(proj.image_rect.center[1], prev_pos[1] - 20, "y coordinate set wrong in set position")
             prev_pos = proj.image_rect.center
-            if proj.hit_box.bottom < -100:
+            if proj.collider.bottom < -100:
                 self.assertTrue(proj.check_if_out(), f"Projectile is out, should return True")
             else:
                 self.assertFalse(proj.check_if_out(), "Projectile is in, should return False")
```

### Comparing `space-invaders-0.2.0/space_invaders.egg-info/PKG-INFO` & `space-invaders-0.3.0/space_invaders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-invaders
-Version: 0.2.0
+Version: 0.3.0
 Summary: A cool space shooter rouge like game
 Author: Bódi Martin
 Author-email: bodimartin22@gmail.com
 Description-Content-Type: text/markdown
 
 # Space Invaders
 ## HOW TO INSTALL?
```

### Comparing `space-invaders-0.2.0/space_invaders.egg-info/SOURCES.txt` & `space-invaders-0.3.0/space_invaders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

