# Comparing `tmp/RenderWatcher-0.0.2.tar.gz` & `tmp/RenderWatcher-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RenderWatcher-0.0.2.tar", last modified: Wed Jan 11 13:49:35 2023, max compression
+gzip compressed data, was "RenderWatcher-0.0.4.tar", last modified: Sun Apr 30 14:16:00 2023, max compression
```

## Comparing `RenderWatcher-0.0.2.tar` & `RenderWatcher-0.0.4.tar`

### file list

```diff
@@ -1,757 +1,763 @@
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:35.036414 RenderWatcher-0.0.2/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      200 2023-01-11 13:45:59.000000 RenderWatcher-0.0.2/CHANGELOG.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1073 2022-12-20 18:29:21.000000 RenderWatcher-0.0.2/LICENSE
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       25 2022-12-28 01:06:10.000000 RenderWatcher-0.0.2/MANIFEST.in
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      296 2023-01-11 13:49:35.036414 RenderWatcher-0.0.2/PKG-INFO
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      115 2022-12-28 01:08:29.000000 RenderWatcher-0.0.2/README.md
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.284405 RenderWatcher-0.0.2/RenderWatcher.egg-info/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      296 2023-01-11 13:49:34.000000 RenderWatcher-0.0.2/RenderWatcher.egg-info/PKG-INFO
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    44775 2023-01-11 13:49:34.000000 RenderWatcher-0.0.2/RenderWatcher.egg-info/SOURCES.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        1 2023-01-11 13:49:34.000000 RenderWatcher-0.0.2/RenderWatcher.egg-info/dependency_links.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       18 2023-01-11 13:49:34.000000 RenderWatcher-0.0.2/RenderWatcher.egg-info/top_level.txt
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.284405 RenderWatcher-0.0.2/render_watcher/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:46:04.000000 RenderWatcher-0.0.2/render_watcher/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1957 2023-01-11 13:34:48.000000 RenderWatcher-0.0.2/render_watcher/core.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5078 2022-12-28 11:40:03.000000 RenderWatcher-0.0.2/render_watcher/ui.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       38 2023-01-11 13:49:35.036414 RenderWatcher-0.0.2/setup.cfg
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      435 2023-01-11 13:34:48.000000 RenderWatcher-0.0.2/setup.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.272405 RenderWatcher-0.0.2/venv/
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.300405 RenderWatcher-0.0.2/venv/bin/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1200 2022-12-20 18:31:25.000000 RenderWatcher-0.0.2/venv/bin/activate_this.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.272405 RenderWatcher-0.0.2/venv/lib/
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.272405 RenderWatcher-0.0.2/venv/lib/python3.10/
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.320405 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.320405 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/_distutils_hack/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3688 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/_distutils_hack/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       44 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/_distutils_hack/override.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5662 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/_virtualenv.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.332405 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      357 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1198 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/__main__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1444 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/__pip-runner__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.356406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      573 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10234 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/build_env.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10734 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cache.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.372406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      132 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6676 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7842 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    29381 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      774 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2472 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/main.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4338 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10817 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1968 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18172 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5118 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      116 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.380406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3882 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7582 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1685 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/check.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9815 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6573 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5289 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/download.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2951 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1703 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1132 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/help.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4762 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/index.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3374 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31726 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/install.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12343 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/list.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5697 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/search.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/show.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3680 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7396 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13529 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/configuration.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.392406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      858 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1221 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      729 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6494 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1164 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20942 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/exceptions.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.392406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       30 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16503 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/collector.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    37596 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6557 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/sources.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.396406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17552 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6302 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7867 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2573 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/base.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      340 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/main.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.396406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4280 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2595 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25277 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.416406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      107 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1882 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8181 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7457 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9773 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.432407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       63 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      990 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5877 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2520 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1030 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/index.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2617 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18083 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/link.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      738 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4644 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1907 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3858 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3600 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.436407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       50 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12190 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/auth.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2145 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/cache.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6096 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/download.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7638 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18443 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/session.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4073 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/utils.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1791 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.436407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.448407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4133 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1404 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1456 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2198 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1063 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1405 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3064 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5109 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/check.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9784 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.448407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       51 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1354 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4105 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    27407 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25091 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7074 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/pyproject.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.452407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2807 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16611 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17646 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    35600 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2858 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24045 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.452407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      583 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.452407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.464407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5220 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18963 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    27878 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5705 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9914 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2526 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5455 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11533 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8020 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.480407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1015 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1665 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1884 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5377 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      242 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5764 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3206 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1115 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2203 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1169 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3064 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5122 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      716 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3110 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4831 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      795 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11632 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21617 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1193 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/models.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2108 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5662 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9197 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7702 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8821 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1759 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3459 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4549 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.480407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      596 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3518 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18116 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5238 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11728 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22811 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13079 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.484408 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4966 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/__init__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.492407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      465 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1379 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5033 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1535 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.492407 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      242 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5271 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1033 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      778 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16416 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3946 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4154 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7105 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      774 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.496408 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       94 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      255 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4279 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.524408 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3705 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31274 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1741 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9608 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3817 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4801 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.524408 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2406 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3559 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1838 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1619 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3864 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12021 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3676 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13566 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1731 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    36913 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1731 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20735 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1737 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13919 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25796 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    42498 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1730 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    26797 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   104562 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    98484 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    98196 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   101363 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   128035 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   102774 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    95372 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5260 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3367 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2056 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30068 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.524408 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13280 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6199 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3749 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13288 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8289 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2709 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      242 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.536408 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      239 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2522 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10830 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1915 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5404 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6438 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.568409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      581 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    41259 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    51697 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20834 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    51991 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14811 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5058 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    39801 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10820 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18102 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    66262 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    23513 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    43898 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.572409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      981 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       64 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    48841 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.572409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      849 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3374 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      321 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12950 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    44375 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1881 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       21 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   206539 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.580409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1132 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1081 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6080 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34557 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.600409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      661 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      497 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11488 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4378 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1431 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8487 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4676 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30110 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15699 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4200 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14665 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.600409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      130 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      138 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/_compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3443 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/build.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6083 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/check.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3994 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      607 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6081 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.600409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      872 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10801 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2520 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12721 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.616409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   108287 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      562 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.624409 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12831 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1176 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4068 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4910 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2655 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6910 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       78 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6439 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.672410 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2999 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      353 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    23685 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1697 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1938 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.676410 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    40386 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2917 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.700410 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4810 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4104 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3314 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5086 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    35441 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21938 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5871 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19351 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5073 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2212 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5014 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7335 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4674 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11753 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    32005 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.700410 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11174 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    70232 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    53376 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      986 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2591 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3072 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3092 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4630 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6257 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.704410 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3419 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6184 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    63187 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9110 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.716410 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9171 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6426 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12936 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   213344 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.716410 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    23685 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9023 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    39129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25341 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13402 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10787 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6805 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.748411 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5178 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      440 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1397 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21443 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6377 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10187 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      575 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1286 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18560 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3823 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3879 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      733 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    35287 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      695 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30180 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4235 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2912 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    33240 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.748411 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      537 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.748411 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      156 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5872 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1583 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17592 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4794 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.844412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5944 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8808 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10096 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   140235 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1064 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2114 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      265 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9695 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3225 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1236 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7063 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      423 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5472 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19919 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      351 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      417 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22820 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1926 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2783 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1840 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      890 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10368 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6820 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3264 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9864 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4503 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17957 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1054 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7131 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    95885 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1288 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5497 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6630 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7954 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      972 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2501 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      642 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1616 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2507 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9585 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5051 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3252 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14074 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14172 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3667 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11471 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8198 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5305 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4970 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      828 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3396 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8744 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    36576 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    59746 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8161 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11303 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1391 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      166 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4449 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4773 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2842 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1591 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24224 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4374 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4425 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    26240 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1258 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34697 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    39515 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3370 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    44666 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3627 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      102 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    26060 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9169 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34549 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/six.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.848412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18364 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3314 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1944 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1496 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1376 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1908 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1383 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7550 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2790 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2145 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8011 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.848412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      396 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22633 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2943 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      254 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    80114 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.852412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3333 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10811 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       64 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20070 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    39093 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.856412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      957 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.856412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17632 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13922 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11034 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4538 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17182 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34448 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7097 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8217 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8579 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2440 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.856412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.856412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1417 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34665 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19786 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5985 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30109 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.860412 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1155 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4901 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1605 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      498 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3997 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3510 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22001 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17177 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5758 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6895 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10003 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14287 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5403 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      469 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.872413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10579 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8979 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1305 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6563 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4307 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.340406 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1093 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      125 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/entry_points.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        4 2022-12-25 02:38:31.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/top_level.txt
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.872413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   108202 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/__init__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.872413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24701 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.880413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      736 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      562 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1128 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2022 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1812 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_typing.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9518 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4929 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31944 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24067 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1811 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15470 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   232056 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.880413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/extern/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2362 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.276405 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/tests/
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.276405 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/tests/data/
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.880413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      104 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.896413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7681 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      218 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_deprecation_warning.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.944413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      250 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20813 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8572 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14894 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    47607 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18079 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.984414 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      799 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5562 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4913 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    35579 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21537 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16030 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5767 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8022 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31685 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17190 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6232 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5637 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2776 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13117 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    27482 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2822 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2603 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1298 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8397 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2017 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      671 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11712 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19005 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7597 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4827 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/config.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8876 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/core.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16380 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      139 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/debug.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3491 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7778 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    50421 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3577 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10515 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17784 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8148 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12832 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1969 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/log.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30453 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    23540 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      455 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/py35compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      212 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4691 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21349 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12483 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14696 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20985 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/util.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12514 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/version.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5133 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2392 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_imp.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.992414 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.992414 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       82 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   117968 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16256 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15130 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.996414 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      736 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      562 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1128 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2022 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1812 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_typing.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9509 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4917 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31944 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24067 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1811 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15470 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   232056 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7077 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/archive_util.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10280 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/build_meta.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:35.028415 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      217 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2381 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/alias.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16604 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      900 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4415 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_clib.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13027 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_ext.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8930 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_py.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8045 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/develop.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      960 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/dist_info.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    85308 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/easy_install.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25335 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/egg_info.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4705 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2203 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3875 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_lib.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2593 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4946 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/py36compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      468 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/register.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2128 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/rotate.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      658 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/saveopts.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5967 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/sdist.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5051 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/setopt.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9490 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/test.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      462 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/upload.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7218 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22279 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/config.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      949 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/dep_util.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5474 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/depends.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    42374 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/dist.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      524 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/errors.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1684 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/extension.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:35.028415 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/extern/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2407 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/extern/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4873 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/glob.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3567 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/installer.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      812 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/launch.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2335 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/lib2to3_ex.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5217 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/monkey.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    50561 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/msvc.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3093 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/namespaces.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    40173 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/package_index.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      245 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/py34compat.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14151 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/sandbox.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8565 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/ssl_support.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      941 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/unicode_utils.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      144 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/version.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8288 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/wheel.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      714 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/windows_support.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:34.900413 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      239 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/dependency_links.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2869 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/entry_points.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       41 2022-12-20 18:31:24.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/top_level.txt
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:35.032415 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       23 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      417 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/__main__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19075 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/bdist_wheel.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:35.032415 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2572 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9498 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/convert.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3208 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/pack.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      673 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/unpack.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15931 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/macosx_libfile.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4344 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/metadata.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1257 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/pkginfo.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      938 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/util.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:35.032415 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/__init__.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:35.032415 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/__init__.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1812 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_typing.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    28937 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7336 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/wheelfile.py
-drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-01-11 13:49:35.032415 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1125 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/LICENSE.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      108 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/entry_points.txt
--rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        6 2022-12-20 18:31:23.000000 RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/top_level.txt
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.100339 RenderWatcher-0.0.4/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      514 2023-04-13 12:09:13.000000 RenderWatcher-0.0.4/CHANGELOG.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1073 2022-12-20 18:29:21.000000 RenderWatcher-0.0.4/LICENSE
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       25 2022-12-28 01:06:10.000000 RenderWatcher-0.0.4/MANIFEST.in
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      296 2023-04-30 14:16:00.100339 RenderWatcher-0.0.4/PKG-INFO
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      115 2022-12-28 01:08:29.000000 RenderWatcher-0.0.4/README.md
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.404330 RenderWatcher-0.0.4/RenderWatcher.egg-info/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      296 2023-04-30 14:15:59.000000 RenderWatcher-0.0.4/RenderWatcher.egg-info/PKG-INFO
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    45026 2023-04-30 14:15:59.000000 RenderWatcher-0.0.4/RenderWatcher.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        1 2023-04-30 14:15:59.000000 RenderWatcher-0.0.4/RenderWatcher.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       18 2023-04-30 14:15:59.000000 RenderWatcher-0.0.4/RenderWatcher.egg-info/top_level.txt
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.420330 RenderWatcher-0.0.4/render_watcher/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:46:04.000000 RenderWatcher-0.0.4/render_watcher/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1571 2023-04-13 12:17:58.000000 RenderWatcher-0.0.4/render_watcher/core.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6889 2023-04-30 14:13:12.000000 RenderWatcher-0.0.4/render_watcher/ui.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       38 2023-04-30 14:16:00.100339 RenderWatcher-0.0.4/setup.cfg
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      435 2023-04-09 15:07:58.000000 RenderWatcher-0.0.4/setup.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.368329 RenderWatcher-0.0.4/venv/
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.420330 RenderWatcher-0.0.4/venv/bin/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1200 2022-12-20 18:31:25.000000 RenderWatcher-0.0.4/venv/bin/activate_this.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.368329 RenderWatcher-0.0.4/venv/lib/
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.368329 RenderWatcher-0.0.4/venv/lib/python3.10/
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.444331 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.444331 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/RenderWatcher-0.0.3.dist-info/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       18 2023-04-07 20:48:40.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/RenderWatcher-0.0.3.dist-info/top_level.txt
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.460331 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/_distutils_hack/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3688 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/_distutils_hack/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       44 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/_distutils_hack/override.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5662 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/_virtualenv.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.476331 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      357 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1198 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/__main__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1444 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/__pip-runner__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.500331 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      573 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10234 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/build_env.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10734 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cache.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.516331 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      132 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6676 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7842 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    29381 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      774 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2472 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/main.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4338 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10817 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1968 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18172 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5118 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      116 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.532332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3882 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7582 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1685 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/check.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9815 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6573 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5289 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/download.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2951 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1703 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1132 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/help.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4762 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/index.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3374 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31726 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/install.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12343 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/list.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5697 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/search.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/show.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3680 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7396 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13529 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/configuration.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.536332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      858 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1221 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      729 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6494 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1164 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20942 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/exceptions.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.536332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/index/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       30 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16503 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/index/collector.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    37596 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6557 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/index/sources.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.540332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17552 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6302 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7867 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2573 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/base.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      340 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/main.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.548332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4280 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2595 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25277 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.548332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      107 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1882 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8181 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7457 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9773 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.576332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       63 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      990 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5877 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2520 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1030 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/index.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2617 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18083 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/link.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      738 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4644 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1907 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3858 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3600 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.576332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       50 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12190 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/auth.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2145 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/cache.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6096 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/download.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7638 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18443 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/session.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4073 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/utils.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1791 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.576332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.580332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4133 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1404 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1456 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2198 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1063 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1405 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3064 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5109 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/check.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9784 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.580332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/install/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       51 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1354 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4105 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    27407 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25091 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7074 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/pyproject.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.584332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2807 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16611 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17646 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    35600 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2858 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24045 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.584332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      583 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.584332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.588332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5220 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18963 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    27878 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5705 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9914 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2526 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5455 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11533 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8020 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.600332 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1015 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1665 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1884 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5377 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      242 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5764 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3206 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1115 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2203 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1169 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3064 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5122 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      716 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3110 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4831 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      795 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11632 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21617 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1193 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/models.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2108 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5662 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9197 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7702 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8821 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1759 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3459 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4549 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.604333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      596 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3518 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18116 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5238 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11728 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22811 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13079 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.604333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4966 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/__init__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.616333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      465 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1379 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5033 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1535 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.616333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      242 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5271 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1033 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      778 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16416 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3946 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4154 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7105 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      774 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.616333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       94 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      255 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4279 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.632333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3705 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31274 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1741 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9608 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3817 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4801 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.632333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2406 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3559 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1838 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1619 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3864 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12021 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3676 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13566 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1731 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    36913 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1731 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20735 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1737 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13919 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25796 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    42498 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1730 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    26797 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   104562 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    98484 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    98196 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   101363 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   128035 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   102774 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    95372 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5260 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3367 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2056 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30068 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.632333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13280 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6199 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3749 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13288 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8289 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2709 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      242 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.644333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      239 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2522 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10830 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1915 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5404 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6438 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.668333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      581 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    41259 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    51697 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20834 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    51991 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14811 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5058 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    39801 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10820 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18102 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    66262 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    23513 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    43898 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.668333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distro/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      981 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       64 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    48841 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.672333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      849 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3374 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      321 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12950 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    44375 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1881 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       21 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   206539 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.680333 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1132 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1081 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6080 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34557 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.700334 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      661 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      497 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11488 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4378 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1431 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8487 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4676 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30110 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15699 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4200 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14665 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.712334 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      130 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      138 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/_compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3443 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/build.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6083 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/check.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3994 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      607 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6081 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.712334 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      872 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10801 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2520 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12721 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.724334 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   108287 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      562 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.736334 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12831 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1176 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4068 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4910 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2655 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6910 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       78 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6439 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.772335 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2999 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      353 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    23685 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1697 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1938 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.776335 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    40386 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2917 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.812335 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4810 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4104 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3314 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5086 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    35441 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21938 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5871 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19351 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5073 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2212 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5014 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7335 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4674 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11753 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    32005 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.812335 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11174 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    70232 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    53376 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      986 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2591 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3072 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3092 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4630 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6257 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.812335 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3419 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6184 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    63187 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9110 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.828335 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9171 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6426 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12936 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   213344 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.828335 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    23685 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9023 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    39129 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25341 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13402 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10787 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6805 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.848336 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5178 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      440 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1397 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21443 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6377 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10187 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      575 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1286 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18560 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3823 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3879 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      733 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    35287 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      695 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30180 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4235 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2912 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    33240 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.852336 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      537 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.852336 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      156 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5872 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1583 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17592 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4794 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.944337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5944 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8808 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10096 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   140235 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1064 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2114 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      265 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9695 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3225 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1236 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7063 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      423 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5472 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19919 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      351 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      417 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22820 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1926 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2783 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1840 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      890 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10368 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6820 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3264 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9864 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4503 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17957 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1054 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7131 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    95885 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1288 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5497 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6630 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7954 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      972 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2501 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      642 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1616 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2507 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9585 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5051 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3252 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14074 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14172 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3667 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11471 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8198 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5305 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4970 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      828 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3396 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8744 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    36576 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    59746 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8161 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11303 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1391 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      166 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4449 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4773 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2842 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1591 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24224 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4374 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4425 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    26240 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1258 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34697 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    39515 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3370 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    44666 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3627 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      102 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    26060 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9169 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34549 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/six.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.948337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18364 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3314 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1944 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1496 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1376 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1908 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1383 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7550 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2790 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2145 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8011 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.948337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tomli/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      396 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22633 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2943 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      254 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    80114 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.952337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3333 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10811 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       64 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20070 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    39093 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.952337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      957 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.952337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17632 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13922 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11034 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4538 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17182 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34448 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7097 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8217 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8579 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2440 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.952337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.952337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1417 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    34665 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19786 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5985 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30109 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.956337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1155 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4901 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1605 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      498 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3997 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3510 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22001 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17177 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5758 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6895 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10003 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14287 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5403 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      469 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.960337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10579 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8979 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1305 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6563 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4307 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.484331 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1093 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      125 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/entry_points.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        4 2022-12-25 02:38:31.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/top_level.txt
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.960337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   108202 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/__init__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.960337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24701 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.968337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      736 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      562 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1128 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2022 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1812 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_typing.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9518 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4929 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31944 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24067 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1811 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15470 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   232056 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.968337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/extern/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2362 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.372330 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/tests/
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.372330 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/tests/data/
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.968337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      104 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.968337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/render_watcher/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-07 20:48:40.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/render_watcher/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1802 2023-04-07 20:48:40.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/render_watcher/core.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5099 2023-04-07 20:48:40.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/render_watcher/ui.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.976337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7681 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      218 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_deprecation_warning.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.008338 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      250 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20813 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8572 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14894 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    47607 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    18079 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.060338 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      799 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5562 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4913 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    35579 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21537 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16030 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5767 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8022 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31685 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17190 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     6232 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5637 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2776 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13117 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    27482 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2822 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2603 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1298 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8397 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2017 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      671 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    11712 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19005 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7597 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4827 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/config.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8876 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/core.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16380 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      139 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/debug.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3491 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7778 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    50421 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3577 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10515 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    17784 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8148 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12832 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1969 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/log.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    30453 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    23540 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      455 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/py35compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      212 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4691 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    21349 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12483 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14696 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    20985 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/util.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    12514 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/version.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5133 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2392 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_imp.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.068338 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.072338 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       82 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   117968 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16256 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15130 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.072338 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      736 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      562 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1128 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2022 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1812 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_typing.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9509 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4917 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    31944 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    24067 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1811 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15470 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)   232056 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7077 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/archive_util.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    10280 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/build_meta.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.096339 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      217 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2381 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/alias.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    16604 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      900 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4415 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/build_clib.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    13027 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/build_ext.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8930 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/build_py.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8045 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/develop.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      960 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/dist_info.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    85308 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/easy_install.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    25335 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/egg_info.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4705 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/install.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2203 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3875 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/install_lib.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2593 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4946 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/py36compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      468 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/register.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2128 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/rotate.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      658 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/saveopts.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5967 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/sdist.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5051 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/setopt.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9490 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/test.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      462 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/upload.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7218 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    22279 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/config.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      949 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/dep_util.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5474 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/depends.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    42374 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/dist.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      524 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/errors.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1684 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/extension.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.096339 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/extern/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2407 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/extern/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4873 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/glob.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3567 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/installer.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      812 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/launch.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2335 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/lib2to3_ex.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     5217 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/monkey.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    50561 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/msvc.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3093 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/namespaces.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    40173 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/package_index.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      245 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/py34compat.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    14151 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/sandbox.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8565 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/ssl_support.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      941 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/unicode_utils.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      144 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/version.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     8288 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/wheel.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      714 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/windows_support.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:15:59.976337 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      239 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/dependency_links.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2869 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/entry_points.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       41 2022-12-20 18:31:24.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/top_level.txt
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.096339 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)       23 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      417 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/__main__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    19075 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/bdist_wheel.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.100339 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     2572 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     9498 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/convert.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     3208 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/pack.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      673 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/unpack.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    15931 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/macosx_libfile.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     4344 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/metadata.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1257 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/pkginfo.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      938 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/util.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.100339 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/vendored/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/vendored/__init__.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.100339 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/vendored/packaging/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        0 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/vendored/packaging/__init__.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1812 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_typing.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)    28937 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     7336 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/wheelfile.py
+drwxrwxr-x   0 jlonghurst  (1000) jlonghurst  (1000)        0 2023-04-30 14:16:00.096339 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)     1125 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/LICENSE.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)      108 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/entry_points.txt
+-rw-rw-r--   0 jlonghurst  (1000) jlonghurst  (1000)        6 2022-12-20 18:31:23.000000 RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/top_level.txt
```

### Comparing `RenderWatcher-0.0.2/LICENSE` & `RenderWatcher-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/RenderWatcher.egg-info/SOURCES.txt` & `RenderWatcher-0.0.4/RenderWatcher.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 RenderWatcher.egg-info/dependency_links.txt
 RenderWatcher.egg-info/top_level.txt
 render_watcher/__init__.py
 render_watcher/core.py
 render_watcher/ui.py
 venv/bin/activate_this.py
 venv/lib/python3.10/site-packages/_virtualenv.py
+venv/lib/python3.10/site-packages/RenderWatcher-0.0.3.dist-info/top_level.txt
 venv/lib/python3.10/site-packages/_distutils_hack/__init__.py
 venv/lib/python3.10/site-packages/_distutils_hack/override.py
 venv/lib/python3.10/site-packages/pip/__init__.py
 venv/lib/python3.10/site-packages/pip/__main__.py
 venv/lib/python3.10/site-packages/pip/__pip-runner__.py
 venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt
 venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/entry_points.txt
@@ -517,14 +518,17 @@
 venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
 venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
 venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
 venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
 venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
 venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
 venv/lib/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+venv/lib/python3.10/site-packages/render_watcher/__init__.py
+venv/lib/python3.10/site-packages/render_watcher/core.py
+venv/lib/python3.10/site-packages/render_watcher/ui.py
 venv/lib/python3.10/site-packages/setuptools/__init__.py
 venv/lib/python3.10/site-packages/setuptools/_deprecation_warning.py
 venv/lib/python3.10/site-packages/setuptools/_imp.py
 venv/lib/python3.10/site-packages/setuptools/archive_util.py
 venv/lib/python3.10/site-packages/setuptools/build_meta.py
 venv/lib/python3.10/site-packages/setuptools/config.py
 venv/lib/python3.10/site-packages/setuptools/dep_util.py
```

### Comparing `RenderWatcher-0.0.2/render_watcher/core.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/render_watcher/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 from katana_render_submitter import util
 
 
 PACKAGE_DIR = '/tlg/shows/{}/tmp'.format(util.get_shot_context())
 
 
-#TODO, want to inspect the job, create a dictionary of this, max the threads at 4?
-#e.g {job:{thread1:pass1, thread2:pass2, thread3:pass3, thread4:pass4}}
 
 def get_render_jobs():
     jobs = [j for j in os.listdir(PACKAGE_DIR) if j.endswith('.json')]
     if jobs:
         return jobs
     else:
         return None
```

### Comparing `RenderWatcher-0.0.2/render_watcher/ui.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/render_watcher/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,16 @@
                 progress_widget = self.tree.itemWidget(item, 4)
                 progress_widget.setValue(frame_number + 1)
                 break
             iterator += 1
 
     def populate_render_job_widget(self):
         jobs = core.get_render_jobs()
-        self.render_job_window.addItems(jobs)
+        if jobs:
+            self.render_job_window.addItems(jobs)
 
 
 
 def launch_render_watcher(arg):
     # running from terminal
     app = QtWidgets.QApplication(arg)
     render_watcher = RenderWatcher()
```

### Comparing `RenderWatcher-0.0.2/venv/bin/activate_this.py` & `RenderWatcher-0.0.4/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/_distutils_hack/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/_virtualenv.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/__main__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/__pip-runner__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/build_env.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cache.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/main.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/check.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/download.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/help.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/index.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/install.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/list.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/search.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/show.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/configuration.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/exceptions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/collector.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/index/sources.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/locations/base.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/index.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/link.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/auth.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/cache.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/download.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/session.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/utils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/check.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/pyproject.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/models.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/build.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/check.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/six.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_typing.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/config.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/core.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/log.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/version.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_imp.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_typing.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/archive_util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/build_meta.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/alias.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_clib.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_ext.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/build_py.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/develop.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/dist_info.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/easy_install.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/egg_info.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_lib.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/py36compat.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/rotate.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/saveopts.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/sdist.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/setopt.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/test.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/config.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/config.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/dep_util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/depends.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/dist.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/errors.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/extension.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/extern/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/glob.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/installer.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/launch.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/lib2to3_ex.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/lib2to3_ex.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/monkey.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/msvc.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/namespaces.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/package_index.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/sandbox.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/ssl_support.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/ssl_support.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/unicode_utils.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools/windows_support.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/entry_points.txt` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/setuptools-57.0.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/bdist_wheel.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/__init__.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/convert.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/pack.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/cli/unpack.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/macosx_libfile.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/metadata.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/pkginfo.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/util.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_typing.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/vendored/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel/wheelfile.py` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `RenderWatcher-0.0.2/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/LICENSE.txt` & `RenderWatcher-0.0.4/venv/lib/python3.10/site-packages/wheel-0.36.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

