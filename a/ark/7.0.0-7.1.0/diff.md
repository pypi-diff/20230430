# Comparing `tmp/ark-7.0.0.tar.gz` & `tmp/ark-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ark-7.0.0.tar", last modified: Fri Apr 28 23:31:16 2023, max compression
+gzip compressed data, was "ark-7.1.0.tar", last modified: Sun Apr 30 12:00:28 2023, max compression
```

## Comparing `ark-7.0.0.tar` & `ark-7.1.0.tar`

### file list

```diff
@@ -1,111 +1,97 @@
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.687283 ark-7.0.0/
--rw-r--r--   0 dmulholl   (501) staff       (20)       96 2023-04-28 23:31:16.000000 ark-7.0.0/MANIFEST.in
--rw-r--r--   0 dmulholl   (501) staff       (20)      667 2023-04-28 23:31:16.686889 ark-7.0.0/PKG-INFO
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.651821 ark-7.0.0/ark/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1798 2023-04-28 21:56:21.000000 ark-7.0.0/ark/__init__.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      630 2023-04-28 22:09:04.000000 ark-7.0.0/ark/__main__.py
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.654314 ark-7.0.0/ark/bundle/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.654734 ark-7.0.0/ark/bundle/inc/
--rw-r--r--   0 dmulholl   (501) staff       (20)      162 2021-11-15 13:56:09.000000 ark-7.0.0/ark/bundle/inc/menu.md
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.646541 ark-7.0.0/ark/bundle/lib/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.655495 ark-7.0.0/ark/bundle/lib/debug/
--rw-r--r--   0 dmulholl   (501) staff       (20)      607 2022-03-04 18:57:03.000000 ark-7.0.0/ark/bundle/lib/debug/license.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)      217 2023-04-28 22:12:12.000000 ark-7.0.0/ark/bundle/lib/debug/readme.md
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.656223 ark-7.0.0/ark/bundle/lib/debug/resources/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1760 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/debug/resources/debug.css
--rw-r--r--   0 dmulholl   (501) staff       (20)     4840 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/lib/debug/resources/pygments.css
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.656664 ark-7.0.0/ark/bundle/lib/debug/templates/
--rw-r--r--   0 dmulholl   (501) staff       (20)     2486 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/debug/templates/node.ibis
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.657507 ark-7.0.0/ark/bundle/lib/graphite/
--rw-r--r--   0 dmulholl   (501) staff       (20)      607 2022-03-04 18:57:03.000000 ark-7.0.0/ark/bundle/lib/graphite/license.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)     1245 2023-04-28 22:13:18.000000 ark-7.0.0/ark/bundle/lib/graphite/readme.md
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.646766 ark-7.0.0/ark/bundle/lib/graphite/resources/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.658954 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.666831 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    93768 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    13172 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    75680 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    14196 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    99800 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    14648 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)   189596 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    13612 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    77596 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    14200 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)    75580 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf
--rw-r--r--   0 dmulholl   (501) staff       (20)    14388 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2
--rwxr-xr-x   0 dmulholl   (501) staff       (20)     4512 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)     2047 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts.css
--rw-r--r--   0 dmulholl   (501) staff       (20)    11077 2023-04-07 20:56:01.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/graphite.css
--rw-r--r--   0 dmulholl   (501) staff       (20)     5027 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/pygments.css
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.667194 ark-7.0.0/ark/bundle/lib/graphite/templates/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1800 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/templates/node.ibis
--rw-r--r--   0 dmulholl   (501) staff       (20)      448 2023-04-28 22:18:55.000000 ark-7.0.0/ark/bundle/site.py
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.668336 ark-7.0.0/ark/bundle/src/
--rw-r--r--   0 dmulholl   (501) staff       (20)      551 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/src/about.md
--rw-r--r--   0 dmulholl   (501) staff       (20)     4349 2021-11-13 17:10:33.000000 ark-7.0.0/ark/bundle/src/index.stx
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.669079 ark-7.0.0/ark/bundle/src/parent/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/src/parent/child-one.md
--rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/src/parent/child-two.md
--rw-r--r--   0 dmulholl   (501) staff       (20)     1097 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/src/parent.md
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.672855 ark-7.0.0/ark/cli/
--rw-r--r--   0 dmulholl   (501) staff       (20)     1831 2023-04-28 22:15:02.000000 ark-7.0.0/ark/cli/__init__.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2704 2023-04-28 22:16:17.000000 ark-7.0.0/ark/cli/add.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     3091 2023-04-28 22:16:49.000000 ark-7.0.0/ark/cli/build.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      903 2023-04-28 22:15:53.000000 ark-7.0.0/ark/cli/clear.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1375 2023-04-28 22:16:35.000000 ark-7.0.0/ark/cli/deploy.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1244 2023-04-28 22:10:48.000000 ark-7.0.0/ark/cli/init.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1313 2023-04-28 22:11:19.000000 ark-7.0.0/ark/cli/open.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2904 2023-04-28 22:15:41.000000 ark-7.0.0/ark/cli/serve.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2319 2023-04-28 22:16:28.000000 ark-7.0.0/ark/cli/tree.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     4019 2023-04-28 22:12:43.000000 ark-7.0.0/ark/cli/watch.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2882 2023-04-28 22:19:16.000000 ark-7.0.0/ark/events.py
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.675524 ark-7.0.0/ark/extensions/
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.686367 ark-7.0.0/ark/extensions/__pycache__/
--rw-r--r--   0 dmulholl   (501) staff       (20)     3625 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_automenu.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1256 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_ibis.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1556 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_jinja.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      935 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_markdown.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1600 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_shortcodes.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      828 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_syntext.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1267 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_yaml.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1817 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_automenu.cpython-310.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     3625 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_automenu.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      692 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_ibis.cpython-310.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1256 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_ibis.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      842 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_jinja.cpython-310.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1556 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_jinja.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      538 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_markdown.cpython-310.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      935 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_markdown.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      885 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_shortcodes.cpython-310.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1600 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_shortcodes.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      510 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_syntext.cpython-310.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      828 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_syntext.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)      663 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_yaml.cpython-310.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     1267 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_yaml.cpython-311.pyc
--rw-r--r--   0 dmulholl   (501) staff       (20)     3038 2023-04-28 22:02:17.000000 ark-7.0.0/ark/extensions/ark_automenu.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      484 2023-04-28 22:03:31.000000 ark-7.0.0/ark/extensions/ark_ibis.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      731 2023-04-28 22:03:48.000000 ark-7.0.0/ark/extensions/ark_jinja.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      368 2023-04-28 22:04:06.000000 ark-7.0.0/ark/extensions/ark_markdown.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1057 2023-04-28 22:04:30.000000 ark-7.0.0/ark/extensions/ark_shortcodes.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      335 2023-04-28 22:04:44.000000 ark-7.0.0/ark/extensions/ark_syntext.py
--rw-r--r--   0 dmulholl   (501) staff       (20)      541 2023-04-28 22:05:00.000000 ark-7.0.0/ark/extensions/ark_yaml.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1658 2023-04-28 22:18:34.000000 ark-7.0.0/ark/extensions.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     3051 2023-04-28 22:17:38.000000 ark-7.0.0/ark/filters.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2604 2023-04-28 22:08:26.000000 ark-7.0.0/ark/hashes.py
--rw-r--r--   0 dmulholl   (501) staff       (20)    11019 2023-04-28 22:17:50.000000 ark-7.0.0/ark/nodes.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     1880 2023-04-28 22:09:28.000000 ark-7.0.0/ark/renderers.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     7623 2023-04-28 22:00:03.000000 ark-7.0.0/ark/site.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     2606 2023-04-28 22:07:18.000000 ark-7.0.0/ark/templates.py
--rw-r--r--   0 dmulholl   (501) staff       (20)     6549 2022-04-15 14:06:24.000000 ark-7.0.0/ark/utils.py
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.653890 ark-7.0.0/ark.egg-info/
--rw-r--r--   0 dmulholl   (501) staff       (20)      667 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/PKG-INFO
--rw-r--r--   0 dmulholl   (501) staff       (20)     3475 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/SOURCES.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)        1 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/dependency_links.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)       33 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/entry_points.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)      118 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/requires.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)        4 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/top_level.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)     1212 2016-08-25 13:09:14.000000 ark-7.0.0/license.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)      208 2023-04-28 21:54:32.000000 ark-7.0.0/readme.md
--rw-r--r--   0 dmulholl   (501) staff       (20)       38 2023-04-28 23:31:16.687413 ark-7.0.0/setup.cfg
--rwxr-xr-x   0 dmulholl   (501) staff       (20)     2084 2023-04-28 21:51:45.000000 ark-7.0.0/setup.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.819955 ark-7.1.0/
+-rw-r--r--   0 dmulholl   (501) staff       (20)       96 2023-04-30 12:00:28.000000 ark-7.1.0/MANIFEST.in
+-rw-r--r--   0 dmulholl   (501) staff       (20)      667 2023-04-30 12:00:28.819335 ark-7.1.0/PKG-INFO
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.779084 ark-7.1.0/ark/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1798 2023-04-30 11:32:33.000000 ark-7.1.0/ark/__init__.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      630 2023-04-29 12:10:51.000000 ark-7.1.0/ark/__main__.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.781816 ark-7.1.0/ark/bundle/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.782575 ark-7.1.0/ark/bundle/inc/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      162 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/inc/menu.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.771254 ark-7.1.0/ark/bundle/lib/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.783903 ark-7.1.0/ark/bundle/lib/debug/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      607 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      217 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/readme.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.784945 ark-7.1.0/ark/bundle/lib/debug/resources/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1760 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/resources/debug.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4840 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/resources/pygments.css
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.785791 ark-7.1.0/ark/bundle/lib/debug/templates/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2486 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/debug/templates/node.ibis
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.786962 ark-7.1.0/ark/bundle/lib/graphite/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      607 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1245 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/readme.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.771439 ark-7.1.0/ark/bundle/lib/graphite/resources/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.788891 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.802458 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    93768 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    13172 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    75680 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14196 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    99800 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14648 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)   189596 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    13612 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    77596 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14200 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    75580 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14388 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)     4512 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2047 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)    11077 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/graphite.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)     5027 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/resources/assets/pygments.css
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.802940 ark-7.1.0/ark/bundle/lib/graphite/templates/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1800 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/lib/graphite/templates/node.ibis
+-rw-r--r--   0 dmulholl   (501) staff       (20)      448 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/site.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.804494 ark-7.1.0/ark/bundle/src/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      551 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/about.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4349 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/index.stx
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.805345 ark-7.1.0/ark/bundle/src/parent/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/parent/child-one.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/parent/child-two.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1097 2023-04-29 12:10:51.000000 ark-7.1.0/ark/bundle/src/parent.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.810592 ark-7.1.0/ark/cli/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1831 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/__init__.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2704 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/add.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3091 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/build.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      903 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/clear.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1375 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/deploy.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1244 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/init.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1313 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/open.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2904 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/serve.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2319 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/tree.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4019 2023-04-29 12:10:51.000000 ark-7.1.0/ark/cli/watch.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2882 2023-04-29 12:10:51.000000 ark-7.1.0/ark/events.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.813867 ark-7.1.0/ark/extensions/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.818509 ark-7.1.0/ark/extensions/__pycache__/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3625 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_automenu.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1256 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_ibis.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1556 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_jinja.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      935 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_markdown.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1600 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_shortcodes.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      828 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_syntext.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1267 2023-04-29 12:13:49.000000 ark-7.1.0/ark/extensions/__pycache__/ark_yaml.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3038 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_automenu.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      484 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_ibis.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      731 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_jinja.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      368 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_markdown.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1057 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_shortcodes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      335 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_syntext.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      541 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions/ark_yaml.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1658 2023-04-29 12:10:51.000000 ark-7.1.0/ark/extensions.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3051 2023-04-29 12:10:51.000000 ark-7.1.0/ark/filters.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2604 2023-04-29 12:10:51.000000 ark-7.1.0/ark/hashes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)    11019 2023-04-29 12:10:51.000000 ark-7.1.0/ark/nodes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1880 2023-04-29 12:10:51.000000 ark-7.1.0/ark/renderers.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     7623 2023-04-29 12:10:51.000000 ark-7.1.0/ark/site.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2606 2023-04-29 12:10:51.000000 ark-7.1.0/ark/templates.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     6549 2023-04-29 12:10:51.000000 ark-7.1.0/ark/utils.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-30 12:00:28.781495 ark-7.1.0/ark.egg-info/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      667 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/PKG-INFO
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2711 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/SOURCES.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        1 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/dependency_links.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)       33 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/entry_points.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      118 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/requires.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        4 2023-04-30 12:00:28.000000 ark-7.1.0/ark.egg-info/top_level.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1212 2016-08-25 13:09:14.000000 ark-7.1.0/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      208 2023-04-29 12:10:51.000000 ark-7.1.0/readme.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)       38 2023-04-30 12:00:28.820130 ark-7.1.0/setup.cfg
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)     2084 2023-04-30 11:29:49.000000 ark-7.1.0/setup.py
```

### Comparing `ark-7.0.0/PKG-INFO` & `ark-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ark
-Version: 7.0.0
+Version: 7.1.0
 Summary: A static website generator for people who enjoy the simpler things in life.
 Home-page: https://github.com/dmulholl/ark
 Author: Darren Mulholland
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Public Domain
```

### Comparing `ark-7.0.0/ark/__init__.py` & `ark-7.1.0/ark/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ------------------------------------------------------------------------------
 # Ark: a static website generator.
 # ------------------------------------------------------------------------------
 
-__version__ = '7.0.0'
+__version__ = '7.1.0'
 
 import sys
 if sys.version_info < (3, 10):
     sys.exit('Error: Ark requires Python 3.10 or later.')
 
 
 # On Windows, use the 'colorama' package if it's available to support ANSI
```

### Comparing `ark-7.0.0/ark/__main__.py` & `ark-7.1.0/ark/__main__.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/debug/license.txt` & `ark-7.1.0/ark/bundle/lib/debug/license.txt`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/debug/resources/debug.css` & `ark-7.1.0/ark/bundle/lib/debug/resources/debug.css`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/debug/resources/pygments.css` & `ark-7.1.0/ark/bundle/lib/debug/resources/pygments.css`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/debug/templates/node.ibis` & `ark-7.1.0/ark/bundle/lib/debug/templates/node.ibis`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/license.txt` & `ark-7.1.0/ark/bundle/lib/graphite/license.txt`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/readme.md` & `ark-7.1.0/ark/bundle/lib/graphite/readme.md`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts.css` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/fonts.css`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/graphite.css` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/graphite.css`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/pygments.css` & `ark-7.1.0/ark/bundle/lib/graphite/resources/assets/pygments.css`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/lib/graphite/templates/node.ibis` & `ark-7.1.0/ark/bundle/lib/graphite/templates/node.ibis`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/src/about.md` & `ark-7.1.0/ark/bundle/src/about.md`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/src/index.stx` & `ark-7.1.0/ark/bundle/src/index.stx`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/src/parent/child-one.md` & `ark-7.1.0/ark/bundle/src/parent/child-one.md`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/src/parent/child-two.md` & `ark-7.1.0/ark/bundle/src/parent/child-two.md`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/bundle/src/parent.md` & `ark-7.1.0/ark/bundle/src/parent.md`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/__init__.py` & `ark-7.1.0/ark/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/add.py` & `ark-7.1.0/ark/cli/add.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/build.py` & `ark-7.1.0/ark/cli/build.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/clear.py` & `ark-7.1.0/ark/cli/clear.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/deploy.py` & `ark-7.1.0/ark/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/init.py` & `ark-7.1.0/ark/cli/init.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/open.py` & `ark-7.1.0/ark/cli/open.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/serve.py` & `ark-7.1.0/ark/cli/serve.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/tree.py` & `ark-7.1.0/ark/cli/tree.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/cli/watch.py` & `ark-7.1.0/ark/cli/watch.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/events.py` & `ark-7.1.0/ark/events.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/extensions/__pycache__/ark_automenu.cpython-311.pyc` & `ark-7.1.0/ark/extensions/__pycache__/ark_automenu.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x69424c64 (Fri Apr 28 22:02:17 2023 UTC)
+moddate:  0x4b094d64 (Sat Apr 29 12:10:51 2023 UTC)
 files sz: 3038
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `ark-7.0.0/ark/extensions/__pycache__/ark_ibis.cpython-311.pyc` & `ark-7.1.0/ark/extensions/__pycache__/ark_ibis.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb3424c64 (Fri Apr 28 22:03:31 2023 UTC)
+moddate:  0x4b094d64 (Sat Apr 29 12:10:51 2023 UTC)
 files sz: 484
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `ark-7.0.0/ark/extensions/__pycache__/ark_jinja.cpython-311.pyc` & `ark-7.1.0/ark/extensions/__pycache__/ark_jinja.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc4424c64 (Fri Apr 28 22:03:48 2023 UTC)
+moddate:  0x4b094d64 (Sat Apr 29 12:10:51 2023 UTC)
 files sz: 731
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `ark-7.0.0/ark/extensions/__pycache__/ark_markdown.cpython-311.pyc` & `ark-7.1.0/ark/extensions/__pycache__/ark_markdown.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd6424c64 (Fri Apr 28 22:04:06 2023 UTC)
+moddate:  0x4b094d64 (Sat Apr 29 12:10:51 2023 UTC)
 files sz: 368
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `ark-7.0.0/ark/extensions/__pycache__/ark_shortcodes.cpython-311.pyc` & `ark-7.1.0/ark/extensions/__pycache__/ark_shortcodes.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xee424c64 (Fri Apr 28 22:04:30 2023 UTC)
+moddate:  0x4b094d64 (Sat Apr 29 12:10:51 2023 UTC)
 files sz: 1057
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `ark-7.0.0/ark/extensions/__pycache__/ark_syntext.cpython-311.pyc` & `ark-7.1.0/ark/extensions/__pycache__/ark_syntext.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfc424c64 (Fri Apr 28 22:04:44 2023 UTC)
+moddate:  0x4b094d64 (Sat Apr 29 12:10:51 2023 UTC)
 files sz: 335
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `ark-7.0.0/ark/extensions/__pycache__/ark_yaml.cpython-311.pyc` & `ark-7.1.0/ark/extensions/__pycache__/ark_yaml.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0c434c64 (Fri Apr 28 22:05:00 2023 UTC)
+moddate:  0x4b094d64 (Sat Apr 29 12:10:51 2023 UTC)
 files sz: 541
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `ark-7.0.0/ark/extensions/ark_automenu.py` & `ark-7.1.0/ark/extensions/ark_automenu.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/extensions/ark_jinja.py` & `ark-7.1.0/ark/extensions/ark_jinja.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/extensions/ark_shortcodes.py` & `ark-7.1.0/ark/extensions/ark_shortcodes.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/extensions/ark_yaml.py` & `ark-7.1.0/ark/extensions/ark_yaml.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/extensions.py` & `ark-7.1.0/ark/extensions.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/filters.py` & `ark-7.1.0/ark/filters.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/hashes.py` & `ark-7.1.0/ark/hashes.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/nodes.py` & `ark-7.1.0/ark/nodes.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/renderers.py` & `ark-7.1.0/ark/renderers.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/site.py` & `ark-7.1.0/ark/site.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/templates.py` & `ark-7.1.0/ark/templates.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark/utils.py` & `ark-7.1.0/ark/utils.py`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/ark.egg-info/PKG-INFO` & `ark-7.1.0/ark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ark
-Version: 7.0.0
+Version: 7.1.0
 Summary: A static website generator for people who enjoy the simpler things in life.
 Home-page: https://github.com/dmulholl/ark
 Author: Darren Mulholland
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Public Domain
```

### Comparing `ark-7.0.0/ark.egg-info/SOURCES.txt` & `ark-7.1.0/ark.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -69,22 +69,8 @@
 ark/extensions/ark_yaml.py
 ark/extensions/__pycache__/ark_automenu.cpython-311.pyc
 ark/extensions/__pycache__/ark_ibis.cpython-311.pyc
 ark/extensions/__pycache__/ark_jinja.cpython-311.pyc
 ark/extensions/__pycache__/ark_markdown.cpython-311.pyc
 ark/extensions/__pycache__/ark_shortcodes.cpython-311.pyc
 ark/extensions/__pycache__/ark_syntext.cpython-311.pyc
-ark/extensions/__pycache__/ark_yaml.cpython-311.pyc
-ark/extensions/__pycache__/ivy_automenu.cpython-310.pyc
-ark/extensions/__pycache__/ivy_automenu.cpython-311.pyc
-ark/extensions/__pycache__/ivy_ibis.cpython-310.pyc
-ark/extensions/__pycache__/ivy_ibis.cpython-311.pyc
-ark/extensions/__pycache__/ivy_jinja.cpython-310.pyc
-ark/extensions/__pycache__/ivy_jinja.cpython-311.pyc
-ark/extensions/__pycache__/ivy_markdown.cpython-310.pyc
-ark/extensions/__pycache__/ivy_markdown.cpython-311.pyc
-ark/extensions/__pycache__/ivy_shortcodes.cpython-310.pyc
-ark/extensions/__pycache__/ivy_shortcodes.cpython-311.pyc
-ark/extensions/__pycache__/ivy_syntext.cpython-310.pyc
-ark/extensions/__pycache__/ivy_syntext.cpython-311.pyc
-ark/extensions/__pycache__/ivy_yaml.cpython-310.pyc
-ark/extensions/__pycache__/ivy_yaml.cpython-311.pyc
+ark/extensions/__pycache__/ark_yaml.cpython-311.pyc
```

### Comparing `ark-7.0.0/license.txt` & `ark-7.1.0/license.txt`

 * *Files identical despite different names*

### Comparing `ark-7.0.0/setup.py` & `ark-7.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         'console_scripts': [
             'ark = ark:main',
         ],
     },
     install_requires = [
         'markdown ~= 3.0',
         'pygments ~= 2.0',
-        'pyyaml ~= 5.0',
-        'jinja2 ~= 2.0',
+        'pyyaml ~= 6.0',
+        'jinja2 ~= 3.0',
         'syntext ~= 3.0',
         'ibis ~= 3.0',
         'shortcodes ~= 5.1',
         'argslib ~= 2.0',
         'colorama ~= 0.4',
     ],
     python_requires = ">=3.8",
```

