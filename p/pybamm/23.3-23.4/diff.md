# Comparing `tmp/pybamm-23.3.tar.gz` & `tmp/pybamm-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybamm-23.3.tar", last modified: Sat Apr  1 10:11:21 2023, max compression
+gzip compressed data, was "pybamm-23.4.tar", last modified: Sun Apr 30 16:34:27 2023, max compression
```

## Comparing `pybamm-23.3.tar` & `pybamm-23.4.tar`

### file list

```diff
@@ -1,457 +1,457 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.876129 pybamm-23.3/
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-01 10:11:18.000000 pybamm-23.3/CMakeBuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-01 10:11:18.000000 pybamm-23.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    41261 2023-04-01 10:11:21.876129 pybamm-23.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38852 2023-04-01 10:11:18.000000 pybamm-23.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.840129 pybamm-23.3/pybamm/
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/CITATIONS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/batch_study.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/citations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.840129 pybamm-23.3/pybamm/discretisations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/discretisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/discretisations/discretisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/doc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.840129 pybamm-23.3/pybamm/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/experiments/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.840129 pybamm-23.3/pybamm/expression_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/averages.py
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/binary_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/broadcasts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/concatenations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/independent_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/input_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/interpolant.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.844129 pybamm-23.3/pybamm/expression_tree/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/operations/convert_to_casadi.py
--rw-r--r--   0 runner    (1001) docker     (123)    26233 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/operations/evaluate_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/operations/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/operations/latexify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/operations/unpack_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.844129 pybamm-23.3/pybamm/expression_tree/printing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/printing/print_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/printing/sympy_overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/state_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/unary_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/expression_tree/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.844129 pybamm-23.3/pybamm/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/geometry/battery_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/geometry/standard_spatial_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.844129 pybamm-23.3/pybamm/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.836129 pybamm-23.3/pybamm/input/discharge_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.844129 pybamm-23.3/pybamm/input/discharge_data/Ecker2015/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Ecker2015/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.844129 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/
--rw-r--r--   0 runner    (1001) docker     (123)   685399 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)   180796 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   156316 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)   129670 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38056 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   125368 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)    63563 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)   158837 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30602 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    13539 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    13828 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.848129 pybamm-23.3/pybamm/input/drive_cycles/
--rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/drive_cycles/UDDS.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/drive_cycles/US06.csv
--rw-r--r--   0 runner    (1001) docker     (123)   299508 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/drive_cycles/WLTC.csv
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/drive_cycles/car_current.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.848129 pybamm-23.3/pybamm/input/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.848129 pybamm-23.3/pybamm/input/parameters/ecm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/ecm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.848129 pybamm-23.3/pybamm/input/parameters/ecm/data/
--rw-r--r--   0 runner    (1001) docker     (123)   135520 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_c1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149886 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_r0.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149222 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_r1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/ecm/example_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.848129 pybamm-23.3/pybamm/input/parameters/lead_acid/
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lead_acid/Sulzer2019.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lead_acid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.848129 pybamm-23.3/pybamm/input/parameters/lithium_ion/
--rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Chen2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Chen2020_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Ecker2015.py
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Marquis2019.py
--rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Mohtat2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py
--rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/OKane2022.py
--rw-r--r--   0 runner    (1001) docker     (123)    30791 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/ORegan2022.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Prada2013.py
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Ramadass2004.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/Xu2019.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.848129 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/lico2_data_example.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.836129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/cells/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/parameters.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/cells/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_TDF_EC_DMC_1_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_conductivity_EC_DMC_1_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_diffusivity_EC_DMC_1_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_transference_number_EC_DMC_1_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_TDF_EC_EMC_3_7_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_base_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_conductivity_EC_EMC_3_7_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_diffusivity_EC_EMC_3_7_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_transference_number_EC_EMC_3_7_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_TDF_EMC_FEC_19_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_conductivity_EMC_FEC_19_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_diffusivity_EMC_FEC_19_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_transference_number_EMC_FEC_19_1_Landesfeind2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/dlnf_dlnc_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_conductivity_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_diffusivity_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/experiments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/parameters.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.852129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_cracking_rate_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_diffusivity_Dualfoil1998.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_electrolyte_exchange_current_density_Dualfoil1998.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_volume_change_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_cracking_rate_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_diffusivity_Dualfoil1998.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_electrolyte_exchange_current_density_Dualfoil1998.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_entropic_change_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_entropic_change_Ai2020_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_volume_change_Ai2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.836129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/seis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/seis/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/seis/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/seis/example/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/separators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/separators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/parameters.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/install_odes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/meshes/meshes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/meshes/one_dimensional_submeshes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/meshes/scikit_fem_submeshes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/meshes/zero_dimensional_submesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47327 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/models/full_battery_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56548 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/base_battery_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/models/full_battery_models/equivalent_circuit/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/equivalent_circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.856129 pybamm-23.3/pybamm/models/full_battery_models/lead_acid/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lead_acid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lead_acid/basic_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lead_acid/full.py
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lead_acid/loqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/Yang2017.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/basic_spm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/dfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/mpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/spm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/spme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/active_material/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/active_material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/active_material/base_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/active_material/constant_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/active_material/loss_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/active_material/total_active_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/base_submodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/convection/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/base_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/convection/through_cell/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/through_cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/through_cell/explicit_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/through_cell/full_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/through_cell/no_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/convection/transverse/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/transverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/transverse/base_transverse_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/transverse/full_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/transverse/no_convection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/convection/transverse/uniform_convection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/current_collector/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/current_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/current_collector/base_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/current_collector/homogeneous_current_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/current_collector/potential_pair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/electrode/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/base_electrode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/electrode/ohm/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/ohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/ohm/base_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/ohm/composite_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/ohm/full_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/ohm/leading_ohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/ohm/li_metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.860129 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/external_circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/external_circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/external_circuit/base_external_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/external_circuit/function_control_external_circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/base_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/interface/kinetics/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/base_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/butler_volmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/diffusion_limited.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/interface/kinetics/inverse_kinetics/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/inverse_kinetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/marcus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/no_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/tafel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.864129 pybamm-23.3/pybamm/models/submodels/interface/lithium_plating/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/lithium_plating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/lithium_plating/base_plating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/lithium_plating/no_plating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/lithium_plating/plating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/interface/open_circuit_potential/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/open_circuit_potential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/interface/sei/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/sei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/sei/base_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/sei/constant_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/sei/no_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/sei/sei_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/sei/total_sei.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/interface/total_interfacial_current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/particle/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle/base_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle/fickian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle/polynomial_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle/total_particle_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/particle_mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle_mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle_mechanics/base_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle_mechanics/crack_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle_mechanics/no_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/particle_mechanics/swelling_only.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/porosity/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/porosity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/porosity/base_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/porosity/constant_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/porosity/reaction_driven_porosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/thermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/thermal/base_thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/thermal/isothermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/thermal/lumped.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/thermal/pouch_cell/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/thermal/pouch_cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/thermal/x_full.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.868129 pybamm-23.3/pybamm/models/submodels/transport_efficiency/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/transport_efficiency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.872129 pybamm-23.3/pybamm/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/base_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/bpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/ecm_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/electrical_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/geometric_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/lead_acid_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/lithium_ion_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/parameter_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)    43719 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/parameter_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/process_parameter_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/size_distribution_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters/thermal_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/parameters_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.872129 pybamm-23.3/pybamm/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/plotting/dynamic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/plotting/plot2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/plotting/plot_summary_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/plotting/plot_voltage_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/plotting/quick_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.872129 pybamm-23.3/pybamm/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/algebraic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    64653 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/base_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.872129 pybamm-23.3/pybamm/solvers/c_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/c_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/casadi_algebraic_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    31572 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/casadi_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/dummy_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20516 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/idaklu_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    39216 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/jax_bdf_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/jax_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/lrudict.py
--rw-r--r--   0 runner    (1001) docker     (123)    24251 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/processed_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/scikits_dae_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/scikits_ode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/scipy_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    31865 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/solvers/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.872129 pybamm-23.3/pybamm/spatial_methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/spatial_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57884 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/spatial_methods/finite_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/spatial_methods/scikit_finite_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/spatial_methods/spatial_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    28643 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/spatial_methods/spectral_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/spatial_methods/zero_dimensional_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 10:11:19.000000 pybamm-23.3/pybamm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 10:11:21.840129 pybamm-23.3/pybamm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41261 2023-04-01 10:11:21.000000 pybamm-23.3/pybamm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-04-01 10:11:21.000000 pybamm-23.3/pybamm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 10:11:21.000000 pybamm-23.3/pybamm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-01 10:11:21.000000 pybamm-23.3/pybamm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-01 10:11:21.000000 pybamm-23.3/pybamm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-01 10:11:21.000000 pybamm-23.3/pybamm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 10:11:21.876129 pybamm-23.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-01 10:11:19.000000 pybamm-23.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.855407 pybamm-23.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-30 16:34:20.000000 pybamm-23.4/CMakeBuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-30 16:34:20.000000 pybamm-23.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    41856 2023-04-30 16:34:27.855407 pybamm-23.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38853 2023-04-30 16:34:20.000000 pybamm-23.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.775407 pybamm-23.4/pybamm/
+-rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/CITATIONS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/batch_study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/citations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.779407 pybamm-23.4/pybamm/discretisations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/discretisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/discretisations/discretisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/doc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.779407 pybamm-23.4/pybamm/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/experiments/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.783407 pybamm-23.4/pybamm/expression_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/averages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/binary_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/broadcasts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/concatenations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/independent_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/input_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/interpolant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.783407 pybamm-23.4/pybamm/expression_tree/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/operations/convert_to_casadi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26233 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/operations/evaluate_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/operations/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/operations/latexify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/operations/unpack_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.787407 pybamm-23.4/pybamm/expression_tree/printing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/printing/print_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/printing/sympy_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/state_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/unary_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/expression_tree/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.787407 pybamm-23.4/pybamm/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/geometry/battery_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/geometry/standard_spatial_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.787407 pybamm-23.4/pybamm/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.763407 pybamm-23.4/pybamm/input/discharge_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.787407 pybamm-23.4/pybamm/input/discharge_data/Ecker2015/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Ecker2015/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.791407 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/
+-rw-r--r--   0 runner    (1001) docker     (123)   685399 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   180796 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   156316 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   129670 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38056 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   125368 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    63563 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   158837 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30602 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13539 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13828 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.795407 pybamm-23.4/pybamm/input/drive_cycles/
+-rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/drive_cycles/UDDS.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/drive_cycles/US06.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   299508 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/drive_cycles/WLTC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/drive_cycles/car_current.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.795407 pybamm-23.4/pybamm/input/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.795407 pybamm-23.4/pybamm/input/parameters/ecm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/ecm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.795407 pybamm-23.4/pybamm/input/parameters/ecm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   135520 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_c1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149886 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_r0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149222 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_r1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/ecm/example_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.795407 pybamm-23.4/pybamm/input/parameters/lead_acid/
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lead_acid/Sulzer2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lead_acid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.799407 pybamm-23.4/pybamm/input/parameters/lithium_ion/
+-rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Chen2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Chen2020_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Ecker2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Marquis2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Mohtat2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/OKane2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30791 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/ORegan2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Prada2013.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Ramadass2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/Xu2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.803407 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/lico2_data_example.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.763407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.803407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/cells/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.803407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/parameters.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/cells/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.803407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.803407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_TDF_EC_DMC_1_1_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_conductivity_EC_DMC_1_1_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_diffusivity_EC_DMC_1_1_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_transference_number_EC_DMC_1_1_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.807407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_TDF_EC_EMC_3_7_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_base_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_conductivity_EC_EMC_3_7_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_diffusivity_EC_EMC_3_7_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_transference_number_EC_EMC_3_7_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.807407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_TDF_EMC_FEC_19_1_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_conductivity_EMC_FEC_19_1_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_diffusivity_EMC_FEC_19_1_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_transference_number_EMC_FEC_19_1_Landesfeind2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.807407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/dlnf_dlnc_Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_conductivity_Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_diffusivity_Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.811407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/experiments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.811407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/parameters.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.811407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.811407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_cracking_rate_Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_diffusivity_Dualfoil1998.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_electrolyte_exchange_current_density_Dualfoil1998.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_volume_change_Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.811407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.815407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_cracking_rate_Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_diffusivity_Dualfoil1998.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_electrolyte_exchange_current_density_Dualfoil1998.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_entropic_change_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_entropic_change_Ai2020_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_volume_change_Ai2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.763407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/seis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.815407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/seis/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/seis/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/seis/example/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.815407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/separators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/separators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.815407 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/parameters.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/install_odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.819407 pybamm-23.4/pybamm/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/meshes/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/meshes/one_dimensional_submeshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/meshes/scikit_fem_submeshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/meshes/zero_dimensional_submesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.819407 pybamm-23.4/pybamm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47327 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.819407 pybamm-23.4/pybamm/models/full_battery_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56548 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/base_battery_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.819407 pybamm-23.4/pybamm/models/full_battery_models/equivalent_circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/equivalent_circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.819407 pybamm-23.4/pybamm/models/full_battery_models/lead_acid/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lead_acid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lead_acid/basic_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lead_acid/full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lead_acid/loqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.823408 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/Yang2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/basic_spm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/dfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/mpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/spm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/spme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.823408 pybamm-23.4/pybamm/models/submodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.827407 pybamm-23.4/pybamm/models/submodels/active_material/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/active_material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/active_material/base_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/active_material/constant_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/active_material/loss_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/active_material/total_active_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/base_submodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.827407 pybamm-23.4/pybamm/models/submodels/convection/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/base_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.827407 pybamm-23.4/pybamm/models/submodels/convection/through_cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/through_cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/through_cell/explicit_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/through_cell/full_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/through_cell/no_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.827407 pybamm-23.4/pybamm/models/submodels/convection/transverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/transverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/transverse/base_transverse_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/transverse/full_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/transverse/no_convection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/convection/transverse/uniform_convection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.827407 pybamm-23.4/pybamm/models/submodels/current_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/current_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/current_collector/base_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/current_collector/homogeneous_current_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/current_collector/potential_pair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.827407 pybamm-23.4/pybamm/models/submodels/electrode/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/base_electrode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.831407 pybamm-23.4/pybamm/models/submodels/electrode/ohm/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/ohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/ohm/base_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/ohm/composite_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/ohm/full_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/ohm/leading_ohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/ohm/li_metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.831407 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.831407 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.831407 pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.835407 pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.835407 pybamm-23.4/pybamm/models/submodels/external_circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/external_circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/external_circuit/base_external_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/external_circuit/function_control_external_circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.835407 pybamm-23.4/pybamm/models/submodels/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/base_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.835407 pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.839408 pybamm-23.4/pybamm/models/submodels/interface/kinetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/base_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/butler_volmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/diffusion_limited.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.839408 pybamm-23.4/pybamm/models/submodels/interface/kinetics/inverse_kinetics/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/inverse_kinetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/marcus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/no_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/tafel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.839408 pybamm-23.4/pybamm/models/submodels/interface/lithium_plating/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/lithium_plating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/lithium_plating/base_plating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/lithium_plating/no_plating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/lithium_plating/plating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.839408 pybamm-23.4/pybamm/models/submodels/interface/open_circuit_potential/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/open_circuit_potential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.839408 pybamm-23.4/pybamm/models/submodels/interface/sei/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/sei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/sei/base_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/sei/constant_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/sei/no_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/sei/sei_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/sei/total_sei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/interface/total_interfacial_current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.839408 pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.843407 pybamm-23.4/pybamm/models/submodels/particle/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle/base_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle/fickian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle/polynomial_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle/total_particle_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.843407 pybamm-23.4/pybamm/models/submodels/particle_mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle_mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle_mechanics/base_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle_mechanics/crack_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle_mechanics/no_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/particle_mechanics/swelling_only.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.843407 pybamm-23.4/pybamm/models/submodels/porosity/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/porosity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/porosity/base_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/porosity/constant_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/porosity/reaction_driven_porosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.843407 pybamm-23.4/pybamm/models/submodels/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/thermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/thermal/base_thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/thermal/isothermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/thermal/lumped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.847407 pybamm-23.4/pybamm/models/submodels/thermal/pouch_cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/thermal/pouch_cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/thermal/x_full.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.847407 pybamm-23.4/pybamm/models/submodels/transport_efficiency/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/transport_efficiency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.847407 pybamm-23.4/pybamm/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/base_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/bpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/ecm_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/electrical_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/geometric_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/lead_acid_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/lithium_ion_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/parameter_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43817 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/parameter_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/process_parameter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/size_distribution_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters/thermal_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/parameters_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.851407 pybamm-23.4/pybamm/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/plotting/dynamic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/plotting/plot2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/plotting/plot_summary_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/plotting/plot_voltage_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/plotting/quick_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46927 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.851407 pybamm-23.4/pybamm/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/algebraic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64653 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/base_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.851407 pybamm-23.4/pybamm/solvers/c_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/c_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/casadi_algebraic_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32025 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/casadi_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/dummy_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/idaklu_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39216 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/jax_bdf_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/jax_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/lrudict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/processed_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/scikits_dae_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/scikits_ode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/scipy_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31865 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/solvers/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.855407 pybamm-23.4/pybamm/spatial_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/spatial_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57884 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/spatial_methods/finite_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/spatial_methods/scikit_finite_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/spatial_methods/spatial_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28643 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/spatial_methods/spectral_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/spatial_methods/zero_dimensional_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-30 16:34:20.000000 pybamm-23.4/pybamm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:34:27.775407 pybamm-23.4/pybamm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41856 2023-04-30 16:34:27.000000 pybamm-23.4/pybamm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-04-30 16:34:27.000000 pybamm-23.4/pybamm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:34:27.000000 pybamm-23.4/pybamm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-30 16:34:27.000000 pybamm-23.4/pybamm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-30 16:34:27.000000 pybamm-23.4/pybamm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-30 16:34:27.000000 pybamm-23.4/pybamm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:34:27.855407 pybamm-23.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-30 16:34:20.000000 pybamm-23.4/setup.py
```

### Comparing `pybamm-23.3/CMakeBuild.py` & `pybamm-23.4/CMakeBuild.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/LICENSE.txt` & `pybamm-23.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/PKG-INFO` & `pybamm-23.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybamm
-Version: 23.3
+Version: 23.4
 Summary: Python Battery Mathematical Modelling.
 Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN
 Description: ![PyBaMM_logo](https://user-images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-7ebef7c72a1e.png)
         
         #
         
@@ -231,15 +231,15 @@
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/alibh95"><img src="https://avatars.githubusercontent.com/u/65511923?v=4?s=100" width="100px;" alt="Ali Hussain Umar Bhatti"/><br /><sub><b>Ali Hussain Umar Bhatti</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=alibh95" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=alibh95" title="Tests">⚠️</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/molel-gt"><img src="https://avatars.githubusercontent.com/u/81125862?v=4?s=100" width="100px;" alt="Leshinka Molel"/><br /><sub><b>Leshinka Molel</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=molel-gt" title="Code">💻</a> <a href="#ideas-molel-gt" title="Ideas, Planning, & Feedback">🤔</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/tobykirk"><img src="https://avatars.githubusercontent.com/u/42966045?v=4?s=100" width="100px;" alt="tobykirk"/><br /><sub><b>tobykirk</b></sub></a><br /><a href="#ideas-tobykirk" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=tobykirk" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=tobykirk" title="Tests">⚠️</a> <a href="#tutorial-tobykirk" title="Tutorials">✅</a></td>
             </tr>
             <tr>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/chuckliu1979"><img src="https://avatars.githubusercontent.com/u/13491954?v=4?s=100" width="100px;" alt="Chuck Liu"/><br /><sub><b>Chuck Liu</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Achuckliu1979" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=chuckliu1979" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/partben"><img src="https://avatars.githubusercontent.com/u/88316576?v=4?s=100" width="100px;" alt="partben"/><br /><sub><b>partben</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=partben" title="Documentation">📖</a></td>
-              <td align="center" valign="top" width="14.28%"><a href="https://gavinw.me"><img src="https://avatars.githubusercontent.com/u/6828967?v=4?s=100" width="100px;" alt="Gavin Wiggins"/><br /><sub><b>Gavin Wiggins</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Awigging" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=wigging" title="Code">💻</a></td>
+              <td align="center" valign="top" width="14.28%"><a href="https://wigging.me"><img src="https://avatars.githubusercontent.com/u/6828967?v=4?s=100" width="100px;" alt="Gavin Wiggins"/><br /><sub><b>Gavin Wiggins</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Awigging" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=wigging" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/dion-w"><img src="https://avatars.githubusercontent.com/u/91852142?v=4?s=100" width="100px;" alt="Dion Wilde"/><br /><sub><b>Dion Wilde</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Adion-w" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=dion-w" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://www.ehtec.co"><img src="https://avatars.githubusercontent.com/u/48386220?v=4?s=100" width="100px;" alt="Elias Hohl"/><br /><sub><b>Elias Hohl</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=ehtec" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/KAschad"><img src="https://avatars.githubusercontent.com/u/93784399?v=4?s=100" width="100px;" alt="KAschad"/><br /><sub><b>KAschad</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3AKAschad" title="Bug reports">🐛</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/Vaibhav-Chopra-GT"><img src="https://avatars.githubusercontent.com/u/92637595?v=4?s=100" width="100px;" alt="Vaibhav-Chopra-GT"/><br /><sub><b>Vaibhav-Chopra-GT</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=Vaibhav-Chopra-GT" title="Code">💻</a></td>
             </tr>
             <tr>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/bardsleypt"><img src="https://avatars.githubusercontent.com/u/54084289?v=4?s=100" width="100px;" alt="bardsleypt"/><br /><sub><b>bardsleypt</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Abardsleypt" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=bardsleypt" title="Code">💻</a></td>
@@ -265,11 +265,23 @@
         <!-- prettier-ignore-end -->
         
         <!-- ALL-CONTRIBUTORS-LIST:END -->
         
         This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
         
 Platform: UNKNOWN
-Requires-Python: >=3.8,<3.10
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybamm Version: 23.3 Summary: Python Battery
+Metadata-Version: 2.1 Name: pybamm Version: 23.4 Summary: Python Battery
 Mathematical Modelling. Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN Description: ![PyBaMM_logo](https://user-
 images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-
 7ebef7c72a1e.png) #
   [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-
   orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org) [!
   [Build](https://github.com/pybamm-team/PyBaMM/workflows/PyBaMM/badge.svg)]
@@ -149,9 +149,17 @@
                                                         bardsleypt                                                                            ndrewwang                                                                            MichaPhilipp                                                                 Alec_Bills                                                                    Agriya_Khetarpal                                                                Alex_Wadell                                                                    iatzak
                                                          ð ð»                                                                    ð ð»                                                                        ð                                                                    ð»                                                                    ð ð» ð                                                  ð» â ï¸ ð                                                ð ð ð»
                                                           [Ankit_Kumar]                                                                   [Aniket_Singh_Rawat]                                                        [Jerom_Palimattom_Tom]                                                                 [Brady_Planden]                                                                      [jsbrittain]                                                                          [Arjun]
                                                            Ankit_Kumar                                                                     Aniket_Singh_Rawat                                                          Jerom_Palimattom_Tom                                                                   Brady_Planden                                                                        jsbrittain                                                                            Arjun
                                                               ð»                                                                            ð»                                                               ð ð» â ï¸                                                           ð¡                                                                         ð» â ï¸                                                                 ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
-welcome! Platform: UNKNOWN Requires-Python: >=3.8,<3.10 Description-Content-
-Type: text/markdown Provides-Extra: docs Provides-Extra: dev
+welcome! Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering Requires-Python: >=3.8,<3.12 Description-Content-Type: text/
+markdown Provides-Extra: docs Provides-Extra: dev
```

### Comparing `pybamm-23.3/README.md` & `pybamm-23.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/alibh95"><img src="https://avatars.githubusercontent.com/u/65511923?v=4?s=100" width="100px;" alt="Ali Hussain Umar Bhatti"/><br /><sub><b>Ali Hussain Umar Bhatti</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=alibh95" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=alibh95" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/molel-gt"><img src="https://avatars.githubusercontent.com/u/81125862?v=4?s=100" width="100px;" alt="Leshinka Molel"/><br /><sub><b>Leshinka Molel</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=molel-gt" title="Code">💻</a> <a href="#ideas-molel-gt" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tobykirk"><img src="https://avatars.githubusercontent.com/u/42966045?v=4?s=100" width="100px;" alt="tobykirk"/><br /><sub><b>tobykirk</b></sub></a><br /><a href="#ideas-tobykirk" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=tobykirk" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=tobykirk" title="Tests">⚠️</a> <a href="#tutorial-tobykirk" title="Tutorials">✅</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chuckliu1979"><img src="https://avatars.githubusercontent.com/u/13491954?v=4?s=100" width="100px;" alt="Chuck Liu"/><br /><sub><b>Chuck Liu</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Achuckliu1979" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=chuckliu1979" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/partben"><img src="https://avatars.githubusercontent.com/u/88316576?v=4?s=100" width="100px;" alt="partben"/><br /><sub><b>partben</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=partben" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://gavinw.me"><img src="https://avatars.githubusercontent.com/u/6828967?v=4?s=100" width="100px;" alt="Gavin Wiggins"/><br /><sub><b>Gavin Wiggins</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Awigging" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=wigging" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://wigging.me"><img src="https://avatars.githubusercontent.com/u/6828967?v=4?s=100" width="100px;" alt="Gavin Wiggins"/><br /><sub><b>Gavin Wiggins</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Awigging" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=wigging" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dion-w"><img src="https://avatars.githubusercontent.com/u/91852142?v=4?s=100" width="100px;" alt="Dion Wilde"/><br /><sub><b>Dion Wilde</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Adion-w" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=dion-w" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.ehtec.co"><img src="https://avatars.githubusercontent.com/u/48386220?v=4?s=100" width="100px;" alt="Elias Hohl"/><br /><sub><b>Elias Hohl</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=ehtec" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/KAschad"><img src="https://avatars.githubusercontent.com/u/93784399?v=4?s=100" width="100px;" alt="KAschad"/><br /><sub><b>KAschad</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3AKAschad" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Vaibhav-Chopra-GT"><img src="https://avatars.githubusercontent.com/u/92637595?v=4?s=100" width="100px;" alt="Vaibhav-Chopra-GT"/><br /><sub><b>Vaibhav-Chopra-GT</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=Vaibhav-Chopra-GT" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bardsleypt"><img src="https://avatars.githubusercontent.com/u/54084289?v=4?s=100" width="100px;" alt="bardsleypt"/><br /><sub><b>bardsleypt</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Abardsleypt" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=bardsleypt" title="Code">💻</a></td>
```

### Comparing `pybamm-23.3/pybamm/CITATIONS.txt` & `pybamm-23.4/pybamm/CITATIONS.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/__init__.py` & `pybamm-23.4/pybamm/__init__.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/batch_study.py` & `pybamm-23.4/pybamm/batch_study.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/callbacks.py` & `pybamm-23.4/pybamm/callbacks.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/discretisations/discretisation.py` & `pybamm-23.4/pybamm/discretisations/discretisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/doc_utils.py` & `pybamm-23.4/pybamm/doc_utils.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/experiments/experiment.py` & `pybamm-23.4/pybamm/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/array.py` & `pybamm-23.4/pybamm/expression_tree/array.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/averages.py` & `pybamm-23.4/pybamm/expression_tree/averages.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/binary_operators.py` & `pybamm-23.4/pybamm/expression_tree/binary_operators.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/broadcasts.py` & `pybamm-23.4/pybamm/expression_tree/broadcasts.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/concatenations.py` & `pybamm-23.4/pybamm/expression_tree/concatenations.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/exceptions.py` & `pybamm-23.4/pybamm/expression_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/functions.py` & `pybamm-23.4/pybamm/expression_tree/functions.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/independent_variable.py` & `pybamm-23.4/pybamm/expression_tree/independent_variable.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/input_parameter.py` & `pybamm-23.4/pybamm/expression_tree/input_parameter.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/interpolant.py` & `pybamm-23.4/pybamm/expression_tree/interpolant.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/matrix.py` & `pybamm-23.4/pybamm/expression_tree/matrix.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/operations/convert_to_casadi.py` & `pybamm-23.4/pybamm/expression_tree/operations/convert_to_casadi.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/operations/evaluate_python.py` & `pybamm-23.4/pybamm/expression_tree/operations/evaluate_python.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/operations/jacobian.py` & `pybamm-23.4/pybamm/expression_tree/operations/jacobian.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/operations/latexify.py` & `pybamm-23.4/pybamm/expression_tree/operations/latexify.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/operations/unpack_symbols.py` & `pybamm-23.4/pybamm/expression_tree/operations/unpack_symbols.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/parameter.py` & `pybamm-23.4/pybamm/expression_tree/parameter.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/printing/print_name.py` & `pybamm-23.4/pybamm/expression_tree/printing/print_name.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/printing/sympy_overrides.py` & `pybamm-23.4/pybamm/expression_tree/printing/sympy_overrides.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/scalar.py` & `pybamm-23.4/pybamm/expression_tree/scalar.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/state_vector.py` & `pybamm-23.4/pybamm/expression_tree/state_vector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/symbol.py` & `pybamm-23.4/pybamm/expression_tree/symbol.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/unary_operators.py` & `pybamm-23.4/pybamm/expression_tree/unary_operators.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/variable.py` & `pybamm-23.4/pybamm/expression_tree/variable.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/expression_tree/vector.py` & `pybamm-23.4/pybamm/expression_tree/vector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/geometry/battery_geometry.py` & `pybamm-23.4/pybamm/geometry/battery_geometry.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/geometry/geometry.py` & `pybamm-23.4/pybamm/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/geometry/standard_spatial_vars.py` & `pybamm-23.4/pybamm/geometry/standard_spatial_vars.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv` & `pybamm-23.4/pybamm/input/discharge_data/Ecker2015/Ecker_1C.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv` & `pybamm-23.4/pybamm/input/discharge_data/Ecker2015/Ecker_5C.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Ecker2015/README.md` & `pybamm-23.4/pybamm/input/discharge_data/Ecker2015/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.1C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/0.5C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/1C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/1C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/1C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/2C_discharge_T.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/2C_discharge_U.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/2C_discharge_displacement.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/README.md` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/stn_2C.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt` & `pybamm-23.4/pybamm/input/discharge_data/Enertech_cells/stp_2C.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/drive_cycles/UDDS.csv` & `pybamm-23.4/pybamm/input/drive_cycles/UDDS.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/drive_cycles/US06.csv` & `pybamm-23.4/pybamm/input/drive_cycles/US06.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/drive_cycles/WLTC.csv` & `pybamm-23.4/pybamm/input/drive_cycles/WLTC.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_c1.csv` & `pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_c1.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv` & `pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_dudt.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv` & `pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_ocv.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_r0.csv` & `pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_r0.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/ecm/data/ecm_example_r1.csv` & `pybamm-23.4/pybamm/input/parameters/ecm/data/ecm_example_r1.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/ecm/example_set.py` & `pybamm-23.4/pybamm/input/parameters/ecm/example_set.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lead_acid/Sulzer2019.py` & `pybamm-23.4/pybamm/input/parameters/lead_acid/Sulzer2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Ai2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Chen2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Chen2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Chen2020_composite.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Chen2020_composite.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Ecker2015.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Ecker2015.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Marquis2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Marquis2019.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,14 +376,15 @@
     return {
         "chemistry": "lithium_ion",
         # sei
         "Ratio of lithium moles to SEI moles": 2.0,
         "Inner SEI reaction proportion": 0.5,
         "Inner SEI partial molar volume [m3.mol-1]": 9.585e-05,
         "Outer SEI partial molar volume [m3.mol-1]": 9.585e-05,
+        "SEI growth transfer coefficient": 0.5,
         "SEI reaction exchange current density [A.m-2]": 1.5e-07,
         "SEI resistivity [Ohm.m]": 200000.0,
         "Outer SEI solvent diffusivity [m2.s-1]": 2.5000000000000002e-22,
         "Bulk solvent concentration [mol.m-3]": 2636.0,
         "Inner SEI open-circuit potential [V]": 0.1,
         "Outer SEI open-circuit potential [V]": 0.8,
         "Inner SEI electron conductivity [S.m-1]": 8.95e-14,
```

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Mohtat2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Mohtat2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/NCA_Kim2011.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/OKane2022.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/OKane2022.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/ORegan2022.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/ORegan2022.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Prada2013.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Prada2013.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Ramadass2004.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Ramadass2004.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/Xu2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/Xu2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/graphite_LGM50_ocp_Chen2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/graphite_ocp_Enertech_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/lico2_data_example.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/lico2_data_example.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/lico2_ocp_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/measured_graphite_diffusivity_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/measured_nco_diffusivity_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/nca_ocp_Kim2011_data.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/nco_ocp_Ecker2015.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/data/nmc_LGM50_ocp_Chen2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/README.md` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/parameters.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/cells/Enertech_Ai2020/parameters.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_TDF_EC_DMC_1_1_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_TDF_EC_DMC_1_1_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_conductivity_EC_DMC_1_1_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_conductivity_EC_DMC_1_1_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_diffusivity_EC_DMC_1_1_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_diffusivity_EC_DMC_1_1_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_transference_number_EC_DMC_1_1_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/electrolyte_transference_number_EC_DMC_1_1_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/parameters.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_DMC_1_1_Landesfeind2019/parameters.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_TDF_EC_EMC_3_7_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_TDF_EC_EMC_3_7_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_base_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_base_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_conductivity_EC_EMC_3_7_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_conductivity_EC_EMC_3_7_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_diffusivity_EC_EMC_3_7_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_diffusivity_EC_EMC_3_7_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_transference_number_EC_EMC_3_7_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/electrolyte_transference_number_EC_EMC_3_7_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/parameters.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EC_EMC_3_7_Landesfeind2019/parameters.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_TDF_EMC_FEC_19_1_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_TDF_EMC_FEC_19_1_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_base_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_conductivity_EMC_FEC_19_1_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_conductivity_EMC_FEC_19_1_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_diffusivity_EMC_FEC_19_1_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_diffusivity_EMC_FEC_19_1_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_transference_number_EMC_FEC_19_1_Landesfeind2019.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/electrolyte_transference_number_EMC_FEC_19_1_Landesfeind2019.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/parameters.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_EMC_FEC_19_1_Landesfeind2019/parameters.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/README.md` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/dlnf_dlnc_Ai2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/dlnf_dlnc_Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_conductivity_Ai2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_conductivity_Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_diffusivity_Ai2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/electrolytes/lipf6_Enertech_Ai2020/electrolyte_diffusivity_Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/README.md` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/parameters.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/experiments/1C_discharge_from_full_Ai2020/parameters.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/README.md` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_cracking_rate_Ai2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_cracking_rate_Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_diffusivity_Dualfoil1998.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_diffusivity_Dualfoil1998.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_electrolyte_exchange_current_density_Dualfoil1998.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_electrolyte_exchange_current_density_Dualfoil1998.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020_function.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_entropy_Enertech_Ai2020_function.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020_function.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_ocp_Enertech_Ai2020_function.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_volume_change_Ai2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/graphite_volume_change_Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/parameters.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/negative_electrodes/graphite_Ai2020/parameters.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/README.md` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_cracking_rate_Ai2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_cracking_rate_Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_diffusivity_Dualfoil1998.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_diffusivity_Dualfoil1998.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_electrolyte_exchange_current_density_Dualfoil1998.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_electrolyte_exchange_current_density_Dualfoil1998.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_entropic_change_Ai2020_function.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_entropic_change_Ai2020_function.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020_function.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_ocp_Ai2020_function.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_volume_change_Ai2020.py` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/lico2_volume_change_Ai2020.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/parameters.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/positive_electrodes/lico2_Ai2020/parameters.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/seis/example/README.md` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/seis/example/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/seis/example/parameters.csv` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/seis/example/parameters.csv`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/README.md` & `pybamm-23.4/pybamm/input/parameters/lithium_ion/testing_only/separators/separator_Ai2020/README.md`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/install_odes.py` & `pybamm-23.4/pybamm/install_odes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/logger.py` & `pybamm-23.4/pybamm/logger.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/meshes/meshes.py` & `pybamm-23.4/pybamm/meshes/meshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/meshes/one_dimensional_submeshes.py` & `pybamm-23.4/pybamm/meshes/one_dimensional_submeshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/meshes/scikit_fem_submeshes.py` & `pybamm-23.4/pybamm/meshes/scikit_fem_submeshes.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/meshes/zero_dimensional_submesh.py` & `pybamm-23.4/pybamm/meshes/zero_dimensional_submesh.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/base_model.py` & `pybamm-23.4/pybamm/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/event.py` & `pybamm-23.4/pybamm/models/event.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/base_battery_model.py` & `pybamm-23.4/pybamm/models/full_battery_models/base_battery_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py` & `pybamm-23.4/pybamm/models/full_battery_models/equivalent_circuit/ecm_model_options.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py` & `pybamm-23.4/pybamm/models/full_battery_models/equivalent_circuit/thevenin.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py` & `pybamm-23.4/pybamm/models/full_battery_models/lead_acid/base_lead_acid_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lead_acid/basic_full.py` & `pybamm-23.4/pybamm/models/full_battery_models/lead_acid/basic_full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lead_acid/full.py` & `pybamm-23.4/pybamm/models/full_battery_models/lead_acid/full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lead_acid/loqs.py` & `pybamm-23.4/pybamm/models/full_battery_models/lead_acid/loqs.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/__init__.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/__init__.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/base_lithium_ion_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/basic_dfn.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/basic_dfn_composite.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/basic_dfn_half_cell.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/basic_spm.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/basic_spm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/dfn.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/dfn.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/electrode_soh.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/electrode_soh_half_cell.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/mpm.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/mpm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/newman_tobias.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/spm.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/spm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/full_battery_models/lithium_ion/spme.py` & `pybamm-23.4/pybamm/models/full_battery_models/lithium_ion/spme.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/active_material/base_active_material.py` & `pybamm-23.4/pybamm/models/submodels/active_material/base_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/active_material/constant_active_material.py` & `pybamm-23.4/pybamm/models/submodels/active_material/constant_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/active_material/loss_active_material.py` & `pybamm-23.4/pybamm/models/submodels/active_material/loss_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/active_material/total_active_material.py` & `pybamm-23.4/pybamm/models/submodels/active_material/total_active_material.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/base_submodel.py` & `pybamm-23.4/pybamm/models/submodels/base_submodel.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/base_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/base_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/through_cell/base_through_cell_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/through_cell/explicit_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/through_cell/explicit_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/through_cell/full_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/through_cell/full_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/through_cell/no_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/through_cell/no_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/transverse/base_transverse_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/transverse/base_transverse_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/transverse/full_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/transverse/full_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/transverse/no_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/transverse/no_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/convection/transverse/uniform_convection.py` & `pybamm-23.4/pybamm/models/submodels/convection/transverse/uniform_convection.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/current_collector/base_current_collector.py` & `pybamm-23.4/pybamm/models/submodels/current_collector/base_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py` & `pybamm-23.4/pybamm/models/submodels/current_collector/effective_resistance_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/current_collector/homogeneous_current_collector.py` & `pybamm-23.4/pybamm/models/submodels/current_collector/homogeneous_current_collector.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/current_collector/potential_pair.py` & `pybamm-23.4/pybamm/models/submodels/current_collector/potential_pair.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrode/base_electrode.py` & `pybamm-23.4/pybamm/models/submodels/electrode/base_electrode.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrode/ohm/base_ohm.py` & `pybamm-23.4/pybamm/models/submodels/electrode/ohm/base_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrode/ohm/composite_ohm.py` & `pybamm-23.4/pybamm/models/submodels/electrode/ohm/composite_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrode/ohm/full_ohm.py` & `pybamm-23.4/pybamm/models/submodels/electrode/ohm/full_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrode/ohm/leading_ohm.py` & `pybamm-23.4/pybamm/models/submodels/electrode/ohm/leading_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrode/ohm/li_metal.py` & `pybamm-23.4/pybamm/models/submodels/electrode/ohm/li_metal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py` & `pybamm-23.4/pybamm/models/submodels/electrode/ohm/surface_form_ohm.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/base_electrolyte_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/composite_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/full_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/integrated_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/leading_order_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/composite_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/explicit_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/full_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_conductivity/surface_potential_form/leading_surface_form_conductivity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/base_electrolyte_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/constant_concentration.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/full_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py` & `pybamm-23.4/pybamm/models/submodels/electrolyte_diffusion/leading_order_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py` & `pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/ocv_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py` & `pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/rc_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py` & `pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/resistor_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/thermal.py` & `pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/thermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py` & `pybamm-23.4/pybamm/models/submodels/equivalent_circuit_elements/voltage_model.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/external_circuit/base_external_circuit.py` & `pybamm-23.4/pybamm/models/submodels/external_circuit/base_external_circuit.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py` & `pybamm-23.4/pybamm/models/submodels/external_circuit/explicit_control_external_circuit.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/external_circuit/function_control_external_circuit.py` & `pybamm-23.4/pybamm/models/submodels/external_circuit/function_control_external_circuit.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/base_interface.py` & `pybamm-23.4/pybamm/models/submodels/interface/base_interface.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py` & `pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/base_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py` & `pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/constant_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py` & `pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/current_driven_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py` & `pybamm-23.4/pybamm/models/submodels/interface/interface_utilisation/full_utilisation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/__init__.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/__init__.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/base_kinetics.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/base_kinetics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/butler_volmer.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/butler_volmer.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/diffusion_limited.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/diffusion_limited.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/inverse_kinetics/inverse_butler_volmer.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/linear.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/linear.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/marcus.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/marcus.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/no_reaction.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/no_reaction.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/tafel.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/tafel.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py` & `pybamm-23.4/pybamm/models/submodels/interface/kinetics/total_main_kinetics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/lithium_plating/base_plating.py` & `pybamm-23.4/pybamm/models/submodels/interface/lithium_plating/base_plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/lithium_plating/no_plating.py` & `pybamm-23.4/pybamm/models/submodels/interface/lithium_plating/no_plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/lithium_plating/plating.py` & `pybamm-23.4/pybamm/models/submodels/interface/lithium_plating/plating.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py` & `pybamm-23.4/pybamm/models/submodels/interface/open_circuit_potential/base_ocp.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py` & `pybamm-23.4/pybamm/models/submodels/interface/open_circuit_potential/current_sigmoid_ocp.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py` & `pybamm-23.4/pybamm/models/submodels/interface/open_circuit_potential/single_ocp.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/sei/base_sei.py` & `pybamm-23.4/pybamm/models/submodels/interface/sei/base_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/sei/constant_sei.py` & `pybamm-23.4/pybamm/models/submodels/interface/sei/constant_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/sei/no_sei.py` & `pybamm-23.4/pybamm/models/submodels/interface/sei/no_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/sei/sei_growth.py` & `pybamm-23.4/pybamm/models/submodels/interface/sei/sei_growth.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/sei/total_sei.py` & `pybamm-23.4/pybamm/models/submodels/interface/sei/total_sei.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/interface/total_interfacial_current.py` & `pybamm-23.4/pybamm/models/submodels/interface/total_interfacial_current.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py` & `pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/base_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py` & `pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/full_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py` & `pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/leading_oxygen_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py` & `pybamm-23.4/pybamm/models/submodels/oxygen_diffusion/no_oxygen.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle/base_particle.py` & `pybamm-23.4/pybamm/models/submodels/particle/base_particle.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle/fickian_diffusion.py` & `pybamm-23.4/pybamm/models/submodels/particle/fickian_diffusion.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle/polynomial_profile.py` & `pybamm-23.4/pybamm/models/submodels/particle/polynomial_profile.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle/total_particle_concentration.py` & `pybamm-23.4/pybamm/models/submodels/particle/total_particle_concentration.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py` & `pybamm-23.4/pybamm/models/submodels/particle/x_averaged_polynomial_profile.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle_mechanics/base_mechanics.py` & `pybamm-23.4/pybamm/models/submodels/particle_mechanics/base_mechanics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle_mechanics/crack_propagation.py` & `pybamm-23.4/pybamm/models/submodels/particle_mechanics/crack_propagation.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle_mechanics/no_mechanics.py` & `pybamm-23.4/pybamm/models/submodels/particle_mechanics/no_mechanics.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/particle_mechanics/swelling_only.py` & `pybamm-23.4/pybamm/models/submodels/particle_mechanics/swelling_only.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/porosity/base_porosity.py` & `pybamm-23.4/pybamm/models/submodels/porosity/base_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/porosity/constant_porosity.py` & `pybamm-23.4/pybamm/models/submodels/porosity/constant_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/porosity/reaction_driven_porosity.py` & `pybamm-23.4/pybamm/models/submodels/porosity/reaction_driven_porosity.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py` & `pybamm-23.4/pybamm/models/submodels/porosity/reaction_driven_porosity_ode.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/thermal/base_thermal.py` & `pybamm-23.4/pybamm/models/submodels/thermal/base_thermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/thermal/isothermal.py` & `pybamm-23.4/pybamm/models/submodels/thermal/isothermal.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/thermal/lumped.py` & `pybamm-23.4/pybamm/models/submodels/thermal/lumped.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py` & `pybamm-23.4/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_1D_current_collectors.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py` & `pybamm-23.4/pybamm/models/submodels/thermal/pouch_cell/pouch_cell_2D_current_collectors.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/thermal/x_full.py` & `pybamm-23.4/pybamm/models/submodels/thermal/x_full.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py` & `pybamm-23.4/pybamm/models/submodels/transport_efficiency/base_transport_efficiency.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py` & `pybamm-23.4/pybamm/models/submodels/transport_efficiency/bruggeman_transport_efficiency.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/base_parameters.py` & `pybamm-23.4/pybamm/parameters/base_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/bpx.py` & `pybamm-23.4/pybamm/parameters/bpx.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/ecm_parameters.py` & `pybamm-23.4/pybamm/parameters/ecm_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/electrical_parameters.py` & `pybamm-23.4/pybamm/parameters/electrical_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/geometric_parameters.py` & `pybamm-23.4/pybamm/parameters/geometric_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/lead_acid_parameters.py` & `pybamm-23.4/pybamm/parameters/lead_acid_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/lithium_ion_parameters.py` & `pybamm-23.4/pybamm/parameters/lithium_ion_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/parameter_sets.py` & `pybamm-23.4/pybamm/parameters/parameter_sets.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/parameter_values.py` & `pybamm-23.4/pybamm/parameters/parameter_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,20 +66,22 @@
                     "Creating a parameter set from a dictionary of components has "
                     "been deprecated and will be removed in a future release. "
                     "Define the parameter set in a python script instead.",
                     DeprecationWarning,
                 )
                 self.update_from_chemistry(values)
             else:
+                # Remove chemistry if present
+                values.pop("chemistry", None)
                 self.update(values, check_already_exists=False)
         else:
             # Check if values is a named parameter set
             if isinstance(values, str) and values in pybamm.parameter_sets:
                 values = pybamm.parameter_sets[values]
-                values.pop("chemistry")
+                values.pop("chemistry", None)
                 self.update(values, check_already_exists=False)
 
             else:
                 # In this case it might be a filename, load from that filename
                 file_path = self.find_parameter(values)
                 path = os.path.split(file_path)[0]
                 values = self.read_parameters_csv(file_path)
```

### Comparing `pybamm-23.3/pybamm/parameters/process_parameter_data.py` & `pybamm-23.4/pybamm/parameters/process_parameter_data.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/size_distribution_parameters.py` & `pybamm-23.4/pybamm/parameters/size_distribution_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/parameters/thermal_parameters.py` & `pybamm-23.4/pybamm/parameters/thermal_parameters.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/plotting/dynamic_plot.py` & `pybamm-23.4/pybamm/plotting/dynamic_plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/plotting/plot.py` & `pybamm-23.4/pybamm/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/plotting/plot2D.py` & `pybamm-23.4/pybamm/plotting/plot2D.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/plotting/plot_summary_variables.py` & `pybamm-23.4/pybamm/plotting/plot_summary_variables.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/plotting/plot_voltage_components.py` & `pybamm-23.4/pybamm/plotting/plot_voltage_components.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/plotting/quick_plot.py` & `pybamm-23.4/pybamm/plotting/quick_plot.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/settings.py` & `pybamm-23.4/pybamm/settings.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/simulation.py` & `pybamm-23.4/pybamm/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pickle
 import pybamm
 import numpy as np
 import copy
 import warnings
 import sys
 from functools import lru_cache
+import tqdm
 
 
 def is_notebook():
     try:
         shell = get_ipython().__class__.__name__
         if shell == "ZMQInteractiveShell":  # pragma: no cover
             # Jupyter notebook or qtconsole
@@ -506,14 +507,15 @@
         solver=None,
         check_model=True,
         save_at_cycles=None,
         calc_esoh=True,
         starting_solution=None,
         initial_soc=None,
         callbacks=None,
+        showprogress=False,
         **kwargs,
     ):
         """
         A method to solve the model. This method will automatically build
         and set the model parameters if not already done so.
 
         Parameters
@@ -553,14 +555,18 @@
         initial_soc : float, optional
             Initial State of Charge (SOC) for the simulation. Must be between 0 and 1.
             If given, overwrites the initial concentrations provided in the parameter
             set.
         callbacks : list of callbacks, optional
             A list of callbacks to be called at each time step. Each callback must
             implement all the methods defined in :class:`pybamm.callbacks.BaseCallback`.
+        showprogress : bool, optional
+            Whether to show a progress bar for cycling. If true, shows a progress bar
+            for cycles. Has no effect when not used with an experiment.
+            Default is False.
         **kwargs
             Additional key-word arguments passed to `solver.solve`.
             See :meth:`pybamm.BaseSolver.solve`.
         """
         # Setup
         if solver is None:
             solver = self.solver
@@ -694,15 +700,21 @@
             voltage_stop = self.experiment.termination.get("voltage")
             logs["stopping conditions"] = {"voltage": voltage_stop}
 
             idx = 0
             num_cycles = len(self.experiment.cycle_lengths)
             feasible = True  # simulation will stop if experiment is infeasible
             for cycle_num, cycle_length in enumerate(
-                self.experiment.cycle_lengths, start=1
+                # tqdm is the progress bar.
+                tqdm.tqdm(
+                    self.experiment.cycle_lengths,
+                    disable=(not showprogress),
+                    desc="Cycling",
+                ),
+                start=1,
             ):
                 logs["cycle number"] = (
                     cycle_num + cycle_offset,
                     num_cycles + cycle_offset,
                 )
                 logs["elapsed time"] = timer.time()
                 callbacks.on_cycle_start(logs)
```

### Comparing `pybamm-23.3/pybamm/solvers/algebraic_solver.py` & `pybamm-23.4/pybamm/solvers/algebraic_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/base_solver.py` & `pybamm-23.4/pybamm/solvers/base_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/casadi_algebraic_solver.py` & `pybamm-23.4/pybamm/solvers/casadi_algebraic_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/casadi_solver.py` & `pybamm-23.4/pybamm/solvers/casadi_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,17 +512,19 @@
             # Otherwise, create new integrator with an updated grid
             # We don't need to update the grid if reusing the same t_eval
             # (up to a shift by a constant)
             else:
                 if t_eval_shifted_rounded in self.integrators[model]:
                     return self.integrators[model][t_eval_shifted_rounded]
                 else:
-                    method, problem, options = self.integrator_specs[model]
-                    options["grid"] = t_eval_shifted
-                    integrator = casadi.integrator("F", method, problem, options)
+                    method, problem, options, time_args = self.integrator_specs[model]
+                    time_args = [t_eval_shifted[0], t_eval_shifted[1:]]
+                    integrator = casadi.integrator(
+                        "F", method, problem, *time_args, options
+                    )
                     self.integrators[model][t_eval_shifted_rounded] = integrator
                     return integrator
         else:
             rhs = model.casadi_rhs
             algebraic = model.casadi_algebraic
 
             options = {
@@ -538,23 +540,24 @@
             y0 = model.y0
 
             y_diff = casadi.MX.sym("y_diff", rhs(0, y0, p).shape[0])
             y_alg = casadi.MX.sym("y_alg", algebraic(0, y0, p).shape[0])
             y_full = casadi.vertcat(y_diff, y_alg)
 
             if use_grid is False:
+                time_args = []
                 # rescale time
                 t_min = casadi.MX.sym("t_min")
                 t_max = casadi.MX.sym("t_max")
                 t_max_minus_t_min = t_max - t_min
                 t_scaled = t_min + (t_max - t_min) * t
                 # add time limits as inputs
                 p_with_tlims = casadi.vertcat(p, t_min, t_max)
             else:
-                options.update({"grid": t_eval_shifted, "output_t0": True})
+                time_args = [t_eval_shifted[0], t_eval_shifted[1:]]
                 # rescale time
                 t_min = casadi.MX.sym("t_min")
                 # Set dummy parameters for consistency with rescaled time
                 t_max_minus_t_min = 1
                 t_scaled = t_min + t
                 p_with_tlims = casadi.vertcat(p, t_min)
 
@@ -579,16 +582,16 @@
                 method = "idas"
                 problem.update(
                     {
                         "z": y_alg,
                         "alg": algebraic(t_scaled, y_full, p),
                     }
                 )
-            integrator = casadi.integrator("F", method, problem, options)
-            self.integrator_specs[model] = method, problem, options
+            integrator = casadi.integrator("F", method, problem, *time_args, options)
+            self.integrator_specs[model] = method, problem, options, time_args
             if use_grid is False:
                 self.integrators[model] = {"no grid": integrator}
             else:
                 self.integrators[model] = {t_eval_shifted_rounded: integrator}
 
             return integrator
 
@@ -651,21 +654,23 @@
         # Check y0 to see if it includes sensitivities
         if explicit_sensitivities:
             num_parameters = model.len_rhs_sens // model.len_rhs
             len_rhs = len_rhs * (num_parameters + 1)
             len_alg = len_alg * (num_parameters + 1)
 
         y0_diff = y0[:len_rhs]
-        y0_alg = y0[len_rhs:]
+        y0_alg_exact = y0[len_rhs:]
         if self.perturb_algebraic_initial_conditions and len_alg > 0:
             # Add a tiny perturbation to the algebraic initial conditions
             # For some reason this helps with convergence
             # The actual value of the initial conditions for the algebraic variables
             # doesn't matter
-            y0_alg = y0_alg * (1 + 1e-6 * casadi.DM(np.random.rand(len_alg)))
+            y0_alg = y0_alg_exact * (1 + 1e-6 * casadi.DM(np.random.rand(len_alg)))
+        else:
+            y0_alg = y0_alg_exact
         pybamm.logger.spam("Finished preliminary setup for integrator run")
 
         # Solve
         # Try solving
         if use_grid is True:
             t_min = t_eval[0]
             inputs_with_tmin = casadi.vertcat(inputs, t_min)
@@ -678,29 +683,35 @@
                 )
             except RuntimeError as error:
                 # If it doesn't work raise error
                 pybamm.logger.debug(f"Casadi integrator failed with error {error}")
                 raise pybamm.SolverError(error.args[0])
             pybamm.logger.debug("Finished casadi integrator")
             integration_time = timer.time()
-            y_sol = casadi.vertcat(casadi_sol["xf"], casadi_sol["zf"])
+            # Manually add initial conditions and concatenate
+            x_sol = casadi.horzcat(y0_diff, casadi_sol["xf"])
+            if len_alg > 0:
+                z_sol = casadi.horzcat(y0_alg_exact, casadi_sol["zf"])
+                y_sol = casadi.vertcat(x_sol, z_sol)
+            else:
+                y_sol = x_sol
             sol = pybamm.Solution(
                 t_eval,
                 y_sol,
                 model,
                 inputs_dict,
                 sensitivities=extract_sensitivities_in_solution,
                 check_solution=False,
             )
             sol.integration_time = integration_time
             return sol
         else:
             # Repeated calls to the integrator
             x = y0_diff
-            z = y0_alg
+            z = y0_alg_exact
             y_diff = x
             y_alg = z
             for i in range(len(t_eval) - 1):
                 t_min = t_eval[i]
                 t_max = t_eval[i + 1]
                 inputs_with_tlims = casadi.vertcat(inputs, t_min, t_max)
                 timer = pybamm.Timer()
```

### Comparing `pybamm-23.3/pybamm/solvers/dummy_solver.py` & `pybamm-23.4/pybamm/solvers/dummy_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/idaklu_solver.py` & `pybamm-23.4/pybamm/solvers/idaklu_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,22 +528,27 @@
         sensitivity_names = self._setup["sensitivity_names"]
         t = sol.t
         number_of_timesteps = t.size
         number_of_states = y0.size
         y_out = sol.y.reshape((number_of_timesteps, number_of_states))
 
         # return sensitivity solution, we need to flatten yS to
-        # (#timesteps * #states,) to match format used by Solution
+        # (#timesteps * #states (where t is changing the quickest),)
+        # to match format used by Solution
+        # note that yS is (n_p, n_t, n_y)
         if number_of_sensitivity_parameters != 0:
             yS_out = {
                 name: sol.yS[i].reshape(-1, 1)
                 for i, name in enumerate(sensitivity_names)
             }
+            # add "all" stacked sensitivities ((#timesteps * #states,#sens_params))
+            yS_out["all"] = np.hstack([yS_out[name] for name in sensitivity_names])
         else:
             yS_out = False
+
         if sol.flag in [0, 2]:
             # 0 = solved for all t_eval
             if sol.flag == 0:
                 termination = "final time"
             # 2 = found root(s)
             elif sol.flag == 2:
                 termination = "event"
```

### Comparing `pybamm-23.3/pybamm/solvers/jax_bdf_solver.py` & `pybamm-23.4/pybamm/solvers/jax_bdf_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/jax_solver.py` & `pybamm-23.4/pybamm/solvers/jax_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/lrudict.py` & `pybamm-23.4/pybamm/solvers/lrudict.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/processed_variable.py` & `pybamm-23.4/pybamm/solvers/processed_variable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # Processed Variable class
 #
 import casadi
 import numbers
 import numpy as np
 import pybamm
-import scipy.interpolate as interp
 from scipy.integrate import cumulative_trapezoid
+import xarray as xr
 
 
 class ProcessedVariable(object):
     """
     An object that can be evaluated at arbitrary (scalars or vectors) t and x, and
     returns the (interpolated) value of the base variable at that t and x.
 
@@ -127,26 +127,15 @@
 
         if self.cumtrapz_ic is not None:
             entries = cumulative_trapezoid(
                 entries, self.t_pts, initial=float(self.cumtrapz_ic)
             )
 
         # set up interpolation
-        if len(self.t_pts) == 1:
-            # Variable is just a scalar value, but we need to create a callable
-            # function to be consistent with other processed variables
-            self._interpolation_function = Interpolant0D(entries)
-        else:
-            self._interpolation_function = interp.interp1d(
-                self.t_pts,
-                entries,
-                kind="linear",
-                fill_value=np.nan,
-                bounds_error=False,
-            )
+        self._xr_data_array = xr.DataArray(entries, coords=[("t", self.t_pts)])
 
         self.entries = entries
         self.dimensions = 0
 
     def initialise_1D(self, fixed_t=False):
         len_space = self.base_eval.shape[0]
         entries = np.empty((len_space, len(self.t_pts)))
@@ -207,30 +196,18 @@
         pts_for_interp = space
         self.internal_boundaries = self.mesh.internal_boundaries
 
         # Set first_dim_pts to edges for nicer plotting
         self.first_dim_pts = edges
 
         # set up interpolation
-        if len(self.t_pts) == 1:
-            # function of space only
-            self._interpolation_function = Interpolant1D(
-                pts_for_interp, entries_for_interp
-            )
-        else:
-            # function of space and time. Note that the order of 't' and 'space'
-            # is the reverse of what you'd expect
-            self._interpolation_function = interp.interp2d(
-                self.t_pts,
-                pts_for_interp,
-                entries_for_interp,
-                kind="linear",
-                fill_value=np.nan,
-                bounds_error=False,
-            )
+        self._xr_data_array = xr.DataArray(
+            entries_for_interp,
+            coords=[(self.first_dimension, pts_for_interp), ("t", self.t_pts)],
+        )
 
     def initialise_2D(self):
         """
         Initialise a 2D object that depends on x and r, x and z, x and R, or R and r.
         """
         first_dim_nodes = self.mesh.nodes
         first_dim_edges = self.mesh.edges
@@ -358,29 +335,22 @@
         second_dim_pts_for_interp = second_dim_pts
 
         # Set pts to edges for nicer plotting
         self.first_dim_pts = first_dim_edges
         self.second_dim_pts = second_dim_edges
 
         # set up interpolation
-        if len(self.t_pts) == 1:
-            # function of space only. Note the order of the points is the reverse
-            # of what you'd expect
-            self._interpolation_function = Interpolant2D(
-                first_dim_pts_for_interp, second_dim_pts_for_interp, entries_for_interp
-            )
-        else:
-            # function of space and time.
-            self._interpolation_function = interp.RegularGridInterpolator(
-                (first_dim_pts_for_interp, second_dim_pts_for_interp, self.t_pts),
-                entries_for_interp,
-                method="linear",
-                fill_value=np.nan,
-                bounds_error=False,
-            )
+        self._xr_data_array = xr.DataArray(
+            entries_for_interp,
+            coords={
+                self.first_dimension: first_dim_pts_for_interp,
+                self.second_dimension: second_dim_pts_for_interp,
+                "t": self.t_pts,
+            },
+        )
 
     def initialise_2D_scikit_fem(self):
         y_sol = self.mesh.edges["y"]
         len_y = len(y_sol)
         z_sol = self.mesh.edges["z"]
         len_z = len(z_sol)
         entries = np.empty((len_y, len_z, len(self.t_pts)))
@@ -407,82 +377,29 @@
         self.z_sol = z_sol
         self.first_dimension = "y"
         self.second_dimension = "z"
         self.first_dim_pts = y_sol
         self.second_dim_pts = z_sol
 
         # set up interpolation
-        if len(self.t_pts) == 1:
-            # function of space only. Note the order of the points is the reverse
-            # of what you'd expect
-            self._interpolation_function = Interpolant2D(
-                self.first_dim_pts, self.second_dim_pts, entries
-            )
-        else:
-            # function of space and time.
-            self._interpolation_function = interp.RegularGridInterpolator(
-                (self.first_dim_pts, self.second_dim_pts, self.t_pts),
-                entries,
-                method="linear",
-                fill_value=np.nan,
-                bounds_error=False,
-            )
+        self._xr_data_array = xr.DataArray(
+            entries,
+            coords={"y": y_sol, "z": z_sol, "t": self.t_pts},
+        )
 
     def __call__(self, t=None, x=None, r=None, y=None, z=None, R=None, warn=True):
         """
         Evaluate the variable at arbitrary *dimensional* t (and x, r, y, z and/or R),
         using interpolation
         """
-        # If t is None and there is only one value of time in the soluton (i.e.
-        # the solution is independent of time) then we set t equal to the value
-        # stored in the solution. If the variable is constant (doesn't depend on
-        # time) evaluate arbitrarily at the first value of t. Otherwise, raise
-        # an error
-        if t is None:
-            if len(self.t_pts) == 1:
-                t = self.t_pts
-            elif len(self.base_variables) == 1 and self.base_variables[0].is_constant():
-                t = self.t_pts[0]
-            else:
-                raise ValueError(
-                    "t cannot be None for variable {}".format(self.base_variables)
-                )
-
-        # Call interpolant of correct spatial dimension
-        if self.dimensions == 0:
-            out = self._interpolation_function(t)
-        elif self.dimensions == 1:
-            out = self.call_1D(t, x, r, z, R)
-        elif self.dimensions == 2:
-            out = self.call_2D(t, x, r, y, z, R)
-        if warn is True and np.isnan(out).any():
-            pybamm.logger.warning(
-                "Calling variable outside interpolation range (returns 'nan')"
-            )
-        return out
-
-    def call_1D(self, t, x, r, z, R):
-        """Evaluate a 1D variable"""
-        spatial_var = eval_dimension_name(self.first_dimension, x, r, None, z, R)
-        return self._interpolation_function(t, spatial_var)
-
-    def call_2D(self, t, x, r, y, z, R):
-        """Evaluate a 2D variable"""
-        first_dim = eval_dimension_name(self.first_dimension, x, r, y, z, R)
-        second_dim = eval_dimension_name(self.second_dimension, x, r, y, z, R)
-        if isinstance(first_dim, np.ndarray):
-            if isinstance(second_dim, np.ndarray) and isinstance(t, np.ndarray):
-                first_dim = first_dim[:, np.newaxis, np.newaxis]
-                second_dim = second_dim[:, np.newaxis]
-            elif isinstance(second_dim, np.ndarray) or isinstance(t, np.ndarray):
-                first_dim = first_dim[:, np.newaxis]
-        else:
-            if isinstance(second_dim, np.ndarray) and isinstance(t, np.ndarray):
-                second_dim = second_dim[:, np.newaxis]
-        return self._interpolation_function((first_dim, second_dim, t))
+        kwargs = {"t": t, "x": x, "r": r, "y": y, "z": z, "R": R}
+        # Remove any None arguments
+        kwargs = {key: value for key, value in kwargs.items() if value is not None}
+        # Use xarray interpolation, return numpy array
+        return self._xr_data_array.interp(**kwargs).values
 
     @property
     def data(self):
         """Same as entries, but different name"""
         return self.entries
 
     @property
@@ -560,83 +477,7 @@
         for name, inp in self.all_inputs[0].items():
             end = start + inp.shape[0]
             sensitivities[name] = S_var[:, start:end]
             start = end
 
         # Save attribute
         self._sensitivities = sensitivities
-
-
-class Interpolant0D:
-    def __init__(self, entries):
-        self.entries = entries
-
-    def __call__(self, t):
-        return self.entries
-
-
-class Interpolant1D:
-    def __init__(self, pts_for_interp, entries_for_interp):
-        self.interpolant = interp.interp1d(
-            pts_for_interp,
-            entries_for_interp[:, 0],
-            kind="linear",
-            fill_value=np.nan,
-            bounds_error=False,
-        )
-
-    def __call__(self, t, z):
-        if isinstance(z, np.ndarray):
-            return self.interpolant(z)[:, np.newaxis]
-        else:
-            return self.interpolant(z)
-
-
-class Interpolant2D:
-    def __init__(
-        self, first_dim_pts_for_interp, second_dim_pts_for_interp, entries_for_interp
-    ):
-        self.interpolant = interp.interp2d(
-            second_dim_pts_for_interp,
-            first_dim_pts_for_interp,
-            entries_for_interp[:, :, 0],
-            kind="linear",
-            fill_value=np.nan,
-            bounds_error=False,
-        )
-
-    def __call__(self, input):
-        """
-        Calls and returns a 2D interpolant of the correct shape depending on the
-        shape of the input
-        """
-        first_dim, second_dim, _ = input
-        if isinstance(first_dim, np.ndarray) and isinstance(second_dim, np.ndarray):
-            first_dim = first_dim[:, 0, 0]
-            second_dim = second_dim[:, 0]
-            return self.interpolant(second_dim, first_dim)
-        elif isinstance(first_dim, np.ndarray):
-            first_dim = first_dim[:, 0]
-            return self.interpolant(second_dim, first_dim)[:, 0]
-        elif isinstance(second_dim, np.ndarray):
-            second_dim = second_dim[:, 0]
-            return self.interpolant(second_dim, first_dim)
-        else:
-            return self.interpolant(second_dim, first_dim)[0]
-
-
-def eval_dimension_name(name, x, r, y, z, R):
-    if name == "x":
-        out = x
-    elif name == "r":
-        out = r
-    elif name == "y":
-        out = y
-    elif name == "z":
-        out = z
-    elif name == "R":
-        out = R
-
-    if out is None:
-        raise ValueError("inputs {} cannot be None".format(name))
-    else:
-        return out
```

### Comparing `pybamm-23.3/pybamm/solvers/scikits_dae_solver.py` & `pybamm-23.4/pybamm/solvers/scikits_dae_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/scikits_ode_solver.py` & `pybamm-23.4/pybamm/solvers/scikits_ode_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/scipy_solver.py` & `pybamm-23.4/pybamm/solvers/scipy_solver.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/solvers/solution.py` & `pybamm-23.4/pybamm/solvers/solution.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/spatial_methods/finite_volume.py` & `pybamm-23.4/pybamm/spatial_methods/finite_volume.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/spatial_methods/scikit_finite_element.py` & `pybamm-23.4/pybamm/spatial_methods/scikit_finite_element.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/spatial_methods/spatial_method.py` & `pybamm-23.4/pybamm/spatial_methods/spatial_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             out = pybamm.Matrix(matrix) @ symbol
         elif broadcast_type.startswith("tertiary"):
             # Make copies of the child stacked on top of each other
             identity = eye(symbol.shape[0])
             matrix = vstack([identity for _ in range(tertiary_domain_size)])
             out = pybamm.Matrix(matrix) @ symbol
         elif broadcast_type.startswith("full"):
-            out = symbol * pybamm.Vector(np.ones(full_domain_size))
+            out = symbol * pybamm.Vector(np.ones(full_domain_size), domains=domains)
 
         out.domains = domains.copy()
         return out
 
     def gradient(self, symbol, discretised_symbol, boundary_conditions):
         """
         Implements the gradient for a spatial method.
```

### Comparing `pybamm-23.3/pybamm/spatial_methods/spectral_volume.py` & `pybamm-23.4/pybamm/spatial_methods/spectral_volume.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/spatial_methods/zero_dimensional_method.py` & `pybamm-23.4/pybamm/spatial_methods/zero_dimensional_method.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm/util.py` & `pybamm-23.4/pybamm/util.py`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm.egg-info/PKG-INFO` & `pybamm-23.4/pybamm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybamm
-Version: 23.3
+Version: 23.4
 Summary: Python Battery Mathematical Modelling.
 Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN
 Description: ![PyBaMM_logo](https://user-images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-7ebef7c72a1e.png)
         
         #
         
@@ -231,15 +231,15 @@
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/alibh95"><img src="https://avatars.githubusercontent.com/u/65511923?v=4?s=100" width="100px;" alt="Ali Hussain Umar Bhatti"/><br /><sub><b>Ali Hussain Umar Bhatti</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=alibh95" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=alibh95" title="Tests">⚠️</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/molel-gt"><img src="https://avatars.githubusercontent.com/u/81125862?v=4?s=100" width="100px;" alt="Leshinka Molel"/><br /><sub><b>Leshinka Molel</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=molel-gt" title="Code">💻</a> <a href="#ideas-molel-gt" title="Ideas, Planning, & Feedback">🤔</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/tobykirk"><img src="https://avatars.githubusercontent.com/u/42966045?v=4?s=100" width="100px;" alt="tobykirk"/><br /><sub><b>tobykirk</b></sub></a><br /><a href="#ideas-tobykirk" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=tobykirk" title="Code">💻</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=tobykirk" title="Tests">⚠️</a> <a href="#tutorial-tobykirk" title="Tutorials">✅</a></td>
             </tr>
             <tr>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/chuckliu1979"><img src="https://avatars.githubusercontent.com/u/13491954?v=4?s=100" width="100px;" alt="Chuck Liu"/><br /><sub><b>Chuck Liu</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Achuckliu1979" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=chuckliu1979" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/partben"><img src="https://avatars.githubusercontent.com/u/88316576?v=4?s=100" width="100px;" alt="partben"/><br /><sub><b>partben</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=partben" title="Documentation">📖</a></td>
-              <td align="center" valign="top" width="14.28%"><a href="https://gavinw.me"><img src="https://avatars.githubusercontent.com/u/6828967?v=4?s=100" width="100px;" alt="Gavin Wiggins"/><br /><sub><b>Gavin Wiggins</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Awigging" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=wigging" title="Code">💻</a></td>
+              <td align="center" valign="top" width="14.28%"><a href="https://wigging.me"><img src="https://avatars.githubusercontent.com/u/6828967?v=4?s=100" width="100px;" alt="Gavin Wiggins"/><br /><sub><b>Gavin Wiggins</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Awigging" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=wigging" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/dion-w"><img src="https://avatars.githubusercontent.com/u/91852142?v=4?s=100" width="100px;" alt="Dion Wilde"/><br /><sub><b>Dion Wilde</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Adion-w" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=dion-w" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://www.ehtec.co"><img src="https://avatars.githubusercontent.com/u/48386220?v=4?s=100" width="100px;" alt="Elias Hohl"/><br /><sub><b>Elias Hohl</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=ehtec" title="Code">💻</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/KAschad"><img src="https://avatars.githubusercontent.com/u/93784399?v=4?s=100" width="100px;" alt="KAschad"/><br /><sub><b>KAschad</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3AKAschad" title="Bug reports">🐛</a></td>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/Vaibhav-Chopra-GT"><img src="https://avatars.githubusercontent.com/u/92637595?v=4?s=100" width="100px;" alt="Vaibhav-Chopra-GT"/><br /><sub><b>Vaibhav-Chopra-GT</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/commits?author=Vaibhav-Chopra-GT" title="Code">💻</a></td>
             </tr>
             <tr>
               <td align="center" valign="top" width="14.28%"><a href="https://github.com/bardsleypt"><img src="https://avatars.githubusercontent.com/u/54084289?v=4?s=100" width="100px;" alt="bardsleypt"/><br /><sub><b>bardsleypt</b></sub></a><br /><a href="https://github.com/pybamm-team/PyBaMM/issues?q=author%3Abardsleypt" title="Bug reports">🐛</a> <a href="https://github.com/pybamm-team/PyBaMM/commits?author=bardsleypt" title="Code">💻</a></td>
@@ -265,11 +265,23 @@
         <!-- prettier-ignore-end -->
         
         <!-- ALL-CONTRIBUTORS-LIST:END -->
         
         This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
         
 Platform: UNKNOWN
-Requires-Python: >=3.8,<3.10
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybamm Version: 23.3 Summary: Python Battery
+Metadata-Version: 2.1 Name: pybamm Version: 23.4 Summary: Python Battery
 Mathematical Modelling. Home-page: https://github.com/pybamm-team/PyBaMM
 License: UNKNOWN Description: ![PyBaMM_logo](https://user-
 images.githubusercontent.com/20817509/107091287-8ad46a80-67cf-11eb-86f5-
 7ebef7c72a1e.png) #
   [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-
   orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org) [!
   [Build](https://github.com/pybamm-team/PyBaMM/workflows/PyBaMM/badge.svg)]
@@ -149,9 +149,17 @@
                                                         bardsleypt                                                                            ndrewwang                                                                            MichaPhilipp                                                                 Alec_Bills                                                                    Agriya_Khetarpal                                                                Alex_Wadell                                                                    iatzak
                                                          ð ð»                                                                    ð ð»                                                                        ð                                                                    ð»                                                                    ð ð» ð                                                  ð» â ï¸ ð                                                ð ð ð»
                                                           [Ankit_Kumar]                                                                   [Aniket_Singh_Rawat]                                                        [Jerom_Palimattom_Tom]                                                                 [Brady_Planden]                                                                      [jsbrittain]                                                                          [Arjun]
                                                            Ankit_Kumar                                                                     Aniket_Singh_Rawat                                                          Jerom_Palimattom_Tom                                                                   Brady_Planden                                                                        jsbrittain                                                                            Arjun
                                                               ð»                                                                            ð»                                                               ð ð» â ï¸                                                           ð¡                                                                         ð» â ï¸                                                                 ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
-welcome! Platform: UNKNOWN Requires-Python: >=3.8,<3.10 Description-Content-
-Type: text/markdown Provides-Extra: docs Provides-Extra: dev
+welcome! Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering Requires-Python: >=3.8,<3.12 Description-Content-Type: text/
+markdown Provides-Extra: docs Provides-Extra: dev
```

### Comparing `pybamm-23.3/pybamm.egg-info/SOURCES.txt` & `pybamm-23.4/pybamm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/pybamm.egg-info/entry_points.txt` & `pybamm-23.4/pybamm.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pybamm-23.3/setup.py` & `pybamm-23.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -182,29 +182,45 @@
     cmdclass={
         "build_ext": CMakeBuild.CMakeBuild,
         "bdist_wheel": bdist_wheel,
         "install": CustomInstall,
     },
     package_data={"pybamm": pybamm_data},
     # Python version
-    python_requires=">=3.8,<3.10",
+    python_requires=">=3.8,<3.12",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Scientific/Engineering",
+    ],
     # List of dependencies
     install_requires=[
         "numpy>=1.16",
         "scipy>=1.3",
         "pandas>=0.24",
         "anytree>=2.4.3",
         "autograd>=1.2",
         "scikit-fem>=0.2.0",
-        "casadi>=3.5.0",
+        "casadi>=3.6.0",
         "imageio>=2.9.0",
-        "jupyter",  # For example notebooks
+        "importlib-metadata",
         "pybtex>=0.24.0",
         "sympy>=1.8",
+        "xarray",
         "bpx",
+        "tqdm",
         # Note: Matplotlib is loaded for debug plots, but to ensure pybamm runs
         # on systems without an attached display, it should never be imported
         # outside of plot() methods.
         # Should not be imported
         "matplotlib>=2.0",
     ],
     extras_require={
@@ -214,14 +230,15 @@
             "sphinx_design",
             "sphinx-copybutton",
             "myst-parser",
         ],  # For doc generation
         "dev": [
             "pre-commit",  # For code style checking
             "black",  # For code style auto-formatting
+            "jupyter",  # For example notebooks
         ],
     },
     entry_points={
         "console_scripts": [
             "pybamm_edit_parameter = pybamm.parameters_cli:edit_parameter",
             "pybamm_add_parameter = pybamm.parameters_cli:add_parameter",
             "pybamm_rm_parameter = pybamm.parameters_cli:remove_parameter",
```

