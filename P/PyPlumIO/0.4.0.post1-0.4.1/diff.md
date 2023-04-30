# Comparing `tmp/PyPlumIO-0.4.0.post1.tar.gz` & `tmp/PyPlumIO-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPlumIO-0.4.0.post1.tar", last modified: Thu Apr 13 21:49:20 2023, max compression
+gzip compressed data, was "PyPlumIO-0.4.1.tar", last modified: Sun Apr 30 06:06:34 2023, max compression
```

## Comparing `PyPlumIO-0.4.0.post1.tar` & `PyPlumIO-0.4.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.732936 PyPlumIO-0.4.0.post1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.732936 PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.732936 PyPlumIO-0.4.0.post1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.732936 PyPlumIO-0.4.0.post1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.736935 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.736935 PyPlumIO-0.4.0.post1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.736935 PyPlumIO-0.4.0.post1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/source/protocol.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.736935 PyPlumIO-0.4.0.post1/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/images/ecomax.png
--rw-r--r--   0 runner    (1001) docker     (123)   133458 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/images/rs485.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.740936 PyPlumIO-0.4.0.post1/pyplumio/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/pyplumio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.740936 PyPlumIO-0.4.0.post1/pyplumio/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/ecomax.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/ecoster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.740936 PyPlumIO-0.4.0.post1/pyplumio/frames/
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/frames/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/frames/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/frames/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.744936 PyPlumIO-0.4.0.post1/pyplumio/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.748936 PyPlumIO-0.4.0.post1/pyplumio/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/data_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/ecomax_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/fan_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/frame_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/fuel_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/lambda_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/mixer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/mixer_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/network_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/output_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/pending_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/product_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/program_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/regulator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/temperatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/thermostat_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/thermostat_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.748936 PyPlumIO-0.4.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/tests/frames/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/frames/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/frames/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/frames/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/frames/test_responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21987 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/PyPlumIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/source/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/images/ecomax.png
+-rw-r--r--   0 runner    (1001) docker     (123)   133458 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/images/rs485.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/pyplumio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/pyplumio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.420961 PyPlumIO-0.4.1/pyplumio/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/ecomax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/ecoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.420961 PyPlumIO-0.4.1/pyplumio/frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/frames/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/frames/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/frames/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.420961 PyPlumIO-0.4.1/pyplumio/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/pyplumio/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/data_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/ecomax_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/fan_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/frame_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/fuel_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/lambda_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/mixer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/mixer_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/network_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/output_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/pending_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/product_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/program_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/regulator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/temperatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/thermostat_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/thermostat_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/tests/frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/frames/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/frames/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/frames/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/frames/test_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22215 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tox.ini
```

### Comparing `PyPlumIO-0.4.0.post1/.github/CODE_OF_CONDUCT.md` & `PyPlumIO-0.4.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/feature_request.yml` & `PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/.github/workflows/ci.yml` & `PyPlumIO-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/.github/workflows/codeql-analysis.yml` & `PyPlumIO-0.4.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/.github/workflows/deploy.yml` & `PyPlumIO-0.4.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/.github/workflows/documentation.yml` & `PyPlumIO-0.4.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/.gitignore` & `PyPlumIO-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/.pre-commit-config.yaml` & `PyPlumIO-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/LICENSE` & `PyPlumIO-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/PKG-INFO` & `PyPlumIO-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPlumIO
-Version: 0.4.0.post1
+Version: 0.4.1
 Summary: PyPlumIO is a native ecoNET library for Plum ecoMAX controllers.
 Author-email: Denis Paavilainen <denpa@denpa.pro>
 License: MIT License
 Project-URL: Documentation, https://pyplumio.denpa.pro
 Project-URL: Source Code, https://github.com/denpamusic/PyPlumIO
 Project-URL: Bug Tracker, https://github.com/denpamusic/PyPlumIO/issues
 Keywords: home,automation,heating
```

### Comparing `PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/PKG-INFO` & `PyPlumIO-0.4.1/PyPlumIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPlumIO
-Version: 0.4.0.post1
+Version: 0.4.1
 Summary: PyPlumIO is a native ecoNET library for Plum ecoMAX controllers.
 Author-email: Denis Paavilainen <denpa@denpa.pro>
 License: MIT License
 Project-URL: Documentation, https://pyplumio.denpa.pro
 Project-URL: Source Code, https://github.com/denpamusic/PyPlumIO
 Project-URL: Bug Tracker, https://github.com/denpamusic/PyPlumIO/issues
 Keywords: home,automation,heating
```

### Comparing `PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/SOURCES.txt` & `PyPlumIO-0.4.1/PyPlumIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/README.md` & `PyPlumIO-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/docs/Makefile` & `PyPlumIO-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/docs/make.bat` & `PyPlumIO-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/docs/source/conf.py` & `PyPlumIO-0.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/docs/source/index.rst` & `PyPlumIO-0.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/docs/source/protocol.rst` & `PyPlumIO-0.4.1/docs/source/protocol.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/docs/source/usage.rst` & `PyPlumIO-0.4.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/images/ecomax.png` & `PyPlumIO-0.4.1/images/ecomax.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/images/rs485.png` & `PyPlumIO-0.4.1/images/rs485.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/__init__.py` & `PyPlumIO-0.4.1/pyplumio/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/connection.py` & `PyPlumIO-0.4.1/pyplumio/connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/const.py` & `PyPlumIO-0.4.1/pyplumio/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 STATE_ON: Final = "on"
 STATE_OFF: Final = "off"
 
 # General attributes.
 ATTR_CONNECTED: Final = "connected"
 ATTR_CURRENT_TEMP: Final = "current_temp"
 ATTR_DEVICE_INDEX: Final = "device_index"
+ATTR_FRAME_ERRORS: Final = "frame_errors"
 ATTR_INDEX: Final = "index"
 ATTR_LOADED: Final = "loaded"
 ATTR_OFFSET: Final = "offset"
 ATTR_PARAMETER: Final = "parameter"
 ATTR_PASSWORD: Final = "password"
 ATTR_SCHEDULE: Final = "schedule"
 ATTR_SENSORS: Final = "sensors"
```

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/devices/__init__.py` & `PyPlumIO-0.4.1/pyplumio/devices/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import ClassVar
 
 from pyplumio import util
-from pyplumio.const import ATTR_LOADED, DeviceType, FrameType
+from pyplumio.const import ATTR_FRAME_ERRORS, ATTR_LOADED, DeviceType, FrameType
 from pyplumio.exceptions import ParameterNotFoundError, UnknownDeviceError
 from pyplumio.frames import DataFrameDescription, Frame, Request, get_frame_handler
 from pyplumio.helpers.event_manager import EventManager
 from pyplumio.helpers.factory import factory
 from pyplumio.helpers.parameter import SET_RETRIES, Parameter
 from pyplumio.helpers.typing import ParameterValueType
 from pyplumio.structures.network_info import NetworkInfo
@@ -95,30 +95,31 @@
         """Handle received frame."""
         if frame.data is not None:
             for name, value in frame.data.items():
                 self.dispatch_nowait(name, value)
 
     async def async_setup(self) -> bool:
         """Setup addressable device object."""
-        try:
-            await asyncio.gather(
-                *{
-                    self.create_task(
-                        self.request(description.provides, description.frame_type)
-                    )
-                    for description in self._frame_types
-                },
-                return_exceptions=False,
-            )
-            await self.dispatch(ATTR_LOADED, True)
-            return True
-        except ValueError as e:
-            _LOGGER.error("Request failed: %s", e)
-            await self.dispatch(ATTR_LOADED, False)
-            return False
+        results = await asyncio.gather(
+            *{
+                self.create_task(
+                    self.request(description.provides, description.frame_type)
+                )
+                for description in self._frame_types
+            },
+            return_exceptions=True,
+        )
+
+        errors = [
+            result.args[1] for result in results if isinstance(result, ValueError)
+        ]
+
+        await self.dispatch(ATTR_FRAME_ERRORS, errors)
+        await self.dispatch(ATTR_LOADED, True)
+        return True
 
     async def request(
         self,
         name: str,
         frame_type: FrameType,
         retries: int = 3,
         timeout: float = 3.0,
@@ -132,15 +133,15 @@
         while retries > 0:
             try:
                 self.queue.put_nowait(request)
                 return await self.get(name, timeout=timeout)
             except asyncio.TimeoutError:
                 retries -= 1
 
-        raise ValueError(f'could not request "{name}" with "{frame_type.name}"')
+        raise ValueError(f'could not request "{name}"', frame_type)
 
 
 class SubDevice(Device):
     """Represents the sub-device."""
 
     parent: Addressable
     index: int
```

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/devices/ecomax.py` & `PyPlumIO-0.4.1/pyplumio/devices/ecomax.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import asyncio
 from collections.abc import Generator, Iterable, Sequence
 import logging
 import time
 from typing import ClassVar, Final
 
 from pyplumio.const import (
+    ATTR_FRAME_ERRORS,
     ATTR_PASSWORD,
     ATTR_SENSORS,
     ATTR_STATE,
     STATE_OFF,
     STATE_ON,
     DeviceState,
     DeviceType,
@@ -136,20 +137,32 @@
             FrameType.REQUEST_CHECK_DEVICE,
             FrameType.REQUEST_PROGRAM_VERSION,
         ):
             self.queue.put_nowait(frame.response(data={ATTR_NETWORK: self._network}))
 
         super().handle_frame(frame)
 
+    def _has_frame_version(self, frame_type: FrameType | int, version: int) -> bool:
+        """Check if device instance has a version of the frame."""
+        return (
+            frame_type in self._frame_versions
+            and self._frame_versions[frame_type] == version
+        )
+
+    def _frame_is_supported(self, frame_type: FrameType | int) -> bool:
+        """Check if frame is supported by the device."""
+        return frame_type not in self.data.get(ATTR_FRAME_ERRORS, [])
+
     async def _update_frame_versions(self, versions: dict[int, int]) -> None:
         """Check versions and fetch outdated frames."""
         for frame_type, version in versions.items():
-            if is_known_frame_type(frame_type) and (
-                frame_type not in self._frame_versions
-                or self._frame_versions[frame_type] != version
+            if (
+                is_known_frame_type(frame_type)
+                and self._frame_is_supported(frame_type)
+                and not self._has_frame_version(frame_type, version)
             ):
                 # We don't have this frame or it's version has changed.
                 request = factory(get_frame_handler(frame_type), recipient=self.address)
                 self.queue.put_nowait(request)
                 self._frame_versions[frame_type] = version
 
     def _mixers(self, indexes: Iterable[int]) -> Generator[Mixer, None, None]:
```

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/devices/mixer.py` & `PyPlumIO-0.4.1/pyplumio/devices/mixer.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/devices/thermostat.py` & `PyPlumIO-0.4.1/pyplumio/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/exceptions.py` & `PyPlumIO-0.4.1/pyplumio/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/filters.py` & `PyPlumIO-0.4.1/pyplumio/filters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/frames/__init__.py` & `PyPlumIO-0.4.1/pyplumio/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/frames/messages.py` & `PyPlumIO-0.4.1/pyplumio/frames/messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/frames/requests.py` & `PyPlumIO-0.4.1/pyplumio/frames/requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/frames/responses.py` & `PyPlumIO-0.4.1/pyplumio/frames/responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/helpers/data_types.py` & `PyPlumIO-0.4.1/pyplumio/helpers/data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/helpers/event_manager.py` & `PyPlumIO-0.4.1/pyplumio/helpers/event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/helpers/factory.py` & `PyPlumIO-0.4.1/pyplumio/helpers/factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/helpers/parameter.py` & `PyPlumIO-0.4.1/pyplumio/helpers/parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/helpers/schedule.py` & `PyPlumIO-0.4.1/pyplumio/helpers/schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/helpers/task_manager.py` & `PyPlumIO-0.4.1/pyplumio/helpers/task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/helpers/timeout.py` & `PyPlumIO-0.4.1/pyplumio/helpers/timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/helpers/uid.py` & `PyPlumIO-0.4.1/pyplumio/helpers/uid.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/protocol.py` & `PyPlumIO-0.4.1/pyplumio/protocol.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/stream.py` & `PyPlumIO-0.4.1/pyplumio/stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/__init__.py` & `PyPlumIO-0.4.1/pyplumio/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/alerts.py` & `PyPlumIO-0.4.1/pyplumio/structures/alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/data_schema.py` & `PyPlumIO-0.4.1/pyplumio/structures/data_schema.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/ecomax_parameters.py` & `PyPlumIO-0.4.1/pyplumio/structures/ecomax_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 from pyplumio import util
 from pyplumio.const import ATTR_INDEX, ATTR_OFFSET, ATTR_SIZE, ATTR_VALUE
 from pyplumio.devices import Addressable
 from pyplumio.frames import Request
 from pyplumio.helpers.factory import factory
 from pyplumio.helpers.parameter import BinaryParameter, Parameter, ParameterDescription
-from pyplumio.helpers.typing import EventDataType, ParameterDataType, ParameterValueType
+from pyplumio.helpers.typing import EventDataType, ParameterValueType
 from pyplumio.structures import StructureDecoder, ensure_device_data
 from pyplumio.structures.thermostat_parameters import ATTR_THERMOSTAT_PROFILE
 
 ATTR_ECOMAX_CONTROL: Final = "ecomax_control"
 ATTR_ECOMAX_PARAMETERS: Final = "ecomax_parameters"
 
+ECOMAX_PARAMETER_SIZE: Final = 3
+
 
 class EcomaxParameter(Parameter):
     """Represents ecoMAX parameter."""
 
     device: Addressable
     description: EcomaxParameterDescription
 
@@ -297,26 +299,37 @@
 
 THERMOSTAT_PROFILE_PARAMETER = EcomaxParameterDescription(name=ATTR_THERMOSTAT_PROFILE)
 
 
 class EcomaxParametersStructure(StructureDecoder):
     """Represents ecoMAX parameters data structure."""
 
+    _offset: int
+
+    def _ecomax_parameter(self, message: bytearray, start: int, end: int):
+        """Yields ecoMAX parameters."""
+        for index in range(start, start + end):
+            if parameter := util.unpack_parameter(message, self._offset):
+                yield (index, parameter)
+
+            self._offset += ECOMAX_PARAMETER_SIZE
+
     def decode(
         self, message: bytearray, offset: int = 0, data: EventDataType | None = None
     ) -> tuple[EventDataType, int]:
         """Decode bytes and return message data and offset."""
-        first_index = message[offset + 1]
-        last_index = message[offset + 2]
-        offset += 3
-        ecomax_parameters: list[tuple[int, ParameterDataType]] = []
-        for index in range(first_index, first_index + last_index):
-            parameter = util.unpack_parameter(message, offset)
-            if parameter is not None:
-                ecomax_parameters.append((index, parameter))
 
-            offset += 3
+        start = message[offset + 1]
+        end = message[offset + 2]
+        self._offset = offset + 3
 
         return (
-            ensure_device_data(data, {ATTR_ECOMAX_PARAMETERS: ecomax_parameters}),
-            offset,
+            ensure_device_data(
+                data,
+                {
+                    ATTR_ECOMAX_PARAMETERS: list(
+                        self._ecomax_parameter(message, start, end)
+                    )
+                },
+            ),
+            self._offset,
         )
```

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/fan_power.py` & `PyPlumIO-0.4.1/pyplumio/structures/fan_power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/frame_versions.py` & `PyPlumIO-0.4.1/pyplumio/structures/frame_versions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/fuel_consumption.py` & `PyPlumIO-0.4.1/pyplumio/structures/fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/fuel_level.py` & `PyPlumIO-0.4.1/pyplumio/structures/fuel_level.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/lambda_sensor.py` & `PyPlumIO-0.4.1/pyplumio/structures/lambda_sensor.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/load.py` & `PyPlumIO-0.4.1/pyplumio/structures/load.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/mixer_parameters.py` & `PyPlumIO-0.4.1/pyplumio/structures/mixer_parameters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Contains mixer parameter structure decoder."""
 from __future__ import annotations
 
-from collections.abc import Iterable
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Final
 
 from pyplumio import util
 from pyplumio.const import ATTR_DEVICE_INDEX, ATTR_INDEX, ATTR_VALUE
 from pyplumio.frames import Request
 from pyplumio.helpers.factory import factory
@@ -14,14 +13,16 @@
 from pyplumio.structures import StructureDecoder, ensure_device_data
 
 if TYPE_CHECKING:
     from pyplumio.devices.mixer import Mixer
 
 ATTR_MIXER_PARAMETERS: Final = "mixer_parameters"
 
+MIXER_PARAMETER_SIZE: Final = 3
+
 
 class MixerParameter(Parameter):
     """Represents mixer parameter."""
 
     device: Mixer
     description: MixerParameterDescription
 
@@ -113,52 +114,45 @@
     MixerParameterDescription(name="heating_curve", multiplier=10),
     MixerParameterDescription(name="heating_curve_shift", offset=20),
     MixerParameterDescription(name="thermostat_function"),
     MixerParameterDescription(name="thermostat_decrease_temp"),
 )
 
 
-def _decode_mixer_parameters(
-    message: bytearray, offset: int, indexes: Iterable
-) -> tuple[list[tuple[int, ParameterDataType]], int]:
-    """Decode parameters for a single mixer."""
-    parameters: list[tuple[int, ParameterDataType]] = []
-    for index in indexes:
-        parameter = util.unpack_parameter(message, offset)
-        if parameter is not None:
-            parameters.append((index, parameter))
+class MixerParametersStructure(StructureDecoder):
+    """Represent mixer parameters data structure."""
 
-        offset += 3
+    _offset: int
 
-    return parameters, offset
+    def _mixer_parameter(self, message: bytearray, start: int, end: int):
+        """Yields mixer parameters."""
+        for index in range(start, start + end):
+            if (parameter := util.unpack_parameter(message, self._offset)) is not None:
+                yield (index, parameter)
 
-
-class MixerParametersStructure(StructureDecoder):
-    """Represent mixer parameters data structure."""
+            self._offset += MIXER_PARAMETER_SIZE
 
     def decode(
         self, message: bytearray, offset: int = 0, data: EventDataType | None = None
     ) -> tuple[EventDataType, int]:
         """Decode bytes and return message data and offset."""
-        first_index = message[offset + 1]
-        last_index = message[offset + 2]
-        mixer_count = message[offset + 3]
-        parameter_count_per_mixer = first_index + last_index
-        offset += 4
+        start = message[offset + 1]
+        end = message[offset + 2]
+        mixers = message[offset + 3]
+        self._offset = offset + 4
+
         mixer_parameters: dict[int, list[tuple[int, ParameterDataType]]] = {}
-        for index in range(mixer_count):
-            parameters, offset = _decode_mixer_parameters(
-                message,
-                offset,
-                range(first_index, parameter_count_per_mixer),
-            )
-            if parameters:
-                mixer_parameters[index] = parameters
-
-        if not mixer_parameters:
-            # No mixer parameters detected.
-            return ensure_device_data(data, {ATTR_MIXER_PARAMETERS: None}), offset
+        for mixer in range(mixers):
+            if parameters := list(self._mixer_parameter(message, start, end)):
+                mixer_parameters[mixer] = parameters
 
         return (
-            ensure_device_data(data, {ATTR_MIXER_PARAMETERS: mixer_parameters}),
-            offset,
+            ensure_device_data(
+                data,
+                {
+                    ATTR_MIXER_PARAMETERS: (
+                        None if not mixer_parameters else mixer_parameters
+                    )
+                },
+            ),
+            self._offset,
         )
```

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/mixer_sensors.py` & `PyPlumIO-0.4.1/pyplumio/structures/mixer_sensors.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/modules.py` & `PyPlumIO-0.4.1/pyplumio/structures/modules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/network_info.py` & `PyPlumIO-0.4.1/pyplumio/structures/network_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/output_flags.py` & `PyPlumIO-0.4.1/pyplumio/structures/output_flags.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/outputs.py` & `PyPlumIO-0.4.1/pyplumio/structures/outputs.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/pending_alerts.py` & `PyPlumIO-0.4.1/pyplumio/structures/pending_alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/power.py` & `PyPlumIO-0.4.1/pyplumio/structures/power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/product_info.py` & `PyPlumIO-0.4.1/pyplumio/structures/product_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/program_version.py` & `PyPlumIO-0.4.1/pyplumio/structures/program_version.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/regulator_data.py` & `PyPlumIO-0.4.1/pyplumio/structures/regulator_data.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/schedules.py` & `PyPlumIO-0.4.1/pyplumio/structures/schedules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/statuses.py` & `PyPlumIO-0.4.1/pyplumio/structures/statuses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/temperatures.py` & `PyPlumIO-0.4.1/pyplumio/structures/temperatures.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/thermostat_parameters.py` & `PyPlumIO-0.4.1/pyplumio/structures/thermostat_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Contains thermostat parameter structure decoder."""
 from __future__ import annotations
 
-from collections.abc import Iterable
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Final
 
 from pyplumio import util
 from pyplumio.const import ATTR_INDEX, ATTR_OFFSET, ATTR_SIZE, ATTR_VALUE
 from pyplumio.frames import Request
 from pyplumio.helpers.factory import factory
 from pyplumio.helpers.parameter import BinaryParameter, Parameter, ParameterDescription
 from pyplumio.helpers.typing import EventDataType, ParameterDataType, ParameterValueType
 from pyplumio.structures import StructureDecoder, ensure_device_data
 from pyplumio.structures.thermostat_sensors import ATTR_THERMOSTAT_COUNT
 
+if TYPE_CHECKING:
+    from pyplumio.devices.thermostat import Thermostat
+
+
 ATTR_THERMOSTAT_PROFILE: Final = "thermostat_profile"
 ATTR_THERMOSTAT_PARAMETERS: Final = "thermostat_parameters"
 ATTR_THERMOSTAT_PARAMETERS_DECODER: Final = "thermostat_parameters_decoder"
 
-if TYPE_CHECKING:
-    from pyplumio.devices.thermostat import Thermostat
+THERMOSTAT_PARAMETER_SIZE: Final = 3
 
 
 class ThermostatParameter(Parameter):
     """Represents thermostat parameter."""
 
     device: Thermostat
     description: ThermostatParameterDescription
@@ -103,76 +105,72 @@
     ),
     ThermostatParameterDescription(name="heating_target_temp", size=2, multiplier=10),
     ThermostatParameterDescription(name="heating_timer"),
     ThermostatParameterDescription(name="off_timer"),
 )
 
 
-def _decode_thermostat_parameters(
-    message: bytearray, offset: int, indexes: Iterable
-) -> tuple[list[tuple[int, ParameterDataType]], int]:
-    """Decode parameters for a single thermostat."""
-    parameters: list[tuple[int, ParameterDataType]] = []
-    for index in indexes:
-        description = THERMOSTAT_PARAMETERS[index]
-        parameter = util.unpack_parameter(message, offset, size=description.size)
-        if parameter is not None:
-            parameters.append((index, parameter))
-
-        offset += 3 * description.size
-
-    return parameters, offset
+def _empty_response(
+    offset: int, data: EventDataType | None = None
+) -> tuple[EventDataType, int]:
+    """Return empty response."""
+    return (
+        ensure_device_data(
+            data,
+            {ATTR_THERMOSTAT_PARAMETERS: None, ATTR_THERMOSTAT_PROFILE: None},
+        ),
+        offset,
+    )
 
 
 class ThermostatParametersStructure(StructureDecoder):
     """Represent thermostat parameters data structure."""
 
+    _offset: int
+
+    def _thermostat_parameter(
+        self, message: bytearray, thermostats: int, start: int, end: int
+    ):
+        """Yields thermostat parameters."""
+        for index in range(start, (start + end) // thermostats):
+            description = THERMOSTAT_PARAMETERS[index]
+            if (
+                parameter := util.unpack_parameter(
+                    message, self._offset, size=description.size
+                )
+            ) is not None:
+                yield (index, parameter)
+
+            self._offset += THERMOSTAT_PARAMETER_SIZE * description.size
+
     def decode(
         self, message: bytearray, offset: int = 0, data: EventDataType | None = None
     ) -> tuple[EventDataType, int]:
         """Decode bytes and return message data and offset."""
         data = ensure_device_data(data)
-        thermostat_count = data.get(ATTR_THERMOSTAT_COUNT, 0)
-        if thermostat_count == 0:
-            return (
-                ensure_device_data(
-                    data,
-                    {ATTR_THERMOSTAT_PARAMETERS: None, ATTR_THERMOSTAT_PROFILE: None},
-                ),
-                offset,
-            )
+        thermostats = data.get(ATTR_THERMOSTAT_COUNT, 0)
+        if thermostats == 0:
+            return _empty_response(offset, data)
 
-        first_index = message[offset + 1]
-        last_index = message[offset + 2]
+        start = message[offset + 1]
+        end = message[offset + 2]
         thermostat_profile = util.unpack_parameter(message, offset + 3)
-        parameter_count_per_thermostat = (first_index + last_index) // thermostat_count
-        offset += 6
+        self._offset = offset + 6
         thermostat_parameters: dict[int, list[tuple[int, ParameterDataType]]] = {}
-        for index in range(thermostat_count):
-            parameters, offset = _decode_thermostat_parameters(
-                message,
-                offset,
-                range(first_index, parameter_count_per_thermostat),
-            )
-            if parameters:
-                thermostat_parameters[index] = parameters
-
-        if not thermostat_parameters:
-            # No thermostat parameters detected.
-            return (
-                ensure_device_data(
-                    data,
-                    {ATTR_THERMOSTAT_PARAMETERS: None, ATTR_THERMOSTAT_PROFILE: None},
-                ),
-                offset,
-            )
+        for thermostat in range(thermostats):
+            if parameters := list(
+                self._thermostat_parameter(message, thermostats, start, end)
+            ):
+                thermostat_parameters[thermostat] = parameters
 
         return (
             ensure_device_data(
                 data,
                 {
                     ATTR_THERMOSTAT_PROFILE: thermostat_profile,
-                    ATTR_THERMOSTAT_PARAMETERS: thermostat_parameters,
+                    ATTR_THERMOSTAT_PARAMETERS: None
+                    if not thermostat_parameters
+                    else thermostat_parameters,
                 },
             ),
-            offset,
+            self._offset,
         )
```

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/structures/thermostat_sensors.py` & `PyPlumIO-0.4.1/pyplumio/structures/thermostat_sensors.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyplumio/util.py` & `PyPlumIO-0.4.1/pyplumio/util.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/pyproject.toml` & `PyPlumIO-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/conftest.py` & `PyPlumIO-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/frames/test_init.py` & `PyPlumIO-0.4.1/tests/frames/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/frames/test_messages.py` & `PyPlumIO-0.4.1/tests/frames/test_messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/frames/test_requests.py` & `PyPlumIO-0.4.1/tests/frames/test_requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/frames/test_responses.py` & `PyPlumIO-0.4.1/tests/frames/test_responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/helpers/test_data_types.py` & `PyPlumIO-0.4.1/tests/helpers/test_data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/helpers/test_event_manager.py` & `PyPlumIO-0.4.1/tests/helpers/test_event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/helpers/test_factory.py` & `PyPlumIO-0.4.1/tests/helpers/test_factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/helpers/test_parameter.py` & `PyPlumIO-0.4.1/tests/helpers/test_parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/helpers/test_schedule.py` & `PyPlumIO-0.4.1/tests/helpers/test_schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/helpers/test_task_manager.py` & `PyPlumIO-0.4.1/tests/helpers/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/helpers/test_timeout.py` & `PyPlumIO-0.4.1/tests/helpers/test_timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/test_connection.py` & `PyPlumIO-0.4.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/test_devices.py` & `PyPlumIO-0.4.1/tests/test_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 from unittest.mock import AsyncMock, Mock, call, patch
 
 import pytest
 
 from pyplumio.const import (
     ATTR_DEVICE_INDEX,
+    ATTR_FRAME_ERRORS,
     ATTR_INDEX,
     ATTR_LOADED,
     ATTR_OFFSET,
     ATTR_PARAMETER,
     ATTR_SCHEDULE,
     ATTR_SIZE,
     ATTR_SWITCH,
@@ -113,30 +114,40 @@
         "pyplumio.devices.ecomax.EcoMAX.request",
         side_effect=(True, True, True, True, True, True, True, True),
     ) as mock_request:
         await ecomax.async_setup()
         await ecomax.wait_until_done()
 
     assert await ecomax.get(ATTR_LOADED)
+    assert not ecomax.data[ATTR_FRAME_ERRORS]
     assert mock_request.await_count == len(DATA_FRAME_TYPES)
 
 
 async def test_async_setup_error(caplog) -> None:
     """Test with error during requesting initial data frames."""
     ecomax = EcoMAX(asyncio.Queue(), network=NetworkInfo())
 
     with patch("pyplumio.devices.ecomax.EcoMAX.wait_for"), patch(
         "pyplumio.devices.ecomax.EcoMAX.request",
-        side_effect=(ValueError("test"), True, True, True, True, True, True, True),
+        side_effect=(
+            ValueError("test", FrameType.REQUEST_ALERTS),
+            True,
+            True,
+            True,
+            True,
+            True,
+            True,
+            True,
+        ),
     ) as mock_request:
         await ecomax.async_setup()
         await ecomax.wait_until_done()
 
-    assert "Request failed" in caplog.text
-    assert not await ecomax.get(ATTR_LOADED)
+    assert await ecomax.get(ATTR_LOADED)
+    assert ecomax.data[ATTR_FRAME_ERRORS][0] == FrameType.REQUEST_ALERTS
     assert mock_request.await_count == len(DATA_FRAME_TYPES)
 
 
 async def test_frame_versions_update(
     ecomax: EcoMAX, messages: dict[FrameType, bytearray]
 ) -> None:
     """Test requesting updated frames."""
```

### Comparing `PyPlumIO-0.4.0.post1/tests/test_filters.py` & `PyPlumIO-0.4.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/test_init.py` & `PyPlumIO-0.4.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/test_main.py` & `PyPlumIO-0.4.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/test_protocol.py` & `PyPlumIO-0.4.1/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/test_stream.py` & `PyPlumIO-0.4.1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tests/test_util.py` & `PyPlumIO-0.4.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0.post1/tox.ini` & `PyPlumIO-0.4.1/tox.ini`

 * *Files identical despite different names*

