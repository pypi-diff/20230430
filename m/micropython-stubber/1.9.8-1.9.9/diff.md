# Comparing `tmp/micropython-stubber-1.9.8.tar.gz` & `tmp/micropython-stubber-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-stubber-1.9.8.tar", max compression
+gzip compressed data, was "micropython-stubber-1.9.9.tar", max compression
```

## Comparing `micropython-stubber-1.9.8.tar` & `micropython-stubber-1.9.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1542 2021-06-29 07:00:41.068055 micropython-stubber-1.9.8/LICENSE
--rw-r--r--   0        0        0     5814 2022-10-03 19:21:15.128716 micropython-stubber-1.9.8/pyproject.toml
--rw-r--r--   0        0        0    14847 2022-08-09 09:32:51.712855 micropython-stubber-1.9.8/readme.md
--rw-r--r--   0        0        0       98 2022-09-26 10:18:32.235851 micropython-stubber-1.9.8/src/stubber/__init__.py
--rw-r--r--   0        0        0     7836 2022-10-03 19:18:31.715261 micropython-stubber-1.9.8/src/stubber/basicgit.py
--rw-r--r--   0        0        0        0 2022-08-09 09:32:51.722844 micropython-stubber-1.9.8/src/stubber/codemod/__init__.py
--rw-r--r--   0        0        0     2019 2022-09-26 10:18:32.238387 micropython-stubber-1.9.8/src/stubber/codemod/add_comment.py
--rw-r--r--   0        0        0     4075 2022-09-16 15:47:17.777922 micropython-stubber-1.9.8/src/stubber/codemod/enrich.py
--rw-r--r--   0        0        0     7630 2022-09-26 10:18:32.241385 micropython-stubber-1.9.8/src/stubber/codemod/merge_docstub.py
--rw-r--r--   0        0        0        0 2022-09-16 15:47:17.788923 micropython-stubber-1.9.8/src/stubber/commands/__init__.py
--rw-r--r--   0        0        0     1334 2022-09-16 15:47:17.790921 micropython-stubber-1.9.8/src/stubber/commands/cli.py
--rw-r--r--   0        0        0     2579 2022-09-26 10:18:32.243384 micropython-stubber-1.9.8/src/stubber/commands/clone_cmd.py
--rw-r--r--   0        0        0     1076 2022-09-27 07:44:53.367027 micropython-stubber-1.9.8/src/stubber/commands/config_cmd.py
--rw-r--r--   0        0        0     1512 2022-09-26 10:18:32.247383 micropython-stubber-1.9.8/src/stubber/commands/enrich_folder_cmd.py
--rw-r--r--   0        0        0     2052 2022-09-16 15:47:17.797922 micropython-stubber-1.9.8/src/stubber/commands/get_core_cmd.py
--rw-r--r--   0        0        0     2666 2022-09-26 10:18:32.250383 micropython-stubber-1.9.8/src/stubber/commands/get_docstubs_cmd.py
--rw-r--r--   0        0        0     2462 2022-09-26 10:18:32.254386 micropython-stubber-1.9.8/src/stubber/commands/get_frozen_cmd.py
--rw-r--r--   0        0        0     1440 2022-09-26 10:18:32.256385 micropython-stubber-1.9.8/src/stubber/commands/get_lobo_cmd.py
--rw-r--r--   0        0        0     1038 2022-09-26 10:18:32.259382 micropython-stubber-1.9.8/src/stubber/commands/merge_cmd.py
--rw-r--r--   0        0        0     2067 2022-09-27 07:40:47.561485 micropython-stubber-1.9.8/src/stubber/commands/minify_cmd.py
--rw-r--r--   0        0        0     3229 2022-09-26 10:18:32.261383 micropython-stubber-1.9.8/src/stubber/commands/publish_cmd.py
--rw-r--r--   0        0        0      957 2022-09-16 15:47:17.813920 micropython-stubber-1.9.8/src/stubber/commands/stub_cmd.py
--rw-r--r--   0        0        0     3139 2022-09-27 09:36:41.326494 micropython-stubber-1.9.8/src/stubber/commands/switch_cmd.py
--rw-r--r--   0        0        0     1054 2022-09-16 15:47:17.817931 micropython-stubber-1.9.8/src/stubber/commands/upd_fallback_cmd.py
--rw-r--r--   0        0        0     5930 2022-09-26 10:18:32.265381 micropython-stubber-1.9.8/src/stubber/cst_transformer.py
--rw-r--r--   0        0        0     1909 2022-09-16 15:47:17.819920 micropython-stubber-1.9.8/src/stubber/data/micropython_tags.csv
--rw-r--r--   0        0        0     1270 2022-08-08 21:23:09.496109 micropython-stubber-1.9.8/src/stubber/data/requirements-core-micropython.txt
--rw-r--r--   0        0        0     1003 2022-08-08 21:23:09.497699 micropython-stubber-1.9.8/src/stubber/data/requirements-core-pycopy.txt
--rw-r--r--   0        0        0     1202 2022-09-16 15:47:17.822919 micropython-stubber-1.9.8/src/stubber/downloader.py
--rw-r--r--   0        0        0        0 2022-09-26 10:18:32.267387 micropython-stubber-1.9.8/src/stubber/freeze/__init__.py
--rw-r--r--   0        0        0     2557 2022-09-26 10:18:32.270386 micropython-stubber-1.9.8/src/stubber/freeze/common.py
--rw-r--r--   0        0        0     2359 2022-09-26 10:18:32.271386 micropython-stubber-1.9.8/src/stubber/freeze/freeze_folder.py
--rw-r--r--   0        0        0     2941 2022-09-26 10:18:32.273384 micropython-stubber-1.9.8/src/stubber/freeze/freeze_manifest_1.py
--rw-r--r--   0        0        0     3973 2022-09-26 10:18:32.275385 micropython-stubber-1.9.8/src/stubber/freeze/freeze_manifest_2.py
--rw-r--r--   0        0        0     5197 2022-09-26 10:18:32.277385 micropython-stubber-1.9.8/src/stubber/freeze/get_frozen.py
--rw-r--r--   0        0        0     6925 2022-09-26 10:18:32.278382 micropython-stubber-1.9.8/src/stubber/freeze/makemanifest_1.py
--rw-r--r--   0        0        0     3687 2022-09-26 10:18:32.281383 micropython-stubber-1.9.8/src/stubber/get_cpython.py
--rw-r--r--   0        0        0     1769 2022-09-26 10:18:32.283382 micropython-stubber-1.9.8/src/stubber/get_lobo.py
--rw-r--r--   0        0        0     9021 2022-09-26 10:18:32.285385 micropython-stubber-1.9.8/src/stubber/minify.py
--rw-r--r--   0        0        0        0 2022-09-16 15:47:17.851448 micropython-stubber-1.9.8/src/stubber/publish/__init__.py
--rw-r--r--   0        0        0     1440 2022-09-16 15:47:17.853448 micropython-stubber-1.9.8/src/stubber/publish/bump.py
--rw-r--r--   0        0        0     7715 2022-09-16 15:47:17.855448 micropython-stubber-1.9.8/src/stubber/publish/candidates.py
--rw-r--r--   0        0        0      579 2022-09-16 15:47:17.856446 micropython-stubber-1.9.8/src/stubber/publish/database.py
--rw-r--r--   0        0        0     1059 2022-09-16 15:47:17.858449 micropython-stubber-1.9.8/src/stubber/publish/enums.py
--rw-r--r--   0        0        0     3135 2022-09-16 15:47:17.860451 micropython-stubber-1.9.8/src/stubber/publish/merge_docstubs.py
--rw-r--r--   0        0        0     4175 2022-09-16 15:47:17.862450 micropython-stubber-1.9.8/src/stubber/publish/package.py
--rw-r--r--   0        0        0     8738 2022-09-26 10:18:32.289385 micropython-stubber-1.9.8/src/stubber/publish/publish.py
--rw-r--r--   0        0        0      919 2022-09-16 15:47:17.866448 micropython-stubber-1.9.8/src/stubber/publish/pypi.py
--rw-r--r--   0        0        0    21964 2022-09-26 10:18:32.291386 micropython-stubber-1.9.8/src/stubber/publish/stubpacker.py
--rw-r--r--   0        0        0      232 2022-08-08 21:23:09.506031 micropython-stubber-1.9.8/src/stubber/rst/__init__.py
--rw-r--r--   0        0        0     2649 2022-09-16 15:47:17.871448 micropython-stubber-1.9.8/src/stubber/rst/classsort.py
--rw-r--r--   0        0        0     8879 2022-08-12 19:41:26.665183 micropython-stubber-1.9.8/src/stubber/rst/lookup.py
--rw-r--r--   0        0        0    11506 2022-09-26 10:18:32.293385 micropython-stubber-1.9.8/src/stubber/rst/output_dict.py
--rw-r--r--   0        0        0     2825 2022-09-26 10:18:32.296386 micropython-stubber-1.9.8/src/stubber/rst/report_return.py
--rw-r--r--   0        0        0    17835 2022-09-26 10:18:32.298384 micropython-stubber-1.9.8/src/stubber/rst/rst_utils.py
--rw-r--r--   0        0        0     1869 2022-09-16 15:47:17.880448 micropython-stubber-1.9.8/src/stubber/stubber.py
--rw-r--r--   0        0        0    32807 2022-09-26 10:18:32.301384 micropython-stubber-1.9.8/src/stubber/stubs_from_docs.py
--rw-r--r--   0        0        0        0 2022-09-26 10:18:32.302385 micropython-stubber-1.9.8/src/stubber/tools/__init__.py
--rw-r--r--   0        0        0    19575 2022-09-26 10:18:32.305386 micropython-stubber-1.9.8/src/stubber/tools/manifestfile.py
--rw-r--r--   0        0        0    26785 2022-08-08 21:23:09.516163 micropython-stubber-1.9.8/src/stubber/tools/pyboard.py
--rw-r--r--   0        0        0     4555 2022-09-26 10:18:32.307393 micropython-stubber-1.9.8/src/stubber/update_fallback.py
--rw-r--r--   0        0        0     4822 2022-09-16 15:47:17.888450 micropython-stubber-1.9.8/src/stubber/update_module_list.py
--rw-r--r--   0        0        0      237 2022-09-26 10:18:32.309385 micropython-stubber-1.9.8/src/stubber/utils/__init__.py
--rw-r--r--   0        0        0     3194 2022-09-27 07:45:08.279974 micropython-stubber-1.9.8/src/stubber/utils/config.py
--rw-r--r--   0        0        0     2721 2022-09-16 15:47:17.892446 micropython-stubber-1.9.8/src/stubber/utils/makeversionhdr.py
--rw-r--r--   0        0        0     3225 2022-09-26 10:18:32.311385 micropython-stubber-1.9.8/src/stubber/utils/manifest.py
--rw-r--r--   0        0        0      393 2022-09-16 15:47:17.898447 micropython-stubber-1.9.8/src/stubber/utils/my_version.py
--rw-r--r--   0        0        0     1384 2022-09-16 15:47:17.904448 micropython-stubber-1.9.8/src/stubber/utils/post.py
--rw-r--r--   0        0        0     2774 2022-09-26 10:18:32.314382 micropython-stubber-1.9.8/src/stubber/utils/repos.py
--rw-r--r--   0        0        0     3907 2022-09-26 10:18:32.316385 micropython-stubber-1.9.8/src/stubber/utils/stubmaker.py
--rw-r--r--   0        0        0     2723 2022-09-26 10:18:32.318388 micropython-stubber-1.9.8/src/stubber/utils/typed_config_toml.py
--rw-r--r--   0        0        0     1753 2022-09-26 10:18:32.321383 micropython-stubber-1.9.8/src/stubber/utils/versions.py
--rw-r--r--   0        0        0    16515 2022-10-03 19:21:36.029266 micropython-stubber-1.9.8/setup.py
--rw-r--r--   0        0        0    16588 2022-10-03 19:21:36.029266 micropython-stubber-1.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1542 2021-06-29 07:00:41.068055 micropython-stubber-1.9.9/LICENSE
+-rw-r--r--   0        0        0     5814 2022-10-03 20:10:45.588910 micropython-stubber-1.9.9/pyproject.toml
+-rw-r--r--   0        0        0    14847 2022-08-09 09:32:51.712855 micropython-stubber-1.9.9/readme.md
+-rw-r--r--   0        0        0       98 2022-09-26 10:18:32.235851 micropython-stubber-1.9.9/src/stubber/__init__.py
+-rw-r--r--   0        0        0     7854 2022-10-03 20:10:09.154942 micropython-stubber-1.9.9/src/stubber/basicgit.py
+-rw-r--r--   0        0        0        0 2022-08-09 09:32:51.722844 micropython-stubber-1.9.9/src/stubber/codemod/__init__.py
+-rw-r--r--   0        0        0     2019 2022-09-26 10:18:32.238387 micropython-stubber-1.9.9/src/stubber/codemod/add_comment.py
+-rw-r--r--   0        0        0     4075 2022-09-16 15:47:17.777922 micropython-stubber-1.9.9/src/stubber/codemod/enrich.py
+-rw-r--r--   0        0        0     7630 2022-09-26 10:18:32.241385 micropython-stubber-1.9.9/src/stubber/codemod/merge_docstub.py
+-rw-r--r--   0        0        0        0 2022-09-16 15:47:17.788923 micropython-stubber-1.9.9/src/stubber/commands/__init__.py
+-rw-r--r--   0        0        0     1334 2022-09-16 15:47:17.790921 micropython-stubber-1.9.9/src/stubber/commands/cli.py
+-rw-r--r--   0        0        0     2579 2022-09-26 10:18:32.243384 micropython-stubber-1.9.9/src/stubber/commands/clone_cmd.py
+-rw-r--r--   0        0        0     1076 2022-09-27 07:44:53.367027 micropython-stubber-1.9.9/src/stubber/commands/config_cmd.py
+-rw-r--r--   0        0        0     1512 2022-09-26 10:18:32.247383 micropython-stubber-1.9.9/src/stubber/commands/enrich_folder_cmd.py
+-rw-r--r--   0        0        0     2052 2022-09-16 15:47:17.797922 micropython-stubber-1.9.9/src/stubber/commands/get_core_cmd.py
+-rw-r--r--   0        0        0     2666 2022-09-26 10:18:32.250383 micropython-stubber-1.9.9/src/stubber/commands/get_docstubs_cmd.py
+-rw-r--r--   0        0        0     2462 2022-09-26 10:18:32.254386 micropython-stubber-1.9.9/src/stubber/commands/get_frozen_cmd.py
+-rw-r--r--   0        0        0     1440 2022-09-26 10:18:32.256385 micropython-stubber-1.9.9/src/stubber/commands/get_lobo_cmd.py
+-rw-r--r--   0        0        0     1038 2022-09-26 10:18:32.259382 micropython-stubber-1.9.9/src/stubber/commands/merge_cmd.py
+-rw-r--r--   0        0        0     2067 2022-09-27 07:40:47.561485 micropython-stubber-1.9.9/src/stubber/commands/minify_cmd.py
+-rw-r--r--   0        0        0     3229 2022-09-26 10:18:32.261383 micropython-stubber-1.9.9/src/stubber/commands/publish_cmd.py
+-rw-r--r--   0        0        0      957 2022-09-16 15:47:17.813920 micropython-stubber-1.9.9/src/stubber/commands/stub_cmd.py
+-rw-r--r--   0        0        0     3139 2022-09-27 09:36:41.326494 micropython-stubber-1.9.9/src/stubber/commands/switch_cmd.py
+-rw-r--r--   0        0        0     1054 2022-09-16 15:47:17.817931 micropython-stubber-1.9.9/src/stubber/commands/upd_fallback_cmd.py
+-rw-r--r--   0        0        0     5930 2022-09-26 10:18:32.265381 micropython-stubber-1.9.9/src/stubber/cst_transformer.py
+-rw-r--r--   0        0        0     1909 2022-09-16 15:47:17.819920 micropython-stubber-1.9.9/src/stubber/data/micropython_tags.csv
+-rw-r--r--   0        0        0     1270 2022-08-08 21:23:09.496109 micropython-stubber-1.9.9/src/stubber/data/requirements-core-micropython.txt
+-rw-r--r--   0        0        0     1003 2022-08-08 21:23:09.497699 micropython-stubber-1.9.9/src/stubber/data/requirements-core-pycopy.txt
+-rw-r--r--   0        0        0     1202 2022-09-16 15:47:17.822919 micropython-stubber-1.9.9/src/stubber/downloader.py
+-rw-r--r--   0        0        0        0 2022-09-26 10:18:32.267387 micropython-stubber-1.9.9/src/stubber/freeze/__init__.py
+-rw-r--r--   0        0        0     2557 2022-09-26 10:18:32.270386 micropython-stubber-1.9.9/src/stubber/freeze/common.py
+-rw-r--r--   0        0        0     2359 2022-09-26 10:18:32.271386 micropython-stubber-1.9.9/src/stubber/freeze/freeze_folder.py
+-rw-r--r--   0        0        0     2941 2022-09-26 10:18:32.273384 micropython-stubber-1.9.9/src/stubber/freeze/freeze_manifest_1.py
+-rw-r--r--   0        0        0     3973 2022-09-26 10:18:32.275385 micropython-stubber-1.9.9/src/stubber/freeze/freeze_manifest_2.py
+-rw-r--r--   0        0        0     5197 2022-09-26 10:18:32.277385 micropython-stubber-1.9.9/src/stubber/freeze/get_frozen.py
+-rw-r--r--   0        0        0     6925 2022-09-26 10:18:32.278382 micropython-stubber-1.9.9/src/stubber/freeze/makemanifest_1.py
+-rw-r--r--   0        0        0     3687 2022-09-26 10:18:32.281383 micropython-stubber-1.9.9/src/stubber/get_cpython.py
+-rw-r--r--   0        0        0     1769 2022-09-26 10:18:32.283382 micropython-stubber-1.9.9/src/stubber/get_lobo.py
+-rw-r--r--   0        0        0     9021 2022-09-26 10:18:32.285385 micropython-stubber-1.9.9/src/stubber/minify.py
+-rw-r--r--   0        0        0        0 2022-09-16 15:47:17.851448 micropython-stubber-1.9.9/src/stubber/publish/__init__.py
+-rw-r--r--   0        0        0     1440 2022-09-16 15:47:17.853448 micropython-stubber-1.9.9/src/stubber/publish/bump.py
+-rw-r--r--   0        0        0     7715 2022-09-16 15:47:17.855448 micropython-stubber-1.9.9/src/stubber/publish/candidates.py
+-rw-r--r--   0        0        0      579 2022-09-16 15:47:17.856446 micropython-stubber-1.9.9/src/stubber/publish/database.py
+-rw-r--r--   0        0        0     1059 2022-09-16 15:47:17.858449 micropython-stubber-1.9.9/src/stubber/publish/enums.py
+-rw-r--r--   0        0        0     3135 2022-09-16 15:47:17.860451 micropython-stubber-1.9.9/src/stubber/publish/merge_docstubs.py
+-rw-r--r--   0        0        0     4175 2022-09-16 15:47:17.862450 micropython-stubber-1.9.9/src/stubber/publish/package.py
+-rw-r--r--   0        0        0     8738 2022-09-26 10:18:32.289385 micropython-stubber-1.9.9/src/stubber/publish/publish.py
+-rw-r--r--   0        0        0      919 2022-09-16 15:47:17.866448 micropython-stubber-1.9.9/src/stubber/publish/pypi.py
+-rw-r--r--   0        0        0    21964 2022-09-26 10:18:32.291386 micropython-stubber-1.9.9/src/stubber/publish/stubpacker.py
+-rw-r--r--   0        0        0      232 2022-08-08 21:23:09.506031 micropython-stubber-1.9.9/src/stubber/rst/__init__.py
+-rw-r--r--   0        0        0     2649 2022-09-16 15:47:17.871448 micropython-stubber-1.9.9/src/stubber/rst/classsort.py
+-rw-r--r--   0        0        0     8879 2022-08-12 19:41:26.665183 micropython-stubber-1.9.9/src/stubber/rst/lookup.py
+-rw-r--r--   0        0        0    11506 2022-09-26 10:18:32.293385 micropython-stubber-1.9.9/src/stubber/rst/output_dict.py
+-rw-r--r--   0        0        0     2825 2022-09-26 10:18:32.296386 micropython-stubber-1.9.9/src/stubber/rst/report_return.py
+-rw-r--r--   0        0        0    17835 2022-09-26 10:18:32.298384 micropython-stubber-1.9.9/src/stubber/rst/rst_utils.py
+-rw-r--r--   0        0        0     1869 2022-09-16 15:47:17.880448 micropython-stubber-1.9.9/src/stubber/stubber.py
+-rw-r--r--   0        0        0    32807 2022-09-26 10:18:32.301384 micropython-stubber-1.9.9/src/stubber/stubs_from_docs.py
+-rw-r--r--   0        0        0        0 2022-09-26 10:18:32.302385 micropython-stubber-1.9.9/src/stubber/tools/__init__.py
+-rw-r--r--   0        0        0    19575 2022-09-26 10:18:32.305386 micropython-stubber-1.9.9/src/stubber/tools/manifestfile.py
+-rw-r--r--   0        0        0    26785 2022-08-08 21:23:09.516163 micropython-stubber-1.9.9/src/stubber/tools/pyboard.py
+-rw-r--r--   0        0        0     4555 2022-09-26 10:18:32.307393 micropython-stubber-1.9.9/src/stubber/update_fallback.py
+-rw-r--r--   0        0        0     4822 2022-09-16 15:47:17.888450 micropython-stubber-1.9.9/src/stubber/update_module_list.py
+-rw-r--r--   0        0        0      237 2022-09-26 10:18:32.309385 micropython-stubber-1.9.9/src/stubber/utils/__init__.py
+-rw-r--r--   0        0        0     3194 2022-09-27 07:45:08.279974 micropython-stubber-1.9.9/src/stubber/utils/config.py
+-rw-r--r--   0        0        0     2721 2022-09-16 15:47:17.892446 micropython-stubber-1.9.9/src/stubber/utils/makeversionhdr.py
+-rw-r--r--   0        0        0     3225 2022-09-26 10:18:32.311385 micropython-stubber-1.9.9/src/stubber/utils/manifest.py
+-rw-r--r--   0        0        0      393 2022-09-16 15:47:17.898447 micropython-stubber-1.9.9/src/stubber/utils/my_version.py
+-rw-r--r--   0        0        0     1384 2022-09-16 15:47:17.904448 micropython-stubber-1.9.9/src/stubber/utils/post.py
+-rw-r--r--   0        0        0     2774 2022-09-26 10:18:32.314382 micropython-stubber-1.9.9/src/stubber/utils/repos.py
+-rw-r--r--   0        0        0     3907 2022-09-26 10:18:32.316385 micropython-stubber-1.9.9/src/stubber/utils/stubmaker.py
+-rw-r--r--   0        0        0     2723 2022-09-26 10:18:32.318388 micropython-stubber-1.9.9/src/stubber/utils/typed_config_toml.py
+-rw-r--r--   0        0        0     1753 2022-09-26 10:18:32.321383 micropython-stubber-1.9.9/src/stubber/utils/versions.py
+-rw-r--r--   0        0        0    16515 2022-10-03 20:11:22.855571 micropython-stubber-1.9.9/setup.py
+-rw-r--r--   0        0        0    16588 2022-10-03 20:11:22.855571 micropython-stubber-1.9.9/PKG-INFO
```

### Comparing `micropython-stubber-1.9.8/LICENSE` & `micropython-stubber-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/pyproject.toml` & `micropython-stubber-1.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # publish-path = "./repos/micropython-stubs/publish"
 # template-path = "./repos/micropython-stubs/publish/template"
 
 
 [tool.poetry]
 name = "micropython-stubber"
-version = "1.9.8"
+version = "1.9.9"
 description = "Tooling to create and maintain stubs for MicroPython"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "readme.md"
 keywords = ["Micropython", "stubs", "vscode", "static type check"]
 documentation = "https://micropython-stubber.readthedocs.io/"
 homepage = "https://github.com/Josverl/micropython-stubber#readme"
```

### Comparing `micropython-stubber-1.9.8/readme.md` & `micropython-stubber-1.9.9/readme.md`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/basicgit.py` & `micropython-stubber-1.9.9/src/stubber/basicgit.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             result = subprocess.run(cmd, capture_output=capture_output, check=True)
     except (NotADirectoryError, FileNotFoundError) as e:  # pragma: no cover
         return None
     except subprocess.CalledProcessError as e:  # pragma: no cover
         # add some logging for github actions
         log.error("Exception on process, rc=", e.returncode, "output=", e.output.decode("utf-8"), "\nstderr=", e.stderr.decode("utf-8"))
         return None
-    if result.stderr != b"":
+    if result.stderr and result.stderr != b"":
         stderr = result.stderr.decode("utf-8")
         if "warning" in stderr.lower():
             log.warning(stderr)
             expect_stderr = True
         elif capture_output and echo_output:  # pragma: no cover
             log.error(stderr)
         if not expect_stderr:
```

### Comparing `micropython-stubber-1.9.8/src/stubber/codemod/add_comment.py` & `micropython-stubber-1.9.9/src/stubber/codemod/add_comment.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/codemod/enrich.py` & `micropython-stubber-1.9.9/src/stubber/codemod/enrich.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/codemod/merge_docstub.py` & `micropython-stubber-1.9.9/src/stubber/codemod/merge_docstub.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/cli.py` & `micropython-stubber-1.9.9/src/stubber/commands/cli.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/clone_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/clone_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/config_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/config_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/enrich_folder_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/enrich_folder_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/get_core_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/get_core_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/get_docstubs_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/get_docstubs_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/get_frozen_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/get_frozen_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/get_lobo_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/get_lobo_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/merge_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/merge_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/minify_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/minify_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/publish_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/publish_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/stub_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/stub_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/switch_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/switch_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/commands/upd_fallback_cmd.py` & `micropython-stubber-1.9.9/src/stubber/commands/upd_fallback_cmd.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/cst_transformer.py` & `micropython-stubber-1.9.9/src/stubber/cst_transformer.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/data/micropython_tags.csv` & `micropython-stubber-1.9.9/src/stubber/data/micropython_tags.csv`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/data/requirements-core-micropython.txt` & `micropython-stubber-1.9.9/src/stubber/data/requirements-core-micropython.txt`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/data/requirements-core-pycopy.txt` & `micropython-stubber-1.9.9/src/stubber/data/requirements-core-pycopy.txt`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/downloader.py` & `micropython-stubber-1.9.9/src/stubber/downloader.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/freeze/common.py` & `micropython-stubber-1.9.9/src/stubber/freeze/common.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/freeze/freeze_folder.py` & `micropython-stubber-1.9.9/src/stubber/freeze/freeze_folder.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/freeze/freeze_manifest_1.py` & `micropython-stubber-1.9.9/src/stubber/freeze/freeze_manifest_1.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/freeze/freeze_manifest_2.py` & `micropython-stubber-1.9.9/src/stubber/freeze/freeze_manifest_2.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/freeze/get_frozen.py` & `micropython-stubber-1.9.9/src/stubber/freeze/get_frozen.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/freeze/makemanifest_1.py` & `micropython-stubber-1.9.9/src/stubber/freeze/makemanifest_1.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/get_cpython.py` & `micropython-stubber-1.9.9/src/stubber/get_cpython.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/get_lobo.py` & `micropython-stubber-1.9.9/src/stubber/get_lobo.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/minify.py` & `micropython-stubber-1.9.9/src/stubber/minify.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/bump.py` & `micropython-stubber-1.9.9/src/stubber/publish/bump.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/candidates.py` & `micropython-stubber-1.9.9/src/stubber/publish/candidates.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/database.py` & `micropython-stubber-1.9.9/src/stubber/publish/database.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/enums.py` & `micropython-stubber-1.9.9/src/stubber/publish/enums.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/merge_docstubs.py` & `micropython-stubber-1.9.9/src/stubber/publish/merge_docstubs.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/package.py` & `micropython-stubber-1.9.9/src/stubber/publish/package.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/publish.py` & `micropython-stubber-1.9.9/src/stubber/publish/publish.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/pypi.py` & `micropython-stubber-1.9.9/src/stubber/publish/pypi.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/publish/stubpacker.py` & `micropython-stubber-1.9.9/src/stubber/publish/stubpacker.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/rst/classsort.py` & `micropython-stubber-1.9.9/src/stubber/rst/classsort.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/rst/lookup.py` & `micropython-stubber-1.9.9/src/stubber/rst/lookup.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/rst/output_dict.py` & `micropython-stubber-1.9.9/src/stubber/rst/output_dict.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/rst/report_return.py` & `micropython-stubber-1.9.9/src/stubber/rst/report_return.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/rst/rst_utils.py` & `micropython-stubber-1.9.9/src/stubber/rst/rst_utils.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/stubber.py` & `micropython-stubber-1.9.9/src/stubber/stubber.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/stubs_from_docs.py` & `micropython-stubber-1.9.9/src/stubber/stubs_from_docs.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/tools/manifestfile.py` & `micropython-stubber-1.9.9/src/stubber/tools/manifestfile.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/tools/pyboard.py` & `micropython-stubber-1.9.9/src/stubber/tools/pyboard.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/update_fallback.py` & `micropython-stubber-1.9.9/src/stubber/update_fallback.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/update_module_list.py` & `micropython-stubber-1.9.9/src/stubber/update_module_list.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/utils/config.py` & `micropython-stubber-1.9.9/src/stubber/utils/config.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/utils/makeversionhdr.py` & `micropython-stubber-1.9.9/src/stubber/utils/makeversionhdr.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/utils/manifest.py` & `micropython-stubber-1.9.9/src/stubber/utils/manifest.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/utils/post.py` & `micropython-stubber-1.9.9/src/stubber/utils/post.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/utils/repos.py` & `micropython-stubber-1.9.9/src/stubber/utils/repos.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/utils/stubmaker.py` & `micropython-stubber-1.9.9/src/stubber/utils/stubmaker.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/utils/typed_config_toml.py` & `micropython-stubber-1.9.9/src/stubber/utils/typed_config_toml.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/src/stubber/utils/versions.py` & `micropython-stubber-1.9.9/src/stubber/utils/versions.py`

 * *Files identical despite different names*

### Comparing `micropython-stubber-1.9.8/setup.py` & `micropython-stubber-1.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 entry_points = \
 {'console_scripts': ['pyboard = stubber.tools.pyboard:main',
                      'stubber = stubber.stubber:stubber_cli']}
 
 setup_kwargs = {
     'name': 'micropython-stubber',
-    'version': '1.9.8',
+    'version': '1.9.9',
     'description': 'Tooling to create and maintain stubs for MicroPython',
     'long_description': '# Boost MicroPython productivity in VSCode\n \n  [![pypi version](https://badgen.net/pypi/v/micropython-stubber)](https://pypi.org/project/micropython-stubber/)\n  [![python versions](https://badgen.net/pypi/python/micropython-stubber)](https://badgen.net/pypi/python/micropython-stubber)\n  [![Documentation Status](https://readthedocs.org/projects/micropython-stubber/badge/?version=latest)](https://micropython-stubber.readthedocs.io/en/latest/?badge=latest "Document build status badge")\n  [![Star on GitHub](https://img.shields.io/github/stars/josverl/micropython-stubber.svg?style=social)](https://github.com/josverl/micropython-stubber/stargazers)\n  [![All Contributors](https://img.shields.io/badge/all_contributors-19-green.svg?style=flat-square)](#Contributions)\n  <!-- break -->\n  [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Josverl/micropython-stubber.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Josverl/micropython-stubber/context:python)\n  [![pytest tests/common](https://github.com/Josverl/micropython-stubber/actions/workflows/pytest.yml/badge.svg)](https://github.com/Josverl/micropython-stubber/actions/workflows/pytest.yml)\n  [![codecov](https://codecov.io/gh/Josverl/micropython-stubber/branch/main/graph/badge.svg?token=WJFGMKBHOV)](https://codecov.io/gh/Josverl/micropython-stubber)\n  [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black "Black badge")\n  <!-- break -->\n  [![Open in VSCode](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc\n)](https://open.vscode.dev/josverl/micropython-stubber)\n  \nThe intellisense and code linting that is so prevalent in modern editors, does not work out-of-the-gate for MicroPython projects.\nWhile the language is Python, the modules used are different from CPython , and also different ports have different modules and classes , or the same class with different parameters.\n\nWriting MicroPython code in a modern editor should not need to involve keeping a browser open to check for the exact parameters to read a sensor, light-up a led or send a network request.\n\nFortunately with some additional configuration and data, it is possible to make the editors understand your flavor of MicroPython, wether you use one of the pre-compiled firmwares, but also if you run a one-off custom firmware version.\n\n\n![demo][]]\n\nIn order to achieve this a few things are needed:\n1) Stub files for the native / enabled modules in the firmware using PEP 484 Type Hints\n2) Specific configuration of the VSCode Python extensions \n3) Specific configuration of Pylint [ Optional ]\n4) Suppression of warnings that collide with the MicroPython principals or code optimization.\n\nPlease review the documentation on [https://micropython-stubber.readthedocs.io]  \n\nWith that in place, VSCode will understand MicroPython for the most part, and help you to write code, and catch more errors before deploying it to your board. \n\nNote that the above is not limited to VSCode and pylint, but it happens to be the combination that I use. \n\nA lot of subs have already been generated and are shared on github or other means,  so it is quite likely that you can just grab a copy be be productive in a few minutes.\n\nFor now you will need to [configure this by hand](#manual-configuration), or use the [micropy cli` tool](#using-micropy-cli)\n\n1. The sister-repo [**MicroPython-stubs**][stubs-repo] contains [all stubs][all-stubs] I have collected with the help of others, and which can be used directly.\nThat repo also contains examples configuration files that can be easily adopted to your setup.\n\n2. A second repo [micropy-stubs repo][stubs-repo2] maintained by BradenM, also contains stubs, but in a structure only used and distributed by the [micropy-cli](#using-micropy-cli) tool.\nYou should use micropy-cli to consume stubs from that repo.\n\nThe (stretch) goal is to create a VSCode add-in to simplify the configuration, and allow easy switching between different firmwares and versions.\n\n\n## Install and basic usage\n\n``` sh\npip install micropython-stubber\n\n# go to your working folder \ncd my_stub_folder\nmkdir all-stubs\n\n# clone the micropython repo\'s and switch to a specific version \nstubber clone\nstubber switch --version v1.18\n\n# get the document stubs for the current version ( v1.18 )\nstubber get-docstubs\n\n# get the frozen stubs for the current version ( v1.18 )\nstubber get-frozen\n\n# get the core CPython compatibility stubs from PyPi \nstubber get-core\n\n# Update the fallback stubs\nstubber update-fallback\n\n#\nls all-stubs\ndir all-stubs\n```\n\n\n## Developing & testing \n\nThis is described in more detail in the [developing](docs/developing.md) and [testing](docs/testing.md)  documents in the docs folder.\n\n## Branch Main\nThe name of the default branch has been changed to `main`.\nIf you have cloned this repo before you main need to adjust the local repro to be aware of this, or create a fresh clone.\n\nTo update run the below command:  \n``` bash\ngit branch -m master main                    \ngit fetch origin\ngit branch -u origin/main main                      \ngit remote set-head origin -a\n```\n\nfor more info see [**Renaming a branch**](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-branches-in-your-repository/renaming-a-branch#updating-a-local-clone-after-a-branch-name-changes)\n\n## Licensing \n\nMicroPython-Stubber is licensed under the MIT license, and all contributions should follow this [LICENSE](LICENSE).\n\n\n# Contributions\n<!-- spell-checker: disable -->\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://github.com/Josverl"><img src="https://avatars2.githubusercontent.com/u/981654?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jos Verlinde</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/commits?author=josverl" title="Code">💻</a> <a href="#research-josverl" title="Research">🔬</a> <a href="#ideas-josverl" title="Ideas, Planning, & Feedback">🤔</a> <a href="#content-josverl" title="Content">🖋</a> <a href="#stubs-josverl" title="MicroPython stubs">📚</a> <a href="#test-josverl" title="Test">✔</a></td>\n    <td align="center"><a href="https://thonny.org/"><img src="https://avatars1.githubusercontent.com/u/46202078?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Thonny, Python IDE for beginners</b></sub></a><br /><a href="#ideas-thonny" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-thonny" title="Research">🔬</a></td>\n    <td align="center"><a href="https://micropython.org/"><img src="https://avatars1.githubusercontent.com/u/6298560?v=4?s=100" width="100px;" alt=""/><br /><sub><b>MicroPython</b></sub></a><br /><a href="#data-micropython" title="Data">🔣</a> <a href="#stubs-micropython" title="MicroPython stubs">📚</a></td>\n    <td align="center"><a href="https://github.com/loboris"><img src="https://avatars3.githubusercontent.com/u/6280349?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Boris Lovosevic</b></sub></a><br /><a href="#data-loboris" title="Data">🔣</a> <a href="#stubs-loboris" title="MicroPython stubs">📚</a></td>\n    <td align="center"><a href="https://github.com/pfalcon"><img src="https://avatars3.githubusercontent.com/u/500451?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Paul Sokolovsky</b></sub></a><br /><a href="#data-pfalcon" title="Data">🔣</a> <a href="#stubs-pfalcon" title="MicroPython stubs">📚</a></td>\n    <td align="center"><a href="https://github.com/pycopy"><img src="https://avatars0.githubusercontent.com/u/67273174?v=4?s=100" width="100px;" alt=""/><br /><sub><b>pycopy</b></sub></a><br /><a href="#data-pycopy" title="Data">🔣</a> <a href="#stubs-pycopy" title="MicroPython stubs">📚</a></td>\n    <td align="center"><a href="https://github.com/pycom"><img src="https://avatars2.githubusercontent.com/u/16415153?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pycom</b></sub></a><br /><a href="#infra-pycom" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>\n  </tr>\n  <tr>\n    <td align="center"><a href="https://github.com/BradenM"><img src="https://avatars1.githubusercontent.com/u/5913808?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Braden Mars</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3ABradenM" title="Bug reports">🐛</a> <a href="https://github.com/Josverl/micropython-stubber/commits?author=BradenM" title="Code">💻</a> <a href="#stubs-BradenM" title="MicroPython stubs">📚</a> <a href="#platform-BradenM" title="Packaging/porting to new platform">📦</a></td>\n    <td align="center"><a href="https://binary.com.au/"><img src="https://avatars2.githubusercontent.com/u/175909?v=4?s=100" width="100px;" alt=""/><br /><sub><b>James Manners</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/commits?author=jmannau" title="Code">💻</a> <a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3Ajmannau" title="Bug reports">🐛</a></td>\n    <td align="center"><a href="http://patrickwalters.us/"><img src="https://avatars0.githubusercontent.com/u/4002194?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Patrick</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3Aaskpatrickw" title="Bug reports">🐛</a> <a href="https://github.com/Josverl/micropython-stubber/commits?author=askpatrickw" title="Code">💻</a> <a href="#stubs-askpatrickw" title="MicroPython stubs">📚</a></td>\n    <td align="center"><a href="https://opencollective.com/pythonseverywhere"><img src="https://avatars3.githubusercontent.com/u/16009100?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Paul m. p. P.</b></sub></a><br /><a href="#ideas-pmp-p" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-pmp-p" title="Research">🔬</a></td>\n    <td align="center"><a href="https://github.com/edreamleo"><img src="https://avatars0.githubusercontent.com/u/592928?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Edward K. Ream</b></sub></a><br /><a href="#plugin-edreamleo" title="Plugin/utility libraries">🔌</a></td>\n    <td align="center"><a href="https://github.com/dastultz"><img src="https://avatars3.githubusercontent.com/u/4334042?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Daryl Stultz</b></sub></a><br /><a href="#stubs-dastultz" title="MicroPython stubs">📚</a></td>\n    <td align="center"><a href="https://github.com/cabletie"><img src="https://avatars1.githubusercontent.com/u/2356734?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Keeping things together</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3Acabletie" title="Bug reports">🐛</a></td>\n  </tr>\n  <tr>\n    <td align="center"><a href="https://github.com/vbolshakov"><img src="https://avatars2.githubusercontent.com/u/2453324?v=4?s=100" width="100px;" alt=""/><br /><sub><b>vbolshakov</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3Avbolshakov" title="Bug reports">🐛</a> <a href="#stubs-vbolshakov" title="MicroPython stubs">📚</a></td>\n    <td align="center"><a href="https://lemariva.com/"><img src="https://avatars2.githubusercontent.com/u/15173329?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mauro Riva</b></sub></a><br /><a href="#blog-lemariva" title="Blogposts">📝</a> <a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3Alemariva" title="Bug reports">🐛</a></td>\n    <td align="center"><a href="https://github.com/MathijsNL"><img src="https://avatars0.githubusercontent.com/u/1612886?v=4?s=100" width="100px;" alt=""/><br /><sub><b>MathijsNL</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3AMathijsNL" title="Bug reports">🐛</a></td>\n    <td align="center"><a href="http://comingsoon.tm/"><img src="https://avatars0.githubusercontent.com/u/13251689?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Callum Jacob Hays</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3ACallumJHays" title="Bug reports">🐛</a> <a href="#test-CallumJHays" title="Test">✔</a></td>\n    <td align="center"><a href="https://github.com/v923z"><img src="https://avatars0.githubusercontent.com/u/1310472?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Zoltán Vörös</b></sub></a><br /><a href="#data-v923z" title="Data">🔣</a></td>\n    <td align="center"><a href="https://github.com/vincent-l-j"><img src="https://avatars.githubusercontent.com/u/20021376?v=4?s=100" width="100px;" alt=""/><br /><sub><b>vincent-l-j</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/commits?author=vincent-l-j" title="Documentation">📖</a></td>\n    <td align="center"><a href="https://github.com/yegorLitvinov"><img src="https://avatars.githubusercontent.com/u/20367310?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Egor Litvinov</b></sub></a><br /><a href="https://github.com/Josverl/micropython-stubber/issues?q=author%3AyegorLitvinov" title="Bug reports">🐛</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n----------------------------\n\n--------------------------------\n\n\n\n[stubs-repo]:   https://github.com/Josverl/micropython-stubs\n[stubs-repo2]:  https://github.com/BradenM/micropy-stubs\n[micropython-stubber]: https://github.com/Josverl/micropython-stubber\n[micropython-stubs]: https://github.com/Josverl/micropython-stubs#micropython-stubs\n[micropy-cli]: https://github.com/BradenM/micropy-cli\n[using-the-stubs]: https://github.com/Josverl/micropython-stubs#using-the-stubs\n[demo]:         https://github.com/Josverl/micropython-stubber/blob/main/docs/img/demo.gif?raw=true\t"demo of writing code using the stubs"\n[stub processing order]: https://github.com/Josverl/micropython-stubber/blob/main/docs/img/stuborder_pylance.png?raw=true\t"recommended stub processing order"\n[naming-convention]: #naming-convention-and-stub-folder-structure\n[all-stubs]: https://github.com/Josverl/micropython-stubs/blob/main/firmwares.md\n[micropython]: https://github.com/micropython/micropython\n[micropython-lib]:  https://github.com/micropython/micropython-lib\n[pycopy]: https://github.com/pfalcon/pycopy\n[pycopy-lib]: https://github.com/pfalcon/pycopy-lib\n\n',
     'author': 'Jos Verlinde',
     'author_email': 'jos_verlinde@hotmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Josverl/micropython-stubber#readme',
```

### Comparing `micropython-stubber-1.9.8/PKG-INFO` & `micropython-stubber-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-stubber
-Version: 1.9.8
+Version: 1.9.9
 Summary: Tooling to create and maintain stubs for MicroPython
 Home-page: https://github.com/Josverl/micropython-stubber#readme
 License: MIT
 Keywords: Micropython,stubs,vscode,static type check
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8,<3.11
```

