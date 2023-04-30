# Comparing `tmp/pyascore-0.7.0b0.tar.gz` & `tmp/pyascore-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyAscore/pyAscore/dist/tmp8rvu25bz/pyascore-0.7.0b0.tar", last modified: Sun Apr 24 20:56:11 2022, max compression
+gzip compressed data, was "/home/runner/work/pyAscore/pyAscore/dist/.tmp-qfs5czua/pyascore-1.0.0b0.tar", last modified: Sun Apr 30 03:54:22 2023, max compression
```

## Comparing `pyascore-0.7.0b0.tar` & `pyascore-1.0.0b0.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/static/
--rw-r--r--   0 runner    (1001) docker     (116)    33955 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      877 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/.github/workflows/linux-build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1399 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/.github/workflows/windows-build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     3252 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     7756 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7007 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      182 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1068 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)     1040 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      125 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore/
--rw-r--r--   0 runner    (1001) docker     (116)     5854 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     6490 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      522 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/
--rw-r--r--   0 runner    (1001) docker     (116)      885 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/Ascore.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1505 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/ModifiedPeptide.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3802 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/Spectra.pyx
--rw-r--r--   0 runner    (1001) docker     (116)      702 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/Util.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3933 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/Util.pyx
--rw-r--r--   0 runner    (1001) docker     (116)    12170 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/Ascore.pyx
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/
--rw-r--r--   0 runner    (1001) docker     (116)     1176 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Util.h
--rw-r--r--   0 runner    (1001) docker     (116)     4657 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Util.cpp
--rw-r--r--   0 runner    (1001) docker     (116)    22020 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/ModifiedPeptide.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3867 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Spectra.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     3711 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/ModifiedPeptide.h
--rw-r--r--   0 runner    (1001) docker     (116)      800 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Types.h
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Spectra.h
--rw-r--r--   0 runner    (1001) docker     (116)     1911 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Ascore.h
--rw-r--r--   0 runner    (1001) docker     (116)    12387 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Ascore.cpp
--rw-r--r--   0 runner    (1001) docker     (116)   883079 2022-04-24 20:56:10.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/PTMScoring.cpp
--rw-r--r--   0 runner    (1001) docker     (116)      688 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/Spectra.pxd
--rw-r--r--   0 runner    (1001) docker     (116)    13379 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/ModifiedPeptide.pyx
--rw-r--r--   0 runner    (1001) docker     (116)      121 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/ptm_scoring/PTMScoring.pyx
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore/parsing/
--rw-r--r--   0 runner    (1001) docker     (116)      159 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    27002 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/parsing/id_parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)     8891 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/pyascore/parsing/spec_parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)      560 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/test/
--rw-r--r--   0 runner    (1001) docker     (116)     3572 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (116)    26267 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/test_modified_peptide_container.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/test/example_inputs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/test/example_inputs/psms/
--rw-r--r--   0 runner    (1001) docker     (116)    39634 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/example_inputs/psms/test_psms.pep.xml
--rw-r--r--   0 runner    (1001) docker     (116)    32111 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/example_inputs/psms/test_psms.mzid
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/test/example_inputs/spectra/
--rw-r--r--   0 runner    (1001) docker     (116)    50778 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/example_inputs/spectra/test_spectra.mzXML
--rw-r--r--   0 runner    (1001) docker     (116)    89239 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/example_inputs/spectra/test_spectra.mzML
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/test/match_spectra_pairs/
--rw-r--r--   0 runner    (1001) docker     (116)    84735 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/match_spectra_pairs/velos_spectra_2_mods.pkl
--rw-r--r--   0 runner    (1001) docker     (116)     1651 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/match_spectra_pairs/velos_matches_1_mods.pkl
--rw-r--r--   0 runner    (1001) docker     (116)    88783 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/match_spectra_pairs/velos_spectra_3_mods.pkl
--rw-r--r--   0 runner    (1001) docker     (116)     1763 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/match_spectra_pairs/velos_matches_2_mods.pkl
--rw-r--r--   0 runner    (1001) docker     (116)      389 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/match_spectra_pairs/velos_matches_aux.pkl
--rw-r--r--   0 runner    (1001) docker     (116)     3667 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/match_spectra_pairs/velos_spectra_aux.pkl
--rw-r--r--   0 runner    (1001) docker     (116)    63307 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/match_spectra_pairs/velos_spectra_1_mods.pkl
--rw-r--r--   0 runner    (1001) docker     (116)     1983 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/match_spectra_pairs/velos_matches_3_mods.pkl
--rw-r--r--   0 runner    (1001) docker     (116)    12439 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/test_id_parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1953 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/test_spec_parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)     7658 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/test_ascore.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/test/pyteomics_examples/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/test/pyteomics_examples/mzml/
--rw-r--r--   0 runner    (1001) docker     (116)    48186 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/pyteomics_examples/mzml/velos_mzml_examples.pkl
--rw-r--r--   0 runner    (1001) docker     (116)    48055 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/pyteomics_examples/mzml/qexactive_mzml_examples.pkl
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/test/pyteomics_examples/pepxml/
--rw-r--r--   0 runner    (1001) docker     (116)    15789 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/pyteomics_examples/pepxml/comet_velos_pepxml_examples.pkl
--rw-r--r--   0 runner    (1001) docker     (116)     3432 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/pyteomics_examples/pepxml/percolator_velos_pepxml_examples.pkl
--rw-r--r--   0 runner    (1001) docker     (116)    20741 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/pyteomics_examples/pepxml/comet_qexactive_pepxml_examples.pkl
--rw-r--r--   0 runner    (1001) docker     (116)     6320 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/pyteomics_examples/pepxml/percolator_qexactive_pepxml_examples.pkl
--rw-r--r--   0 runner    (1001) docker     (116)     2539 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/test/test_spectra_container.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      804 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (116)     2798 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/source/api/modified_peptides.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3201 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/source/api/scoring.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3637 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2876 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/source/api/parsing.rst
--rw-r--r--   0 runner    (1001) docker     (116)     7598 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4440 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2037 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      638 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     1714 2022-04-24 20:55:46.000000 pyascore-0.7.0b0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7756 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       53 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      174 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2556 2022-04-24 20:56:11.000000 pyascore-0.7.0b0/pyascore.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/.github/workflows/linux-build.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/.github/workflows/mac-build.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/.github/workflows/windows-build.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7791 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7062 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     3637 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2798 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/source/api/modified_peptides.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/source/api/parsing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3201 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/source/api/scoring.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7598 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4434 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore/
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6490 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5854 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27074 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/parsing/id_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8927 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/parsing/spec_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/Ascore.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    12170 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/Ascore.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/ModifiedPeptide.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    13379 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/ModifiedPeptide.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   897485 2023-04-30 03:54:21.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/PTMScoring.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/PTMScoring.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/Spectra.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/Spectra.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      702 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/Util.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/Util.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/
+-rw-r--r--   0 runner    (1001) docker     (122)    12133 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Ascore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Ascore.h
+-rw-r--r--   0 runner    (1001) docker     (122)    21996 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/ModifiedPeptide.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3711 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/ModifiedPeptide.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3867 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Spectra.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Spectra.h
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Types.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4660 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Util.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Util.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7791 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/pyascore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/static/
+-rw-r--r--   0 runner    (1001) docker     (122)    33955 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/test/example_inputs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/test/example_inputs/psms/
+-rw-r--r--   0 runner    (1001) docker     (122)    32111 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/example_inputs/psms/test_psms.mzid
+-rw-r--r--   0 runner    (1001) docker     (122)    39634 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/example_inputs/psms/test_psms.pep.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/test/example_inputs/spectra/
+-rw-r--r--   0 runner    (1001) docker     (122)    89239 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/example_inputs/spectra/test_spectra.mzML
+-rw-r--r--   0 runner    (1001) docker     (122)    50778 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/example_inputs/spectra/test_spectra.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/test/match_spectra_pairs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/match_spectra_pairs/velos_matches_1_mods.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/match_spectra_pairs/velos_matches_2_mods.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)     1983 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/match_spectra_pairs/velos_matches_3_mods.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/match_spectra_pairs/velos_matches_aux.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)    63307 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/match_spectra_pairs/velos_spectra_1_mods.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)    84735 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/match_spectra_pairs/velos_spectra_2_mods.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)    88783 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/match_spectra_pairs/velos_spectra_3_mods.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/match_spectra_pairs/velos_spectra_aux.pkl
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/test/pyteomics_examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/test/pyteomics_examples/mzml/
+-rw-r--r--   0 runner    (1001) docker     (122)    48055 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/pyteomics_examples/mzml/qexactive_mzml_examples.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)    48186 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/pyteomics_examples/mzml/velos_mzml_examples.pkl
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 03:54:22.000000 pyascore-1.0.0b0/test/pyteomics_examples/pepxml/
+-rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/pyteomics_examples/pepxml/comet_qexactive_pepxml_examples.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)    15789 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/pyteomics_examples/pepxml/comet_velos_pepxml_examples.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)     6320 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/pyteomics_examples/pepxml/percolator_qexactive_pepxml_examples.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/pyteomics_examples/pepxml/percolator_velos_pepxml_examples.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)     7658 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/test_ascore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12439 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/test_id_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26267 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/test_modified_peptide_container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/test_spec_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/test_spectra_container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3572 2023-04-30 03:53:57.000000 pyascore-1.0.0b0/test/test_util.py
```

### Comparing `pyascore-0.7.0b0/static/logo.png` & `pyascore-1.0.0b0/static/logo.png`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/.github/workflows/linux-build.yml` & `pyascore-1.0.0b0/.github/workflows/linux-build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
   unittest:
 
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.6", "3.7", "3.8", "3.9"]
 
     steps:
     - uses: actions/checkout@v2
```

### Comparing `pyascore-0.7.0b0/.github/workflows/windows-build.yml` & `pyascore-1.0.0b0/.github/workflows/windows-build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -30,13 +30,12 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
         architecture: x64
     - name: Install in place
       run: |
-        $env:PYASCORE_COMPILE_ARGS = '/std:c++latest'
         python -m pip install --upgrade pip
         pip install -e .
     - name: Run python unittest
       run:
         python -m unittest
```

### Comparing `pyascore-0.7.0b0/.github/workflows/publish.yml` & `pyascore-1.0.0b0/.github/workflows/publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 on:
   release:
     types: [created]
 
 jobs:
   deploy-src:
 
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     strategy:
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
-        python-version: 3.6
+        python-version: 3.7
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install twine build
     - name: Build and publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
       run: |
         python -m build --sdist .
         twine upload dist/*
 
   deploy-linux-wheel:
 
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.6", "3.7", "3.8", "3.9"]
 
     steps:
     - uses: actions/checkout@v2
@@ -63,14 +63,40 @@
       run: |
         python -m build --wheel .
         auditwheel repair --plat manylinux_2_27_x86_64 dist/*.whl
         mv wheelhouse/* dist
         rm dist/*-linux_x86_64.whl
         twine upload dist/*
 
+  deploy-mac-wheel:
+
+    runs-on: macos-12
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.6", "3.7", "3.8", "3.9"]
+
+    steps:
+      - uses: actions/checout@v2
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install wheel auditwheel twine build
+      - name: Build and publish
+        env:
+          TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
+          TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
+        run: |
+          python -m build --wheel .
+          twine upload dist/*
+
   deploy-windows-wheel:
 
     runs-on: windows-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.6", "3.7", "3.8", "3.9"]
```

### Comparing `pyascore-0.7.0b0/PKG-INFO` & `pyascore-1.0.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pyascore
-Version: 0.7.0b0
+Version: 1.0.0b0
 Summary: A python module for fast post translational modification localization.
 Home-page: https://github.com/AnthonyOfSeattle/pyAscore
 Author: Anthony S. Barente
 Author-email: valenta4@uw.edu
 License: MIT
 Project-URL: Documentation, https://pyascore.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/AnthonyOfSeattle/pyAscore/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE.md
 
 <img src="https://raw.githubusercontent.com/AnthonyOfSeattle/pyAscore/main/static/logo.png" width="300" title="pyAscore Logo">
 
-![Linux Build](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/linux-build.yml/badge.svg)
-[![Windows Build](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/windows-build.yml/badge.svg)](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/windows-build.yml)
+[![Linux Build](https://github.com/Villen-Lab/pyAscore/actions/workflows/linux-build.yml/badge.svg)](https://github.com/Villen-Lab/pyAscore/actions/workflows/linux-build.yml)
+[![Windows Build](https://github.com/Villen-Lab/pyAscore/actions/workflows/windows-build.yml/badge.svg)](https://github.com/Villen-Lab/pyAscore/actions/workflows/windows-build.yml)
 [![Documentation Status](https://readthedocs.org/projects/pyascore/badge/?version=latest)](https://pyascore.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/pyascore?color=green)](https://pypi.org/project/pyascore/)
 
 ## Intro
 
 The **pyAscore** package provides a blazingly fast implementation of the Ascore algorithm for localizing peptide post-translational modifications from mass spectrometry data.
 In order to provide efficient scoring, pyAscore implements dynamic programming over a custom modified peptide fragment tree and caches scoring calculations whenever possible.
@@ -47,15 +46,15 @@
 ```
 
 ### Installing from a local clone
 
 If you would like to contribute, first fork the main repository, and then follow the following steps to compile and test.
 
 ```
-git clone https://github.com/YOUR-USERNAME/pyAscore.git
+git clone https://github.com/[USERNAME]/pyAscore.git
 cd pyAscore
 python setup.py build_ext --inplace
 python -m unittest 
 ```
 ### Usage
 
 The pyAscore package can be used straight from the command line as a module. 
@@ -146,9 +145,7 @@
                         The type of file supplied for spectra. One of mzML or
                         mzXML. Default: mzML.
   --ident_file_type IDENT_FILE_TYPE
                         The type of file supplied for identifications. One of
                         pepXML, mzIdentML, percolatorTXT, or mokapotTXT.
                         Default: pepXML.
 ```
-
-
```

### Comparing `pyascore-0.7.0b0/README.md` & `pyascore-1.0.0b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <img src="https://raw.githubusercontent.com/AnthonyOfSeattle/pyAscore/main/static/logo.png" width="300" title="pyAscore Logo">
 
-![Linux Build](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/linux-build.yml/badge.svg)
-[![Windows Build](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/windows-build.yml/badge.svg)](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/windows-build.yml)
+[![Linux Build](https://github.com/Villen-Lab/pyAscore/actions/workflows/linux-build.yml/badge.svg)](https://github.com/Villen-Lab/pyAscore/actions/workflows/linux-build.yml)
+[![Windows Build](https://github.com/Villen-Lab/pyAscore/actions/workflows/windows-build.yml/badge.svg)](https://github.com/Villen-Lab/pyAscore/actions/workflows/windows-build.yml)
 [![Documentation Status](https://readthedocs.org/projects/pyascore/badge/?version=latest)](https://pyascore.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/pyascore?color=green)](https://pypi.org/project/pyascore/)
 
 ## Intro
 
 The **pyAscore** package provides a blazingly fast implementation of the Ascore algorithm for localizing peptide post-translational modifications from mass spectrometry data.
 In order to provide efficient scoring, pyAscore implements dynamic programming over a custom modified peptide fragment tree and caches scoring calculations whenever possible.
@@ -27,15 +27,15 @@
 ```
 
 ### Installing from a local clone
 
 If you would like to contribute, first fork the main repository, and then follow the following steps to compile and test.
 
 ```
-git clone https://github.com/YOUR-USERNAME/pyAscore.git
+git clone https://github.com/[USERNAME]/pyAscore.git
 cd pyAscore
 python setup.py build_ext --inplace
 python -m unittest 
 ```
 ### Usage
 
 The pyAscore package can be used straight from the command line as a module.
```

### Comparing `pyascore-0.7.0b0/LICENSE.md` & `pyascore-1.0.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/setup.cfg` & `pyascore-1.0.0b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/config.py` & `pyascore-1.0.0b0/pyascore/config.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/__main__.py` & `pyascore-1.0.0b0/pyascore/__main__.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/__init__.py` & `pyascore-1.0.0b0/pyascore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/Ascore.pxd` & `pyascore-1.0.0b0/pyascore/ptm_scoring/Ascore.pxd`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/ModifiedPeptide.pxd` & `pyascore-1.0.0b0/pyascore/ptm_scoring/ModifiedPeptide.pxd`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/Spectra.pyx` & `pyascore-1.0.0b0/pyascore/ptm_scoring/Spectra.pyx`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/Util.pxd` & `pyascore-1.0.0b0/pyascore/ptm_scoring/Util.pxd`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/Util.pyx` & `pyascore-1.0.0b0/pyascore/ptm_scoring/Util.pyx`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/Ascore.pyx` & `pyascore-1.0.0b0/pyascore/ptm_scoring/Ascore.pyx`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Util.h` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Util.h`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Util.cpp` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Util.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     float BinomialDist::log_pvalue (size_t successes, size_t trials) {
         if (successes > trials) {
             std::cout << "ERROR -- Successes more than trials:" << successes << " > " << trials << std::endl;
             throw 10;
         } else if (successes == 0) { return 0.; }
 
         size_t starting_k = successes;
-        while(cache.count(bit_concat(starting_k, trials)) == 0 and starting_k < trials + 1) {
+        while((cache.count(bit_concat(starting_k, trials)) == 0) && (starting_k < trials + 1)) {
             starting_k++;
         }
 
         if (starting_k == trials + 1) {cache[bit_concat(trials + 1, trials)] = -INFINITY;}
 
         for (starting_k--; starting_k >= successes; starting_k--) {
             cache[bit_concat(starting_k, trials)] = lmath.log_sum(cache.at(bit_concat(starting_k + 1, trials)),
```

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/ModifiedPeptide.cpp` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/ModifiedPeptide.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -128,18 +128,18 @@
         it = lower_bound(fragments.begin(), fragments.end(), mz - .5);
 
         float ppm_low;
         float ppm_high;
         for(; it < fragments.end(); it++) {
             ppm_low = *it - mz_error;
             ppm_high = *it + mz_error;
-            if (mz > ppm_low and mz < ppm_high) {
-                if (!fragment_scores.count(*it) or std::get<1>(fragment_scores.at(*it)) > rank) {
-                    fragment_scores[*it] = {mz, rank}; // The theoretical mz needs to be the key
-                }
+            if ((mz > ppm_low) && (mz < ppm_high)) {
+		    if ((!fragment_scores.count(*it)) || (std::get<1>(fragment_scores.at(*it)) > rank)) {
+			    fragment_scores[*it] = {mz, rank}; // The theoretical mz needs to be the key
+		    }
             } else if (mz < ppm_low) {break;}
         }
 
     }
 
     bool ModifiedPeptide::hasMatch (float mz) const {
         return fragment_scores.count(mz);
@@ -179,15 +179,15 @@
             if (res_it.size() > 1) {n_modifiable += 1;} 
         }
         return n_modifiable;
     }
 
     size_t ModifiedPeptide::getPosOfNthModifiable (size_t n) const {
         for (size_t ind = 0; ind < residues.size(); ind++) {
-            if (residues.at(ind).size() > 1 and n == 0) {
+            if ((residues.at(ind).size() > 1) && (n == 0)) {
                 return ind;
             } else if (residues.at(ind).size() > 1) {
                 n--;
             }
         }
         return residues.size();
     }
@@ -432,15 +432,15 @@
         // Don't attempt to increment if signature end
         if (isSignatureEnd()) {throw 40;}
         
         // Otherwise, one mod is outstanding to start
         n_mods_outstanding = 1;
         size_t final_index = modified_peptide->residues.size();
         for (std::vector<size_t>::iterator it = --modifiable.end();
-             it >= modifiable.begin() and n_mods_outstanding; 
+             it >= modifiable.begin() && n_mods_outstanding; 
              it--) {
             if ( signature.at(*it) > 0 ) {
                 final_index = *it;
                 signature.at(*it) = 0;
 
                 size_t n_pos_until_end = modifiable.end() - it;
                 if (  n_mods_outstanding == n_pos_until_end ) {
@@ -495,15 +495,15 @@
         resetResidueInd();
         calculateFragment();
         updateLosses();
     }
 
     void ModifiedPeptide::FragmentGraph::incrFragment () {
         // Don't increment if fragment end or signature end
-        if (isSignatureEnd() or isFragmentEnd()) {throw 40;}
+        if (isSignatureEnd() || isFragmentEnd()) {throw 40;}
 
         // Only increment residue if more losses are not available
         if ( neutral_loss_iter.hasNext() ) {
             neutral_loss_iter.next();
         } else {
             incrResidueInd();
             if (!isFragmentEnd()) {
```

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Spectra.cpp` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Spectra.cpp`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/ModifiedPeptide.h` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/ModifiedPeptide.h`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Types.h` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Types.h`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Spectra.h` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Spectra.h`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Ascore.h` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Ascore.h`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/cpp/Ascore.cpp` & `pyascore-1.0.0b0/pyascore/ptm_scoring/cpp/Ascore.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,14 @@
             }
         }
     }
 
     bool Ascore::isUnambiguous () {
 
         if (modified_peptide_ptr->getNumberOfMods() >= modified_peptide_ptr->getNumberModifiable()){
-            peptide_scores_.push_back( {} );
-            peptide_scores_.front().signature.resize(modified_peptide_ptr->getNumberOfMods(), 1);
-            peptide_scores_.front().weighted_score = std::numeric_limits<float>::infinity();
             for (size_t ind = 0; ind < modified_peptide_ptr->getNumberOfMods(); ind++){
                 ascore_containers_.push_back({
                     ind, {}, {}, {std::numeric_limits<float>::infinity()}
                 });
             }
             return true;
         } else {
@@ -181,23 +178,23 @@
             std::vector<std::vector<float>> ions = modified_peptide_ptr->getSiteDeterminingIons(
                 ref.signature, other.signature, fragment_type,
 		modified_peptide_ptr->getMaxFragmentCharge()
             );
 
             ion_trials[0] += ions[0].size();
             for (float mz : ions[0]){
-                if (modified_peptide_ptr->hasMatch(mz) and
+                if (modified_peptide_ptr->hasMatch(mz) &&
                     std::get<1>(modified_peptide_ptr->getMatch(mz)) <= max_score_depth){
                     ion_counts[0]++;
                 }
             }
 
             ion_trials[1] += ions[1].size();
             for (float mz : ions[1]){
-                if (modified_peptide_ptr->hasMatch(mz) and
+                if (modified_peptide_ptr->hasMatch(mz) &&
                     std::get<1>(modified_peptide_ptr->getMatch(mz)) <= max_score_depth){
                     ion_counts[1]++;
                 }
             }
         }
 
         std::vector<float> scores(2);
@@ -226,19 +223,19 @@
 
             size_t same_count = 0;
             size_t ascore_ind = 0;
             size_t comp_sig_ind = 0;
             std::vector<size_t>::iterator best_it = best_score.signature.begin();
             std::vector<size_t>::iterator comp_it = competing_score.signature.begin();
             for (; best_it < best_score.signature.end(); best_it++, comp_it++) {
-                if (*best_it and *comp_it) {
+                if (*best_it && *comp_it) {
                     same_count++;
-                } else if (*best_it and not *comp_it) {
+                } else if (*best_it && (!*comp_it)) {
                     ascore_ind = same_count;
-                } else if (not *best_it and *comp_it) {
+                } else if ((! *best_it) && *comp_it) {
                     comp_sig_ind = comp_it - competing_score.signature.begin();
                 }
             }
 
             AscoreContainer & cont = ascore_containers_.at(ascore_ind);
             if (cont.ascores.empty() || 
                 competing_score.weighted_score == cont.pep_scores.back() ) {
@@ -260,17 +257,18 @@
                         const ModifiedPeptide & modified_peptide) {
         // Reinitialize for every peptide that comes in
         modified_peptide_ptr = &modified_peptide;
         binned_spectra_ptr = &binned_spectra;
         resetInternalState();
 
         // Score pipeline
-        if ( not isUnambiguous() ){
-            accumulateCounts();
-            calculateFullScores();
+	accumulateCounts();
+        calculateFullScores();
+	    
+        if ( !isUnambiguous() ){
             sortScores();
             calculateAscores();
         }
     }
 
     std::string Ascore::getBestSequence () {
         if ( peptide_scores_.size() ) {
```

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/PTMScoring.cpp` & `pyascore-1.0.0b0/pyascore/ptm_scoring/PTMScoring.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/core/include"
+            "/tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "pyascore.ptm_scoring",
         "sources": [
             "pyascore/ptm_scoring/PTMScoring.pyx"
         ]
     },
@@ -25,16 +28,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -65,14 +68,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -101,18 +105,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -142,18 +150,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -165,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -195,31 +252,34 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -525,35 +585,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -677,16 +737,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -715,14 +777,17 @@
 
 #define __PYX_HAVE__pyascore__ptm_scoring
 #define __PYX_HAVE_API__pyascore__ptm_scoring
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "cpp/Spectra.cpp"
 #include "ios"
 #include "new"
@@ -1008,195 +1073,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1232,42 +1297,42 @@
 struct __pyx_obj_8pyascore_11ptm_scoring_PyAscore;
 struct __pyx_obj_8pyascore_11ptm_scoring_PyLogMath;
 struct __pyx_obj_8pyascore_11ptm_scoring_PyBinomialDist;
 struct __pyx_obj_8pyascore_11ptm_scoring_PyPowerSetSum;
 struct __pyx_obj_8pyascore_11ptm_scoring___pyx_scope_struct__iter_permutations;
 struct __pyx_obj_8pyascore_11ptm_scoring___pyx_scope_struct_1_iter_fragments;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1638,26 +1703,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1703,14 +1768,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1845,20 +1916,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -2207,14 +2286,24 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
+static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
+static PyTypeObject *__pyx_ptype_5numpy_number = 0;
+static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
+static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
+static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
+static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
+static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
+static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'Spectra' */
 
 /* Module declarations from 'libcpp.vector' */
 
 /* Module declarations from 'libcpp.string' */
@@ -11657,15 +11746,15 @@
   __Pyx_AddTraceback("pyascore.ptm_scoring.PyPowerSetSum.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -11674,29 +11763,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -11707,15 +11796,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -11724,29 +11813,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -11757,15 +11846,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -11774,29 +11863,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -11807,15 +11896,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11824,29 +11913,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -11857,15 +11946,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11874,29 +11963,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -11907,212 +11996,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":868
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":869
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":870
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":868
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":872
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":873
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":874
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":875
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":874
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":876
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":872
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":880
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -12128,15 +12217,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":881
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -12144,84 +12233,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":882
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 882, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":881
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":883
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 883, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":884
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 884, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(5, 884, __pyx_L5_except_error)
+      __PYX_ERR(5, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":881
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":880
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -12236,15 +12325,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":886
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12260,15 +12349,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":887
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -12276,84 +12365,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":888
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 888, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":887
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":889
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 889, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":890
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 890, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(5, 890, __pyx_L5_except_error)
+      __PYX_ERR(5, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":887
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":886
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12368,15 +12457,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":892
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12392,15 +12481,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":893
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -12408,84 +12497,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":894
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 894, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":893
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":895
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 895, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":896
+      /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 896, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(5, 896, __pyx_L5_except_error)
+      __PYX_ERR(5, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":893
+    /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":892
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -12500,14 +12589,188 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":979
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":967
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":994
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":982
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":1004
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":997
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":1011
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":1007
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":1018
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":1014
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
 /* "vector.from_py":45
  * 
  * @cname("__pyx_convert_vector_from_py_size_t")
  * cdef vector[X] __pyx_convert_vector_from_py_size_t(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef vector[X] v
  *     for item in o:
  */
@@ -15070,15 +15333,15 @@
   {&__pyx_n_u_weighted_score, __pyx_k_weighted_score, sizeof(__pyx_k_weighted_score), 0, 1, 0, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 95, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(5, 884, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(5, 945, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 18, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 19, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -15215,33 +15478,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":884
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(5, 884, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(5, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "../../../../../tmp/build-env-siu8no61/lib/python3.6/site-packages/numpy/__init__.pxd":890
+  /* "../../../../../tmp/build-env-txrtpian/lib/python3.7/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(5, 890, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(5, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "FromPyStructUtility":19
  *         value = obj['signature']
  *     except KeyError:
  *         raise ValueError("No value specified for struct attribute 'signature'")             # <<<<<<<<<<<<<<
@@ -15310,15 +15573,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(6, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(6, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(6, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -15461,33 +15724,68 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(7, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(5, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(5, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(5, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(5, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(5, 764, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(5, 200, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(5, 223, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(5, 227, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(5, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(5, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(5, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(5, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(5, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(5, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(5, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(5, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(5, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(5, 787, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(5, 789, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(5, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -15673,15 +15971,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(6, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(6, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(6, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(6, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(6, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(6, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(6, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pyascore__ptm_scoring) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(6, 1, __pyx_L1_error)
@@ -16760,28 +17058,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -17046,15 +17344,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -17322,15 +17620,15 @@
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -17758,25 +18056,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
+#if CYTHON_USE_PYTYPE_LOOKUP
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+#else
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
 #endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -17813,57 +18129,77 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -17950,15 +18286,15 @@
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -18074,14 +18410,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -18137,22 +18479,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -18357,15 +18709,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -18511,15 +18863,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -19649,14 +20001,20 @@
     if (unlikely(!method)) return NULL;
     return __Pyx__PyObject_CallMethod1(method, arg);
 }
 
 /* CoroutineBase */
   #include <structmember.h>
 #include <frameobject.h>
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
 static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
@@ -20636,19 +20994,41 @@
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
```

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/Spectra.pxd` & `pyascore-1.0.0b0/pyascore/ptm_scoring/Spectra.pxd`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/ptm_scoring/ModifiedPeptide.pyx` & `pyascore-1.0.0b0/pyascore/ptm_scoring/ModifiedPeptide.pyx`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore/parsing/id_parsers.py` & `pyascore-1.0.0b0/pyascore/parsing/id_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,24 +697,24 @@
                  score_lower_better=True,
                  score_func=None,
                  static_mods={"C": 57.021464},
                  spec_file_name=None):
 
         # Define a bridge to ID file handling classes
         if id_file_format == "mzIdentML":
-            self._reader = MzIdentML(id_file_name)
+            self._reader = MzIdentML(id_file_name, queue_size=32767)
             self._extractor = MzIdentMLExtractor(score_string)
         elif id_file_format == "pepXML":
-            self._reader = PepXML(id_file_name)
+            self._reader = PepXML(id_file_name, queue_size=32767)
             self._extractor = PepXMLExtractor(score_string)
         elif id_file_format == "percolatorTXT":
-            self._reader = PercolatorTXT(id_file_name)
+            self._reader = PercolatorTXT(id_file_name, queue_size=32767)
             self._extractor = PercolatorTXTExtractor(score_string, static_mods)
         elif id_file_format == "mokapotTXT":
-            self._reader = MokapotTXT(id_file_name)
+            self._reader = MokapotTXT(id_file_name, queue_size=32767)
             self._extractor = MokapotTXTExtractor(score_string, static_mods)
         else:
             raise ValueError("{} not supported at this time."
                              " Must be on of: mzIdentML, pepXML,"
                              " percolatorTXT, or mokapotTXT".format(id_file_format))
         
         # Define containers for modification information
```

### Comparing `pyascore-0.7.0b0/pyascore/parsing/spec_parsers.py` & `pyascore-1.0.0b0/pyascore/parsing/spec_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,18 +200,18 @@
                  spec_file_name,
                  spec_file_format,
                  ms_level=2,
                  custom_filter=None):
 
         # Define a bridge to spectra file handling classes
         if spec_file_format == "mzML":
-            self._reader = MzML(spec_file_name)
+            self._reader = MzML(spec_file_name, queue_size=32767)
             self._extractor = MzMLExtractor()
         elif spec_file_format == "mzXML":
-            self._reader = MzXML(spec_file_name)
+            self._reader = MzXML(spec_file_name, queue_size=32767)
             self._extractor = MzXMLExtractor()
         else:
             raise ValueError("{} not supported at this time."
                              " Should be one of: mzML or mzXML".format(spec_file_format))
 
 
         # Store filtering criteria
```

### Comparing `pyascore-0.7.0b0/setup.py` & `pyascore-1.0.0b0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from setuptools import setup, Extension
 from Cython.Build import cythonize
 from os import path, environ
+from sys import platform
 
 import numpy as np
 
 extra_compile_args=[]
 if "PYASCORE_COMPILE_ARGS" in environ:
     extra_compile_args=environ["PYASCORE_COMPILE_ARGS"].split()
 
+if platform == "darwin":
+    extra_compile_args.append('-std=c++11')
+
 SRC_DIR = "pyascore"
 EXT = [
     Extension(SRC_DIR + ".ptm_scoring",
               [SRC_DIR + "/ptm_scoring/PTMScoring.pyx"],
               include_dirs=[np.get_include()],
               extra_compile_args=extra_compile_args)
 ]
```

### Comparing `pyascore-0.7.0b0/test/test_util.py` & `pyascore-1.0.0b0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/test_modified_peptide_container.py` & `pyascore-1.0.0b0/test/test_modified_peptide_container.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/example_inputs/psms/test_psms.pep.xml` & `pyascore-1.0.0b0/test/example_inputs/psms/test_psms.pep.xml`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/example_inputs/psms/test_psms.mzid` & `pyascore-1.0.0b0/test/example_inputs/psms/test_psms.mzid`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/example_inputs/spectra/test_spectra.mzXML` & `pyascore-1.0.0b0/test/example_inputs/spectra/test_spectra.mzXML`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/example_inputs/spectra/test_spectra.mzML` & `pyascore-1.0.0b0/test/example_inputs/spectra/test_spectra.mzML`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/match_spectra_pairs/velos_spectra_2_mods.pkl` & `pyascore-1.0.0b0/test/match_spectra_pairs/velos_spectra_2_mods.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/match_spectra_pairs/velos_matches_1_mods.pkl` & `pyascore-1.0.0b0/test/match_spectra_pairs/velos_matches_1_mods.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/match_spectra_pairs/velos_spectra_3_mods.pkl` & `pyascore-1.0.0b0/test/match_spectra_pairs/velos_spectra_3_mods.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/match_spectra_pairs/velos_matches_2_mods.pkl` & `pyascore-1.0.0b0/test/match_spectra_pairs/velos_matches_2_mods.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/match_spectra_pairs/velos_spectra_aux.pkl` & `pyascore-1.0.0b0/test/match_spectra_pairs/velos_spectra_aux.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/match_spectra_pairs/velos_spectra_1_mods.pkl` & `pyascore-1.0.0b0/test/match_spectra_pairs/velos_spectra_1_mods.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/match_spectra_pairs/velos_matches_3_mods.pkl` & `pyascore-1.0.0b0/test/match_spectra_pairs/velos_matches_3_mods.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/test_id_parsers.py` & `pyascore-1.0.0b0/test/test_id_parsers.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/test_spec_parsers.py` & `pyascore-1.0.0b0/test/test_spec_parsers.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/test_ascore.py` & `pyascore-1.0.0b0/test/test_ascore.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/pyteomics_examples/mzml/velos_mzml_examples.pkl` & `pyascore-1.0.0b0/test/pyteomics_examples/mzml/velos_mzml_examples.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/pyteomics_examples/mzml/qexactive_mzml_examples.pkl` & `pyascore-1.0.0b0/test/pyteomics_examples/mzml/qexactive_mzml_examples.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/pyteomics_examples/pepxml/comet_velos_pepxml_examples.pkl` & `pyascore-1.0.0b0/test/pyteomics_examples/pepxml/comet_velos_pepxml_examples.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/pyteomics_examples/pepxml/percolator_velos_pepxml_examples.pkl` & `pyascore-1.0.0b0/test/pyteomics_examples/pepxml/percolator_velos_pepxml_examples.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/pyteomics_examples/pepxml/comet_qexactive_pepxml_examples.pkl` & `pyascore-1.0.0b0/test/pyteomics_examples/pepxml/comet_qexactive_pepxml_examples.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/pyteomics_examples/pepxml/percolator_qexactive_pepxml_examples.pkl` & `pyascore-1.0.0b0/test/pyteomics_examples/pepxml/percolator_qexactive_pepxml_examples.pkl`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/test/test_spectra_container.py` & `pyascore-1.0.0b0/test/test_spectra_container.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/docs/make.bat` & `pyascore-1.0.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/docs/source/api/modified_peptides.rst` & `pyascore-1.0.0b0/docs/source/api/modified_peptides.rst`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/docs/source/api/scoring.rst` & `pyascore-1.0.0b0/docs/source/api/scoring.rst`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/docs/source/api/index.rst` & `pyascore-1.0.0b0/docs/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/docs/source/api/parsing.rst` & `pyascore-1.0.0b0/docs/source/api/parsing.rst`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/docs/source/cli.rst` & `pyascore-1.0.0b0/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/docs/source/index.rst` & `pyascore-1.0.0b0/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
    $ pip install pyascore
 
 If you would like to contribute, first fork the main repository, and then follow
 the following steps to compile and test.
 
 .. code-block:: bash
 
-   $ git clone https://github.com/AnthonyOfSeattle/pyAscore.git
+   $ git clone https://github.com/[USERNAME]/pyAscore.git
    $ cd pyAscore
    $ python setup.py build_ext --inplace
    $ python -m unittest 
 
 Basic Usage
 -----------
```

### Comparing `pyascore-0.7.0b0/docs/source/conf.py` & `pyascore-1.0.0b0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/docs/Makefile` & `pyascore-1.0.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/.gitignore` & `pyascore-1.0.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyascore-0.7.0b0/pyascore.egg-info/PKG-INFO` & `pyascore-1.0.0b0/pyascore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pyascore
-Version: 0.7.0b0
+Version: 1.0.0b0
 Summary: A python module for fast post translational modification localization.
 Home-page: https://github.com/AnthonyOfSeattle/pyAscore
 Author: Anthony S. Barente
 Author-email: valenta4@uw.edu
 License: MIT
 Project-URL: Documentation, https://pyascore.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/AnthonyOfSeattle/pyAscore/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE.md
 
 <img src="https://raw.githubusercontent.com/AnthonyOfSeattle/pyAscore/main/static/logo.png" width="300" title="pyAscore Logo">
 
-![Linux Build](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/linux-build.yml/badge.svg)
-[![Windows Build](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/windows-build.yml/badge.svg)](https://github.com/AnthonyOfSeattle/pyAscore/actions/workflows/windows-build.yml)
+[![Linux Build](https://github.com/Villen-Lab/pyAscore/actions/workflows/linux-build.yml/badge.svg)](https://github.com/Villen-Lab/pyAscore/actions/workflows/linux-build.yml)
+[![Windows Build](https://github.com/Villen-Lab/pyAscore/actions/workflows/windows-build.yml/badge.svg)](https://github.com/Villen-Lab/pyAscore/actions/workflows/windows-build.yml)
 [![Documentation Status](https://readthedocs.org/projects/pyascore/badge/?version=latest)](https://pyascore.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/pyascore?color=green)](https://pypi.org/project/pyascore/)
 
 ## Intro
 
 The **pyAscore** package provides a blazingly fast implementation of the Ascore algorithm for localizing peptide post-translational modifications from mass spectrometry data.
 In order to provide efficient scoring, pyAscore implements dynamic programming over a custom modified peptide fragment tree and caches scoring calculations whenever possible.
@@ -47,15 +46,15 @@
 ```
 
 ### Installing from a local clone
 
 If you would like to contribute, first fork the main repository, and then follow the following steps to compile and test.
 
 ```
-git clone https://github.com/YOUR-USERNAME/pyAscore.git
+git clone https://github.com/[USERNAME]/pyAscore.git
 cd pyAscore
 python setup.py build_ext --inplace
 python -m unittest 
 ```
 ### Usage
 
 The pyAscore package can be used straight from the command line as a module. 
@@ -146,9 +145,7 @@
                         The type of file supplied for spectra. One of mzML or
                         mzXML. Default: mzML.
   --ident_file_type IDENT_FILE_TYPE
                         The type of file supplied for identifications. One of
                         pepXML, mzIdentML, percolatorTXT, or mokapotTXT.
                         Default: pepXML.
 ```
-
-
```

### Comparing `pyascore-0.7.0b0/pyascore.egg-info/SOURCES.txt` & `pyascore-1.0.0b0/pyascore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .readthedocs.yaml
 LICENSE.md
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/linux-build.yml
+.github/workflows/mac-build.yml
 .github/workflows/publish.yml
 .github/workflows/windows-build.yml
 docs/Makefile
 docs/make.bat
 docs/source/cli.rst
 docs/source/conf.py
 docs/source/index.rst
```

