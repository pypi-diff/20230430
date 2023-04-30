# Comparing `tmp/cellpy-0.4.3a2.tar.gz` & `tmp/cellpy-0.4.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-0.4.3a2.tar", last modified: Sat Feb 18 18:41:17 2023, max compression
+gzip compressed data, was "cellpy-0.4.3a3.tar", last modified: Fri Mar 10 08:46:43 2023, max compression
```

## Comparing `cellpy-0.4.3a2.tar` & `cellpy-0.4.3a3.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.562717 cellpy-0.4.3a2/
--rw-rw-rw-   0        0        0      456 2022-06-03 19:47:44.000000 cellpy-0.4.3a2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3086 2022-09-20 08:21:07.000000 cellpy-0.4.3a2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     3139 2023-02-18 18:40:50.000000 cellpy-0.4.3a2/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/LICENSE
--rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-0.4.3a2/MANIFEST.in
--rw-rw-rw-   0        0        0     5437 2023-02-18 18:41:17.561717 cellpy-0.4.3a2/PKG-INFO
--rw-rw-rw-   0        0        0     1573 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:16.994721 cellpy-0.4.3a2/cellpy/
--rw-rw-rw-   0        0        0      874 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/__init__.py
--rw-rw-rw-   0        0        0       25 2023-02-18 18:41:07.000000 cellpy-0.4.3a2/cellpy/_version.py
--rw-rw-rw-   0        0        0    49054 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/cli.py
--rw-rw-rw-   0        0        0     1192 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/exceptions.py
--rw-rw-rw-   0        0        0     4699 2022-10-27 14:47:16.000000 cellpy-0.4.3a2/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.033713 cellpy-0.4.3a2/cellpy/parameters/
--rw-rw-rw-   0        0        0     3144 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        4 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    13754 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/parameters/internal_settings.py
--rw-rw-rw-   0        0        0    12042 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/parameters/internal_settings_old.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.040720 cellpy-0.4.3a2/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0     8784 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/parameters/legacy/internal_settings.py
--rw-rw-rw-   0        0        0     9455 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0     9373 2023-02-18 18:40:50.000000 cellpy-0.4.3a2/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.065721 cellpy-0.4.3a2/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   223023 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    29817 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    22382 2022-06-29 14:40:38.000000 cellpy-0.4.3a2/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0     8120 2022-06-03 19:58:41.000000 cellpy-0.4.3a2/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.135721 cellpy-0.4.3a2/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    58172 2023-02-18 18:40:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    19484 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    11188 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     9930 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    46783 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/backup_arbin.py
--rw-rw-rw-   0        0        0    25239 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    23336 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.169716 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     1699 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_four.py
--rw-rw-rw-   0        0        0     4083 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     1989 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1787 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3548 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2323 2023-02-18 18:40:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/neware_txt_one.py
--rw-rw-rw-   0        0        0     2256 2023-02-18 18:40:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10316 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/custom.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.186713 cellpy-0.4.3a2/cellpy/readers/instruments/delete_these_in_february2022/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/delete_these_in_february2022/__init__.py
--rw-rw-rw-   0        0        0     4073 2022-05-27 12:07:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/delete_these_in_february2022/_testing_txt.py
--rw-rw-rw-   0        0        0    27458 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/delete_these_in_february2022/maccor_txt_old.py
--rw-rw-rw-   0        0        0     4177 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.192720 cellpy-0.4.3a2/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-0.4.3a2/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-0.4.3a2/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1056 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    12876 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3520 2023-02-18 18:40:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    20433 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/old_custom.py
--rw-rw-rw-   0        0        0    16728 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.200720 cellpy-0.4.3a2/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    15146 2023-02-18 18:40:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1449 2022-05-27 12:07:50.000000 cellpy-0.4.3a2/cellpy/readers/instruments/processors/pre_processors.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.259720 cellpy-0.4.3a2/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    45082 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.316777 cellpy-0.4.3a2/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7196 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    18126 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    24951 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2925 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    13847 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    23947 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    27767 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0     8794 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/batch_tools/engines.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.320720 cellpy-0.4.3a2/cellpy/utils/data/
--rw-rw-rw-   0        0        0  3145889 2023-02-18 18:32:42.000000 cellpy-0.4.3a2/cellpy/utils/data/20160805_test001_45_cc.h5
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.328713 cellpy-0.4.3a2/cellpy/utils/data/raw/
--rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-0.4.3a2/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-0.4.3a2/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    79018 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     1441 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    38187 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    37632 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-0.4.3a2/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    24083 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    43176 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/cellpy/utils/plotutils.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.007721 cellpy-0.4.3a2/cellpy.egg-info/
--rw-rw-rw-   0        0        0     5437 2023-02-18 18:41:16.000000 cellpy-0.4.3a2/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5124 2023-02-18 18:41:16.000000 cellpy-0.4.3a2/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 18:41:16.000000 cellpy-0.4.3a2/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-02-18 18:41:16.000000 cellpy-0.4.3a2/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-18 18:41:16.000000 cellpy-0.4.3a2/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      259 2023-02-18 18:41:16.000000 cellpy-0.4.3a2/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-18 18:41:16.000000 cellpy-0.4.3a2/cellpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.417715 cellpy-0.4.3a2/docs/
--rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-0.4.3a2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:16.940714 cellpy-0.4.3a2/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:16.940714 cellpy-0.4.3a2/docs/_build/.doctrees/
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.424721 cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    15014 2023-01-20 10:44:21.000000 cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-01-20 10:44:21.000000 cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-01-20 10:44:21.000000 cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    14101 2023-01-15 18:57:55.000000 cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_simple_plot_2_0.png
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.435726 cellpy-0.4.3a2/docs/_build/_images/
--rw-rw-rw-   0        0        0    15014 2023-01-15 18:57:51.000000 cellpy-0.4.3a2/docs/_build/_images/notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-01-15 18:57:51.000000 cellpy-0.4.3a2/docs/_build/_images/notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-01-15 18:57:51.000000 cellpy-0.4.3a2/docs/_build/_images/notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    14101 2023-01-15 18:57:55.000000 cellpy-0.4.3a2/docs/_build/_images/notebooks_tutorial_simple_plot_2_0.png
--rw-rw-rw-   0        0        0    88743 2023-01-18 20:40:28.000000 cellpy-0.4.3a2/docs/_build/_images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/_build/_images/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/_build/_images/tutorials_utils_plotting_fig2.png
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.439713 cellpy-0.4.3a2/docs/_build/_static/
--rw-rw-rw-   0        0        0      286 2021-01-01 06:53:29.000000 cellpy-0.4.3a2/docs/_build/_static/file.png
--rw-rw-rw-   0        0        0       90 2021-01-01 06:53:29.000000 cellpy-0.4.3a2/docs/_build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2021-01-01 06:53:29.000000 cellpy-0.4.3a2/docs/_build/_static/plus.png
--rw-rw-rw-   0        0        0       29 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/authors.rst
--rw-rw-rw-   0        0        0      301 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/basics.rst
--rw-rw-rw-   0        0        0    10477 2023-01-20 10:22:12.000000 cellpy-0.4.3a2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/contributing.rst
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.454720 cellpy-0.4.3a2/docs/developers/
--rw-rw-rw-   0        0        0      821 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/developers/dev_cellpy_data_structure.rst
--rw-rw-rw-   0        0        0     5507 2022-11-17 18:21:31.000000 cellpy-0.4.3a2/docs/developers/dev_cellpy_folder_structure.rst
--rw-rw-rw-   0        0        0     1395 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/developers/dev_various.rst
--rw-rw-rw-   0        0        0      153 2022-06-03 19:47:44.000000 cellpy-0.4.3a2/docs/developers_guide.rst
--rw-rw-rw-   0        0        0      202 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/examples.rst
--rw-rw-rw-   0        0        0    15953 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/formats.rst
--rw-rw-rw-   0        0        0       29 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/history.rst
--rw-rw-rw-   0        0        0      826 2022-06-03 19:47:44.000000 cellpy-0.4.3a2/docs/index.rst
--rw-rw-rw-   0        0        0     4260 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/installation.rst
--rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-0.4.3a2/docs/make.bat
--rw-rw-rw-   0        0        0      174 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/notebooks.rst
--rw-rw-rw-   0        0        0       28 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/readme.rst
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.485720 cellpy-0.4.3a2/docs/source/
--rw-rw-rw-   0        0        0      769 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/source/cellpy.parameters.rst
--rw-rw-rw-   0        0        0     2112 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/source/cellpy.readers.instruments.rst
--rw-rw-rw-   0        0        0      960 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/source/cellpy.readers.rst
--rw-rw-rw-   0        0        0      698 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/source/cellpy.rst
--rw-rw-rw-   0        0        0     2405 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/source/cellpy.utils.batch_tools.rst
--rw-rw-rw-   0        0        0     1824 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/source/cellpy.utils.rst
--rw-rw-rw-   0        0        0       62 2021-12-21 09:11:59.000000 cellpy-0.4.3a2/docs/source/modules.rst
--rw-rw-rw-   0        0        0     1797 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/tips_and_tricks.rst
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.521722 cellpy-0.4.3a2/docs/tutorials/
--rw-rw-rw-   0        0        0     8436 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/tutorials/basic_interaction.rst
--rw-rw-rw-   0        0        0     5898 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/tutorials/configuring.rst
--rw-rw-rw-   0        0        0      981 2022-05-27 12:03:59.000000 cellpy-0.4.3a2/docs/tutorials/data_mining.rst
--rw-rw-rw-   0        0        0    12903 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/tutorials/getting_started_tutorial.rst
--rw-rw-rw-   0        0        0     1222 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/tutorials/pandas.rst
--rw-rw-rw-   0        0        0     1782 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/tutorials/the_cellpy_cmd.rst
--rw-rw-rw-   0        0        0     3444 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.556717 cellpy-0.4.3a2/docs/utils/
--rw-rw-rw-   0        0        0     4368 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/utils/batch.rst
--rw-rw-rw-   0        0        0       87 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/utils/custom_file_loader.rst
--rw-rw-rw-   0        0        0       29 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/utils/easyplot.rst
-drwxrwxrwx   0        0        0        0 2023-02-18 18:41:17.559716 cellpy-0.4.3a2/docs/utils/figures/
--rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/utils/figures/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/utils/figures/tutorials_utils_plotting_fig2.png
--rw-rw-rw-   0        0        0     1080 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/utils/ica.rst
--rw-rw-rw-   0        0        0     1919 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/docs/utils/plotting.rst
--rw-rw-rw-   0        0        0       31 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/utils/templates.rst
--rw-rw-rw-   0        0        0     1186 2022-09-20 08:21:07.000000 cellpy-0.4.3a2/docs/utils/tut_ocv_rlx.rst
--rw-rw-rw-   0        0        0      327 2022-05-27 12:07:51.000000 cellpy-0.4.3a2/docs/utils.rst
--rw-rw-rw-   0        0        0      263 2022-06-03 19:47:44.000000 cellpy-0.4.3a2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-18 18:41:17.562717 cellpy-0.4.3a2/setup.cfg
--rw-rw-rw-   0        0        0     3125 2023-02-18 18:25:18.000000 cellpy-0.4.3a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.517863 cellpy-0.4.3a3/
+-rw-rw-rw-   0        0        0      456 2022-06-03 19:47:44.000000 cellpy-0.4.3a3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3086 2022-09-20 08:21:07.000000 cellpy-0.4.3a3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     3139 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/LICENSE
+-rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-0.4.3a3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5437 2023-03-10 08:46:43.517863 cellpy-0.4.3a3/PKG-INFO
+-rw-rw-rw-   0        0        0     1573 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/README.rst
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.543048 cellpy-0.4.3a3/cellpy/
+-rw-rw-rw-   0        0        0      874 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-03-10 08:46:26.000000 cellpy-0.4.3a3/cellpy/_version.py
+-rw-rw-rw-   0        0        0    48016 2023-03-09 12:36:14.000000 cellpy-0.4.3a3/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1192 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/exceptions.py
+-rw-rw-rw-   0        0        0     4840 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.594049 cellpy-0.4.3a3/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3144 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        4 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    13754 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/parameters/internal_settings.py
+-rw-rw-rw-   0        0        0    12042 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/parameters/internal_settings_old.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.598049 cellpy-0.4.3a3/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0     8784 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/parameters/legacy/internal_settings.py
+-rw-rw-rw-   0        0        0     9455 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0     9373 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.607670 cellpy-0.4.3a3/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   223023 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    29817 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    22382 2022-06-29 14:40:38.000000 cellpy-0.4.3a3/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0     8120 2022-06-03 19:58:41.000000 cellpy-0.4.3a3/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.779173 cellpy-0.4.3a3/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    58172 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    19484 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    11188 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     9930 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    46783 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/backup_arbin.py
+-rw-rw-rw-   0        0        0    25239 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    23336 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.854194 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1699 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_four.py
+-rw-rw-rw-   0        0        0     4083 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     1989 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1787 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3548 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2323 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/neware_txt_one.py
+-rw-rw-rw-   0        0        0     2256 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10316 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/custom.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.881860 cellpy-0.4.3a3/cellpy/readers/instruments/delete_these_in_february2022/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-0.4.3a3/cellpy/readers/instruments/delete_these_in_february2022/__init__.py
+-rw-rw-rw-   0        0        0     4073 2022-05-27 12:07:50.000000 cellpy-0.4.3a3/cellpy/readers/instruments/delete_these_in_february2022/_testing_txt.py
+-rw-rw-rw-   0        0        0    27458 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/delete_these_in_february2022/maccor_txt_old.py
+-rw-rw-rw-   0        0        0     4177 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.894944 cellpy-0.4.3a3/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-0.4.3a3/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-0.4.3a3/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1056 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    12876 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3520 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    20433 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/old_custom.py
+-rw-rw-rw-   0        0        0    16728 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.968943 cellpy-0.4.3a3/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-0.4.3a3/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    15146 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1449 2022-05-27 12:07:50.000000 cellpy-0.4.3a3/cellpy/readers/instruments/processors/pre_processors.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.063951 cellpy-0.4.3a3/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    45082 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.085945 cellpy-0.4.3a3/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7383 2023-03-09 15:37:57.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    18126 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    24951 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2925 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    13847 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    23947 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    27767 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0     8794 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/batch_tools/engines.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.096948 cellpy-0.4.3a3/cellpy/utils/data/
+-rw-rw-rw-   0        0        0  3145889 2023-03-10 08:01:50.000000 cellpy-0.4.3a3/cellpy/utils/data/20160805_test001_45_cc.h5
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.114947 cellpy-0.4.3a3/cellpy/utils/data/raw/
+-rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-0.4.3a3/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-0.4.3a3/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    79018 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     1441 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    38187 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    37632 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-0.4.3a3/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    23184 2023-03-10 07:49:23.000000 cellpy-0.4.3a3/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    43176 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/cellpy/utils/plotutils.py
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.569048 cellpy-0.4.3a3/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     5437 2023-03-10 08:46:42.000000 cellpy-0.4.3a3/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5124 2023-03-10 08:46:42.000000 cellpy-0.4.3a3/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-10 08:46:42.000000 cellpy-0.4.3a3/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-03-10 08:46:42.000000 cellpy-0.4.3a3/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-10 08:46:41.000000 cellpy-0.4.3a3/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      259 2023-03-10 08:46:42.000000 cellpy-0.4.3a3/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-03-10 08:46:42.000000 cellpy-0.4.3a3/cellpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.273010 cellpy-0.4.3a3/docs/
+-rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-0.4.3a3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.483049 cellpy-0.4.3a3/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:42.482049 cellpy-0.4.3a3/docs/_build/.doctrees/
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.285003 cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    15014 2023-01-20 10:44:21.000000 cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-01-20 10:44:21.000000 cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-01-20 10:44:21.000000 cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    14101 2023-01-15 18:57:55.000000 cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_simple_plot_2_0.png
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.305004 cellpy-0.4.3a3/docs/_build/_images/
+-rw-rw-rw-   0        0        0    15014 2023-01-15 18:57:51.000000 cellpy-0.4.3a3/docs/_build/_images/notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-01-15 18:57:51.000000 cellpy-0.4.3a3/docs/_build/_images/notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-01-15 18:57:51.000000 cellpy-0.4.3a3/docs/_build/_images/notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    14101 2023-01-15 18:57:55.000000 cellpy-0.4.3a3/docs/_build/_images/notebooks_tutorial_simple_plot_2_0.png
+-rw-rw-rw-   0        0        0    88743 2023-01-18 20:40:28.000000 cellpy-0.4.3a3/docs/_build/_images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/_build/_images/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/_build/_images/tutorials_utils_plotting_fig2.png
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.312011 cellpy-0.4.3a3/docs/_build/_static/
+-rw-rw-rw-   0        0        0      286 2021-01-01 06:53:29.000000 cellpy-0.4.3a3/docs/_build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2021-01-01 06:53:29.000000 cellpy-0.4.3a3/docs/_build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2021-01-01 06:53:29.000000 cellpy-0.4.3a3/docs/_build/_static/plus.png
+-rw-rw-rw-   0        0        0       29 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/authors.rst
+-rw-rw-rw-   0        0        0      301 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/basics.rst
+-rw-rw-rw-   0        0        0    10477 2023-01-20 10:22:12.000000 cellpy-0.4.3a3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/contributing.rst
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.341004 cellpy-0.4.3a3/docs/developers/
+-rw-rw-rw-   0        0        0      821 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/developers/dev_cellpy_data_structure.rst
+-rw-rw-rw-   0        0        0     5507 2022-11-17 18:21:31.000000 cellpy-0.4.3a3/docs/developers/dev_cellpy_folder_structure.rst
+-rw-rw-rw-   0        0        0     1395 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/developers/dev_various.rst
+-rw-rw-rw-   0        0        0      153 2022-06-03 19:47:44.000000 cellpy-0.4.3a3/docs/developers_guide.rst
+-rw-rw-rw-   0        0        0      202 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/examples.rst
+-rw-rw-rw-   0        0        0    15953 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/formats.rst
+-rw-rw-rw-   0        0        0       29 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/history.rst
+-rw-rw-rw-   0        0        0      826 2022-06-03 19:47:44.000000 cellpy-0.4.3a3/docs/index.rst
+-rw-rw-rw-   0        0        0     4260 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/installation.rst
+-rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-0.4.3a3/docs/make.bat
+-rw-rw-rw-   0        0        0      174 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/notebooks.rst
+-rw-rw-rw-   0        0        0       28 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/readme.rst
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.398863 cellpy-0.4.3a3/docs/source/
+-rw-rw-rw-   0        0        0      769 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/source/cellpy.parameters.rst
+-rw-rw-rw-   0        0        0     2112 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/source/cellpy.readers.instruments.rst
+-rw-rw-rw-   0        0        0      960 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/source/cellpy.readers.rst
+-rw-rw-rw-   0        0        0      698 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/source/cellpy.rst
+-rw-rw-rw-   0        0        0     2405 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/source/cellpy.utils.batch_tools.rst
+-rw-rw-rw-   0        0        0     1824 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/source/cellpy.utils.rst
+-rw-rw-rw-   0        0        0       62 2021-12-21 09:11:59.000000 cellpy-0.4.3a3/docs/source/modules.rst
+-rw-rw-rw-   0        0        0     1797 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/tips_and_tricks.rst
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.451869 cellpy-0.4.3a3/docs/tutorials/
+-rw-rw-rw-   0        0        0     8436 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/tutorials/basic_interaction.rst
+-rw-rw-rw-   0        0        0     5898 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/tutorials/configuring.rst
+-rw-rw-rw-   0        0        0      981 2022-05-27 12:03:59.000000 cellpy-0.4.3a3/docs/tutorials/data_mining.rst
+-rw-rw-rw-   0        0        0    12903 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/tutorials/getting_started_tutorial.rst
+-rw-rw-rw-   0        0        0     1222 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/tutorials/pandas.rst
+-rw-rw-rw-   0        0        0     1782 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/tutorials/the_cellpy_cmd.rst
+-rw-rw-rw-   0        0        0     3444 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.509867 cellpy-0.4.3a3/docs/utils/
+-rw-rw-rw-   0        0        0     4368 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/utils/batch.rst
+-rw-rw-rw-   0        0        0       87 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/utils/custom_file_loader.rst
+-rw-rw-rw-   0        0        0       29 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/utils/easyplot.rst
+drwxrwxrwx   0        0        0        0 2023-03-10 08:46:43.514862 cellpy-0.4.3a3/docs/utils/figures/
+-rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/utils/figures/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/utils/figures/tutorials_utils_plotting_fig2.png
+-rw-rw-rw-   0        0        0     1080 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/utils/ica.rst
+-rw-rw-rw-   0        0        0     1919 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/docs/utils/plotting.rst
+-rw-rw-rw-   0        0        0       31 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/utils/templates.rst
+-rw-rw-rw-   0        0        0     1186 2022-09-20 08:21:07.000000 cellpy-0.4.3a3/docs/utils/tut_ocv_rlx.rst
+-rw-rw-rw-   0        0        0      327 2022-05-27 12:07:51.000000 cellpy-0.4.3a3/docs/utils.rst
+-rw-rw-rw-   0        0        0      263 2022-06-03 19:47:44.000000 cellpy-0.4.3a3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-10 08:46:43.518862 cellpy-0.4.3a3/setup.cfg
+-rw-rw-rw-   0        0        0     3132 2023-03-09 10:27:42.000000 cellpy-0.4.3a3/setup.py
```

### Comparing `cellpy-0.4.3a2/CONTRIBUTING.rst` & `cellpy-0.4.3a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/HISTORY.rst` & `cellpy-0.4.3a3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/LICENSE` & `cellpy-0.4.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/MANIFEST.in` & `cellpy-0.4.3a3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/PKG-INFO` & `cellpy-0.4.3a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 0.4.3a2
+Version: 0.4.3a3
 Summary: Extract and manipulate data from battery cell testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cellpy-0.4.3a2/README.rst` & `cellpy-0.4.3a3/README.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/__init__.py` & `cellpy-0.4.3a3/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/exceptions.py` & `cellpy-0.4.3a3/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/log.py` & `cellpy-0.4.3a3/cellpy/log.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-"""Set up logger instance"""
-
-import datetime
-import json
-import logging
-import logging.config
-import os
-import pathlib
-import shutil
-import tempfile
-import warnings
-
-from cellpy import prms
-
-logging.raiseExceptions = False
-
-
-def setup_logging(
-    default_json_path=None,
-    default_level=None,
-    env_key="LOG_CFG",
-    custom_log_dir=None,
-    reset_big_log=False,
-    max_size=5_000_000,
-    testing=False,
-):
-    """Setup logging configuration.
-
-    Args:
-        default_level: default log-level to screen (std.out).
-        default_json_path: path to config file for setting up logging.
-        env_key (str): use this environment prm to try to get default_json_path.
-        custom_log_dir: path for saving logs.
-        reset_big_log (bool): reset log if too big (max_size).
-        max_size (int): if reset_log, this is the max limit.
-        testing (bool): set as True if testing, and you don't want to create any .log files
-
-    """
-
-    if not default_json_path:
-        default_json_path = os.path.join(
-            os.path.dirname(os.path.realpath(__file__)), "logging.json"
-        )
-    path = default_json_path
-    value = os.getenv(env_key, None)
-    if value:
-        path = value
-
-    if default_level is None:
-        default_level = "CRITICAL"
-
-    # loading logging configs
-    if os.path.exists(path):
-        with open(path, "rt") as f:
-            config = json.load(f)
-
-        if testing:
-            log_dir = tempfile.mkdtemp()
-        elif custom_log_dir:
-            log_dir = custom_log_dir
-        else:
-            log_dir = os.path.abspath(prms.Paths.filelogdir)
-
-        if not os.path.isdir(log_dir):
-            warning_txt = (
-                "\nCould not set custom log-dir - "
-                "non-existing directory"
-                f"\nDir: {log_dir}"
-                "\nUsing current directory instead: "
-                f"{os.getcwd()}"
-            )
-            logging.warning(warning_txt)
-            log_dir = os.getcwd()
-
-        for file_handler in [
-            "error_file_handler",
-            "info_file_handler",
-            "debug_file_handler",
-        ]:
-            try:
-                file_name = config["handlers"][file_handler]["filename"]
-                logging.debug("Setting file handlers for logging.")
-                logging.debug(f"Filename: {file_name}")
-                logging.debug(f"Full path: {os.path.join(log_dir,file_name)}")
-                # print(f"Filename: {file_name}")
-                # print(f"Full path: {os.path.join(log_dir,file_name)}")
-                config["handlers"][file_handler]["filename"] = os.path.join(
-                    log_dir, file_name
-                )
-
-                if reset_big_log:
-                    full_log_file_path = pathlib.Path(log_dir) / file_name
-                    if full_log_file_path.is_file():
-                        file_size = full_log_file_path.lstat().st_size
-                        if file_size > max_size:
-                            d_str = datetime.datetime.now().strftime("%Y_%m_%d_%H_%M")
-                            new_file_name = "_".join([d_str, file_name])
-                            new_full_log_file_path = (
-                                pathlib.Path(log_dir) / new_file_name
-                            )
-                            shutil.copy(full_log_file_path, new_full_log_file_path)
-                    else:
-                        logging.debug(
-                            "Could not reset big log: could not find the file"
-                        )
-
-            except Exception as e:
-                warnings.warn("\nCould not set custom log-dir" + str(e))
-
-        if default_level:
-            w_txt = "\nCould not set custom default level for logger"
-            if default_level not in [
-                "INFO",
-                "DEBUG",
-                "CRITICAL",
-                logging.INFO,
-                logging.DEBUG,
-                logging.CRITICAL,
-            ]:
-                _txt = "\nonly 'INFO', 'DEBUG' and 'CRITICAL' is supported"
-                _txt += " as default_level"
-                warnings.warn(w_txt + _txt)
-
-            else:
-                try:
-                    config["handlers"]["console"]["level"] = default_level
-                    if default_level in ["DEBUG", logging.DEBUG]:
-                        config["handlers"]["console"]["formatter"] = "stamped"
-
-                except Exception as e:
-                    warnings.warn(w_txt + "\n" + str(e))
-
-        logging.config.dictConfig(config)
-    else:
-        if not default_level:
-            default_level = logging.CRITICAL
-        logging.basicConfig(level=default_level)
-
-
-if __name__ == "__main__":
-    setup_logging()
+"""Set up logger instance"""
+
+import datetime
+import json
+import logging
+import logging.config
+import os
+import pathlib
+import shutil
+import tempfile
+import warnings
+
+from cellpy import prms
+
+logging.raiseExceptions = False
+
+
+def setup_logging(
+    default_json_path=None,
+    default_level=None,
+    env_key="LOG_CFG",
+    custom_log_dir=None,
+    reset_big_log=False,
+    max_size=5_000_000,
+    testing=False,
+):
+    """Setup logging configuration.
+
+    Args:
+        default_level: default log-level to screen (std.out).
+        default_json_path: path to config file for setting up logging.
+        env_key (str): use this environment prm to try to get default_json_path.
+        custom_log_dir: path for saving logs.
+        reset_big_log (bool): reset log if too big (max_size).
+        max_size (int): if reset_log, this is the max limit.
+        testing (bool): set as True if testing, and you don't want to create any .log files
+
+    """
+
+    if not default_json_path:
+        default_json_path = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "logging.json"
+        )
+    path = default_json_path
+    value = os.getenv(env_key, None)
+    if value:
+        path = value
+
+    if default_level is None:
+        default_level = "CRITICAL"
+
+    # loading logging configs
+    if os.path.exists(path):
+        with open(path, "rt") as f:
+            config = json.load(f)
+
+        if testing:
+            log_dir = tempfile.mkdtemp()
+        elif custom_log_dir:
+            log_dir = custom_log_dir
+        else:
+            log_dir = os.path.abspath(prms.Paths.filelogdir)
+
+        if not os.path.isdir(log_dir):
+            warning_txt = (
+                "\nCould not set custom log-dir - "
+                "non-existing directory"
+                f"\nDir: {log_dir}"
+                "\nUsing current directory instead: "
+                f"{os.getcwd()}"
+            )
+            logging.warning(warning_txt)
+            log_dir = os.getcwd()
+
+        for file_handler in [
+            "error_file_handler",
+            "info_file_handler",
+            "debug_file_handler",
+        ]:
+            try:
+                file_name = config["handlers"][file_handler]["filename"]
+                logging.debug("Setting file handlers for logging.")
+                logging.debug(f"Filename: {file_name}")
+                logging.debug(f"Full path: {os.path.join(log_dir,file_name)}")
+                # print(f"Filename: {file_name}")
+                # print(f"Full path: {os.path.join(log_dir,file_name)}")
+                config["handlers"][file_handler]["filename"] = os.path.join(
+                    log_dir, file_name
+                )
+
+                if reset_big_log:
+                    full_log_file_path = pathlib.Path(log_dir) / file_name
+                    if full_log_file_path.is_file():
+                        file_size = full_log_file_path.lstat().st_size
+                        if file_size > max_size:
+                            d_str = datetime.datetime.now().strftime("%Y_%m_%d_%H_%M")
+                            new_file_name = "_".join([d_str, file_name])
+                            new_full_log_file_path = (
+                                pathlib.Path(log_dir) / new_file_name
+                            )
+                            shutil.copy(full_log_file_path, new_full_log_file_path)
+                    else:
+                        logging.debug(
+                            "Could not reset big log: could not find the file"
+                        )
+
+            except Exception as e:
+                warnings.warn("\nCould not set custom log-dir" + str(e))
+
+        if default_level:
+            w_txt = "\nCould not set custom default level for logger"
+            if default_level not in [
+                "INFO",
+                "DEBUG",
+                "CRITICAL",
+                logging.INFO,
+                logging.DEBUG,
+                logging.CRITICAL,
+            ]:
+                _txt = "\nonly 'INFO', 'DEBUG' and 'CRITICAL' is supported"
+                _txt += " as default_level"
+                warnings.warn(w_txt + _txt)
+
+            else:
+                try:
+                    config["handlers"]["console"]["level"] = default_level
+                    if default_level in ["DEBUG", logging.DEBUG]:
+                        config["handlers"]["console"]["formatter"] = "stamped"
+
+                except Exception as e:
+                    warnings.warn(w_txt + "\n" + str(e))
+
+        logging.config.dictConfig(config)
+    else:
+        if not default_level:
+            default_level = logging.CRITICAL
+        logging.basicConfig(level=default_level)
+
+
+if __name__ == "__main__":
+    setup_logging()
```

### Comparing `cellpy-0.4.3a2/cellpy/logging.json` & `cellpy-0.4.3a3/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/parameters/.cellpy_prms_default.conf` & `cellpy-0.4.3a3/cellpy/parameters/.cellpy_prms_default.conf`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/parameters/internal_settings.py` & `cellpy-0.4.3a3/cellpy/parameters/internal_settings.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/parameters/internal_settings_old.py` & `cellpy-0.4.3a3/cellpy/parameters/internal_settings_old.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/parameters/legacy/internal_settings.py` & `cellpy-0.4.3a3/cellpy/parameters/legacy/internal_settings.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/parameters/prmreader.py` & `cellpy-0.4.3a3/cellpy/parameters/prmreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/parameters/prms.py` & `cellpy-0.4.3a3/cellpy/parameters/prms.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/cellreader.py` & `cellpy-0.4.3a3/cellpy/readers/cellreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/core.py` & `cellpy-0.4.3a3/cellpy/readers/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/dbreader.py` & `cellpy-0.4.3a3/cellpy/readers/dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/filefinder.py` & `cellpy-0.4.3a3/cellpy/readers/filefinder.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/arbin_res.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/arbin_sql.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/backup_arbin.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/backup_arbin.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/base.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/base.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/biologics_mpr.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_four.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_four.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_two.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/configurations/neware_txt_one.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/configurations/neware_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/custom.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/custom.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/delete_these_in_february2022/_testing_txt.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/delete_these_in_february2022/_testing_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/delete_these_in_february2022/maccor_txt_old.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/delete_these_in_february2022/maccor_txt_old.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/local_instrument.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/local_instrument.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/maccor_txt.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/maccor_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/neware_txt.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/neware_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/old_custom.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/old_custom.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/pec_csv.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/pec_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/processors/post_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-0.4.3a3/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch.py` & `cellpy-0.4.3a3/cellpy/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,187 +1,197 @@
-import logging
-
-import pandas as pd
-
-from cellpy.exceptions import UnderDefined
-from cellpy.utils.batch_tools.batch_core import BaseAnalyzer
-from cellpy.utils.batch_tools.dumpers import ram_dumper
-from cellpy.utils.batch_tools.engines import summary_engine
-from cellpy.utils.ocv_rlx import select_ocv_points
-
-
-class BaseSummaryAnalyzer(BaseAnalyzer):
-    def __init__(self):
-        super().__init__()
-        self._assign_engine(summary_engine)
-        self._assign_dumper(ram_dumper)
-
-
-class ICAAnalyzer(BaseAnalyzer):
-    def __init__(self):
-        super().__init__()
-
-
-class EISAnalyzer(BaseAnalyzer):
-    def __init__(self):
-        super().__init__()
-
-
-class OCVRelaxationAnalyzer(BaseAnalyzer):
-    """Analyze open curcuit relaxation curves.
-
-    This analyzer is still under development.
-    (Partly) implented so far: select_ocv_points -> farms.
-    To get the DataFrames from the farms, you can use
-    >>> ocv_point_frames = OCVRelaxationAnalyzer.last
-
-    Attributes:
-        selection_method: criteria for selecting points
-            (martin: select first and last, and then last/2, last/2/2 etc. until you have reached the wanted number of points; fixed_time: select first, and same interval; defaults to "martin")
-        number_of_points: number of points you want.
-            defaults to 5
-        interval: interval between each point (in use only for methods
-            where interval makes sense). If it is a list, then
-            number_of_points will be calculated as len(interval) + 1 (and
-            override the set number_of_points).
-            defaults to 10
-        relative_voltage: set to True if you would like the voltage to be
-            relative to the voltage before starting the ocv rlx step.
-            Defaults to False. Remark that for the initial rxl step (when
-            you just have put your cell on the tester) does not have any
-            prior voltage. The relative voltage will then be versus the
-            first measurement point.
-            defaults to False
-        report_times: also report the ocv rlx total time if True (defaults
-            to False)
-        direction ("up", "down" or "both"): select "up" if you would like
-            to process only the ocv rlx steps where the voltage is relaxing
-            upwards and vize versa. Defaults to "both
-
-    Notes:
-        This analyzer is not working as intended yet. Todos:
-
-        - include better engine-dumper methodology and dump
-          stuff to both memory and file(s)
-          (should add this to BaseAnalyser)
-        - recieve settings and parameters
-        - option (dumper) for plotting?
-        - automatic fitting of OCV rlx data?
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.engines = []
-        self.dumpers = []
-        self.current_engine = None
-        self._assign_engine(self.ocv_points_engine)
-        # self._assign_dumper(self.screen_dumper)
-        # prms for select_ocv_points
-        self.selection_method = "martin"
-        self.number_of_points = 5
-        self.interval = 10
-        self.relative_voltage = False
-        self.report_times = False
-        self.direction = None
-
-    def _assign_engine(self, engine):
-        self.engines.append(engine)
-
-    def _assign_dumper(self, dumper):
-        self.dumpers.append(dumper)
-
-    def screen_dumper(self, **kwargs):
-        for farm in self.farms:
-            print(farm)
-
-    @property
-    def last(self):
-        return self.farms[-1]
-
-    def run_engine(self, engine):
-        logging.debug(f"start engine::{engine.__name__}]")
-
-        self.current_engine = engine
-
-        self.farms, self.barn = engine(experiments=self.experiments, farms=self.farms)
-        logging.debug("::engine ended")
-
-    def run_dumper(self, dumper):
-        logging.debug(f"start dumper::{dumper.__name__}]")
-        dumper(
-            experiments=self.experiments,
-            farms=self.farms,
-            barn=self.barn,
-            engine=self.current_engine,
-        )
-        logging.debug("::dumper ended")
-
-    def do(self):
-        if not self.experiments:
-            raise UnderDefined("cannot run until you have assigned an experiment")
-
-        for engine in self.engines:
-            self.empty_the_farms()
-            logging.debug(f"running - {str(engine)}")
-            self.run_engine(engine)
-
-            for dumper in self.dumpers:
-                logging.debug(f"exporting - {str(dumper)}")
-                self.run_dumper(dumper)
-
-    def ocv_points_engine(self, **kwargs):
-        experiments = kwargs["experiments"]
-        farms = kwargs["farms"]
-        barn = None
-        for experiment, farm in zip(experiments, farms):
-            for cell_label in experiment.cell_data_frames:
-                logging.info(f"Analyzing {cell_label}")
-                if experiment.all_in_memory:
-                    logging.debug("CellpyData picked from memory")
-                    cell = experiment.cell_data_frames[cell_label]
-                    if cell.empty:
-                        logging.warning("Oh-no! Empty CellpyData-object")
-                else:
-                    logging.debug("CellpyData loaded from Cellpy-file")
-                    cell = experiment.data[cell_label]
-                    if cell.empty:
-                        logging.warning("Oh-no! Empty CellpyData-object")
-
-                df = select_ocv_points(
-                    cell,
-                    selection_method=self.selection_method,
-                    number_of_points=self.number_of_points,
-                    interval=self.interval,
-                    relative_voltage=self.relative_voltage,
-                    report_times=self.report_times,
-                    direction=self.direction,
-                )
-                farm.append(df)
-
-        return farms, barn
-
-    def do2(self):
-        for experiment, farm in zip(self.experiments, self.farms):
-            for cell_label in experiment.cell_data_frames:
-                logging.info(f"Analyzing {cell_label}")
-                if experiment.all_in_memory:
-                    logging.debug("CellpyData picked from memory")
-                    cell = experiment.cell_data_frames[cell_label]
-                    if cell.empty:
-                        logging.warning("Oh-no! Empty CellpyData-object")
-                else:
-                    logging.debug("CellpyData loaded from Cellpy-file")
-                    cell = experiment.data[cell_label]
-                    if cell.empty:
-                        logging.warning("Oh-no! Empty CellpyData-object")
-
-                df = select_ocv_points(
-                    cell,
-                    selection_method=self.selection_method,
-                    number_of_points=self.number_of_points,
-                    interval=self.interval,
-                    relative_voltage=self.relative_voltage,
-                    report_times=self.report_times,
-                    direction=self.direction,
-                )
-                farm.append(df)
-        return self.farms
+import logging
+
+import pandas as pd
+
+from cellpy.exceptions import UnderDefined
+from cellpy.utils.batch_tools.batch_core import BaseAnalyzer
+from cellpy.utils.batch_tools.dumpers import ram_dumper
+from cellpy.utils.batch_tools.engines import summary_engine
+from cellpy.utils.ocv_rlx import select_ocv_points
+
+
+class BaseSummaryAnalyzer(BaseAnalyzer):
+    def __init__(self):
+        super().__init__()
+        self._assign_engine(summary_engine)
+        self._assign_dumper(ram_dumper)
+
+
+class ICAAnalyzer(BaseAnalyzer):
+    def __init__(self):
+        super().__init__()
+
+
+class EISAnalyzer(BaseAnalyzer):
+    def __init__(self):
+        super().__init__()
+
+
+class OCVRelaxationAnalyzer(BaseAnalyzer):
+    """Analyze open curcuit relaxation curves.
+
+    This analyzer is still under development.
+    (Partly) implented so far: select_ocv_points -> farms.
+    To get the DataFrames from the farms, you can use
+    >>> ocv_point_frames = OCVRelaxationAnalyzer.last
+
+    Attributes:
+        selection_method: criteria for selecting points
+            (martin: select first and last, and then last/2, last/2/2 etc. until you have reached the wanted number of points; fixed_time: select first, and same interval; defaults to "martin")
+        number_of_points: number of points you want.
+            defaults to 5
+        interval: interval between each point (in use only for methods
+            where interval makes sense). If it is a list, then
+            number_of_points will be calculated as len(interval) + 1 (and
+            override the set number_of_points).
+            defaults to 10
+        relative_voltage: set to True if you would like the voltage to be
+            relative to the voltage before starting the ocv rlx step.
+            Defaults to False. Remark that for the initial rxl step (when
+            you just have put your cell on the tester) does not have any
+            prior voltage. The relative voltage will then be versus the
+            first measurement point.
+            defaults to False
+        report_times: also report the ocv rlx total time if True (defaults
+            to False)
+        direction ("up", "down" or "both"): select "up" if you would like
+            to process only the ocv rlx steps where the voltage is relaxing
+            upwards and vize versa. Defaults to "both
+
+    Notes:
+        This analyzer is not working as intended yet. Todos:
+
+        - include better engine-dumper methodology and dump
+          stuff to both memory and file(s)
+          (should add this to BaseAnalyser)
+        - recieve settings and parameters
+        - option (dumper) for plotting?
+        - automatic fitting of OCV rlx data?
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.engines = []
+        self.dumpers = []
+        self.current_engine = None
+        self._assign_engine(self.ocv_points_engine)
+        # self._assign_dumper(self.screen_dumper)
+        # prms for select_ocv_points
+        self.selection_method = "martin"
+        self.number_of_points = 5
+        self.interval = 10
+        self.relative_voltage = False
+        self.report_times = False
+        self.include_times = True
+        self.direction = None
+
+    def _assign_engine(self, engine):
+        self.engines.append(engine)
+
+    def _assign_dumper(self, dumper):
+        self.dumpers.append(dumper)
+
+    def screen_dumper(self, **kwargs):
+        for farm in self.farms:
+            print(farm)
+
+    @property
+    def last(self) -> list:
+        return self.farms[-1]
+
+    @property
+    def dframe(self) -> pd.DataFrame:
+        return self.farms[-1][-1]
+
+    def run_engine(self, engine):
+        logging.debug(f"start engine::{engine.__name__}]")
+
+        self.current_engine = engine
+
+        self.farms, self.barn = engine(experiments=self.experiments, farms=self.farms)
+        logging.debug("::engine ended")
+
+    def run_dumper(self, dumper):
+        logging.debug(f"start dumper::{dumper.__name__}]")
+        dumper(
+            experiments=self.experiments,
+            farms=self.farms,
+            barn=self.barn,
+            engine=self.current_engine,
+        )
+        logging.debug("::dumper ended")
+
+    def do(self):
+        if not self.experiments:
+            raise UnderDefined("cannot run until you have assigned an experiment")
+
+        for engine in self.engines:
+            self.empty_the_farms()
+            logging.debug(f"running - {str(engine)}")
+            self.run_engine(engine)
+
+            for dumper in self.dumpers:
+                logging.debug(f"exporting - {str(dumper)}")
+                self.run_dumper(dumper)
+
+    def ocv_points_engine(self, **kwargs):
+        experiments = kwargs["experiments"]
+        farms = kwargs["farms"]
+        barn = None
+        for experiment, farm in zip(experiments, farms):
+            dframes = []
+            for cell_label in experiment.cell_data_frames:
+
+                logging.info(f"Analyzing {cell_label}")
+                if experiment.all_in_memory:
+                    logging.debug("CellpyData picked from memory")
+                    cell = experiment.cell_data_frames[cell_label]
+                    if cell.empty:
+                        logging.warning("Oh-no! Empty CellpyData-object")
+                else:
+                    logging.debug("CellpyData loaded from Cellpy-file")
+                    cell = experiment.data[cell_label]
+                    if cell.empty:
+                        logging.warning("Oh-no! Empty CellpyData-object")
+                df = select_ocv_points(
+                    cell,
+                    cell_label=cell_label,
+                    include_times=self.include_times,
+                    selection_method=self.selection_method,
+                    number_of_points=self.number_of_points,
+                    interval=self.interval,
+                    relative_voltage=self.relative_voltage,
+                    report_times=self.report_times,
+                    direction=self.direction,
+                )
+                dframes.append(df)
+            concat_df = pd.concat(dframes)
+            farm.append(concat_df)
+        return farms, barn
+
+    def do2(self):
+        for experiment, farm in zip(self.experiments, self.farms):
+            for cell_label in experiment.cell_data_frames:
+                logging.info(f"Analyzing {cell_label}")
+                if experiment.all_in_memory:
+                    logging.debug("CellpyData picked from memory")
+                    cell = experiment.cell_data_frames[cell_label]
+                    if cell.empty:
+                        logging.warning("Oh-no! Empty CellpyData-object")
+                else:
+                    logging.debug("CellpyData loaded from Cellpy-file")
+                    cell = experiment.data[cell_label]
+                    if cell.empty:
+                        logging.warning("Oh-no! Empty CellpyData-object")
+
+                df = select_ocv_points(
+                    cell,
+                    cell_label=cell_label,
+                    selection_method=self.selection_method,
+                    number_of_points=self.number_of_points,
+                    interval=self.interval,
+                    relative_voltage=self.relative_voltage,
+                    report_times=self.report_times,
+                    direction=self.direction,
+                )
+                farm.append(df)
+        return self.farms
```

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_core.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_experiments.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_helpers.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_journals.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/dumpers.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/batch_tools/engines.py` & `cellpy-0.4.3a3/cellpy/utils/batch_tools/engines.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/data/20160805_test001_45_cc.h5` & `cellpy-0.4.3a3/cellpy/utils/data/20160805_test001_45_cc.h5`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/data/raw/20160805_test001_45_cc_01.res` & `cellpy-0.4.3a3/cellpy/utils/data/raw/20160805_test001_45_cc_01.res`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/easyplot.py` & `cellpy-0.4.3a3/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/example_data.py` & `cellpy-0.4.3a3/cellpy/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/helpers.py` & `cellpy-0.4.3a3/cellpy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/ica.py` & `cellpy-0.4.3a3/cellpy/utils/ica.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy/utils/ocv_rlx.py` & `cellpy-0.4.3a3/cellpy/utils/ocv_rlx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,724 +1,711 @@
-import datetime
-import logging
-import time
-
-try:
-    from lmfit import Model, Parameters, minimize, report_ci, report_fit
-except ImportError as e:
-    logging.warning(
-        "Could not import lmfit. This is needed " "for fitting (run pip install lmfit)."
-    )
-    logging.debug(e)
-
-import math
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-
-from cellpy import cellreader
-
-# TODO: (28.05.2017 jepe) Docstrings are missing!!!!!!!! - AU: fix!
-
-
-# some utility functions
-
-# TODO: (05.10.2019 jepe) This function is slow due to use of loops. Should fix it.
-def select_ocv_points(
-    cellpydata,
-    cycles=None,
-    selection_method="martin",
-    number_of_points=5,
-    interval=10,
-    relative_voltage=False,
-    report_times=False,
-    direction="both",
-    return_times=False,
-):
-
-    """Select points from the ocvrlx steps.
-
-    Args:
-        cellpydata: ``CellpyData-object``
-        cycles: list of cycle numbers to process (optional)
-        selection_method ('martin' | 'fixed_times'): criteria for selecting points ('martin': select first and last, and
-            then last/2, last/2/2 etc. until you have reached the wanted number of points; 'fixed_times': select first,
-            and then same interval between each subsequent point).
-        number_of_points: number of points you want.
-        interval: interval between each point (in use only for methods
-            where interval makes sense). If it is a list, then
-            number_of_points will be calculated as len(interval) + 1 (and
-            override the set number_of_points).
-        relative_voltage: set to True if you would like the voltage to be
-            relative to the voltage before starting the ocv rlx step.
-            Defaults to False. Remark that for the initial rxl step (when
-            you just have put your cell on the tester) does not have any
-            prior voltage. The relative voltage will then be versus the
-            first measurement point.
-        report_times: also report the ocv rlx total time if True (defaults
-            to False)
-        direction ("up", "down" or "both"): select "up" if you would like
-            to process only the ocv rlx steps where the voltage is relaxing
-            upwards and vice versa. Defaults to "both".
-        return_times (bool): return a DataFrame with information about times.
-
-    Returns:
-        ``pandas.DataFrame`` (and another ``pandas.DataFrame`` if return_times is True)
-
-    """
-
-    t0 = time.time()
-    if cycles is None:
-        cycles = cellpydata.get_cycle_numbers()
-    else:
-        if not isinstance(cycles, (list, tuple)):
-            cycles = [cycles]
-
-    if not isinstance(interval, (list, tuple)):
-        interval = [float(interval) for _ in range(number_of_points - 1)]
-
-    ocv_rlx_id = "ocvrlx"
-
-    step_table = cellpydata.cell.steps
-    dfdata = cellpydata.cell.raw
-
-    ocv_steps = step_table.loc[step_table["cycle"].isin(cycles), :]
-
-    ocv_steps = ocv_steps.loc[ocv_steps.type.str.startswith(ocv_rlx_id, na=False), :]
-
-    t1 = time.time() - t0
-
-    if selection_method in ["fixed_times", "fixed_points", "selected_times"]:
-        number_of_points = len(interval) + 1
-
-    headers2 = []
-    for j in range(number_of_points):
-        n = str(j).zfill(2)
-        headers2.append(f"point_{n}")
-
-    t2 = time.time() - t0
-    # doing an iteration (thought I didnt have to, but...) (fix later)
-
-    results_list = list()
-    info_dict = {"cycle": [], "dt": [], "dv": [], "step": [], "type": [], "method": []}
-
-    iter_range = number_of_points - 1
-    if selection_method == "martin":
-        iter_range -= 1
-
-    # very slow:
-    for index, row in ocv_steps.iterrows():
-
-        # voltage
-        first, last, delta = (
-            row["voltage_first"],
-            row["voltage_last"],
-            row["voltage_delta"],
-        )
-
-        voltage_reference = 0.0
-
-        if relative_voltage:
-            if index > 0:
-                reference_row = step_table.iloc[index - 1, :]
-                voltage_reference = reference_row["voltage_last"]
-
-            else:
-                voltage_reference = first
-                logging.warning("STEP 0: Using first point as ref voltage")
-
-        # time
-        start, end, duration = (
-            row["step_time_first"],
-            row["step_time_last"],
-            row["step_time_delta"],
-        )
-
-        cycle, step = (row["cycle"], row["step"])
-        info = row["type"]
-
-        v_df = dfdata.loc[
-            (dfdata["cycle_index"] == cycle) & (dfdata["step_index"] == step),
-            ["step_time", "voltage"],
-        ]
-
-        poi = []
-
-        _end = end
-        _start = start
-
-        t = datetime.timedelta(seconds=round(end - start, 0))
-
-        info_dict["method"].append(selection_method)
-        info_dict["cycle"].append(cycle)
-        info_dict["step"].append(step)
-        info_dict["type"].append(info)
-        info_dict["dt"].append(t)
-        info_dict["dv"].append(first - last)
-
-        if report_times:
-            print(f"Cycle {cycle}:", end=" ")
-            print(f"dt = {str(t)}, dv = {first-last:6.3f}")
-
-        for i, j in enumerate(range(max(1, iter_range))):
-            if selection_method == "martin":
-                # logging.debug("using the 'martin'-method")
-                _end = _end / 2.0
-                poi.append(_end)
-
-            elif selection_method == "fixed_times":
-                logging.debug(f"using fixed times with interval {interval[i]}")
-                _start = _start + interval[i]
-                logging.debug(f"time: {_start}")
-                poi.append(_start)
-            else:
-                # more methods to come?
-                logging.info("this method is not implemented")
-                return None
-
-        if selection_method == "martin":
-            poi.reverse()
-
-        df_poi = pd.DataFrame({"step_time": poi})
-        df_poi["voltage"] = np.nan
-
-        v_df = v_df.append(df_poi, ignore_index=True)
-        v_df = v_df.sort_values("step_time").reset_index(drop=True)
-        v_df["new"] = v_df["voltage"].interpolate()
-
-        voi = []
-        for p in poi:
-            _v = v_df.loc[v_df["step_time"].isin([p]), "new"].values
-            _v = _v - voltage_reference
-            voi.append(_v[0])
-
-        poi.insert(0, start)
-        voi.insert(0, first - voltage_reference)
-        if selection_method == "martin":
-            poi.append(end)
-            voi.append(last - voltage_reference)
-
-        d1 = {"cycle": cycle}
-        d2 = {h: [v] for h, v in zip(headers2, voi)}
-        d = {**d1, **d2}
-        result = pd.DataFrame(d)
-        result["step"] = step
-        result["type"] = info
-        results_list.append(result)
-
-        if "t0" not in info_dict:
-            for i, p in enumerate(poi):
-                info_dict[f"t{i}"] = [p]
-        else:
-            for i, p in enumerate(poi):
-                info_dict[f"t{i}"].append(p)
-
-    t3 = time.time() - t0
-
-    final = pd.concat(results_list)  # pretty slow
-
-    t4 = time.time() - t0
-
-    if direction == "down":
-        final = final.loc[final["type"] == "ocvrlx_down", :]
-    elif direction == "up":
-        final = final.loc[final["type"] == "ocvrlx_up", :]
-
-    final = final.reset_index(drop=True)
-
-    # print(f"t1: {t1}\nt2: {t2-t1}\nt3: {t3-t2-t1}\nt4: {t4-t3-t2-t1}\n")
-
-    if not return_times:
-        return final
-
-    else:
-        try:
-            info_pd = pd.DataFrame(info_dict)
-        except Exception as e:
-            logging.info("could not create dataframe with time information")
-            logging.info(e)
-            info_pd = None
-        return final, info_pd
-
-
-class MultiCycleOcvFit(object):
-    def __init__(self, cellpydata, cycles, circuits=3):
-        """Object for performing fitting of multiple cycles.
-
-        Args:
-            cellpydata: ``CellpyData-object``
-            cycles (list): cycles to fit.
-            circuits (int): number of circuits to use in fitting.
-        """
-        self.cycles = cycles
-        self.data = cellpydata
-        self.circuits = circuits
-
-        self.fit_cycles = []
-        self.result = []
-        self.best_fit_data = []
-        self.best_fit_parameters = []
-        self.best_fit_parameters_translated = []
-
-    def set_data(self, cellpydata):
-        """Sets the CellpyData."""
-
-        self.data = cellpydata
-
-    def set_cycles(self, cycles):
-        """Sets the cycles."""
-
-        self.cycles = cycles
-
-    def run_fitting(self, direction="up", weighted=True):
-        """
-
-        Args:
-            direction ('up' | 'down'): what type of ocv relaxation to fit
-            weighted (bool): use weighted fitting.
-
-        Returns:
-            None
-
-        """
-        ocv_fitter = OcvFit()
-        ocv_fitter.set_circuits(self.circuits)
-        time_voltage = self.data.get_ocv(direction=direction, cycles=self.cycles[0])
-        time = time_voltage.step_time
-        voltage = time_voltage.voltage
-        if voltage is not None and time is not None:
-            ocv_fitter.set_data(time, voltage)
-        else:
-            ocv_fitter.set_data([0, 1, 2, 3], [2, 2, 2, 2])
-
-        try:
-            ocv_fitter.create_model()
-        except AttributeError as e:
-            print(e)
-            return
-
-        for cycle in self.cycles:
-            print("Fitting cycle " + str(cycle))
-            time_voltage = self.data.get_ocv(direction=direction, cycles=cycle)
-            time = time_voltage.step_time
-            voltage = time_voltage.voltage
-
-            if voltage is not None:
-                step_table = self.data.cell.steps
-                hdr = self.data.headers_step_table
-                if direction == "up":
-                    end_voltage = step_table[
-                        (step_table["cycle"] == cycle)
-                        & (step_table["type"].isin(["discharge"]))
-                    ][hdr.voltage + "_last"].values[0]
-                    end_current = step_table[
-                        (step_table["cycle"] == cycle)
-                        & (step_table["type"].isin(["discharge"]))
-                    ][hdr.current + "_last"].values[0]
-                    ocv_fitter.set_zero_voltage(end_voltage)
-                    ocv_fitter.set_zero_current(end_current)
-                elif direction == "down":
-                    end_voltage = step_table[
-                        (step_table["cycle"] == cycle)
-                        & (step_table["type"].isin(["charge"]))
-                    ][hdr.voltage + "_last"].values[0]
-                    end_current = step_table[
-                        (step_table["cycle"] == cycle)
-                        & (step_table["type"].isin(["charge"]))
-                    ][hdr.current + "_last"].values[0]
-                    ocv_fitter.set_zero_voltage(end_voltage)
-                    ocv_fitter.set_zero_current(end_current)
-
-                ocv_fitter.set_data(time, voltage)
-                if weighted:
-                    ocv_fitter.set_weights_power_law()
-                ocv_fitter.run_fit()
-
-                self.fit_cycles.append(cycle)
-                self.result.append(ocv_fitter.get_result())
-                self.best_fit_parameters.append(ocv_fitter.get_best_fit_parameters())
-                self.best_fit_parameters_translated.append(
-                    ocv_fitter.get_best_fit_parameters_translated()
-                )
-                self.best_fit_data.append(ocv_fitter.get_best_fit_data())
-
-    def get_best_fit_data(self):
-        """Returns the best fit data."""
-        return self.best_fit_data
-
-    def get_best_fit_parameters(self):
-        """Returns parameters for the best fit."""
-        return self.best_fit_parameters
-
-    def get_best_fit_parameters_translated(self):
-        """Returns the parameters in 'real units' for the best fit."""
-        return self.best_fit_parameters_translated
-
-    def get_best_fit_parameters_grouped(self):
-        """Returns a dictionary of the best fit."""
-        result_dict = dict()
-        result_dict["ocv"] = [
-            parameters["ocv"] for parameters in self.best_fit_parameters
-        ]
-
-        for i in range(self.circuits):
-            result_dict["t" + str(i)] = [
-                parameters["t" + str(i)] for parameters in self.best_fit_parameters
-            ]
-            result_dict["w" + str(i)] = [
-                parameters["w" + str(i)] for parameters in self.best_fit_parameters
-            ]
-        return result_dict
-
-    def get_best_fit_parameters_translated_grouped(self):
-        """Returns the parameters as a dictionary of the 'real units'
-        for the best fit."""
-        result_dict = dict()
-        result_dict["ocv"] = [
-            parameters["ocv"] for parameters in self.best_fit_parameters_translated
-        ]
-        result_dict["ir"] = [
-            parameters["ir"] for parameters in self.best_fit_parameters_translated
-        ]
-
-        for i in range(self.circuits):
-            result_dict["r" + str(i)] = [
-                parameters["r" + str(i)]
-                for parameters in self.best_fit_parameters_translated
-            ]
-            result_dict["c" + str(i)] = [
-                parameters["c" + str(i)]
-                for parameters in self.best_fit_parameters_translated
-            ]
-        return result_dict
-
-    def get_fit_cycles(self):
-        """Returns the fit cycles"""
-        return self.fit_cycles
-
-    def plot_summary(self, cycles=None):
-        """Convenience function for plotting the summary of the fit"""
-        if cycles is None:
-            cycles = [0]
-        fig1 = plt.figure()
-        ax1 = fig1.add_subplot(221)
-        ax1.set_title("Fit")
-        ax2 = fig1.add_subplot(222)
-        ax2.set_title("OCV")
-        ax3 = fig1.add_subplot(223)
-        ax3.set_title("Tau")
-        ax3.set_yscale("log")
-        ax4 = fig1.add_subplot(224)
-        ax4.set_title("Voltage Impact")
-
-        plot_data = self.get_best_fit_data()
-        for cycle in cycles:
-            ax1.plot(plot_data[cycle][0], plot_data[cycle][1])
-            ax1.plot(plot_data[cycle][0], plot_data[cycle][2])
-
-        plot_data = self.get_best_fit_parameters_grouped()
-
-        for i in range(self.circuits):
-            ax3.plot(self.get_fit_cycles(), plot_data["t" + str(i)])
-            ax4.plot(self.get_fit_cycles(), plot_data["w" + str(i)])
-
-        ax2.plot(self.get_fit_cycles(), plot_data["ocv"])
-
-    def plot_summary_translated(self):
-        """Convenience function for plotting the summary of the
-        fit (translated)"""
-
-        fig2 = plt.figure()
-        ax1 = fig2.add_subplot(221)
-        ax1.set_title("OCV (V)")
-        ax2 = fig2.add_subplot(222)
-        ax2.set_title("IR (Ohm)")
-        ax3 = fig2.add_subplot(223)
-        ax3.set_title("Resistances (Ohm)")
-        ax4 = fig2.add_subplot(224)
-        ax4.set_title("Capacitances (F)")
-        ax4.set_yscale("log")
-
-        plot_data = self.get_best_fit_parameters_translated_grouped()
-        print(plot_data["ocv"])
-        print(plot_data["ir"])
-        print(plot_data["r0"])
-
-        ax1.plot(self.get_fit_cycles(), plot_data["ocv"])
-        ax2.plot(self.get_fit_cycles(), plot_data["ir"])
-
-        for i in range(self.circuits):
-            ax3.plot(self.get_fit_cycles(), plot_data["r" + str(i)])
-            ax4.plot(self.get_fit_cycles(), plot_data["c" + str(i)])
-
-        plt.show()
-
-
-class OcvFit(object):
-    """Class for fitting open circuit relaxation data."""
-
-    def __init__(self, zero_current=0.1, zero_voltage=0.05):
-        self.data = None
-        self.weights = None
-        self.time = []
-        self.voltage = []
-        self.steps = ""
-        self.circuits = 3
-        self.zero_current = zero_current
-        self.zero_voltage = zero_voltage
-
-        self.model = None
-        self.params = Parameters()
-
-        self.result = None
-        self.best_fit_data = dict()
-        self.best_fit_parameters = dict()
-
-    def set_cellpydata(self, cellpydata, cycle):
-        """Performing fit of the OCV steps in the cycles set by set_cycles()
-        from the data set by set_data()
-
-        r is found by calculating v0 / i_start --> err(r)= err(v0) + err(i_start).
-
-        c is found from using tau / r --> err(c) = err(r) + err(tau).
-
-        Args:
-            cellpydata (CellpyData): data object from cellreader
-            cycle (int): cycle number to get from CellpyData object
-
-        Returns:
-            None
-
-        """
-        self.data = cellpydata
-        self.steps = self.data.cell  # hope it works...
-        time_voltage = self.data.get_ocv(direction="up", cycles=cycle)
-        time = time_voltage.step_time
-        voltage = time_voltage.voltage
-
-        self.time = np.array(time)
-        self.voltage = np.array(voltage)
-
-    def set_data(self, time, voltage):
-        self.time = np.array(time)
-        self.voltage = np.array(voltage)
-
-    def set_zero_current(self, zero_current):
-        self.zero_current = zero_current
-
-    def set_zero_voltage(self, zero_voltage):
-        self.zero_voltage = zero_voltage
-
-    def set_circuits(self, circuits):
-        self.circuits = circuits
-
-    def set_weights(self, weights):
-        self.weights = weights
-
-    def reset_weights(self):
-        self.weights = None
-
-    def set_weights_power_law(self, prefactor=1, power=-2, zero_level=1):
-        if self.voltage is not None:
-            self.weights = [
-                prefactor * pow(time + 1, power) + zero_level for time in self.time
-            ]
-        else:
-            raise NotImplementedError("Data is not set. Set data using set_data().")
-
-    def create_model(self):
-        params = Parameters()
-        params.add("ocv", value=self.voltage[-1], min=0, max=10)
-        taus = [math.pow(10, i) for i in range(self.circuits)]
-        weights = np.zeros(self.circuits)
-
-        params.add("t0", value=taus[0], min=0.01)
-        params.add("w0", value=weights[0])
-
-        for i in range(1, self.circuits):
-            params.add("delta" + str(i), value=taus[i] - taus[i - 1], min=0.0)
-            params.add("t" + str(i), expr="delta" + str(i) + "+t" + str(i - 1))
-            params.add("w" + str(i), value=weights[i])
-        for i in range(self.circuits, 5):
-            params.add("t" + str(i), value=1, vary=False)
-            params.add("w" + str(i), value=0, vary=False)
-
-        self.params = params
-        self.model = Model(self._model)
-
-    @staticmethod
-    def _model(time, ocv, t0, w0, t1, w1, t2, w2, t3, w3, t4, w4):
-        # Calculates a voltage profile for the given
-        # time array for a given set of parameters
-        model = ocv
-        model = (
-            model
-            + w0 * np.exp(-time / t0)
-            + w1 * np.exp(-time / t1)
-            + w2 * np.exp(-time / t2)
-            + w3 * np.exp(-time / t3)
-            + w4 * np.exp(-time / t4)
-        )
-
-        return model
-
-    def fit_model(self):
-
-        if self.model is not None:
-            self.result = self.model.fit(
-                self.voltage, weights=self.weights, time=self.time, params=self.params
-            )
-        else:
-            raise NotImplementedError(
-                "Model is not created. Set model using create_model()."
-            )
-
-        self.best_fit_parameters = self.result.best_values
-        self.best_fit_data = [self.time, self.voltage, self.result.best_fit]
-
-    def run_fit(self):
-        """Performing fit of the OCV steps in the cycles set by set_cycles()
-        from the data set by set_data()
-
-        r is found by calculating v0 / i_start --> err(r)= err(v0) + err(i_start).
-
-        c is found from using tau / r --> err(c) = err(r) + err(tau).
-
-        The resulting best fit parameters are stored in self.result for the given cycles.
-
-        Returns:
-            None
-
-        """
-
-        # Check if data is set
-        if self.time is []:
-            self.result = []
-            return
-
-        try:
-            self.fit_model()
-        except ValueError as e:
-            print(e)
-        except AttributeError as e:
-            print(e)
-
-    def get_result(self):
-        return self.result
-
-    def get_best_fit_data(self):
-        return self.best_fit_data
-
-    def get_best_fit_parameters(self):
-        return self.best_fit_parameters
-
-    def get_best_fit_parameters_translated(self):
-        result_dict = dict()
-        result_dict["ocv"] = self.best_fit_parameters["ocv"]
-        result_dict["ir"] = (
-            -(
-                (
-                    self.best_fit_parameters["ocv"]
-                    + self.best_fit_parameters["w0"]
-                    + self.best_fit_parameters["w1"]
-                    + self.best_fit_parameters["w2"]
-                    + self.best_fit_parameters["w3"]
-                    + self.best_fit_parameters["w4"]
-                )
-                - self.zero_voltage
-            )
-            / self.zero_current
-        )
-
-        for i in range(self.circuits):
-            result_dict["r" + str(i)] = (
-                self.best_fit_parameters["w" + str(i)] / self.zero_current
-            )
-            result_dict["c" + str(i)] = (
-                self.best_fit_parameters["t" + str(i)] / result_dict["r" + str(i)]
-            )
-
-        return result_dict
-
-
-def _main():
-    import os
-
-    import matplotlib.pyplot as plt
-
-    from cellpy import cellreader
-
-    print(50 * "=")
-    print("FITTING OCV ROUTINES - TEST")
-    print(50 * "-")
-
-    # filename(s) and folders etc
-    resfilename = "20160809_TF7_A1_04_cc_02.res"
-    resfilename = "20160216_snx001_01_cc_01.res"
-    resfilename = "20160216_snx001_02_cc_01.res"
-    resfilename = "20170310_snx002_03_cc_01.res"
-    # resfilename = "20160306_snx001_09_cc_01.res"
-    # resfilename = "20150501_TF7_A1_01_cc_01.res"
-    resfilename = "20160805_test001_45_cc_01.res"
-    resfilename = "20160306_snx001_07_cc_02.res"
-    resfilename = "20160306_snx001_08_cc_02.res"
-    resfilename = "20160306_snx001_10_cc_01.res"
-
-    single_cell = False
-
-    datafolder_in = r"..\data_ex"
-    datafolder_out = r"..\outdata"
-
-    # parameters about the run (mass (mg))
-    mass = 0.982
-
-    # cycles to test
-    cycles = [i * 10 for i in range(1, 10)]
-    cycles = [i * 1 for i in range(1, 100)]
-    print(50 * "-")
-    print("Loading data")
-    print(50 * "-")
-
-    print("loading file", end=" ")
-    print(resfilename)
-
-    # Loading dataframe
-    d = cellreader.CellpyData()
-    # noinspection PyDeprecation
-    d.from_raw(os.path.join(datafolder_in, resfilename))
-    d.set_mass(mass)
-    d.make_step_table()
-
-    if single_cell:
-        # Sending data to ocv_fit object and running fit
-        ocv_fit = OcvFit()
-        ocv_fit.set_cellpydata(d, 1)
-        ocv_fit.set_circuits(4)
-        ocv_fit.create_model()
-        ocv_fit.run_fit()
-
-        fig1 = plt.figure()
-        fig1.suptitle("Fit")
-        ax1 = fig1.add_subplot(111)
-
-        plot_data = ocv_fit.get_best_fit_data()
-        ax1.plot(plot_data[0], plot_data[1])
-        ax1.plot(plot_data[0], plot_data[2])
-
-        plt.show()
-
-    else:
-        ocv_fit = MultiCycleOcvFit(d, cycles, circuits=3)
-        ocv_fit.run_fitting(direction="up")
-        ocv_fit.plot_summary([0])
-        ocv_fit.plot_summary_translated()
-
-        # # Printing best fit parameters
-        # for best_fit_parameters in ocv_fit.get_best_fit_parameters():
-        #     print 50 * '-'
-        #     print best_fit_parameters
-
-
-if __name__ == "__main__":
-    print("ocv-rlx".center(80, "="))
-    _main()
+import datetime
+import logging
+import time
+
+try:
+    from lmfit import Model, Parameters, minimize, report_ci, report_fit
+except ImportError as e:
+    logging.warning(
+        "Could not import lmfit. This is needed " "for fitting (run pip install lmfit)."
+    )
+    logging.debug(e)
+
+import math
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+
+from cellpy import cellreader
+
+# TODO: (28.05.2017 jepe) Docstrings are missing!!!!!!!! - AU: fix!
+
+
+# some utility functions
+
+# TODO: (05.10.2019 jepe) This function is slow due to use of loops. Should fix it.
+def select_ocv_points(
+    cellpydata,
+    cycles=None,
+    cell_label=None,
+    include_times=True,
+    selection_method="martin",
+    number_of_points=5,
+    interval=10,
+    relative_voltage=False,
+    report_times=False,
+    direction="both",
+):
+
+    """Select points from the ocvrlx steps.
+
+    Args:
+        cellpydata: ``CellpyData-object``
+        cycles: list of cycle numbers to process (optional)
+        cell_label (str): optional, will be added to the frame if given
+        include_times (bool): include additional information including times.
+        selection_method ('martin' | 'fixed_times'): criteria for selecting points ('martin': select first and last, and
+            then last/2, last/2/2 etc. until you have reached the wanted number of points; 'fixed_times': select first,
+            and then same interval between each subsequent point).
+        number_of_points: number of points you want.
+        interval: interval between each point (in use only for methods
+            where interval makes sense). If it is a list, then
+            number_of_points will be calculated as len(interval) + 1 (and
+            override the set number_of_points).
+        relative_voltage: set to True if you would like the voltage to be
+            relative to the voltage before starting the ocv rlx step.
+            Defaults to False. Remark that for the initial rxl step (when
+            you just have put your cell on the tester) does not have any
+            prior voltage. The relative voltage will then be versus the
+            first measurement point.
+        report_times: also report the ocv rlx total time if True (defaults
+            to False)
+        direction ("up", "down" or "both"): select "up" if you would like
+            to process only the ocv rlx steps where the voltage is relaxing
+            upwards and vice versa. Defaults to "both".
+
+    Returns:
+        ``pandas.DataFrame`` (and another ``pandas.DataFrame`` if return_times is True)
+
+    """
+
+    if cycles is None:
+        cycles = cellpydata.get_cycle_numbers()
+    else:
+        if not isinstance(cycles, (list, tuple)):
+            cycles = [cycles]
+
+    if not isinstance(interval, (list, tuple)):
+        interval = [float(interval) for _ in range(number_of_points - 1)]
+
+    ocv_rlx_id = "ocvrlx"
+
+    step_table = cellpydata.cell.steps
+    dfdata = cellpydata.cell.raw
+
+    ocv_steps = step_table.loc[step_table["cycle"].isin(cycles), :]
+    ocv_steps = ocv_steps.loc[ocv_steps.type.str.startswith(ocv_rlx_id, na=False), :]
+
+    if selection_method in ["fixed_times", "fixed_points", "selected_times"]:
+        number_of_points = len(interval) + 1
+
+    headers2 = []
+    for j in range(number_of_points):
+        n = str(j).zfill(2)
+        headers2.append(f"point_{n}")
+
+    # doing an iteration (thought I didn't have to, but...) (fix later)
+
+    results_list = list()
+    info_dict = {"dt": [], "dv": [], "method": []}
+
+    iter_range = number_of_points - 1
+    if selection_method == "martin":
+        iter_range -= 1
+
+    # very slow:
+    for index, row in ocv_steps.iterrows():
+
+        # voltage
+        first, last, delta = (
+            row["voltage_first"],
+            row["voltage_last"],
+            row["voltage_delta"],
+        )
+
+        voltage_reference = 0.0
+
+        if relative_voltage:
+            if index > 0:
+                reference_row = step_table.iloc[index - 1, :]
+                voltage_reference = reference_row["voltage_last"]
+
+            else:
+                voltage_reference = first
+                logging.warning("STEP 0: Using first point as ref voltage")
+
+        # time
+        start, end, duration = (
+            row["step_time_first"],
+            row["step_time_last"],
+            row["step_time_delta"],
+        )
+
+        cycle, step = (row["cycle"], row["step"])
+        info = row["type"]
+
+        v_df = dfdata.loc[
+            (dfdata["cycle_index"] == cycle) & (dfdata["step_index"] == step),
+            ["step_time", "voltage"],
+        ]
+
+        poi = []
+
+        _end = end
+        _start = start
+
+        t = datetime.timedelta(seconds=round(end - start, 0))
+
+        info_dict["method"].append(selection_method)
+        info_dict["dt"].append(t)
+        info_dict["dv"].append(first - last)
+
+        if report_times:
+            print(f"Cycle {cycle}:", end=" ")
+            print(f"dt = {str(t)}, dv = {first-last:6.3f}")
+
+        for i, j in enumerate(range(max(1, iter_range))):
+            if selection_method == "martin":
+                # logging.debug("using the 'martin'-method")
+                _end = _end / 2.0
+                poi.append(_end)
+
+            elif selection_method == "fixed_times":
+                logging.debug(f"using fixed times with interval {interval[i]}")
+                _start = _start + interval[i]
+                logging.debug(f"time: {_start}")
+                poi.append(_start)
+            else:
+                # more methods to come?
+                logging.info("this method is not implemented")
+                return None
+
+        if selection_method == "martin":
+            poi.reverse()
+
+        df_poi = pd.DataFrame({"step_time": poi})
+        df_poi["voltage"] = np.nan
+
+        v_df = v_df.append(df_poi, ignore_index=True)
+        v_df = v_df.sort_values("step_time").reset_index(drop=True)
+        v_df["new"] = v_df["voltage"].interpolate()
+
+        voi = []
+        for p in poi:
+            _v = v_df.loc[v_df["step_time"].isin([p]), "new"].values
+            _v = _v - voltage_reference
+            voi.append(_v[0])
+
+        poi.insert(0, start)
+        voi.insert(0, first - voltage_reference)
+        if selection_method == "martin":
+            poi.append(end)
+            voi.append(last - voltage_reference)
+
+        d1 = {"cycle": cycle}
+        d2 = {h: [v] for h, v in zip(headers2, voi)}
+        d = {**d1, **d2}
+        result = pd.DataFrame(d)
+        result["step"] = step
+        result["type"] = info
+        results_list.append(result)
+
+        if "t0" not in info_dict:
+            for i, p in enumerate(poi):
+                info_dict[f"t{i}"] = [p]
+        else:
+            for i, p in enumerate(poi):
+                info_dict[f"t{i}"].append(p)
+    final = pd.concat(results_list)
+
+    if direction == "down":
+        final = final.loc[final["type"] == "ocvrlx_down", :]
+    elif direction == "up":
+        final = final.loc[final["type"] == "ocvrlx_up", :]
+
+    if cell_label is not None:
+        final = final.assign(cell=cell_label)
+    final = final.reset_index(drop=True)
+
+    if include_times:
+        try:
+            info_pd = pd.DataFrame(info_dict)
+            final = pd.concat([info_pd, final], axis=1,)
+            final = final.reset_index(drop=True)
+        except Exception as e:
+            logging.info("could not create dataframe with time information")
+            logging.info(e)
+    return final
+
+
+class MultiCycleOcvFit(object):
+    def __init__(self, cellpydata, cycles, circuits=3):
+        """Object for performing fitting of multiple cycles.
+
+        Args:
+            cellpydata: ``CellpyData-object``
+            cycles (list): cycles to fit.
+            circuits (int): number of circuits to use in fitting.
+        """
+        self.cycles = cycles
+        self.data = cellpydata
+        self.circuits = circuits
+
+        self.fit_cycles = []
+        self.result = []
+        self.best_fit_data = []
+        self.best_fit_parameters = []
+        self.best_fit_parameters_translated = []
+
+    def set_data(self, cellpydata):
+        """Sets the CellpyData."""
+
+        self.data = cellpydata
+
+    def set_cycles(self, cycles):
+        """Sets the cycles."""
+
+        self.cycles = cycles
+
+    def run_fitting(self, direction="up", weighted=True):
+        """
+
+        Args:
+            direction ('up' | 'down'): what type of ocv relaxation to fit
+            weighted (bool): use weighted fitting.
+
+        Returns:
+            None
+
+        """
+        ocv_fitter = OcvFit()
+        ocv_fitter.set_circuits(self.circuits)
+        time_voltage = self.data.get_ocv(direction=direction, cycles=self.cycles[0])
+        time = time_voltage.step_time
+        voltage = time_voltage.voltage
+        if voltage is not None and time is not None:
+            ocv_fitter.set_data(time, voltage)
+        else:
+            ocv_fitter.set_data([0, 1, 2, 3], [2, 2, 2, 2])
+
+        try:
+            ocv_fitter.create_model()
+        except AttributeError as e:
+            print(e)
+            return
+
+        for cycle in self.cycles:
+            print("Fitting cycle " + str(cycle))
+            time_voltage = self.data.get_ocv(direction=direction, cycles=cycle)
+            time = time_voltage.step_time
+            voltage = time_voltage.voltage
+
+            if voltage is not None:
+                step_table = self.data.cell.steps
+                hdr = self.data.headers_step_table
+                if direction == "up":
+                    end_voltage = step_table[
+                        (step_table["cycle"] == cycle)
+                        & (step_table["type"].isin(["discharge"]))
+                    ][hdr.voltage + "_last"].values[0]
+                    end_current = step_table[
+                        (step_table["cycle"] == cycle)
+                        & (step_table["type"].isin(["discharge"]))
+                    ][hdr.current + "_last"].values[0]
+                    ocv_fitter.set_zero_voltage(end_voltage)
+                    ocv_fitter.set_zero_current(end_current)
+                elif direction == "down":
+                    end_voltage = step_table[
+                        (step_table["cycle"] == cycle)
+                        & (step_table["type"].isin(["charge"]))
+                    ][hdr.voltage + "_last"].values[0]
+                    end_current = step_table[
+                        (step_table["cycle"] == cycle)
+                        & (step_table["type"].isin(["charge"]))
+                    ][hdr.current + "_last"].values[0]
+                    ocv_fitter.set_zero_voltage(end_voltage)
+                    ocv_fitter.set_zero_current(end_current)
+
+                ocv_fitter.set_data(time, voltage)
+                if weighted:
+                    ocv_fitter.set_weights_power_law()
+                ocv_fitter.run_fit()
+
+                self.fit_cycles.append(cycle)
+                self.result.append(ocv_fitter.get_result())
+                self.best_fit_parameters.append(ocv_fitter.get_best_fit_parameters())
+                self.best_fit_parameters_translated.append(
+                    ocv_fitter.get_best_fit_parameters_translated()
+                )
+                self.best_fit_data.append(ocv_fitter.get_best_fit_data())
+
+    def get_best_fit_data(self):
+        """Returns the best fit data."""
+        return self.best_fit_data
+
+    def get_best_fit_parameters(self):
+        """Returns parameters for the best fit."""
+        return self.best_fit_parameters
+
+    def get_best_fit_parameters_translated(self):
+        """Returns the parameters in 'real units' for the best fit."""
+        return self.best_fit_parameters_translated
+
+    def get_best_fit_parameters_grouped(self):
+        """Returns a dictionary of the best fit."""
+        result_dict = dict()
+        result_dict["ocv"] = [
+            parameters["ocv"] for parameters in self.best_fit_parameters
+        ]
+
+        for i in range(self.circuits):
+            result_dict["t" + str(i)] = [
+                parameters["t" + str(i)] for parameters in self.best_fit_parameters
+            ]
+            result_dict["w" + str(i)] = [
+                parameters["w" + str(i)] for parameters in self.best_fit_parameters
+            ]
+        return result_dict
+
+    def get_best_fit_parameters_translated_grouped(self):
+        """Returns the parameters as a dictionary of the 'real units'
+        for the best fit."""
+        result_dict = dict()
+        result_dict["ocv"] = [
+            parameters["ocv"] for parameters in self.best_fit_parameters_translated
+        ]
+        result_dict["ir"] = [
+            parameters["ir"] for parameters in self.best_fit_parameters_translated
+        ]
+
+        for i in range(self.circuits):
+            result_dict["r" + str(i)] = [
+                parameters["r" + str(i)]
+                for parameters in self.best_fit_parameters_translated
+            ]
+            result_dict["c" + str(i)] = [
+                parameters["c" + str(i)]
+                for parameters in self.best_fit_parameters_translated
+            ]
+        return result_dict
+
+    def get_fit_cycles(self):
+        """Returns the fit cycles"""
+        return self.fit_cycles
+
+    def plot_summary(self, cycles=None):
+        """Convenience function for plotting the summary of the fit"""
+        if cycles is None:
+            cycles = [0]
+        fig1 = plt.figure()
+        ax1 = fig1.add_subplot(221)
+        ax1.set_title("Fit")
+        ax2 = fig1.add_subplot(222)
+        ax2.set_title("OCV")
+        ax3 = fig1.add_subplot(223)
+        ax3.set_title("Tau")
+        ax3.set_yscale("log")
+        ax4 = fig1.add_subplot(224)
+        ax4.set_title("Voltage Impact")
+
+        plot_data = self.get_best_fit_data()
+        for cycle in cycles:
+            ax1.plot(plot_data[cycle][0], plot_data[cycle][1])
+            ax1.plot(plot_data[cycle][0], plot_data[cycle][2])
+
+        plot_data = self.get_best_fit_parameters_grouped()
+
+        for i in range(self.circuits):
+            ax3.plot(self.get_fit_cycles(), plot_data["t" + str(i)])
+            ax4.plot(self.get_fit_cycles(), plot_data["w" + str(i)])
+
+        ax2.plot(self.get_fit_cycles(), plot_data["ocv"])
+
+    def plot_summary_translated(self):
+        """Convenience function for plotting the summary of the
+        fit (translated)"""
+
+        fig2 = plt.figure()
+        ax1 = fig2.add_subplot(221)
+        ax1.set_title("OCV (V)")
+        ax2 = fig2.add_subplot(222)
+        ax2.set_title("IR (Ohm)")
+        ax3 = fig2.add_subplot(223)
+        ax3.set_title("Resistances (Ohm)")
+        ax4 = fig2.add_subplot(224)
+        ax4.set_title("Capacitances (F)")
+        ax4.set_yscale("log")
+
+        plot_data = self.get_best_fit_parameters_translated_grouped()
+        print(plot_data["ocv"])
+        print(plot_data["ir"])
+        print(plot_data["r0"])
+
+        ax1.plot(self.get_fit_cycles(), plot_data["ocv"])
+        ax2.plot(self.get_fit_cycles(), plot_data["ir"])
+
+        for i in range(self.circuits):
+            ax3.plot(self.get_fit_cycles(), plot_data["r" + str(i)])
+            ax4.plot(self.get_fit_cycles(), plot_data["c" + str(i)])
+
+        plt.show()
+
+
+class OcvFit(object):
+    """Class for fitting open circuit relaxation data."""
+
+    def __init__(self, zero_current=0.1, zero_voltage=0.05):
+        self.data = None
+        self.weights = None
+        self.time = []
+        self.voltage = []
+        self.steps = ""
+        self.circuits = 3
+        self.zero_current = zero_current
+        self.zero_voltage = zero_voltage
+
+        self.model = None
+        self.params = Parameters()
+
+        self.result = None
+        self.best_fit_data = dict()
+        self.best_fit_parameters = dict()
+
+    def set_cellpydata(self, cellpydata, cycle):
+        """Performing fit of the OCV steps in the cycles set by set_cycles()
+        from the data set by set_data()
+
+        r is found by calculating v0 / i_start --> err(r)= err(v0) + err(i_start).
+
+        c is found from using tau / r --> err(c) = err(r) + err(tau).
+
+        Args:
+            cellpydata (CellpyData): data object from cellreader
+            cycle (int): cycle number to get from CellpyData object
+
+        Returns:
+            None
+
+        """
+        self.data = cellpydata
+        self.steps = self.data.cell  # hope it works...
+        time_voltage = self.data.get_ocv(direction="up", cycles=cycle)
+        time = time_voltage.step_time
+        voltage = time_voltage.voltage
+
+        self.time = np.array(time)
+        self.voltage = np.array(voltage)
+
+    def set_data(self, time, voltage):
+        self.time = np.array(time)
+        self.voltage = np.array(voltage)
+
+    def set_zero_current(self, zero_current):
+        self.zero_current = zero_current
+
+    def set_zero_voltage(self, zero_voltage):
+        self.zero_voltage = zero_voltage
+
+    def set_circuits(self, circuits):
+        self.circuits = circuits
+
+    def set_weights(self, weights):
+        self.weights = weights
+
+    def reset_weights(self):
+        self.weights = None
+
+    def set_weights_power_law(self, prefactor=1, power=-2, zero_level=1):
+        if self.voltage is not None:
+            self.weights = [
+                prefactor * pow(time + 1, power) + zero_level for time in self.time
+            ]
+        else:
+            raise NotImplementedError("Data is not set. Set data using set_data().")
+
+    def create_model(self):
+        params = Parameters()
+        params.add("ocv", value=self.voltage[-1], min=0, max=10)
+        taus = [math.pow(10, i) for i in range(self.circuits)]
+        weights = np.zeros(self.circuits)
+
+        params.add("t0", value=taus[0], min=0.01)
+        params.add("w0", value=weights[0])
+
+        for i in range(1, self.circuits):
+            params.add("delta" + str(i), value=taus[i] - taus[i - 1], min=0.0)
+            params.add("t" + str(i), expr="delta" + str(i) + "+t" + str(i - 1))
+            params.add("w" + str(i), value=weights[i])
+        for i in range(self.circuits, 5):
+            params.add("t" + str(i), value=1, vary=False)
+            params.add("w" + str(i), value=0, vary=False)
+
+        self.params = params
+        self.model = Model(self._model)
+
+    @staticmethod
+    def _model(time, ocv, t0, w0, t1, w1, t2, w2, t3, w3, t4, w4):
+        # Calculates a voltage profile for the given
+        # time array for a given set of parameters
+        model = ocv
+        model = (
+            model
+            + w0 * np.exp(-time / t0)
+            + w1 * np.exp(-time / t1)
+            + w2 * np.exp(-time / t2)
+            + w3 * np.exp(-time / t3)
+            + w4 * np.exp(-time / t4)
+        )
+
+        return model
+
+    def fit_model(self):
+
+        if self.model is not None:
+            self.result = self.model.fit(
+                self.voltage, weights=self.weights, time=self.time, params=self.params
+            )
+        else:
+            raise NotImplementedError(
+                "Model is not created. Set model using create_model()."
+            )
+
+        self.best_fit_parameters = self.result.best_values
+        self.best_fit_data = [self.time, self.voltage, self.result.best_fit]
+
+    def run_fit(self):
+        """Performing fit of the OCV steps in the cycles set by set_cycles()
+        from the data set by set_data()
+
+        r is found by calculating v0 / i_start --> err(r)= err(v0) + err(i_start).
+
+        c is found from using tau / r --> err(c) = err(r) + err(tau).
+
+        The resulting best fit parameters are stored in self.result for the given cycles.
+
+        Returns:
+            None
+
+        """
+
+        # Check if data is set
+        if self.time is []:
+            self.result = []
+            return
+
+        try:
+            self.fit_model()
+        except ValueError as e:
+            print(e)
+        except AttributeError as e:
+            print(e)
+
+    def get_result(self):
+        return self.result
+
+    def get_best_fit_data(self):
+        return self.best_fit_data
+
+    def get_best_fit_parameters(self):
+        return self.best_fit_parameters
+
+    def get_best_fit_parameters_translated(self):
+        result_dict = dict()
+        result_dict["ocv"] = self.best_fit_parameters["ocv"]
+        result_dict["ir"] = (
+            -(
+                (
+                    self.best_fit_parameters["ocv"]
+                    + self.best_fit_parameters["w0"]
+                    + self.best_fit_parameters["w1"]
+                    + self.best_fit_parameters["w2"]
+                    + self.best_fit_parameters["w3"]
+                    + self.best_fit_parameters["w4"]
+                )
+                - self.zero_voltage
+            )
+            / self.zero_current
+        )
+
+        for i in range(self.circuits):
+            result_dict["r" + str(i)] = (
+                self.best_fit_parameters["w" + str(i)] / self.zero_current
+            )
+            result_dict["c" + str(i)] = (
+                self.best_fit_parameters["t" + str(i)] / result_dict["r" + str(i)]
+            )
+
+        return result_dict
+
+
+def _main():
+    import os
+
+    import matplotlib.pyplot as plt
+
+    from cellpy import cellreader
+
+    print(50 * "=")
+    print("FITTING OCV ROUTINES - TEST")
+    print(50 * "-")
+
+    # filename(s) and folders etc
+    resfilename = "20160809_TF7_A1_04_cc_02.res"
+    resfilename = "20160216_snx001_01_cc_01.res"
+    resfilename = "20160216_snx001_02_cc_01.res"
+    resfilename = "20170310_snx002_03_cc_01.res"
+    # resfilename = "20160306_snx001_09_cc_01.res"
+    # resfilename = "20150501_TF7_A1_01_cc_01.res"
+    resfilename = "20160805_test001_45_cc_01.res"
+    resfilename = "20160306_snx001_07_cc_02.res"
+    resfilename = "20160306_snx001_08_cc_02.res"
+    resfilename = "20160306_snx001_10_cc_01.res"
+
+    single_cell = False
+
+    datafolder_in = r"..\data_ex"
+    datafolder_out = r"..\outdata"
+
+    # parameters about the run (mass (mg))
+    mass = 0.982
+
+    # cycles to test
+    cycles = [i * 10 for i in range(1, 10)]
+    cycles = [i * 1 for i in range(1, 100)]
+    print(50 * "-")
+    print("Loading data")
+    print(50 * "-")
+
+    print("loading file", end=" ")
+    print(resfilename)
+
+    # Loading dataframe
+    d = cellreader.CellpyData()
+    # noinspection PyDeprecation
+    d.from_raw(os.path.join(datafolder_in, resfilename))
+    d.set_mass(mass)
+    d.make_step_table()
+
+    if single_cell:
+        # Sending data to ocv_fit object and running fit
+        ocv_fit = OcvFit()
+        ocv_fit.set_cellpydata(d, 1)
+        ocv_fit.set_circuits(4)
+        ocv_fit.create_model()
+        ocv_fit.run_fit()
+
+        fig1 = plt.figure()
+        fig1.suptitle("Fit")
+        ax1 = fig1.add_subplot(111)
+
+        plot_data = ocv_fit.get_best_fit_data()
+        ax1.plot(plot_data[0], plot_data[1])
+        ax1.plot(plot_data[0], plot_data[2])
+
+        plt.show()
+
+    else:
+        ocv_fit = MultiCycleOcvFit(d, cycles, circuits=3)
+        ocv_fit.run_fitting(direction="up")
+        ocv_fit.plot_summary([0])
+        ocv_fit.plot_summary_translated()
+
+        # # Printing best fit parameters
+        # for best_fit_parameters in ocv_fit.get_best_fit_parameters():
+        #     print 50 * '-'
+        #     print best_fit_parameters
+
+
+if __name__ == "__main__":
+    print("ocv-rlx".center(80, "="))
+    _main()
```

### Comparing `cellpy-0.4.3a2/cellpy/utils/plotutils.py` & `cellpy-0.4.3a3/cellpy/utils/plotutils.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/cellpy.egg-info/PKG-INFO` & `cellpy-0.4.3a3/cellpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 0.4.3a2
+Version: 0.4.3a3
 Summary: Extract and manipulate data from battery cell testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cellpy-0.4.3a2/cellpy.egg-info/SOURCES.txt` & `cellpy-0.4.3a3/cellpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/Makefile` & `cellpy-0.4.3a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_6_0.png` & `cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_7_0.png` & `cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_8_0.png` & `cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_simple_plot_2_0.png` & `cellpy-0.4.3a3/docs/_build/.doctrees/nbsphinx/notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/_images/notebooks_tutorial_get_cap_6_0.png` & `cellpy-0.4.3a3/docs/_build/_images/notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/_images/notebooks_tutorial_get_cap_7_0.png` & `cellpy-0.4.3a3/docs/_build/_images/notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/_images/notebooks_tutorial_get_cap_8_0.png` & `cellpy-0.4.3a3/docs/_build/_images/notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/_images/notebooks_tutorial_simple_plot_2_0.png` & `cellpy-0.4.3a3/docs/_build/_images/notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/_images/templates_jupyterlab_001.png` & `cellpy-0.4.3a3/docs/_build/_images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/_images/tutorials_utils_plotting_fig1.png` & `cellpy-0.4.3a3/docs/_build/_images/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/_build/_images/tutorials_utils_plotting_fig2.png` & `cellpy-0.4.3a3/docs/_build/_images/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/conf.py` & `cellpy-0.4.3a3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/developers/dev_cellpy_data_structure.rst` & `cellpy-0.4.3a3/docs/developers/dev_cellpy_data_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/developers/dev_cellpy_folder_structure.rst` & `cellpy-0.4.3a3/docs/developers/dev_cellpy_folder_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/developers/dev_various.rst` & `cellpy-0.4.3a3/docs/developers/dev_various.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/formats.rst` & `cellpy-0.4.3a3/docs/formats.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/index.rst` & `cellpy-0.4.3a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/installation.rst` & `cellpy-0.4.3a3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/make.bat` & `cellpy-0.4.3a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/source/cellpy.parameters.rst` & `cellpy-0.4.3a3/docs/source/cellpy.parameters.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/source/cellpy.readers.instruments.rst` & `cellpy-0.4.3a3/docs/source/cellpy.readers.instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/source/cellpy.readers.rst` & `cellpy-0.4.3a3/docs/source/cellpy.readers.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/source/cellpy.rst` & `cellpy-0.4.3a3/docs/source/cellpy.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/source/cellpy.utils.batch_tools.rst` & `cellpy-0.4.3a3/docs/source/cellpy.utils.batch_tools.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/source/cellpy.utils.rst` & `cellpy-0.4.3a3/docs/source/cellpy.utils.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/tips_and_tricks.rst` & `cellpy-0.4.3a3/docs/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/tutorials/basic_interaction.rst` & `cellpy-0.4.3a3/docs/tutorials/basic_interaction.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/tutorials/configuring.rst` & `cellpy-0.4.3a3/docs/tutorials/configuring.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/tutorials/data_mining.rst` & `cellpy-0.4.3a3/docs/tutorials/data_mining.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/tutorials/getting_started_tutorial.rst` & `cellpy-0.4.3a3/docs/tutorials/getting_started_tutorial.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/tutorials/pandas.rst` & `cellpy-0.4.3a3/docs/tutorials/pandas.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/tutorials/the_cellpy_cmd.rst` & `cellpy-0.4.3a3/docs/tutorials/the_cellpy_cmd.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/usage.rst` & `cellpy-0.4.3a3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/utils/batch.rst` & `cellpy-0.4.3a3/docs/utils/batch.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/utils/figures/tutorials_utils_plotting_fig1.png` & `cellpy-0.4.3a3/docs/utils/figures/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/utils/figures/tutorials_utils_plotting_fig2.png` & `cellpy-0.4.3a3/docs/utils/figures/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/utils/ica.rst` & `cellpy-0.4.3a3/docs/utils/ica.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/utils/plotting.rst` & `cellpy-0.4.3a3/docs/utils/plotting.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/docs/utils/tut_ocv_rlx.rst` & `cellpy-0.4.3a3/docs/utils/tut_ocv_rlx.rst`

 * *Files identical despite different names*

### Comparing `cellpy-0.4.3a2/setup.py` & `cellpy-0.4.3a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     'sqlalchemy-access;platform_system=="windows"',
     # 'pytables', # not available by pip
 ]
 
 test_requirements = [
     "scipy",
     "numpy>=1.16.4",
-    "pandas",
+    "pandas>=1.5.3",
     "python-box",
     "setuptools",
     "ruamel.yaml",
     "matplotlib",
     "lmfit",
     "pyodbc",
     "openpyxl",
```

