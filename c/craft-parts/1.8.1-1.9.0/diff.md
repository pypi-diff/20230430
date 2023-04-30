# Comparing `tmp/craft-parts-1.8.1.tar.gz` & `tmp/craft-parts-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-parts-1.8.1.tar", last modified: Tue Jul  5 17:12:10 2022, max compression
+gzip compressed data, was "craft-parts-1.9.0.tar", last modified: Fri Jul 15 12:06:22 2022, max compression
```

## Comparing `craft-parts-1.8.1.tar` & `craft-parts-1.9.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.696387 craft-parts-1.8.1/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2021-10-29 12:01:06.000000 craft-parts-1.8.1/LICENSE
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2256 2022-07-05 17:12:10.700387 craft-parts-1.8.1/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      170 2021-12-08 22:19:58.000000 craft-parts-1.8.1/README
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1475 2022-02-07 21:00:11.000000 craft-parts-1.8.1/README.md
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.664386 craft-parts-1.8.1/craft_parts/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1298 2022-07-05 16:51:28.000000 craft-parts-1.8.1/craft_parts/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      776 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/__main__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2374 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/actions.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4794 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/callbacks.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3568 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/ctl.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2205 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/dirs.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    17398 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/errors.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.688387 craft-parts-1.8.1/craft_parts/executor/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      834 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/executor/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4287 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/executor/collisions.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     9044 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/executor/environment.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    10732 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/executor/executor.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     8028 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/executor/filesets.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     8584 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/executor/migration.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3978 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/executor/organize.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    37847 2022-07-05 16:50:03.000000 craft-parts-1.8.1/craft_parts/executor/part_handler.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    12574 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/executor/step_handler.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    16113 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/infos.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    12720 2022-06-30 21:08:31.000000 craft-parts-1.8.1/craft_parts/lifecycle_manager.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    10193 2022-06-30 21:08:31.000000 craft-parts-1.8.1/craft_parts/main.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.688387 craft-parts-1.8.1/craft_parts/overlays/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1375 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/overlays/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5075 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/overlays/chroot.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1960 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/overlays/errors.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5072 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/overlays/layers.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3564 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/overlays/overlay_fs.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     7655 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/overlays/overlay_manager.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4928 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/overlays/overlays.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.688387 craft-parts-1.8.1/craft_parts/packages/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1181 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    14724 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/apt_cache.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     8429 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/base.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    20658 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/deb.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1705 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/deb_package.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     8114 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/errors.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     9915 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/normalize.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1295 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/platform.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    14613 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/packages/snaps.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    13452 2022-06-30 19:24:41.000000 craft-parts-1.8.1/craft_parts/parts.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.692387 craft-parts-1.8.1/craft_parts/plugins/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1240 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3826 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/autotools_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3572 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/base.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4055 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/cmake_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4458 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/dotnet_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2316 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/dump_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4543 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/go_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3374 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/make_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4371 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/meson_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2071 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/nil_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6815 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/npm_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3653 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/plugins.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1331 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/properties.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     7313 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/python_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4641 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/rust_plugin.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6056 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/plugins/validator.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/py.typed
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    15827 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sequencer.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.696387 craft-parts-1.8.1/craft_parts/sources/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1032 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     8268 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/base.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2519 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/cache.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2305 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/checksum.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5273 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/errors.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    10094 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/git_source.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6229 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/local_source.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4761 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/snap_source.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6598 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/sources.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4900 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/tar_source.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3793 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/sources/zip_source.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.696387 craft-parts-1.8.1/craft_parts/state_manager/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      870 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2848 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/build_state.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2445 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/overlay_state.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2482 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/prime_state.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2801 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/pull_state.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4993 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/reports.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2669 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/stage_state.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    17854 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/state_manager.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     4354 2022-06-30 17:02:18.000000 craft-parts-1.8.1/craft_parts/state_manager/states.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5720 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/state_manager/step_state.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2959 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/steps.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.696387 craft-parts-1.8.1/craft_parts/utils/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      832 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/utils/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    10289 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/utils/file_utils.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1454 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/utils/formatting_utils.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    11657 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/utils/os_utils.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2634 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/utils/url_utils.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2713 2022-06-29 23:30:04.000000 craft-parts-1.8.1/craft_parts/xattrs.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-05 17:12:10.684387 craft-parts-1.8.1/craft_parts.egg-info/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2256 2022-07-05 17:12:10.000000 craft-parts-1.8.1/craft_parts.egg-info/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2944 2022-07-05 17:12:10.000000 craft-parts-1.8.1/craft_parts.egg-info/SOURCES.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2022-07-05 17:12:10.000000 craft-parts-1.8.1/craft_parts.egg-info/dependency_links.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       51 2022-07-05 17:12:10.000000 craft-parts-1.8.1/craft_parts.egg-info/entry_points.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2021-06-29 21:00:42.000000 craft-parts-1.8.1/craft_parts.egg-info/not-zip-safe
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      577 2022-07-05 17:12:10.000000 craft-parts-1.8.1/craft_parts.egg-info/requires.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       12 2022-07-05 17:12:10.000000 craft-parts-1.8.1/craft_parts.egg-info/top_level.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      639 2022-06-30 19:24:41.000000 craft-parts-1.8.1/pyproject.toml
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      472 2022-07-05 17:12:10.700387 craft-parts-1.8.1/setup.cfg
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3172 2022-07-05 16:51:28.000000 craft-parts-1.8.1/setup.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.884630 craft-parts-1.9.0/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2021-10-29 12:01:06.000000 craft-parts-1.9.0/LICENSE
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2256 2022-07-15 12:06:22.884630 craft-parts-1.9.0/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      170 2021-12-08 22:19:58.000000 craft-parts-1.9.0/README
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1475 2022-02-07 21:00:11.000000 craft-parts-1.9.0/README.md
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.860630 craft-parts-1.9.0/craft_parts/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1298 2022-07-15 12:06:10.000000 craft-parts-1.9.0/craft_parts/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      776 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/__main__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2374 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/actions.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4794 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/callbacks.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3568 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/ctl.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2205 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/dirs.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    17398 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/errors.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.876630 craft-parts-1.9.0/craft_parts/executor/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      834 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/executor/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4287 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/executor/collisions.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     9044 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/executor/environment.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    10732 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/executor/executor.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     8028 2022-07-15 00:06:50.000000 craft-parts-1.9.0/craft_parts/executor/filesets.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     8584 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/executor/migration.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3978 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/executor/organize.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    37847 2022-07-05 16:50:03.000000 craft-parts-1.9.0/craft_parts/executor/part_handler.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    12574 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/executor/step_handler.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    16113 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/infos.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    12720 2022-06-30 21:08:31.000000 craft-parts-1.9.0/craft_parts/lifecycle_manager.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    10193 2022-06-30 21:08:31.000000 craft-parts-1.9.0/craft_parts/main.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.876630 craft-parts-1.9.0/craft_parts/overlays/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1375 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/overlays/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5075 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/overlays/chroot.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1960 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/overlays/errors.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5072 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/overlays/layers.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3564 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/overlays/overlay_fs.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7655 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/overlays/overlay_manager.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4928 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/overlays/overlays.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.880630 craft-parts-1.9.0/craft_parts/packages/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1181 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/packages/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    14724 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/packages/apt_cache.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     8429 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/packages/base.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    21496 2022-07-11 18:54:43.000000 craft-parts-1.9.0/craft_parts/packages/deb.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1705 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/packages/deb_package.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     8114 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/packages/errors.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     9915 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/packages/normalize.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1295 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/packages/platform.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    14613 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/packages/snaps.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    13452 2022-07-11 16:54:32.000000 craft-parts-1.9.0/craft_parts/parts.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.880630 craft-parts-1.9.0/craft_parts/plugins/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1240 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3826 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/autotools_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3572 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/base.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4055 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/cmake_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4458 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/dotnet_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2316 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/dump_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4543 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/go_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3374 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/make_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4371 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/meson_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2071 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/nil_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6815 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/npm_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3653 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/plugins.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1331 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/properties.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7313 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/python_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4641 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/rust_plugin.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6056 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/plugins/validator.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        0 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/py.typed
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    15827 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sequencer.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.880630 craft-parts-1.9.0/craft_parts/sources/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1032 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     8268 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/base.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2519 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/cache.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2305 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/checksum.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5273 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/errors.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    10094 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/git_source.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6229 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/local_source.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4761 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/snap_source.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6598 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/sources.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4900 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/tar_source.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3793 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/sources/zip_source.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.884630 craft-parts-1.9.0/craft_parts/state_manager/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      870 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2848 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/build_state.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2445 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/overlay_state.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2482 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/prime_state.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2801 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/pull_state.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4993 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/reports.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2669 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/stage_state.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    17854 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/state_manager.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     4354 2022-06-30 17:02:18.000000 craft-parts-1.9.0/craft_parts/state_manager/states.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5720 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/state_manager/step_state.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2959 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/steps.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.884630 craft-parts-1.9.0/craft_parts/utils/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      832 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/utils/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    10289 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/utils/file_utils.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1454 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/utils/formatting_utils.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    11657 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/utils/os_utils.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2634 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/utils/url_utils.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2713 2022-06-29 23:30:04.000000 craft-parts-1.9.0/craft_parts/xattrs.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2022-07-15 12:06:22.872630 craft-parts-1.9.0/craft_parts.egg-info/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2256 2022-07-15 12:06:22.000000 craft-parts-1.9.0/craft_parts.egg-info/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2944 2022-07-15 12:06:22.000000 craft-parts-1.9.0/craft_parts.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2022-07-15 12:06:22.000000 craft-parts-1.9.0/craft_parts.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       51 2022-07-15 12:06:22.000000 craft-parts-1.9.0/craft_parts.egg-info/entry_points.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2021-06-29 21:00:42.000000 craft-parts-1.9.0/craft_parts.egg-info/not-zip-safe
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      577 2022-07-15 12:06:22.000000 craft-parts-1.9.0/craft_parts.egg-info/requires.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       12 2022-07-15 12:06:22.000000 craft-parts-1.9.0/craft_parts.egg-info/top_level.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      639 2022-06-30 19:24:41.000000 craft-parts-1.9.0/pyproject.toml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      472 2022-07-15 12:06:22.884630 craft-parts-1.9.0/setup.cfg
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3172 2022-07-15 12:06:10.000000 craft-parts-1.9.0/setup.py
```

### Comparing `craft-parts-1.8.1/LICENSE` & `craft-parts-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/PKG-INFO` & `craft-parts-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-parts
-Version: 1.8.1
+Version: 1.9.0
 Summary: Craft parts tooling
 Home-page: https://github.com/canonical/craft-parts
 Author: Canonical Ltd.
 Author-email: snapcraft@lists.snapcraft.io
 License: GNU General Public License v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `craft-parts-1.8.1/README.md` & `craft-parts-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/__init__.py` & `craft-parts-1.9.0/craft_parts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Craft a project from several parts."""
 
-__version__ = "1.8.1"
+__version__ = "1.9.0"
 
 from . import plugins
 from .actions import Action, ActionType
 from .dirs import ProjectDirs
 from .errors import PartsError
 from .executor.environment import expand_environment
 from .infos import PartInfo, ProjectInfo, StepInfo
```

### Comparing `craft-parts-1.8.1/craft_parts/__main__.py` & `craft-parts-1.9.0/craft_parts/__main__.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/actions.py` & `craft-parts-1.9.0/craft_parts/actions.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/callbacks.py` & `craft-parts-1.9.0/craft_parts/callbacks.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/ctl.py` & `craft-parts-1.9.0/craft_parts/ctl.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/dirs.py` & `craft-parts-1.9.0/craft_parts/dirs.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/errors.py` & `craft-parts-1.9.0/craft_parts/errors.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/executor/__init__.py` & `craft-parts-1.9.0/craft_parts/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/executor/collisions.py` & `craft-parts-1.9.0/craft_parts/executor/collisions.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/executor/environment.py` & `craft-parts-1.9.0/craft_parts/executor/environment.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/executor/executor.py` & `craft-parts-1.9.0/craft_parts/executor/executor.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/executor/filesets.py` & `craft-parts-1.9.0/craft_parts/executor/filesets.py`

 * *Ordering differences only*

 * *Files identical despite different names*

```diff
@@ -61,28 +61,28 @@
         self._list.remove(item)
 
     def combine(self, other: "Fileset") -> None:
         """Combine the entries in this fileset with entries from another fileset.
 
         :param other: The fileset to combine with.
         """
-        my_excludes = set(self.excludes)
-        other_includes = set(other.includes)
-
-        contradicting_set = set.intersection(my_excludes, other_includes)
-        if contradicting_set:
-            raise errors.FilesetConflict(contradicting_set)
-
         to_combine = False
         # combine if the other fileset has a wildcard
         # XXX: should this only be a single wildcard and possibly excludes?
         if "*" in other.entries:
             to_combine = True
             other.remove("*")
 
+        my_excludes = set(self.excludes)
+        other_includes = set(other.includes)
+
+        contradicting_set = set.intersection(my_excludes, other_includes)
+        if contradicting_set:
+            raise errors.FilesetConflict(contradicting_set)
+
         # combine if the other fileset is only excludes
         if {x[0] for x in other.entries} == set("-"):
             to_combine = True
 
         if to_combine:
             self._list = list(set(self._list + other.entries))
         else:
```

### Comparing `craft-parts-1.8.1/craft_parts/executor/migration.py` & `craft-parts-1.9.0/craft_parts/executor/migration.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/executor/organize.py` & `craft-parts-1.9.0/craft_parts/executor/organize.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/executor/part_handler.py` & `craft-parts-1.9.0/craft_parts/executor/part_handler.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/executor/step_handler.py` & `craft-parts-1.9.0/craft_parts/executor/step_handler.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/infos.py` & `craft-parts-1.9.0/craft_parts/infos.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/lifecycle_manager.py` & `craft-parts-1.9.0/craft_parts/lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/main.py` & `craft-parts-1.9.0/craft_parts/main.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/overlays/__init__.py` & `craft-parts-1.9.0/craft_parts/overlays/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/overlays/chroot.py` & `craft-parts-1.9.0/craft_parts/overlays/chroot.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/overlays/errors.py` & `craft-parts-1.9.0/craft_parts/overlays/errors.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/overlays/layers.py` & `craft-parts-1.9.0/craft_parts/overlays/layers.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/overlays/overlay_fs.py` & `craft-parts-1.9.0/craft_parts/overlays/overlay_fs.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/overlays/overlay_manager.py` & `craft-parts-1.9.0/craft_parts/overlays/overlay_manager.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/overlays/overlays.py` & `craft-parts-1.9.0/craft_parts/overlays/overlays.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/packages/__init__.py` & `craft-parts-1.9.0/craft_parts/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/packages/apt_cache.py` & `craft-parts-1.9.0/craft_parts/packages/apt_cache.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/packages/base.py` & `craft-parts-1.9.0/craft_parts/packages/base.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/packages/deb.py` & `craft-parts-1.9.0/craft_parts/packages/deb.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import os
 import pathlib
 import re
 import subprocess
 import sys
 import tempfile
 from pathlib import Path
-from typing import Dict, List, Set, Tuple
+from typing import Dict, List, Sequence, Set, Tuple
 
 from craft_parts.utils import file_utils, os_utils
 
 from . import errors
 from .base import BaseRepository, get_pkg_name_parts, mark_origin_stage_package
 from .deb_package import DebPackage
 from .normalize import normalize
@@ -414,14 +414,36 @@
                 ):
                     return False
 
         return True
 
     @classmethod
     @_apt_cache_wrapper
+    def _get_installed_package_versions(cls, package_names: Sequence[str]) -> List[str]:
+        packages: List[str] = []
+
+        with AptCache() as apt_cache:
+            for package_name in package_names:
+                package_version = apt_cache.get_installed_version(
+                    package_name, resolve_virtual_packages=True
+                )
+                if package_version is None:
+                    logger.debug("Expected package %s not installed", package_name)
+                    continue
+                logger.debug(
+                    "Found installed version %s for package %s",
+                    package_version,
+                    package_name,
+                )
+                packages.append(f"{package_name}={package_version}")
+
+        return packages
+
+    @classmethod
+    @_apt_cache_wrapper
     def _get_packages_marked_for_installation(
         cls, package_names: List[str]
     ) -> List[Tuple[str, str]]:
         with AptCache() as apt_cache:
             try:
                 apt_cache.mark_packages(set(package_names))
             except errors.PackageNotFound as error:
@@ -475,26 +497,31 @@
         logger.debug("Requested build-packages: %s", package_names)
 
         # Ensure we have an up-to-date cache first if we will have to
         # install anything.
         if not cls._check_if_all_packages_installed(package_names):
             install_required = True
 
+        # Collect the list of marked packages to later construct a manifest
         marked_packages = cls._get_packages_marked_for_installation(package_names)
-        packages = [f"{name}={version}" for name, version in sorted(marked_packages)]
+        marked_package_names = [name for name, _ in sorted(marked_packages)]
 
         if not list_only:
             if refresh_package_cache and install_required:
                 cls.refresh_packages_list()
             if install_required:
-                cls._install_packages(packages)
+                cls._install_packages(package_names)
             else:
-                logger.debug("Requested build-packages already installed: %s", packages)
+                logger.debug(
+                    "Requested build-packages already installed: %s", package_names
+                )
 
-        return packages
+        # This result is a best effort approach for deps and virtual packages
+        # as they are not part of the installation list.
+        return cls._get_installed_package_versions(marked_package_names)
 
     @classmethod
     def _install_packages(cls, package_names: List[str]) -> None:
         logger.debug("Installing packages: %s", " ".join(package_names))
         env = os.environ.copy()
         env.update(
             {
@@ -517,20 +544,14 @@
         # https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=555632
 
         try:
             process_run(apt_command + package_names, env=env, stdin=subprocess.DEVNULL)
         except subprocess.CalledProcessError as err:
             raise errors.BuildPackagesNotInstalled(packages=package_names) from err
 
-        versionless_names = [get_pkg_name_parts(p)[0] for p in package_names]
-        try:
-            process_run(["apt-mark", "auto"] + versionless_names, env=env)
-        except subprocess.CalledProcessError as err:
-            logger.warning("Impossible to mark packages as auto-installed: %s", err)
-
     @classmethod
     @_apt_cache_wrapper
     def fetch_stage_packages(
         cls,
         *,
         cache_dir: Path,
         package_names: List[str],
```

### Comparing `craft-parts-1.8.1/craft_parts/packages/deb_package.py` & `craft-parts-1.9.0/craft_parts/packages/deb_package.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/packages/errors.py` & `craft-parts-1.9.0/craft_parts/packages/errors.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/packages/normalize.py` & `craft-parts-1.9.0/craft_parts/packages/normalize.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/packages/platform.py` & `craft-parts-1.9.0/craft_parts/packages/platform.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/packages/snaps.py` & `craft-parts-1.9.0/craft_parts/packages/snaps.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/parts.py` & `craft-parts-1.9.0/craft_parts/parts.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/__init__.py` & `craft-parts-1.9.0/craft_parts/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/autotools_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/autotools_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/base.py` & `craft-parts-1.9.0/craft_parts/plugins/base.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/cmake_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/cmake_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/dotnet_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/dotnet_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/dump_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/dump_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/go_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/go_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/make_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/make_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/meson_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/meson_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/nil_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/nil_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/npm_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/npm_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/plugins.py` & `craft-parts-1.9.0/craft_parts/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/properties.py` & `craft-parts-1.9.0/craft_parts/plugins/properties.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/python_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/python_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/rust_plugin.py` & `craft-parts-1.9.0/craft_parts/plugins/rust_plugin.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/plugins/validator.py` & `craft-parts-1.9.0/craft_parts/plugins/validator.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sequencer.py` & `craft-parts-1.9.0/craft_parts/sequencer.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/__init__.py` & `craft-parts-1.9.0/craft_parts/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/base.py` & `craft-parts-1.9.0/craft_parts/sources/base.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/cache.py` & `craft-parts-1.9.0/craft_parts/sources/cache.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/checksum.py` & `craft-parts-1.9.0/craft_parts/sources/checksum.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/errors.py` & `craft-parts-1.9.0/craft_parts/sources/errors.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/git_source.py` & `craft-parts-1.9.0/craft_parts/sources/git_source.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/local_source.py` & `craft-parts-1.9.0/craft_parts/sources/local_source.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/snap_source.py` & `craft-parts-1.9.0/craft_parts/sources/snap_source.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/sources.py` & `craft-parts-1.9.0/craft_parts/sources/sources.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/tar_source.py` & `craft-parts-1.9.0/craft_parts/sources/tar_source.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/sources/zip_source.py` & `craft-parts-1.9.0/craft_parts/sources/zip_source.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/__init__.py` & `craft-parts-1.9.0/craft_parts/state_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/build_state.py` & `craft-parts-1.9.0/craft_parts/state_manager/build_state.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/overlay_state.py` & `craft-parts-1.9.0/craft_parts/state_manager/overlay_state.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/prime_state.py` & `craft-parts-1.9.0/craft_parts/state_manager/prime_state.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/pull_state.py` & `craft-parts-1.9.0/craft_parts/state_manager/pull_state.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/reports.py` & `craft-parts-1.9.0/craft_parts/state_manager/reports.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/stage_state.py` & `craft-parts-1.9.0/craft_parts/state_manager/stage_state.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/state_manager.py` & `craft-parts-1.9.0/craft_parts/state_manager/state_manager.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/states.py` & `craft-parts-1.9.0/craft_parts/state_manager/states.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/state_manager/step_state.py` & `craft-parts-1.9.0/craft_parts/state_manager/step_state.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/steps.py` & `craft-parts-1.9.0/craft_parts/steps.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/utils/__init__.py` & `craft-parts-1.9.0/craft_parts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/utils/file_utils.py` & `craft-parts-1.9.0/craft_parts/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/utils/formatting_utils.py` & `craft-parts-1.9.0/craft_parts/utils/formatting_utils.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/utils/os_utils.py` & `craft-parts-1.9.0/craft_parts/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/utils/url_utils.py` & `craft-parts-1.9.0/craft_parts/utils/url_utils.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts/xattrs.py` & `craft-parts-1.9.0/craft_parts/xattrs.py`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts.egg-info/PKG-INFO` & `craft-parts-1.9.0/craft_parts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-parts
-Version: 1.8.1
+Version: 1.9.0
 Summary: Craft parts tooling
 Home-page: https://github.com/canonical/craft-parts
 Author: Canonical Ltd.
 Author-email: snapcraft@lists.snapcraft.io
 License: GNU General Public License v3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `craft-parts-1.8.1/craft_parts.egg-info/SOURCES.txt` & `craft-parts-1.9.0/craft_parts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/craft_parts.egg-info/requires.txt` & `craft-parts-1.9.0/craft_parts.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/pyproject.toml` & `craft-parts-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft-parts-1.8.1/setup.py` & `craft-parts-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     "doc": doc_requires,
     "test": test_requires,
 }
 
 
 setup(
     name="craft-parts",
-    version="1.8.1",
+    version="1.9.0",
     description="Craft parts tooling",
     long_description=readme,
     author="Canonical Ltd.",
     author_email="snapcraft@lists.snapcraft.io",
     url="https://github.com/canonical/craft-parts",
     license="GNU General Public License v3",
     python_requires=">=3.7",
```

