# Comparing `tmp/pyspread-2.2.tar.gz` & `tmp/pyspread-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspread-2.2.tar", last modified: Sun Apr 16 18:40:47 2023, max compression
+gzip compressed data, was "pyspread-2.2.1.tar", last modified: Sun Apr 30 06:59:35 2023, max compression
```

## Comparing `pyspread-2.2.tar` & `pyspread-2.2.1.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.785955 pyspread-2.2/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-16 18:39:21.000000 pyspread-2.2/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    35141 2023-04-16 18:39:21.000000 pyspread-2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-16 18:39:21.000000 pyspread-2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5106 2023-04-16 18:40:47.785955 pyspread-2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2608 2023-04-16 18:39:21.000000 pyspread-2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-16 18:39:21.000000 pyspread-2.2/THANKS
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14668 2023-04-16 18:39:21.000000 pyspread-2.2/changelog
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.671944 pyspread-2.2/pyspread/
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    48145 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     3393 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    34733 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/commands.py
--rw-rw-rw-   0 root         (0) root         (0)    58195 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/dialogs.py
--rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/entryline.py
--rw-rw-rw-   0 root         (0) root         (0)    96463 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/grid.py
--rw-rw-rw-   0 root         (0) root         (0)    31006 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/grid_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     9372 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/icons.py
--rw-rw-rw-   0 root         (0) root         (0)    11094 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/installer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.673944 pyspread-2.2/pyspread/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19559 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/interfaces/pys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.678944 pyspread-2.2/pyspread/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1060 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/attrdict.py
--rw-rw-rw-   0 root         (0) root         (0)     9886 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/charts.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    45208 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/dataclasses.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/exception_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     4077 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/file_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/hashing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.679944 pyspread-2.2/pyspread/lib/packaging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/packaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/packaging/_structures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/packaging/_typing.py
--rw-rw-rw-   0 root         (0) root         (0)    15480 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/packaging/version.py
--rwxrwxrwx   0 root         (0) root         (0)    10984 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/qimage2ndarray.py
--rw-rw-rw-   0 root         (0) root         (0)     2686 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/qimage_svg.py
--rw-rw-rw-   0 root         (0) root         (0)    21086 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/selection.py
--rw-rw-rw-   0 root         (0) root         (0)    25092 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/spelltextedit.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/string_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.686945 pyspread-2.2/pyspread/lib/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/compat.py
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/invalid1.csv
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/invalid2.csv
--rw-rw-rw-   0 root         (0) root         (0)     3569 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_array2qimage.py
--rw-rw-rw-   0 root         (0) root         (0)     5101 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_csv.py
--rw-rw-rw-   0 root         (0) root         (0)     1457 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_file_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_qimageview.py
--rw-rw-rw-   0 root         (0) root         (0)    16899 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_string_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/valid1.csv
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/valid2.csv
--rw-rw-rw-   0 root         (0) root         (0)  2287092 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/valid3.csv
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/valid4.csv
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/typechecks.py
--rw-rw-rw-   0 root         (0) root         (0)    27821 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/main_window.py
--rw-rw-rw-   0 root         (0) root         (0)    16608 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/menus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.687945 pyspread-2.2/pyspread/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    51556 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/model/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.688945 pyspread-2.2/pyspread/model/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/model/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19920 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/model/test/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4539 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/panels.py
--rwxrwxrwx   0 root         (0) root         (0)     2503 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/pyspread.py
--rw-rw-rw-   0 root         (0) root         (0)    12573 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.688945 pyspread-2.2/pyspread/share/
--rw-rw-rw-   0 root         (0) root         (0)    35141 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.688945 pyspread-2.2/pyspread/share/applications/
--rwxrwxrwx   0 root         (0) root         (0)      761 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.657942 pyspread-2.2/pyspread/share/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.691946 pyspread-2.2/pyspread/share/doc/manual/
--rw-rw-rw-   0 root         (0) root         (0)     3575 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/advanced_topics.md
--rw-rw-rw-   0 root         (0) root         (0)    10408 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/basic_concepts.md
--rw-rw-rw-   0 root         (0) root         (0)     4852 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/edit_menu.md
--rw-rw-rw-   0 root         (0) root         (0)     7506 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/file_menu.md
--rw-rw-rw-   0 root         (0) root         (0)     6821 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/format_menu.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.696946 pyspread-2.2/pyspread/share/doc/manual/images/
--rw-rw-rw-   0 root         (0) root         (0)    18661 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_approve_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)   130518 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_chartdialog.png
--rw-rw-rw-   0 root         (0) root         (0)    24102 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_csv_export.png
--rw-rw-rw-   0 root         (0) root         (0)    26708 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_csv_import.png
--rw-rw-rw-   0 root         (0) root         (0)     7186 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_find_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)     7586 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_macros.png
--rw-rw-rw-   0 root         (0) root         (0)    91836 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_main_window.png
--rw-rw-rw-   0 root         (0) root         (0)    11767 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_new_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)     8572 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_paste_as.png
--rw-rw-rw-   0 root         (0) root         (0)    19022 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_preferences_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)    10973 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_print_preview_1.png
--rw-rw-rw-   0 root         (0) root         (0)    27303 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_print_preview_2.png
--rw-rw-rw-   0 root         (0) root         (0)    16783 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_replace_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)     2360 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/macro_menu.md
--rw-rw-rw-   0 root         (0) root         (0)     1289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/overview.md
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/view_menu.md
--rw-rw-rw-   0 root         (0) root         (0)     5723 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/workspace.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.696946 pyspread-2.2/pyspread/share/doc/tutorial/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.698946 pyspread-2.2/pyspread/share/doc/tutorial/images/
--rw-rw-rw-   0 root         (0) root         (0)    61117 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial1.png
--rw-rw-rw-   0 root         (0) root         (0)    45217 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial2.png
--rw-rw-rw-   0 root         (0) root         (0)    54732 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial3.png
--rw-rw-rw-   0 root         (0) root         (0)    64569 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial4.png
--rw-rw-rw-   0 root         (0) root         (0)     4877 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/tutorial.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.709947 pyspread-2.2/pyspread/share/examples/
--rw-rw-rw-   0 root         (0) root         (0)  8812542 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/big.csv
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/conditional_formatting.pysu
--rw-rw-rw-   0 root         (0) root         (0)    17191 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/images and charts.pysu
--rw-rw-rw-   0 root         (0) root         (0)     4185 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/pivot.pysu
--rw-rw-rw-   0 root         (0) root         (0)    11840 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/pyspred_with_plotnine.pysu
--rw-rw-rw-   0 root         (0) root         (0)     5841 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/rpy2_example.pysu
--rw-rw-rw-   0 root         (0) root         (0)    29100 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/test_write.csv
--rw-rw-rw-   0 root         (0) root         (0)    21717 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/wagner_whitin.pysu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.659942 pyspread-2.2/pyspread/share/icons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.746951 pyspread-2.2/pyspread/share/icons/actions/
--rw-rw-rw-   0 root         (0) root         (0)   136218 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-approve.svg
--rw-rw-rw-   0 root         (0) root         (0)    24975 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-export.svg
--rw-rw-rw-   0 root         (0) root         (0)    21023 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-import.svg
--rw-rw-rw-   0 root         (0) root         (0)    19127 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-log-out.svg
--rw-rw-rw-   0 root         (0) root         (0)   165172 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-new-gpg-key.svg
--rw-rw-rw-   0 root         (0) root         (0)    17406 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-new.svg
--rw-rw-rw-   0 root         (0) root         (0)    30805 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-open.svg
--rw-rw-rw-   0 root         (0) root         (0)    29401 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-page-setup.svg
--rw-rw-rw-   0 root         (0) root         (0)    33813 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-print-preview.svg
--rw-rw-rw-   0 root         (0) root         (0)    23333 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-print.svg
--rw-rw-rw-   0 root         (0) root         (0)    25424 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-properties.svg
--rw-rw-rw-   0 root         (0) root         (0)    31913 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-save-as.svg
--rw-rw-rw-   0 root         (0) root         (0)    29894 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-save.svg
--rw-rw-rw-   0 root         (0) root         (0)    19499 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-clear.svg
--rw-rw-rw-   0 root         (0) root         (0)    16456 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-copy-results.svg
--rw-rw-rw-   0 root         (0) root         (0)    15595 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-copy.svg
--rw-rw-rw-   0 root         (0) root         (0)    23051 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-cut.svg
--rw-rw-rw-   0 root         (0) root         (0)    35153 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-delete-column.svg
--rw-rw-rw-   0 root         (0) root         (0)    24107 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-delete-row.svg
--rw-rw-rw-   0 root         (0) root         (0)    21308 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-delete-table.svg
--rw-rw-rw-   0 root         (0) root         (0)    54926 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-delete.svg
--rw-rw-rw-   0 root         (0) root         (0)     4953 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-find-next.svg
--rw-rw-rw-   0 root         (0) root         (0)    45880 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-find-replace.svg
--rw-rw-rw-   0 root         (0) root         (0)    35412 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-find.svg
--rw-rw-rw-   0 root         (0) root         (0)    14246 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-insert-column.svg
--rw-rw-rw-   0 root         (0) root         (0)    13993 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-insert-row.svg
--rw-rw-rw-   0 root         (0) root         (0)    12163 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-insert-table.svg
--rw-rw-rw-   0 root         (0) root         (0)     8988 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-paste-as.svg
--rw-rw-rw-   0 root         (0) root         (0)    23755 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-paste.svg
--rw-rw-rw-   0 root         (0) root         (0)    37205 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-quote.svg
--rw-rw-rw-   0 root         (0) root         (0)     9331 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-redo.svg
--rw-rw-rw-   0 root         (0) root         (0)     6028 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-resize-grid.svg
--rw-rw-rw-   0 root         (0) root         (0)    15903 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-select-all.svg
--rw-rw-rw-   0 root         (0) root         (0)    17679 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-sort-ascending.svg
--rw-rw-rw-   0 root         (0) root         (0)    18405 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-sort-descending.svg
--rw-rw-rw-   0 root         (0) root         (0)     9235 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-undo.svg
--rw-rw-rw-   0 root         (0) root         (0)    10364 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-background-color.svg
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-0.svg
--rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-1.svg
--rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-16.svg
--rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-2.svg
--rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-32.svg
--rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-4.svg
--rw-rw-rw-   0 root         (0) root         (0)     2274 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-64.svg
--rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-8.svg
--rw-rw-rw-   0 root         (0) root         (0)     3709 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-all.svg
--rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-bottom.svg
--rw-rw-rw-   0 root         (0) root         (0)     3906 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-inner.svg
--rw-rw-rw-   0 root         (0) root         (0)     4029 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-left.svg
--rw-rw-rw-   0 root         (0) root         (0)     3799 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-outer.svg
--rw-rw-rw-   0 root         (0) root         (0)     4029 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-right.svg
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-top-bottom.svg
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-top.svg
--rw-rw-rw-   0 root         (0) root         (0)     3801 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-button.svg
--rw-rw-rw-   0 root         (0) root         (0)    44063 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-chart.svg
--rw-rw-rw-   0 root         (0) root         (0)   718331 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-image.svg
--rw-rw-rw-   0 root         (0) root         (0)    41228 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-markup.svg
--rw-rw-rw-   0 root         (0) root         (0)    14454 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-0.svg
--rw-rw-rw-   0 root         (0) root         (0)    14581 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-180.svg
--rw-rw-rw-   0 root         (0) root         (0)    14580 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-270.svg
--rw-rw-rw-   0 root         (0) root         (0)    15749 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-90.svg
--rw-rw-rw-   0 root         (0) root         (0)    27835 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-text.svg
--rw-rw-rw-   0 root         (0) root         (0)    12343 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-copy.svg
--rw-rw-rw-   0 root         (0) root         (0)    12731 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-font.svg
--rw-rw-rw-   0 root         (0) root         (0)    18923 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-freeze.svg
--rw-rw-rw-   0 root         (0) root         (0)    13344 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-justify-center.svg
--rw-rw-rw-   0 root         (0) root         (0)    13332 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-justify-fill.svg
--rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-justify-left.svg
--rw-rw-rw-   0 root         (0) root         (0)    13382 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-justify-right.svg
--rw-rw-rw-   0 root         (0) root         (0)     7716 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-line-color.svg
--rw-rw-rw-   0 root         (0) root         (0)     8658 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-line-color2.svg
--rw-rw-rw-   0 root         (0) root         (0)   143193 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-lock.svg
--rw-rw-rw-   0 root         (0) root         (0)     2441 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-merge-cells.svg
--rw-rw-rw-   0 root         (0) root         (0)    37466 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-paste.svg
--rw-rw-rw-   0 root         (0) root         (0)    12457 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-align-bottom.svg
--rw-rw-rw-   0 root         (0) root         (0)    12574 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-align-center.svg
--rw-rw-rw-   0 root         (0) root         (0)    12794 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-align-top.svg
--rw-rw-rw-   0 root         (0) root         (0)    10953 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-bold.svg
--rw-rw-rw-   0 root         (0) root         (0)     6484 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-color.svg
--rw-rw-rw-   0 root         (0) root         (0)    11302 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-italic.svg
--rw-rw-rw-   0 root         (0) root         (0)    14525 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-strikethrough.svg
--rw-rw-rw-   0 root         (0) root         (0)    14583 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-underline.svg
--rw-rw-rw-   0 root         (0) root         (0)   121867 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/help-browser.svg
--rw-rw-rw-   0 root         (0) root         (0)   353099 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/help-dependencies.svg
--rw-rw-rw-   0 root         (0) root         (0)     5737 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/help-faq.svg
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/help-tutorial.svg
--rw-rw-rw-   0 root         (0) root         (0)    41994 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-insert-chart.svg
--rw-rw-rw-   0 root         (0) root         (0)   396438 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-insert-image.svg
--rw-rw-rw-   0 root         (0) root         (0)    21889 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-insert-sum.svg
--rw-rw-rw-   0 root         (0) root         (0)   388308 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-link-image.svg
--rw-rw-rw-   0 root         (0) root         (0)    10037 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-open.svg
--rw-rw-rw-   0 root         (0) root         (0)    10693 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-save.svg
--rw-rw-rw-   0 root         (0) root         (0)    19612 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/menu-manager.svg
--rw-rw-rw-   0 root         (0) root         (0)    23289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-check-spelling.svg
--rw-rw-rw-   0 root         (0) root         (0)    20295 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-fullscreen.svg
--rw-rw-rw-   0 root         (0) root         (0)     3176 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-goto-cell.svg
--rw-rw-rw-   0 root         (0) root         (0)    16868 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-refresh.svg
--rw-rw-rw-   0 root         (0) root         (0)    20510 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-show-frozen.svg
--rw-rw-rw-   0 root         (0) root         (0)     6161 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-timer.svg
--rw-rw-rw-   0 root         (0) root         (0)    24550 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-zoom-in.svg
--rw-rw-rw-   0 root         (0) root         (0)    24925 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-zoom-original.svg
--rw-rw-rw-   0 root         (0) root         (0)    24352 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-zoom-out.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.771954 pyspread-2.2/pyspread/share/icons/charts/
--rw-rw-rw-   0 root         (0) root         (0)     7186 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_area_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7163 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_area_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6953 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_area_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     7282 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8140 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8922 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     9125 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8637 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    11228 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    11076 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8346 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bubble_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bubble_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    11693 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_color_polar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9249 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_colored_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7079 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_column_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7821 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_column_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_column_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9078 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     9557 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9544 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    10796 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_polar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8201 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8325 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8348 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     8485 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     7829 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8372 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    10603 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    10879 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     7984 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7187 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7179 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6831 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    10289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    10249 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     9901 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_2_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    17196 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    17576 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    17575 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     8307 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8118 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    10151 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    10108 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_4.svg
--rw-rw-rw-   0 root         (0) root         (0)    10598 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    10502 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    11256 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    14956 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     9173 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_pie_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7522 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_pie_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_pie_3_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7603 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_pie_3_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    14131 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_plotnine_geom_bar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9193 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_polar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7456 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_prob_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    11134 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_boxplot_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    11371 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_density2d_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    11557 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_point_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9745 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_graphics_barplot_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    47553 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_lattice_wireframe_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    11561 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_lattice_xyplot_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8665 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    11428 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8669 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    10288 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_ring_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    10284 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_ring_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8886 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9688 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6618 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6903 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     6721 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6933 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     6933 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     9907 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatterhist_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    44800 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    45240 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    45395 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_3.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.659942 pyspread-2.2/pyspread/share/icons/hicolor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.772954 pyspread-2.2/pyspread/share/icons/hicolor/64x64/
--rw-rw-rw-   0 root         (0) root         (0)    10550 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/hicolor/64x64/pyspread.ico
--rw-rw-rw-   0 root         (0) root         (0)     5285 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/hicolor/64x64/pyspread.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.772954 pyspread-2.2/pyspread/share/icons/hicolor/svg/
--rw-rw-rw-   0 root         (0) root         (0)   330549 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/hicolor/svg/pyspread.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.773954 pyspread-2.2/pyspread/share/icons/status/
--rw-rw-rw-   0 root         (0) root         (0)     4870 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/status/status-safe-mode.svg
--rw-rw-rw-   0 root         (0) root         (0)    24423 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/status/status-selection-mode.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.774954 pyspread-2.2/pyspread/share/metainfo/
--rw-rw-rw-   0 root         (0) root         (0)     2199 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/metainfo/io.gitlab.pyspread.pyspread.metainfo.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.660942 pyspread-2.2/pyspread/share/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.779955 pyspread-2.2/pyspread/share/templates/matplotlib/
--rw-rw-rw-   0 root         (0) root         (0)     2879 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_area_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_bar_1_3.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_boxplot_2_2.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_bubble_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_column_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_column_1_2.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_contour_1_2.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_histogram_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_histogram_1_4.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_line_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_matrix_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_pie_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_polar_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_ring_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_scatter_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)     1392 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      542 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_surface_2_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.779955 pyspread-2.2/pyspread/share/templates/plotnine/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/plotnine/chart_plotnine_geom_bar_1_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.781955 pyspread-2.2/pyspread/share/templates/rpy2/
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_boxplot_1_2.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_density2d_1_2.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_point_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_graphics_barplot_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_lattice_wireframe_2_1.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_lattice_xyplot_1_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.785955 pyspread-2.2/pyspread/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2223 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    40334 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_grid.py
--rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_grid_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_invalid_unsigned_1.pysu
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_invalid_unsigned_2.pysu
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_invalid_unsigned_3.pysu
--rw-rw-rw-   0 root         (0) root         (0)     2691 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_pyspread.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_valid_signed.pysu
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_valid_unsigned.pysu
--rwxrwxrwx   0 root         (0) root         (0)     6822 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)    14289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/toolbar.py
--rw-rw-rw-   0 root         (0) root         (0)    22344 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/widgets.py
--rw-rw-rw-   0 root         (0) root         (0)    71033 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/workflows.py
--rwxrwxrwx   0 root         (0) root         (0)      735 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread.desktop
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.673944 pyspread-2.2/pyspread.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5106 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14895 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread.pth
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-04-16 18:39:21.000000 pyspread-2.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-16 18:40:47.786955 pyspread-2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-04-16 18:39:21.000000 pyspread-2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.421002 pyspread-2.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-30 06:58:01.000000 pyspread-2.2.1/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    35141 2023-04-30 06:58:01.000000 pyspread-2.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-30 06:58:01.000000 pyspread-2.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-04-30 06:59:35.421002 pyspread-2.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2608 2023-04-30 06:58:01.000000 pyspread-2.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-30 06:58:01.000000 pyspread-2.2.1/THANKS
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 06:58:01.000000 pyspread-2.2.1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15607 2023-04-30 06:58:01.000000 pyspread-2.2.1/changelog
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.296995 pyspread-2.2.1/pyspread/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    48145 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3393 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    38479 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)    58195 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/dialogs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/entryline.py
+-rw-rw-rw-   0 root         (0) root         (0)    96463 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    30890 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/grid_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     9372 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/icons.py
+-rw-rw-rw-   0 root         (0) root         (0)    11233 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/installer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.299995 pyspread-2.2.1/pyspread/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19559 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/interfaces/pys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.303995 pyspread-2.2.1/pyspread/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/attrdict.py
+-rw-rw-rw-   0 root         (0) root         (0)     9886 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/charts.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    45208 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/dataclasses.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/exception_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     4077 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/file_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/hashing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.305995 pyspread-2.2.1/pyspread/lib/packaging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/packaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/packaging/_structures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/packaging/_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    15480 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/packaging/version.py
+-rwxrwxrwx   0 root         (0) root         (0)    10984 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/qimage2ndarray.py
+-rw-rw-rw-   0 root         (0) root         (0)     2686 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/qimage_svg.py
+-rw-rw-rw-   0 root         (0) root         (0)    21086 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    25092 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/spelltextedit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/string_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.313996 pyspread-2.2.1/pyspread/lib/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/invalid1.csv
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/invalid2.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3569 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/test_array2qimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     5101 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/test_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/test_file_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/test_hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/test_qimageview.py
+-rw-rw-rw-   0 root         (0) root         (0)    16899 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/test_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/test_string_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/valid1.csv
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/valid2.csv
+-rw-rw-rw-   0 root         (0) root         (0)  2287092 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/valid3.csv
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/test/valid4.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/lib/typechecks.py
+-rw-rw-rw-   0 root         (0) root         (0)    27821 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/main_window.py
+-rw-rw-rw-   0 root         (0) root         (0)    16608 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/menus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.314996 pyspread-2.2.1/pyspread/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    51507 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/model/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.315996 pyspread-2.2.1/pyspread/model/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/model/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19920 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/model/test/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4539 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/panels.py
+-rwxrwxrwx   0 root         (0) root         (0)     2503 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/pyspread.py
+-rw-rw-rw-   0 root         (0) root         (0)    12573 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.315996 pyspread-2.2.1/pyspread/share/
+-rw-rw-rw-   0 root         (0) root         (0)    35141 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.315996 pyspread-2.2.1/pyspread/share/applications/
+-rwxrwxrwx   0 root         (0) root         (0)      761 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.281994 pyspread-2.2.1/pyspread/share/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.319996 pyspread-2.2.1/pyspread/share/doc/manual/
+-rw-rw-rw-   0 root         (0) root         (0)     3575 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/advanced_topics.md
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/basic_concepts.md
+-rw-rw-rw-   0 root         (0) root         (0)     4852 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/edit_menu.md
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/file_menu.md
+-rw-rw-rw-   0 root         (0) root         (0)     6821 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/format_menu.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.324996 pyspread-2.2.1/pyspread/share/doc/manual/images/
+-rw-rw-rw-   0 root         (0) root         (0)    18661 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_approve_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)   130518 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_chartdialog.png
+-rw-rw-rw-   0 root         (0) root         (0)    24102 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_csv_export.png
+-rw-rw-rw-   0 root         (0) root         (0)    26708 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_csv_import.png
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_find_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)     7586 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_macros.png
+-rw-rw-rw-   0 root         (0) root         (0)    91836 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_main_window.png
+-rw-rw-rw-   0 root         (0) root         (0)    11767 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_new_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)     8572 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_paste_as.png
+-rw-rw-rw-   0 root         (0) root         (0)    19022 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_preferences_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)    10973 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_print_preview_1.png
+-rw-rw-rw-   0 root         (0) root         (0)    27303 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_print_preview_2.png
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_replace_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)     2360 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/macro_menu.md
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/overview.md
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/view_menu.md
+-rw-rw-rw-   0 root         (0) root         (0)     5723 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/manual/workspace.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.324996 pyspread-2.2.1/pyspread/share/doc/tutorial/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.326996 pyspread-2.2.1/pyspread/share/doc/tutorial/images/
+-rw-rw-rw-   0 root         (0) root         (0)    61117 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/tutorial/images/Tutorial1.png
+-rw-rw-rw-   0 root         (0) root         (0)    45217 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/tutorial/images/Tutorial2.png
+-rw-rw-rw-   0 root         (0) root         (0)    54732 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/tutorial/images/Tutorial3.png
+-rw-rw-rw-   0 root         (0) root         (0)    64569 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/tutorial/images/Tutorial4.png
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/doc/tutorial/tutorial.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.340997 pyspread-2.2.1/pyspread/share/examples/
+-rw-rw-rw-   0 root         (0) root         (0)  8812542 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/examples/big.csv
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/examples/conditional_formatting.pysu
+-rw-rw-rw-   0 root         (0) root         (0)    17191 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/examples/images and charts.pysu
+-rw-rw-rw-   0 root         (0) root         (0)     4185 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/examples/pivot.pysu
+-rw-rw-rw-   0 root         (0) root         (0)    11840 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/examples/pyspred_with_plotnine.pysu
+-rw-rw-rw-   0 root         (0) root         (0)     5841 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/examples/rpy2_example.pysu
+-rw-rw-rw-   0 root         (0) root         (0)    29100 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/examples/test_write.csv
+-rw-rw-rw-   0 root         (0) root         (0)    21717 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/examples/wagner_whitin.pysu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.283994 pyspread-2.2.1/pyspread/share/icons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.381000 pyspread-2.2.1/pyspread/share/icons/actions/
+-rw-rw-rw-   0 root         (0) root         (0)   136218 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-approve.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24975 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-export.svg
+-rw-rw-rw-   0 root         (0) root         (0)    21023 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-import.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19127 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-log-out.svg
+-rw-rw-rw-   0 root         (0) root         (0)   165172 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-new-gpg-key.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17406 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-new.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30805 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-open.svg
+-rw-rw-rw-   0 root         (0) root         (0)    29401 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-page-setup.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33813 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-print-preview.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23333 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-print.svg
+-rw-rw-rw-   0 root         (0) root         (0)    25424 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-properties.svg
+-rw-rw-rw-   0 root         (0) root         (0)    31913 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-save-as.svg
+-rw-rw-rw-   0 root         (0) root         (0)    29894 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/document-save.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19499 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-clear.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16456 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-copy-results.svg
+-rw-rw-rw-   0 root         (0) root         (0)    15595 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-copy.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23051 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-cut.svg
+-rw-rw-rw-   0 root         (0) root         (0)    35153 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-delete-column.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24107 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-delete-row.svg
+-rw-rw-rw-   0 root         (0) root         (0)    21308 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-delete-table.svg
+-rw-rw-rw-   0 root         (0) root         (0)    54926 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-delete.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4953 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-find-next.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45880 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-find-replace.svg
+-rw-rw-rw-   0 root         (0) root         (0)    35412 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-find.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14246 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-insert-column.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13993 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-insert-row.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12163 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-insert-table.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8988 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-paste-as.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23755 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-paste.svg
+-rw-rw-rw-   0 root         (0) root         (0)    37205 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-quote.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9331 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-redo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6028 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-resize-grid.svg
+-rw-rw-rw-   0 root         (0) root         (0)    15903 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-select-all.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17679 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-sort-ascending.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18405 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-sort-descending.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9235 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/edit-undo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-background-color.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-0.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-16.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-32.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-64.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-8.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-all.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-bottom.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3906 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-inner.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-left.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-outer.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-right.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-top-bottom.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-borders-top.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3801 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-button.svg
+-rw-rw-rw-   0 root         (0) root         (0)    44063 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-cell-chart.svg
+-rw-rw-rw-   0 root         (0) root         (0)   718331 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-cell-image.svg
+-rw-rw-rw-   0 root         (0) root         (0)    41228 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-cell-markup.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14454 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-cell-rotate-0.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14581 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-cell-rotate-180.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14580 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-cell-rotate-270.svg
+-rw-rw-rw-   0 root         (0) root         (0)    15749 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-cell-rotate-90.svg
+-rw-rw-rw-   0 root         (0) root         (0)    27835 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-cell-text.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12343 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-copy.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12731 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-font.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18923 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-freeze.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13344 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-justify-center.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13332 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-justify-fill.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-justify-left.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13382 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-justify-right.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7716 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-line-color.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8658 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-line-color2.svg
+-rw-rw-rw-   0 root         (0) root         (0)   143193 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-lock.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-merge-cells.svg
+-rw-rw-rw-   0 root         (0) root         (0)    37466 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-paste.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12457 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-text-align-bottom.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12574 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-text-align-center.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12794 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-text-align-top.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10953 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-text-bold.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6484 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-text-color.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11302 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-text-italic.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14525 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-text-strikethrough.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14583 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/format-text-underline.svg
+-rw-rw-rw-   0 root         (0) root         (0)   121867 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/help-browser.svg
+-rw-rw-rw-   0 root         (0) root         (0)   353099 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/help-dependencies.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5737 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/help-faq.svg
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/help-tutorial.svg
+-rw-rw-rw-   0 root         (0) root         (0)    41994 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/macro-insert-chart.svg
+-rw-rw-rw-   0 root         (0) root         (0)   396438 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/macro-insert-image.svg
+-rw-rw-rw-   0 root         (0) root         (0)    21889 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/macro-insert-sum.svg
+-rw-rw-rw-   0 root         (0) root         (0)   388308 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/macro-link-image.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10037 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/macro-open.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10693 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/macro-save.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19612 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/menu-manager.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23289 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-check-spelling.svg
+-rw-rw-rw-   0 root         (0) root         (0)    20295 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-fullscreen.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-goto-cell.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16868 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-refresh.svg
+-rw-rw-rw-   0 root         (0) root         (0)    20510 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-show-frozen.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-timer.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24550 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-zoom-in.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24925 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-zoom-original.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24352 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/actions/view-zoom-out.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.407001 pyspread-2.2.1/pyspread/share/icons/charts/
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_area_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_area_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_area_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7282 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_bar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8140 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_bar_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8922 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_bar_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9125 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_boxplot_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8637 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_boxplot_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11228 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_boxplot_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11076 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_boxplot_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8346 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_bubble_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_bubble_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11693 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_color_polar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9249 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_colored_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7079 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_column_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7821 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_column_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_column_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9078 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9557 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9544 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10796 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_polar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8201 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_dropbar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8325 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_dropbar_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8348 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_dropbar_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8485 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_dropbar_1_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7829 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8372 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10603 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10879 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_1_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7187 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_line_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7179 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_line_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6831 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_line_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10289 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_line_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10249 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_line_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_line_2_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17196 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_matrix_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17576 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_matrix_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17575 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_matrix_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8307 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8118 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10151 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10108 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_1_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10598 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10502 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11256 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_2_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14956 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_2_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9173 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_pie_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7522 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_pie_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_pie_3_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7603 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_pie_3_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14131 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_plotnine_geom_bar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9193 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_polar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7456 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_prob_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11134 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_r_ggplot2_geom_boxplot_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11371 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_r_ggplot2_geom_density2d_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11557 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_r_ggplot2_geom_point_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9745 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_r_graphics_barplot_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    47553 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_r_lattice_wireframe_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11561 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_r_lattice_xyplot_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8665 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_radar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11428 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_radar_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8669 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_radar_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10288 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_ring_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10284 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_ring_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8886 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9688 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_3_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6618 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_3_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6903 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_3_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6721 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_4_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_4_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6933 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_4_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6933 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_4_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9907 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_scatterhist_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    44800 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_surface_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45240 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_surface_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45395 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/charts/chart_surface_2_3.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.283994 pyspread-2.2.1/pyspread/share/icons/hicolor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.408001 pyspread-2.2.1/pyspread/share/icons/hicolor/64x64/
+-rw-rw-rw-   0 root         (0) root         (0)    10550 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/hicolor/64x64/pyspread.ico
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/hicolor/64x64/pyspread.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.408001 pyspread-2.2.1/pyspread/share/icons/hicolor/svg/
+-rw-rw-rw-   0 root         (0) root         (0)   330549 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/hicolor/svg/pyspread.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.409001 pyspread-2.2.1/pyspread/share/icons/status/
+-rw-rw-rw-   0 root         (0) root         (0)     4870 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/status/status-safe-mode.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24423 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/icons/status/status-selection-mode.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.409001 pyspread-2.2.1/pyspread/share/metainfo/
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/metainfo/io.gitlab.pyspread.pyspread.metainfo.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.284994 pyspread-2.2.1/pyspread/share/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.415002 pyspread-2.2.1/pyspread/share/templates/matplotlib/
+-rw-rw-rw-   0 root         (0) root         (0)     2879 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_area_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_bar_1_3.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_boxplot_2_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_bubble_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_column_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_column_1_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_contour_1_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_histogram_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_histogram_1_4.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_line_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_matrix_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_pie_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_polar_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_ring_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_scatter_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1392 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_surface_2_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.416002 pyspread-2.2.1/pyspread/share/templates/plotnine/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/plotnine/chart_plotnine_geom_bar_1_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.418002 pyspread-2.2.1/pyspread/share/templates/rpy2/
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_boxplot_1_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_density2d_1_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_point_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_graphics_barplot_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_lattice_wireframe_2_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_lattice_xyplot_1_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.421002 pyspread-2.2.1/pyspread/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2223 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    40334 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_grid_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_invalid_unsigned_1.pysu
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_invalid_unsigned_2.pysu
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_invalid_unsigned_3.pysu
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_pyspread.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_valid_signed.pysu
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_valid_unsigned.pysu
+-rwxrwxrwx   0 root         (0) root         (0)     6822 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/test/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)    14432 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/toolbar.py
+-rw-rw-rw-   0 root         (0) root         (0)    22344 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/widgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    69455 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread/workflows.py
+-rwxrwxrwx   0 root         (0) root         (0)      735 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread.desktop
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 06:59:35.298995 pyspread-2.2.1/pyspread.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-04-30 06:59:35.000000 pyspread-2.2.1/pyspread.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14895 2023-04-30 06:59:35.000000 pyspread-2.2.1/pyspread.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 06:59:35.000000 pyspread-2.2.1/pyspread.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-30 06:59:35.000000 pyspread-2.2.1/pyspread.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-30 06:59:35.000000 pyspread-2.2.1/pyspread.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-30 06:59:35.000000 pyspread-2.2.1/pyspread.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-30 06:58:01.000000 pyspread-2.2.1/pyspread.pth
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-04-30 06:58:01.000000 pyspread-2.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-30 06:59:35.422002 pyspread-2.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-04-30 06:58:01.000000 pyspread-2.2.1/setup.py
```

### Comparing `pyspread-2.2/LICENSE` & `pyspread-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/PKG-INFO` & `pyspread-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspread
-Version: 2.2
+Version: 2.2.1
 Summary: Pyspread is a non-traditional spreadsheet application that is based on and written in the programming language Python.
 Home-page: https://pyspread.gitlab.io
 Author: Martin Manns
 Author-email: mmanns@gmx.net
 License: GPL v3 :: GNU General Public License
 Project-URL: Bug Tracker, https://gitlab.com/pyspread/pyspread/issues
 Project-URL: Documentation, https://pyspread.gitlab.io/docs.html
```

### Comparing `pyspread-2.2/README.md` & `pyspread-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/changelog` & `pyspread-2.2.1/changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 Changelog for pyspread
 ======================
 
 Note: This changelog does not comprise development of pyspread for Python2
       It starts with the first Alpha release 1.99.0.0
 
+      
+2.2.1
+---
+
+This is a bugfix release
+Note that missing libvoikko, nuspell and hspell may lead to warning messages if pyenchant is installed. However,  pyspread is still functional as this affects only spellchecking.
+
+Dependencies:
+ * Mandatory: Python (≥ 3.6), numpy (>=1.1), PyQt5 (≥ 5.10, requires PyQt5.Svg), setuptools (>=40.0), markdown2 (>= 2.3)
+ * Recommended: matplotlib (>=1.1.1), pyenchant (>=1.1), pip (>=18), python-dateutil (>= 2.7.0), py-moneyed (>=2.0), rpy2 (>=3.4), plotnine (>=0.8), libvoikko (>=4.0), libvoikko (>=4.3), nuspell (>=5.1), hspell (>= 1.4), ggplot2 (>=3.4)
+ * For building the apidocs with Sphinx see apidocs/requirements.txt
+
+Bug fixes:
+ * Chart dialog now correctly starts if rpy2 is not installed and if optional R modules are missing.
+ * Deleting large selections is now significantly faster.
+ * Pasting into large selections is now significantly faster.
+ * QPen cache now is limited in size.
 
 2.2
 ---
 
 This release adds R charts via rpy2. Examples are available in the chart dialog.
 Note that the R packages graphics, lattice and ggplot2 are used for the examples.
```

### Comparing `pyspread-2.2/pyspread/__main__.py` & `pyspread-2.2.1/pyspread/__main__.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/actions.py` & `pyspread-2.2.1/pyspread/actions.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/cli.py` & `pyspread-2.2.1/pyspread/cli.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/commands.py` & `pyspread-2.2.1/pyspread/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 * :class:`SetColumnWidth`
 * :class:`SetRowHeight`
 
 
 """
 
 from copy import copy
+from itertools import cycle
 from math import isclose
 from typing import List, Iterable, Tuple
 
 from PyQt5.QtCore import Qt, QModelIndex, QAbstractTableModel
 from PyQt5.QtGui import QTextDocument
 from PyQt5.QtWidgets import QUndoCommand, QTableView, QPlainTextEdit
 
@@ -110,14 +111,79 @@
 
         for row, column, table in self.deleted_cells:
             index = model.index(row, column, QModelIndex())
             code = self.deleted_cells[(row, column, table)]
             model.setData(index, code, Qt.EditRole, raw=True, table=table)
 
 
+class PasteSelectedCellData(QUndoCommand):
+    """Paste selected cells"""
+
+    def __init__(self, grid: QTableView, model: QAbstractTableModel,
+                 selection: Selection, data: str, description: str):
+        """
+        :param grid: The main grid object
+        :param model: Model of the grid object
+        :param selection: Selection into which cells are pasted
+        :param data: Data to be pasted
+        :param description: Command description
+
+        """
+        super().__init__(description)
+        self.grid = grid
+        self.model = model
+        self.selection = selection
+        self.data = data
+
+    def redo(self):
+        """Redo cell data deletion, updates screen"""
+
+        self.old_code = {}
+
+        code_array = self.model.code_array
+        shape = self.model.shape
+        table = self.grid.table
+        selection = self.selection
+
+        (top, left), (bottom, right) = selection.get_grid_bbox(shape)
+
+        paste_gen = (line.split("\t") for line in self.data.split("\n"))
+        for row, line in enumerate(cycle(paste_gen)):
+            paste_row = row + top
+            if paste_row > bottom or (paste_row, 0, table) not in code_array:
+                break
+            for column, value in enumerate(cycle(line)):
+                paste_column = column + left
+                paste_key = paste_row, paste_column, table
+                if (paste_key in code_array
+                        and paste_column <= right):
+                    if ((paste_row, paste_column) in selection and not
+                            code_array.cell_attributes[paste_key].locked):
+                        key = paste_row, paste_column, table
+                        # Preserve line breaks
+                        value = value.replace("\u000C", "\n")
+                        try:
+                            self.old_code[key] = code_array(key)
+                            code_array[key] = value
+                        except IndexError:
+                            pass
+                else:
+                    break
+
+        self.model.dataChanged.emit(QModelIndex(), QModelIndex())
+
+    def undo(self):
+        """Undo row insertion, updates screen"""
+
+        for key in self.old_code:
+            self.model.code_array[key] = self.old_code[key]
+        self.old_code.clear()
+        self.model.dataChanged.emit(QModelIndex(), QModelIndex())
+
+
 class SetCellCode(QUndoCommand):
     """Sets cell code in grid"""
 
     def __init__(self, code: str, model: QAbstractTableModel,
                  index: QModelIndex, description: str):
         """
         :param code: The main grid object
@@ -343,14 +409,54 @@
                     except KeyError:
                         pass
                 else:
                     code_array.col_widths[(column, self.table)] = \
                         self.old_width
 
 
+class DeleteSelectedCellData(QUndoCommand):
+    """Delete selected cells"""
+
+    def __init__(self, grid: QTableView, model: QAbstractTableModel,
+                 selection: Selection, description: str):
+        """
+        :param grid: The main grid object
+        :param model: Model of the grid object
+        :param selection: Selected cells to be deleted
+        :param description: Command description
+
+        """
+        super().__init__(description)
+        self.grid = grid
+        self.model = model
+        self.selection = selection
+
+    def redo(self):
+        """Redo cell data deletion, updates screen"""
+
+        self.old_code = {}
+        for key in self.selection.cell_generator(self.model.shape,
+                                                 self.grid.table):
+            if not self.model.code_array.cell_attributes[key]['locked']:
+                try:
+                    self.old_code[key] = self.model.code_array.pop(key)
+                except KeyError:
+                    pass
+
+        self.model.dataChanged.emit(QModelIndex(), QModelIndex())
+
+    def undo(self):
+        """Undo row insertion, updates screen"""
+
+        for key in self.old_code:
+            self.model.code_array[key] = self.old_code[key]
+        self.old_code.clear()
+        self.model.dataChanged.emit(QModelIndex(), QModelIndex())
+
+
 class InsertRows(QUndoCommand):
     """Inserts grid rows"""
 
     def __init__(self, grid: QTableView, model: QAbstractTableModel,
                  index: QModelIndex, row: int, count: int, description: str):
         """
         :param grid: The main grid object
```

### Comparing `pyspread-2.2/pyspread/dialogs.py` & `pyspread-2.2.1/pyspread/dialogs.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/entryline.py` & `pyspread-2.2.1/pyspread/entryline.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/grid.py` & `pyspread-2.2.1/pyspread/grid.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/grid_renderer.py` & `pyspread-2.2.1/pyspread/grid_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 from PyQt5.QtCore import Qt, QModelIndex, QRectF, QPointF
 from PyQt5.QtGui import (QBrush, QPainter, QPalette, QPen,
                          QPainterPath, QPolygonF, QPainterPathStroker)
 
 from PyQt5.QtGui import QColor as __QColor
 from PyQt5.QtWidgets import QTableView, QStyleOptionViewItem
+from functools import lru_cache
 
 
 @contextmanager
 def painter_save(painter: QPainter):
     """Context manager saving and restoring painter state
 
     :param painter: Painter, for which the state is preserved
@@ -451,16 +452,14 @@
      * Cell borders that are thicker than 1 are painted on all borders.
      * At the edges, borders are painted in the following order:
         1. Thin borders are painted first
         2. If border width is equal, lighter colors are painted first
 
     """
 
-    _pen_cache = {}
-
     def __init__(self, grid: QTableView, painter: QPainter,
                  option: QStyleOptionViewItem, index: QModelIndex):
         """
         :param grid: The main grid widget
         :param painter: Painter with which borders are drawn
         :param option: Style option for rendering
         :param index: Index of cell to be rendered
@@ -520,34 +519,28 @@
 
         """
 
         with painter_zoom(self.painter, self.grid.zoom, rect) as zrect:
             self.grid.delegate.paint_(self.painter, zrect, self.option,
                                       self.index)
 
-    def _get_border_pen(self, width, zoom):
+    @staticmethod
+    @lru_cache(maxsize=65536)
+    def _get_border_pen(width, zoom):
         """Gets zoomed border pen, white, fully transparent
 
         :param width: Unzoomed line width
         :param zoom: Current zoom level of grid
 
         """
 
-        try:
-            return self._pen_cache[(width, zoom)]
-        except KeyError:
-            pass
-
         zoomed_width = max(1, width * zoom)
 
-        pen = QPen(QColor(255, 255, 255, 0), zoomed_width,
-                   Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
-        self._pen_cache[(width, zoom)] = pen
-
-        return pen
+        return QPen(QColor(255, 255, 255, 0), zoomed_width,
+                    Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
 
     def _draw_line(self, point1: QPointF, point2: QPointF, width: float,
                    color: QColor, clip_path: QPainterPath):
         """Draws line
 
         Uses drawLine for screen painting and QPainterPathStroker for
         svg painting.
```

### Comparing `pyspread-2.2/pyspread/icons.py` & `pyspread-2.2.1/pyspread/icons.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/installer.py` & `pyspread-2.2.1/pyspread/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
            required_version=version.parse("2.7.0")),
     Module(name="py-moneyed",
            description="Import money from csv using the py-moneyed module",
            required_version=version.parse("2.0")),
     Module(name="matplotlib",
            description="Create charts",
            required_version=version.parse("3.4")),
+    Module(name="rpy2",
+           description="Interface to R, required for R charts",
+           required_version=version.parse("3.4")),
     Module(name="plotnine",
            description="Grammar of graphics for simpler R ggplot2 charts",
            required_version=version.parse("0.8")),
 ]
 
 DEPENDENCIES = REQUIRED_DEPENDENCIES + OPTIONAL_DEPENDENCIES
```

### Comparing `pyspread-2.2/pyspread/interfaces/pys.py` & `pyspread-2.2.1/pyspread/interfaces/pys.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/attrdict.py` & `pyspread-2.2.1/pyspread/lib/attrdict.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/charts.py` & `pyspread-2.2.1/pyspread/lib/charts.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/csv.py` & `pyspread-2.2.1/pyspread/lib/csv.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/dataclasses.py` & `pyspread-2.2.1/pyspread/lib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/exception_handling.py` & `pyspread-2.2.1/pyspread/lib/exception_handling.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/file_helpers.py` & `pyspread-2.2.1/pyspread/lib/file_helpers.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/hashing.py` & `pyspread-2.2.1/pyspread/lib/hashing.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/packaging/_structures.py` & `pyspread-2.2.1/pyspread/lib/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/packaging/_typing.py` & `pyspread-2.2.1/pyspread/lib/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/packaging/version.py` & `pyspread-2.2.1/pyspread/lib/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/qimage2ndarray.py` & `pyspread-2.2.1/pyspread/lib/qimage2ndarray.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/qimage_svg.py` & `pyspread-2.2.1/pyspread/lib/qimage_svg.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/selection.py` & `pyspread-2.2.1/pyspread/lib/selection.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/spelltextedit.py` & `pyspread-2.2.1/pyspread/lib/spelltextedit.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/string_helpers.py` & `pyspread-2.2.1/pyspread/lib/string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/compat.py` & `pyspread-2.2.1/pyspread/lib/test/compat.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/test_array2qimage.py` & `pyspread-2.2.1/pyspread/lib/test/test_array2qimage.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/test_csv.py` & `pyspread-2.2.1/pyspread/lib/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/test_file_helpers.py` & `pyspread-2.2.1/pyspread/lib/test/test_file_helpers.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/test_hashing.py` & `pyspread-2.2.1/pyspread/lib/test/test_hashing.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/test_qimageview.py` & `pyspread-2.2.1/pyspread/lib/test/test_qimageview.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/test_selection.py` & `pyspread-2.2.1/pyspread/lib/test/test_selection.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/test_string_helpers.py` & `pyspread-2.2.1/pyspread/lib/test/test_string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/test/valid3.csv` & `pyspread-2.2.1/pyspread/lib/test/valid3.csv`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/lib/typechecks.py` & `pyspread-2.2.1/pyspread/lib/typechecks.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/main_window.py` & `pyspread-2.2.1/pyspread/main_window.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/menus.py` & `pyspread-2.2.1/pyspread/menus.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/model/model.py` & `pyspread-2.2.1/pyspread/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1217,17 +1217,14 @@
 
     # Cache for results from __getitem__ calls
     result_cache = {}
 
     # Cache for frozen objects
     frozen_cache = {}
 
-    # Custom font storage
-    custom_fonts = {}
-
     # Safe mode: If True then Whether pyspread is operating in safe_mode
     # In safe_mode, cells are not evaluated but its code is returned instead.
     safe_mode = False
 
     def __setitem__(self, key: Tuple[Union[int, slice], Union[int, slice],
                                      Union[int, slice]], value: str):
         """Sets cell code and resets result cache
```

### Comparing `pyspread-2.2/pyspread/model/test/test_model.py` & `pyspread-2.2.1/pyspread/model/test/test_model.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/panels.py` & `pyspread-2.2.1/pyspread/panels.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/pyspread.py` & `pyspread-2.2.1/pyspread/pyspread.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/settings.py` & `pyspread-2.2.1/pyspread/settings.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/LICENSE` & `pyspread-2.2.1/pyspread/share/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop` & `pyspread-2.2.1/pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/advanced_topics.md` & `pyspread-2.2.1/pyspread/share/doc/manual/advanced_topics.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/basic_concepts.md` & `pyspread-2.2.1/pyspread/share/doc/manual/basic_concepts.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/edit_menu.md` & `pyspread-2.2.1/pyspread/share/doc/manual/edit_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/file_menu.md` & `pyspread-2.2.1/pyspread/share/doc/manual/file_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/format_menu.md` & `pyspread-2.2.1/pyspread/share/doc/manual/format_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_approve_dialog.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_approve_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_chartdialog.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_chartdialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_csv_export.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_csv_export.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_csv_import.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_csv_import.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_find_dialog.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_find_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_macros.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_macros.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_main_window.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_main_window.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_new_dialog.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_new_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_paste_as.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_paste_as.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_preferences_dialog.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_preferences_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_print_preview_1.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_print_preview_1.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_print_preview_2.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_print_preview_2.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_replace_dialog.png` & `pyspread-2.2.1/pyspread/share/doc/manual/images/screenshot_replace_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/macro_menu.md` & `pyspread-2.2.1/pyspread/share/doc/manual/macro_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/overview.md` & `pyspread-2.2.1/pyspread/share/doc/manual/overview.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/view_menu.md` & `pyspread-2.2.1/pyspread/share/doc/manual/view_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/manual/workspace.md` & `pyspread-2.2.1/pyspread/share/doc/manual/workspace.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial1.png` & `pyspread-2.2.1/pyspread/share/doc/tutorial/images/Tutorial1.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial2.png` & `pyspread-2.2.1/pyspread/share/doc/tutorial/images/Tutorial2.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial3.png` & `pyspread-2.2.1/pyspread/share/doc/tutorial/images/Tutorial3.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial4.png` & `pyspread-2.2.1/pyspread/share/doc/tutorial/images/Tutorial4.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/doc/tutorial/tutorial.md` & `pyspread-2.2.1/pyspread/share/doc/tutorial/tutorial.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/examples/images and charts.pysu` & `pyspread-2.2.1/pyspread/share/examples/images and charts.pysu`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/examples/pivot.pysu` & `pyspread-2.2.1/pyspread/share/examples/pivot.pysu`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/examples/pyspred_with_plotnine.pysu` & `pyspread-2.2.1/pyspread/share/examples/pyspred_with_plotnine.pysu`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/examples/rpy2_example.pysu` & `pyspread-2.2.1/pyspread/share/examples/rpy2_example.pysu`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/examples/test_write.csv` & `pyspread-2.2.1/pyspread/share/examples/test_write.csv`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/examples/wagner_whitin.pysu` & `pyspread-2.2.1/pyspread/share/examples/wagner_whitin.pysu`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-approve.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-approve.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-export.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-export.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-import.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-import.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-log-out.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-log-out.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-new-gpg-key.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-new-gpg-key.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-new.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-new.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-open.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-open.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-page-setup.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-page-setup.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-print-preview.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-print.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-print.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-properties.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-properties.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-save-as.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/document-save.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/document-save.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-clear.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-copy-results.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-copy-results.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-copy.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-copy.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-cut.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-cut.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-delete-column.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-delete-column.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-delete-row.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-delete-row.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-delete-table.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-delete-table.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-delete.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-delete.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-find-next.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-find-next.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-find-replace.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-find-replace.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-find.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-find.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-insert-column.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-insert-column.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-insert-row.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-insert-row.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-insert-table.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-insert-table.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-paste-as.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-paste-as.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-paste.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-paste.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-quote.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-quote.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-redo.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-resize-grid.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-resize-grid.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-select-all.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-select-all.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-sort-ascending.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-sort-ascending.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-sort-descending.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-sort-descending.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/edit-undo.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-background-color.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-background-color.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-0.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-0.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-1.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-16.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-16.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-2.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-32.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-32.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-4.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-64.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-64.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-8.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-8.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-all.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-all.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-bottom.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-bottom.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-inner.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-inner.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-left.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-left.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-outer.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-outer.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-right.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-right.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-top-bottom.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-top-bottom.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-borders-top.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-borders-top.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-button.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-button.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-cell-chart.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-cell-chart.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-cell-image.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-cell-image.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-cell-markup.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-cell-markup.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-0.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-cell-rotate-0.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-180.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-cell-rotate-180.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-270.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-cell-rotate-270.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-90.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-cell-rotate-90.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-cell-text.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-cell-text.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-copy.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-copy.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-font.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-font.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-freeze.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-freeze.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-justify-center.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-justify-center.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-justify-fill.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-justify-fill.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-justify-left.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-justify-left.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-justify-right.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-justify-right.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-line-color.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-line-color.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-line-color2.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-line-color2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-lock.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-lock.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-merge-cells.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-merge-cells.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-paste.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-paste.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-text-align-bottom.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-text-align-bottom.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-text-align-center.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-text-align-center.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-text-align-top.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-text-align-top.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-text-bold.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-text-bold.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-text-color.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-text-color.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-text-italic.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-text-italic.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-text-strikethrough.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-text-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/format-text-underline.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/format-text-underline.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/help-browser.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/help-browser.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/help-dependencies.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/help-dependencies.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/help-faq.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/help-faq.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/macro-insert-chart.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/macro-insert-chart.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/macro-insert-image.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/macro-insert-image.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/macro-insert-sum.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/macro-insert-sum.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/macro-link-image.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/macro-link-image.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/macro-open.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/macro-open.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/macro-save.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/macro-save.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/menu-manager.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/menu-manager.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-check-spelling.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-check-spelling.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-fullscreen.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-fullscreen.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-goto-cell.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-goto-cell.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-refresh.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-refresh.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-show-frozen.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-show-frozen.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-timer.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-timer.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-zoom-in.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-zoom-in.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-zoom-original.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-zoom-original.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/actions/view-zoom-out.svg` & `pyspread-2.2.1/pyspread/share/icons/actions/view-zoom-out.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_area_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_area_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_area_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_area_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_area_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_area_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_bar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_bar_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_bar_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_boxplot_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_boxplot_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_2_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_boxplot_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_2_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_boxplot_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_bubble_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_bubble_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_bubble_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_bubble_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_color_polar_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_color_polar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_colored_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_colored_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_column_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_column_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_column_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_column_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_column_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_column_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_contour_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_contour_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_contour_2_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_contour_2_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_contour_polar_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_contour_polar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_dropbar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_dropbar_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_dropbar_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_4.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_dropbar_1_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_4.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_1_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_2_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_histogram_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_line_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_line_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_line_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_line_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_line_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_line_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_line_2_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_line_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_line_2_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_line_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_line_2_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_line_2_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_matrix_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_matrix_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_matrix_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_4.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_1_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_2_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_4.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_minmax_2_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_pie_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_pie_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_pie_2_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_pie_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_pie_3_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_pie_3_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_pie_3_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_pie_3_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_plotnine_geom_bar_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_plotnine_geom_bar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_polar_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_polar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_prob_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_prob_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_boxplot_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_r_ggplot2_geom_boxplot_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_density2d_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_r_ggplot2_geom_density2d_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_point_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_r_ggplot2_geom_point_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_r_graphics_barplot_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_r_graphics_barplot_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_r_lattice_wireframe_2_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_r_lattice_wireframe_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_r_lattice_xyplot_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_r_lattice_xyplot_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_radar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_radar_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_radar_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_ring_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_ring_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_ring_1_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_ring_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_3_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_3_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_3_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_4_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_4_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_4_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_4.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatter_4_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_scatterhist_1_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_scatterhist_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_1.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_surface_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_2.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_surface_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_3.svg` & `pyspread-2.2.1/pyspread/share/icons/charts/chart_surface_2_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/hicolor/64x64/pyspread.ico` & `pyspread-2.2.1/pyspread/share/icons/hicolor/64x64/pyspread.ico`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/hicolor/64x64/pyspread.png` & `pyspread-2.2.1/pyspread/share/icons/hicolor/64x64/pyspread.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/hicolor/svg/pyspread.svg` & `pyspread-2.2.1/pyspread/share/icons/hicolor/svg/pyspread.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/status/status-safe-mode.svg` & `pyspread-2.2.1/pyspread/share/icons/status/status-safe-mode.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/icons/status/status-selection-mode.svg` & `pyspread-2.2.1/pyspread/share/icons/status/status-selection-mode.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/metainfo/io.gitlab.pyspread.pyspread.metainfo.xml` & `pyspread-2.2.1/pyspread/share/metainfo/io.gitlab.pyspread.pyspread.metainfo.xml`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/COPYING` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/COPYING`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_bar_1_3.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_bar_1_3.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_boxplot_2_2.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_boxplot_2_2.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_column_1_1.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_column_1_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_column_1_2.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_column_1_2.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_contour_1_2.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_contour_1_2.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_histogram_1_4.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_histogram_1_4.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_ring_1_1.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_ring_1_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/matplotlib/chart_surface_2_1.py` & `pyspread-2.2.1/pyspread/share/templates/matplotlib/chart_surface_2_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_boxplot_1_2.py` & `pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_boxplot_1_2.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_density2d_1_2.py` & `pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_density2d_1_2.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_point_1_1.py` & `pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_point_1_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/rpy2/chart_r_lattice_wireframe_2_1.py` & `pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_lattice_wireframe_2_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/share/templates/rpy2/chart_r_lattice_xyplot_1_1.py` & `pyspread-2.2.1/pyspread/share/templates/rpy2/chart_r_lattice_xyplot_1_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/test/test_cli.py` & `pyspread-2.2.1/pyspread/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/test/test_grid.py` & `pyspread-2.2.1/pyspread/test/test_grid.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/test/test_grid_renderer.py` & `pyspread-2.2.1/pyspread/test/test_grid_renderer.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/test/test_pyspread.py` & `pyspread-2.2.1/pyspread/test/test_pyspread.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/test/test_workflows.py` & `pyspread-2.2.1/pyspread/test/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/toolbar.py` & `pyspread-2.2.1/pyspread/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 try:
     import matplotlib.figure as matplotlib_figure
 except ImportError:
     matplotlib_figure = None
 
 try:
     import rpy2
-    from rpy2.robjects.packages import importr
+    from rpy2.robjects.packages import importr, PackageNotInstalledError
 except ImportError:
     rpy2 = None
 
 try:
     import plotnine
 except ImportError:
     plotnine = None
@@ -408,18 +408,23 @@
     def is_r_package_installed(package_name):
         """True if the R package is installed
 
         :param package_name: Name of R package to checked
 
         """
 
+        if rpy2 is None:
+            return False
+
         try:
             importr(package_name)
         except RuntimeError:
             return False
+        except PackageNotInstalledError:
+            return False
         return True
 
     def _create_toolbar(self, actions: ChartDialogActions):
         """Fills the chart dialog toolbar with QActions
 
         :param actions: Chart dialog actions
```

### Comparing `pyspread-2.2/pyspread/widgets.py` & `pyspread-2.2.1/pyspread/widgets.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread/workflows.py` & `pyspread-2.2.1/pyspread/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 from ast import literal_eval
 from base64 import b85encode
 import bz2
 from contextlib import contextmanager
 from copy import copy
 import csv
-from itertools import cycle
 import io
 import numpy
 import os.path
 from pathlib import Path
 from shutil import move
 from tempfile import NamedTemporaryFile
 from typing import Iterable, Tuple
@@ -1040,22 +1039,17 @@
         """
 
         grid = self.main_window.focused_grid
         model = grid.model
         selection = grid.selection
 
         description = description_tpl.format(selection)
-
-        for row, column in selection.cell_generator(model.shape):
-            key = row, column, grid.table
-            if not grid.model.code_array.cell_attributes[key]['locked']:
-                # Pop item
-                index = model.index(row, column, QModelIndex())
-                command = commands.SetCellCode(None, model, index, description)
-                self.main_window.undo_stack.push(command)
+        command = commands.DeleteSelectedCellData(grid, model, selection,
+                                                  description)
+        self.main_window.undo_stack.push(command)
 
     def edit_cut(self):
         """Edit -> Cut workflow"""
 
         self.edit_copy()
         self.delete(description_tpl="Cut selection {}")
 
@@ -1202,51 +1196,22 @@
         :param selection: Grid cell selection for pasting
         :param data: Clipboard text
 
         """
 
         grid = self.main_window.focused_grid
         model = grid.model
-        (top, left), (bottom, right) = selection.get_grid_bbox(model.shape)
-        table = grid.table
-        code_array = grid.model.code_array
         undo_stack = self.main_window.undo_stack
 
         description_tpl = "Paste clipboard to {}"
         description = description_tpl.format(selection)
 
-        command = None
-
-        paste_gen = (line.split("\t") for line in data.split("\n"))
-        for row, line in enumerate(cycle(paste_gen)):
-            paste_row = row + top
-            if paste_row > bottom or (paste_row, 0, table) not in code_array:
-                break
-            for column, value in enumerate(cycle(line)):
-                paste_column = column + left
-                paste_key = paste_row, paste_column, table
-                if (paste_key in code_array
-                        and paste_column <= right):
-                    if ((paste_row, paste_column) in selection and not
-                            code_array.cell_attributes[paste_key].locked):
-                        index = model.index(paste_row, paste_column,
-                                            QModelIndex())
-                        # Preserve line breaks
-                        value = value.replace("\u000C", "\n")
-                        cmd = commands.SetCellCode(value, model, index,
-                                                   description)
-                        if command is None:
-                            command = cmd
-                        else:
-                            command.mergeWith(cmd)
-                else:
-                    break
-
-        if command is not None:
-            undo_stack.push(command)
+        cmd = commands.PasteSelectedCellData(grid, model, selection, data,
+                                             description)
+        undo_stack.push(cmd)
 
     def _paste_to_current(self, data: str):
         """Pastes data into grid starting from the current cell
 
         :param data: Clipboard text
 
         """
@@ -1998,15 +1963,15 @@
         selection = grid.selection
         shape = grid.model.shape
 
         (top, left), (bottom, right) = selection.get_grid_bbox(shape)
 
         if bottom >= shape[0] - 1:
             self.main_window.statusBar().showMessage(
-                f"ValueError: Target cell is beyond grid limits")
+                "ValueError: Target cell is beyond grid limits")
             return
 
         key = bottom + 1, right, grid.table
 
         code = f"numpy.sum(eval({repr(selection)}" + \
                f".get_absolute_access_string({shape}, Z)))"
```

### Comparing `pyspread-2.2/pyspread.desktop` & `pyspread-2.2.1/pyspread.desktop`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/pyspread.egg-info/PKG-INFO` & `pyspread-2.2.1/pyspread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspread
-Version: 2.2
+Version: 2.2.1
 Summary: Pyspread is a non-traditional spreadsheet application that is based on and written in the programming language Python.
 Home-page: https://pyspread.gitlab.io
 Author: Martin Manns
 Author-email: mmanns@gmx.net
 License: GPL v3 :: GNU General Public License
 Project-URL: Bug Tracker, https://gitlab.com/pyspread/pyspread/issues
 Project-URL: Documentation, https://pyspread.gitlab.io/docs.html
```

### Comparing `pyspread-2.2/pyspread.egg-info/SOURCES.txt` & `pyspread-2.2.1/pyspread.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspread-2.2/setup.py` & `pyspread-2.2.1/setup.py`

 * *Files identical despite different names*

