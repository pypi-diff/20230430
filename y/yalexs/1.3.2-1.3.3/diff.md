# Comparing `tmp/yalexs-1.3.2.tar.gz` & `tmp/yalexs-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-1.3.2.tar", last modified: Mon Apr 24 17:36:37 2023, max compression
+gzip compressed data, was "yalexs-1.3.3.tar", last modified: Sun Apr 30 06:11:18 2023, max compression
```

## Comparing `yalexs-1.3.2.tar` & `yalexs-1.3.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:36:37.454124 yalexs-1.3.2/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:36:37.440365 yalexs-1.3.2/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:36:37.442760 yalexs-1.3.2/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2383 2023-02-17 14:33:57.000000 yalexs-1.3.2/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.3.2/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.3.2/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.3.2/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-24 17:36:37.454194 yalexs-1.3.2/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.3.2/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.3.2/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.3.2/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.3.2/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       46 2023-02-17 14:03:08.000000 yalexs-1.3.2/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.3.2/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-24 17:36:37.454462 yalexs-1.3.2/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)      972 2023-04-24 17:36:21.000000 yalexs-1.3.2/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:36:37.444032 yalexs-1.3.2/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:36:37.449956 yalexs-1.3.2/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    14702 2023-04-24 17:14:19.000000 yalexs-1.3.2/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    31589 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38166 2023-02-17 14:33:57.000000 yalexs-1.3.2/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8411 2023-02-17 14:03:08.000000 yalexs-1.3.2/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-04-24 17:36:15.000000 yalexs-1.3.2/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    10482 2023-02-17 14:03:03.000000 yalexs-1.3.2/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.3.2/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:36:37.453439 yalexs-1.3.2/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-04-24 17:36:21.000000 yalexs-1.3.2/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    13964 2023-04-24 17:14:19.000000 yalexs-1.3.2/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     9792 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    12351 2023-02-17 14:03:08.000000 yalexs-1.3.2/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    10480 2023-04-14 19:36:42.000000 yalexs-1.3.2/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4740 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5057 2023-02-17 14:03:08.000000 yalexs-1.3.2/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5080 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/authenticator_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4284 2023-02-17 14:03:08.000000 yalexs-1.3.2/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      273 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.3.2/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-04-24 17:36:15.000000 yalexs-1.3.2/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.3.2/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2554 2023-02-17 14:03:08.000000 yalexs-1.3.2/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:36:37.454026 yalexs-1.3.2/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-24 17:36:37.000000 yalexs-1.3.2/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     2799 2023-04-24 17:36:37.000000 yalexs-1.3.2/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-24 17:36:37.000000 yalexs-1.3.2/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-04-24 17:36:37.000000 yalexs-1.3.2/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-04-24 17:36:37.000000 yalexs-1.3.2/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.492865 yalexs-1.3.3/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.474817 yalexs-1.3.3/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.477979 yalexs-1.3.3/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2383 2023-02-17 14:33:57.000000 yalexs-1.3.3/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.3.3/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.3.3/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.3.3/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-30 06:11:18.492962 yalexs-1.3.3/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.3.3/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.3.3/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.3.3/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.3.3/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       46 2023-02-17 14:03:08.000000 yalexs-1.3.3/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.3.3/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 06:11:18.493293 yalexs-1.3.3/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)      972 2023-04-30 06:11:07.000000 yalexs-1.3.3/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.479852 yalexs-1.3.3/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.487983 yalexs-1.3.3/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    14702 2023-04-24 17:14:19.000000 yalexs-1.3.3/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    31589 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38166 2023-02-17 14:33:57.000000 yalexs-1.3.3/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.3.3/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8411 2023-02-17 14:03:08.000000 yalexs-1.3.3/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15108 2023-04-24 17:36:15.000000 yalexs-1.3.3/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14941 2023-04-30 06:10:58.000000 yalexs-1.3.3/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.3.3/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.492190 yalexs-1.3.3/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-04-30 06:11:07.000000 yalexs-1.3.3/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14180 2023-04-30 06:10:58.000000 yalexs-1.3.3/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     9792 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    12351 2023-02-17 14:03:08.000000 yalexs-1.3.3/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    10480 2023-04-14 19:36:42.000000 yalexs-1.3.3/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4740 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5057 2023-02-17 14:03:08.000000 yalexs-1.3.3/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5080 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/authenticator_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4284 2023-02-17 14:03:08.000000 yalexs-1.3.3/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      273 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.3.3/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4396 2023-04-24 17:36:15.000000 yalexs-1.3.3/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.3.3/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3739 2023-04-30 06:10:58.000000 yalexs-1.3.3/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-30 06:11:18.492765 yalexs-1.3.3/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     2799 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-04-30 06:11:18.000000 yalexs-1.3.3/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-1.3.2/.github/workflows/ci.yaml` & `yalexs-1.3.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/.gitignore` & `yalexs-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/LICENSE` & `yalexs-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/PKG-INFO` & `yalexs-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.3.2/README.md` & `yalexs-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/known_activities.md` & `yalexs-1.3.3/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/pylintrc` & `yalexs-1.3.3/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/setup.cfg` & `yalexs-1.3.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.3.2
+current_version = 1.3.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-1.3.2/setup.py` & `yalexs-1.3.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="1.3.2",
+    version="1.3.3",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `yalexs-1.3.2/tests/fixtures/auto_relock_activity.json` & `yalexs-1.3.3/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/auto_unlock_activity.json` & `yalexs-1.3.3/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-1.3.3/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/door_closed_activity.json` & `yalexs-1.3.3/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-1.3.3/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-1.3.3/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/door_open_activity.json` & `yalexs-1.3.3/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/doorbell_motion_activity.json` & `yalexs-1.3.3/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-1.3.3/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-1.3.3/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-1.3.3/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-1.3.3/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_doorbell.json` & `yalexs-1.3.3/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_doorbell.offline.json` & `yalexs-1.3.3/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-1.3.3/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_doorbells.json` & `yalexs-1.3.3/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_house_activities.json` & `yalexs-1.3.3/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-1.3.3/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-1.3.3/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_lock.offline.json` & `yalexs-1.3.3/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_lock.online.json` & `yalexs-1.3.3/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-1.3.3/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-1.3.3/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_lock_v2.online.json` & `yalexs-1.3.3/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/get_pins.json` & `yalexs-1.3.3/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/keypad_lock_activity.json` & `yalexs-1.3.3/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/lock.json` & `yalexs-1.3.3/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/lock_activity.json` & `yalexs-1.3.3/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/lock_without_doorstate.json` & `yalexs-1.3.3/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/remote_lock_activity.json` & `yalexs-1.3.3/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-1.3.3/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/unlock.json` & `yalexs-1.3.3/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/unlock_activity.json` & `yalexs-1.3.3/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/fixtures/unlock_without_doorstate.json` & `yalexs-1.3.3/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/test_activity.py` & `yalexs-1.3.3/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/test_api.py` & `yalexs-1.3.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/test_api_async.py` & `yalexs-1.3.3/tests/test_api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/test_authenticator.py` & `yalexs-1.3.3/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/test_authenticator_async.py` & `yalexs-1.3.3/tests/test_authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tests/test_pubnub_activity.py` & `yalexs-1.3.3/tests/test_pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/tox.ini` & `yalexs-1.3.3/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/activity.py` & `yalexs-1.3.3/yalexs/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
     ACTION_LOCK_MANUAL_UNLOCK: LockStatus.UNLOCKED,
 }
 
 SOURCE_LOCK_OPERATE = "lock_operate"
 SOURCE_PUBNUB = "pubnub"
 SOURCE_LOG = "log"
 
+# If we get a lock operation activity with the same time stamp as a moving
+# activity we want to use the non-moving activity since its the completed state.
+MOVING_STATES = {LockStatus.UNLOCKING, LockStatus.LOCKING}
+
 
 def epoch_to_datetime(epoch: str | int | float) -> datetime:
     return datetime.fromtimestamp(float(epoch) / 1000.0)
 
 
 class ActivityType(Enum):
     DOORBELL_MOTION = "doorbell_motion"
```

### Comparing `yalexs-1.3.2/yalexs/api.py` & `yalexs-1.3.3/yalexs/api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/api_async.py` & `yalexs-1.3.3/yalexs/api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/api_common.py` & `yalexs-1.3.3/yalexs/api_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/authenticator.py` & `yalexs-1.3.3/yalexs/authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/authenticator_async.py` & `yalexs-1.3.3/yalexs/authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/authenticator_common.py` & `yalexs-1.3.3/yalexs/authenticator_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/bridge.py` & `yalexs-1.3.3/yalexs/bridge.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/device.py` & `yalexs-1.3.3/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/doorbell.py` & `yalexs-1.3.3/yalexs/doorbell.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/keypad.py` & `yalexs-1.3.3/yalexs/keypad.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/lock.py` & `yalexs-1.3.3/yalexs/lock.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/pin.py` & `yalexs-1.3.3/yalexs/pin.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/pubnub_activity.py` & `yalexs-1.3.3/yalexs/pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/pubnub_async.py` & `yalexs-1.3.3/yalexs/pubnub_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs/users.py` & `yalexs-1.3.3/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.2/yalexs.egg-info/PKG-INFO` & `yalexs-1.3.3/yalexs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.3.2/yalexs.egg-info/SOURCES.txt` & `yalexs-1.3.3/yalexs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

