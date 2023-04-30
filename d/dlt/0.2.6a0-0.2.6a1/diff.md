# Comparing `tmp/dlt-0.2.6a0.tar.gz` & `tmp/dlt-0.2.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.6a0.tar", max compression
+gzip compressed data, was "dlt-0.2.6a1.tar", max compression
```

## Comparing `dlt-0.2.6a0.tar` & `dlt-0.2.6a1.tar`

### file list

```diff
@@ -1,204 +1,207 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.6a0/LICENSE.txt
--rw-r--r--   0        0        0     5264 2023-04-22 20:26:30.632198 dlt-0.2.6a0/README.md
--rw-r--r--   0        0        0     1677 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/__init__.py
--rw-r--r--   0        0        0       31 2023-03-03 14:20:21.286564 dlt-0.2.6a0/dlt/cli/__init__.py
--rw-r--r--   0        0        0    13282 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3653 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    16663 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0     1683 2023-03-26 19:01:53.563115 dlt-0.2.6a0/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18888 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/cli/init_command.py
--rw-r--r--   0        0        0     6255 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9419 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4404 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0      106 2023-03-03 14:20:18.076564 dlt-0.2.6a0/dlt/cli/typing.py
--rw-r--r--   0        0        0     3662 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.6a0/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     4898 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3448 2023-04-05 15:15:49.779453 dlt-0.2.6a0/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1198 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      252 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1108 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1089 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1193 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     2050 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     5320 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    18084 2023-04-22 20:22:19.252199 dlt-0.2.6a0/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      868 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1679 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0    10914 2023-04-09 16:39:04.593180 dlt-0.2.6a0/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     3190 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     2125 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12020 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/configuration/specs/gcp_client_credentials.py
--rw-r--r--   0        0        0      665 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/load_volume_configuration.py
--rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/normalize_volume_configuration.py
--rw-r--r--   0        0        0     2769 2023-04-06 08:59:11.959561 dlt-0.2.6a0/dlt/common/configuration/specs/postgres_credentials.py
--rw-r--r--   0        0        0     2532 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/configuration/specs/schema_volume_configuration.py
--rw-r--r--   0        0        0     5339 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.6a0/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    10682 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6439 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/git.py
--rw-r--r--   0        0        0     5248 2023-04-10 08:12:53.759595 dlt-0.2.6a0/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.6a0/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.6a0/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13396 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.6a0/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/pendulum.py
--rw-r--r--   0        0        0    14901 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.6a0/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.6a0/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-23 12:08:49.194852 dlt-0.2.6a0/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      210 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0     1079 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0      939 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/init.py
--rw-r--r--   0        0        0     7832 2023-04-03 13:25:54.449156 dlt-0.2.6a0/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      583 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5250 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runners/venv.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0     3828 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0     6320 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2026 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2479 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     1943 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      989 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.6a0/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    21954 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/schema/utils.py
--rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0     9059 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.6a0/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21684 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2525 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2677 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/common/typing.py
--rw-r--r--   0        0        0    11275 2023-04-23 12:08:49.204852 dlt-0.2.6a0/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12301 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      392 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10123 2023-04-23 12:08:49.204852 dlt-0.2.6a0/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     6964 2023-04-23 18:00:31.976853 dlt-0.2.6a0/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.6a0/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4975 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    14398 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0      443 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6066 2023-04-13 08:33:43.967587 dlt-0.2.6a0/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.6a0/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      405 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     6850 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.6a0/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-23 12:08:49.204852 dlt-0.2.6a0/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a0/dlt/extract/__init__.py
--rw-r--r--   0        0        0    22569 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12184 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     7654 2023-04-16 18:26:08.732459 dlt-0.2.6a0/dlt/extract/extract.py
--rw-r--r--   0        0        0    14541 2023-04-23 12:24:07.664852 dlt-0.2.6a0/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31380 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/schema.py
--rw-r--r--   0        0        0    31994 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/source.py
--rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.6a0/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.6a0/dlt/helpers/__init__.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    14293 2023-03-23 14:48:32.561618 dlt-0.2.6a0/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2373 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13039 2023-04-23 12:23:38.014852 dlt-0.2.6a0/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/load/__init__.py
--rw-r--r--   0        0        0     1103 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/load/exceptions.py
--rw-r--r--   0        0        0    20447 2023-04-05 08:03:40.638919 dlt-0.2.6a0/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1182 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a0/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    17989 2023-04-13 12:56:33.587587 dlt-0.2.6a0/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/pipeline/README.md
--rw-r--r--   0        0        0    12224 2023-04-13 08:33:43.967587 dlt-0.2.6a0/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1823 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      363 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     2537 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     1497 2023-04-21 19:04:10.089942 dlt-0.2.6a0/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    58298 2023-04-23 13:33:49.844852 dlt-0.2.6a0/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.6a0/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.6a0/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.6a0/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.6a0/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/reflection/names.py
--rw-r--r--   0        0        0     4986 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      118 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/sources/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.6a0/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9092 2023-04-23 12:08:49.204852 dlt-0.2.6a0/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.6a0/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.6a0/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.6a0/dlt/version.py
--rw-r--r--   0        0        0     3893 2023-04-23 18:00:31.976853 dlt-0.2.6a0/pyproject.toml
--rw-r--r--   0        0        0     8483 1970-01-01 00:00:00.000000 dlt-0.2.6a0/setup.py
--rw-r--r--   0        0        0     8409 1970-01-01 00:00:00.000000 dlt-0.2.6a0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.6a1/LICENSE.txt
+-rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.6a1/README.md
+-rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    15501 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3808 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    16663 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18888 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10489 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9419 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4404 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.6a1/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     4898 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3448 2023-04-05 15:15:49.779453 dlt-0.2.6a1/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1198 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      252 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0     1108 2023-04-26 11:34:23.292768 dlt-0.2.6a1/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1089 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1193 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     2050 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0     5320 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18054 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      868 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1679 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0    10914 2023-04-09 16:39:04.593180 dlt-0.2.6a1/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     3295 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12193 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/specs/gcp_client_credentials.py
+-rw-r--r--   0        0        0      665 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/load_volume_configuration.py
+-rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/normalize_volume_configuration.py
+-rw-r--r--   0        0        0     2843 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/specs/postgres_credentials.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/schema_volume_configuration.py
+-rw-r--r--   0        0        0     5339 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.6a1/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    10682 2023-04-24 11:35:34.867759 dlt-0.2.6a1/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6121 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/git.py
+-rw-r--r--   0        0        0     5248 2023-04-10 08:12:53.759595 dlt-0.2.6a1/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.6a1/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.6a1/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.6a1/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13396 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.6a1/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    16937 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.6a1/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      508 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5250 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4264 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.6a1/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0     9059 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.6a1/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21810 2023-04-29 12:58:55.953219 dlt-0.2.6a1/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2677 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/typing.py
+-rw-r--r--   0        0        0    11275 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12301 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      392 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10123 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7025 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.6a1/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4975 2023-04-24 11:35:34.867759 dlt-0.2.6a1/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    15181 2023-04-29 12:58:55.953219 dlt-0.2.6a1/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0      443 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6066 2023-04-13 08:33:43.967587 dlt-0.2.6a1/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      405 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.6a1/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.6a1/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a1/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    22569 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8449 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14650 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    31567 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/extract/schema.py
+-rw-r--r--   0        0        0    33994 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/source.py
+-rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.6a1/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.6a1/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/helpers/airflow/__init__.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2373 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/helpers/pandas.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/helpers/streamlit.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1019 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19928 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a1/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16576 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/pipeline/README.md
+-rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      363 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8447 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    56164 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.6a1/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.6a1/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.6a1/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.6a1/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/reflection/names.py
+-rw-r--r--   0        0        0     4986 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      118 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.6a1/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9092 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/version.py
+-rw-r--r--   0        0        0     3928 2023-04-30 21:17:44.408805 dlt-0.2.6a1/pyproject.toml
+-rw-r--r--   0        0        0     7395 1970-01-01 00:00:00.000000 dlt-0.2.6a1/setup.py
+-rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 dlt-0.2.6a1/PKG-INFO
```

### Comparing `dlt-0.2.6a0/LICENSE.txt` & `dlt-0.2.6a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/__init__.py` & `dlt-0.2.6a1/dlt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from dlt.common.configuration.specs import CredentialsConfiguration as _CredentialsConfiguration
 from dlt.common.pipeline import source_state as state
 from dlt.common.schema import Schema
 
 from dlt import sources
 from dlt.extract.decorators import source, resource, transformer, defer
 from dlt.pipeline import pipeline as _pipeline, run, attach, Pipeline, dbt, current as _current, mark as _mark
+from dlt.pipeline import progress
 
 pipeline = _pipeline
 current = _current
 mark = _mark
 
 TSecretValue = _TSecretValue
 "When typing source/resource function arguments it indicates that a given argument is a secret and should be taken from dlt.secrets."
```

### Comparing `dlt-0.2.6a0/dlt/cli/_dlt.py` & `dlt-0.2.6a1/dlt/cli/_dlt.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dlt.common.schema import Schema
 from dlt.common.typing import DictStrAny
 
 import dlt.cli.echo as fmt
 from dlt.cli import utils
 from dlt.cli.init_command import init_command, list_pipelines_command, DLT_INIT_DOCS_URL, DEFAULT_PIPELINES_REPO
 from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL
-from dlt.cli.pipeline_command import pipeline_command
+from dlt.cli.pipeline_command import pipeline_command, DLT_PIPELINE_COMMAND_DOCS_URL
 from dlt.pipeline.exceptions import CannotRestorePipelineException
 
 
 @utils.track_command("init", False, "pipeline_name", "destination_name")
 def init_command_wrapper(pipeline_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str) -> int:
     try:
         init_command(pipeline_name, destination_name, use_generic_template, repo_location, branch)
@@ -58,37 +58,43 @@
         return -1
     except InvalidGitRepositoryError:
         click.secho(
             "No git repository found for pipeline script %s.\nAdd your local code to Github as described here: %s" % (fmt.bold(pipeline_script_path), fmt.bold("https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github")),
             err=True,
             fg="red"
         )
+        fmt.note("If you do not have a repository yet, the easiest way to proceed is to create one on Github and then clone it here.")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
         return -1
     except NoSuchPathError as path_ex:
         click.secho(
             "The pipeline script does not exist\n%s" % str(path_ex),
             err=True,
             fg="red"
         )
         return -1
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
         # TODO: display stack trace if with debug flag
-        raise
     return 0
 
 
 @utils.track_command("pipeline", True, "operation")
-def pipeline_command_wrapper(operation: str, pipeline_name: str, pipelines_dir: str, verbosity: int, load_id: str = None) -> int:
+def pipeline_command_wrapper(
+        operation: str, pipeline_name: str, pipelines_dir: str, verbosity: int, **command_kwargs: Any
+) -> int:
     try:
-        pipeline_command(operation, pipeline_name, pipelines_dir, verbosity, load_id)
+        pipeline_command(operation, pipeline_name, pipelines_dir, verbosity, **command_kwargs)
         return 0
-    except (CannotRestorePipelineException, Exception) as ex:
+    except CannotRestorePipelineException as ex:
+        click.secho(str(ex), err=True, fg="red")
+        click.secho("Try command %s to restore the pipeline state from destination" % fmt.bold(f"dlt pipeline {pipeline_name} sync"))
+        return 1
+    except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         return 1
 
 
 @utils.track_command("schema", False, "operation")
 def schema_command_wrapper(file_path: str, format_: str, remove_defaults: bool) -> int:
     with open(file_path, "br") as f:
@@ -176,57 +182,83 @@
     init_cmd.add_argument("pipeline", nargs='?', help="Pipeline name. Adds existing pipeline or creates a new pipeline template if pipeline for your data source is not yet implemented.")
     init_cmd.add_argument("destination", nargs='?', help="Name of a destination ie. bigquery or redshift")
     init_cmd.add_argument("--location", default=DEFAULT_PIPELINES_REPO, help="Advanced. Uses a specific url or local path to pipelines repository.")
     init_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the init repository to fetch the template.")
     init_cmd.add_argument("--generic", default=False, action="store_true", help="When present uses a generic template with all the dlt loading code present will be used. Otherwise a debug template is used that can be immediately run to get familiar with the dlt sources.")
 
     deploy_cmd = subparsers.add_parser("deploy", help="Creates a deployment package for a selected pipeline script")
-    deploy_cmd.add_argument("pipeline-script-path", help="Path to a pipeline script")
-    deploy_cmd.add_argument("deployment-method", choices=["github-action"], default="github-action", help="Deployment method")
+    deploy_cmd.add_argument("pipeline_script_path", metavar="pipeline-script-path", help="Path to a pipeline script")
+    deploy_cmd.add_argument("deployment_method", metavar="deployment-method", choices=["github-action"], default="github-action", help="Deployment method")
     deploy_cmd.add_argument("--schedule", required=True, help="A schedule with which to run the pipeline, in cron format. Example: '*/30 * * * *' will run the pipeline every 30 minutes.")
     deploy_cmd.add_argument("--run-manually", default=True, action="store_true", help="Allows the pipeline to be run manually form Github Actions UI.")
     deploy_cmd.add_argument("--run-on-push", default=False, action="store_true", help="Runs the pipeline with every push to the repository.")
     deploy_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the deploy repository to fetch the template.")
 
     schema = subparsers.add_parser("schema", help="Shows, converts and upgrades schemas")
     schema.add_argument("file", help="Schema file name, in yaml or json format, will autodetect based on extension")
     schema.add_argument("--format", choices=["json", "yaml"], default="yaml", help="Display schema in this format")
     schema.add_argument("--remove-defaults", action="store_true", help="Does not show default hint values")
 
     pipe_cmd = subparsers.add_parser("pipeline", help="Operations on pipelines that were ran locally")
     pipe_cmd.add_argument("--list-pipelines", "-l",  default=False, action="store_true", help="List local pipelines")
-    pipe_cmd.add_argument("name", nargs='?', help="Pipeline name")
+    pipe_cmd.add_argument("pipeline_name", nargs='?', help="Pipeline name")
     pipe_cmd.add_argument("--pipelines-dir", help="Pipelines working directory", default=None)
-    pipe_cmd.add_argument("--verbose", "-v", action='count', default=0, help="Provides more information for certain commands.")
+    pipe_cmd.add_argument("--verbose", "-v", action='count', default=0, help="Provides more information for certain commands.", dest="verbosity")
+    # pipe_cmd.add_argument("--dataset-name", help="Dataset name used to sync destination when local pipeline state is missing.")
+    # pipe_cmd.add_argument("--destination", help="Destination name used to to sync when local pipeline state is missing.")
 
     pipeline_subparsers = pipe_cmd.add_subparsers(dest="operation", required=False)
+
+    pipe_cmd_sync_parent = argparse.ArgumentParser(add_help=False)
+    pipe_cmd_sync_parent.add_argument("--destination", help="Sync from this destination when local pipeline state is missing.")
+    pipe_cmd_sync_parent.add_argument("--dataset-name", help="Dataset name to sync from when local pipeline state is missing.")
+
     pipeline_subparsers.add_parser("info", help="Displays state of the pipeline, use -v or -vv for more info")
     pipeline_subparsers.add_parser("show", help="Generates and launches Streamlit app with the loading status and dataset explorer")
     pipeline_subparsers.add_parser("failed-jobs", help="Displays information on all the failed loads in all completed packages, failed jobs and associated error messages")
-    pipeline_subparsers.add_parser("sync", help="Drops the local state of the pipeline and resets all the schemas and restores it from destination. The destination state, data and schemas are left intact.")
+    pipeline_subparsers.add_parser(
+        "sync",
+        help="Drops the local state of the pipeline and resets all the schemas and restores it from destination. The destination state, data and schemas are left intact.",
+        parents=[pipe_cmd_sync_parent]
+    )
     pipeline_subparsers.add_parser("trace", help="Displays last run trace, use -v or -vv for more info")
     pipe_cmd_schema = pipeline_subparsers.add_parser("schema", help="Displays default schema")
     pipe_cmd_schema.add_argument("--format", choices=["json", "yaml"], default="yaml", help="Display schema in this format")
     pipe_cmd_schema.add_argument("--remove-defaults", action="store_true", help="Does not show default hint values")
 
+    pipe_cmd_drop = pipeline_subparsers.add_parser(
+        "drop",
+        help="Selectively drop tables and reset state",
+        parents=[pipe_cmd_sync_parent],
+        epilog=f"See {DLT_PIPELINE_COMMAND_DOCS_URL}#selectively-drop-tables-and-reset-state for more info"
+    )
+    pipe_cmd_drop.add_argument("resources", nargs="*", help="One or more resources to drop. Can be exact resource name(s) or regex pattern(s). Regex patterns must start with re:")
+    pipe_cmd_drop.add_argument("--drop-all", action="store_true", default=False, help="Drop all resources found in schema. Supersedes [resources] argument.")
+    pipe_cmd_drop.add_argument("--state-paths", nargs="*", help="State keys or json paths to drop", default=())
+    pipe_cmd_drop.add_argument("--schema", help="Schema name to drop from (if other than default schema).", dest="schema_name")
+    pipe_cmd_drop.add_argument("--state-only", action="store_true", help="Only wipe state for matching resources without dropping tables.", default=False)
+
     pipe_cmd_package = pipeline_subparsers.add_parser("load-package", help="Displays information on load package, use -v or -vv for more info")
-    pipe_cmd_package.add_argument("load_id", nargs='?', help="Load id of completed or normalized package. Defaults to the most recent package.")
+    pipe_cmd_package.add_argument("load_id", metavar="load-id", nargs='?', help="Load id of completed or normalized package. Defaults to the most recent package.")
 
     subparsers.add_parser("telemetry", help="Shows telemetry status")
 
     args = parser.parse_args()
 
     if args.command == "schema":
         return schema_command_wrapper(args.file, args.format, args.remove_defaults)
     elif args.command == "pipeline":
         if args.list_pipelines:
-            return pipeline_command_wrapper("list", "-", args.pipelines_dir, args.verbose)
+            return pipeline_command_wrapper("list", "-", args.pipelines_dir, args.verbosity)
         else:
-            load_id = args.load_id if args.operation == "load-package" else None
-            return pipeline_command_wrapper(args.operation or "info", args.name, args.pipelines_dir, args.verbose, load_id)
+            command_kwargs = dict(args._get_kwargs())
+            command_kwargs['operation'] = args.operation or "info"
+            del command_kwargs["command"]
+            del command_kwargs["list_pipelines"]
+            return pipeline_command_wrapper(**command_kwargs)
     elif args.command == "init":
         if args.list_pipelines:
             return list_pipelines_command_wrapper(args.location, args.branch)
         else:
             if not args.pipeline or not args.destination:
                 init_cmd.print_usage()
                 return -1
```

### Comparing `dlt-0.2.6a0/dlt/cli/config_toml_writer.py` & `dlt-0.2.6a1/dlt/cli/config_toml_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,16 +66,19 @@
     if is_base_configuration_inner_hint(hint):
         inner_table = tomlkit.table(False)
         write_spec(inner_table, hint(), overwrite_existing)
         if len(inner_table) > 0:
             toml_table[name] = inner_table
     else:
         if default_value is None:
-            toml_table[name] = generate_typed_example(name, hint)
-            toml_table[name].comment("please set me up!")
+            example_value = generate_typed_example(name, hint)
+            toml_table[name] = example_value
+            # tomlkit not supporting comments on boolean
+            if not isinstance(example_value, bool):
+                toml_table[name].comment("please set me up!")
         elif is_default_of_interest:
             toml_table[name] = default_value
 
 
 def write_spec(toml_table: TOMLTable, config: BaseConfiguration, overwrite_existing: bool) -> None:
     for name, hint in config.get_resolvable_fields().items():
         default_value = getattr(config, name, None)
```

### Comparing `dlt-0.2.6a0/dlt/cli/deploy_command.py` & `dlt-0.2.6a1/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/cli/echo.py` & `dlt-0.2.6a1/dlt/cli/echo.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 style = click.style
 
 
 def bold(msg: str) -> str:
     return click.style(msg, bold=True, reset=True)
 
 
+def error(msg: str) -> None:
+    click.secho("ERROR: " + msg, fg="red")
+
+
 def warning(msg: str) -> None:
     click.secho("WARNING: " + msg, fg="yellow")
 
 
 def note(msg: str) -> None:
     click.secho("NOTE: " + msg, fg="green")
 
@@ -52,7 +56,10 @@
         assert ALWAYS_CHOOSE_VALUE in choices
         return ALWAYS_CHOOSE_VALUE
     if ALWAYS_CHOOSE_DEFAULT:
         assert default is not None
         return default
     click_choices = click.Choice(choices)
     return click.prompt(text, type=click_choices, default=default)
+
+def text_input(text: str) -> str:
+    return click.prompt(text)  # type: ignore[no-any-return]
```

### Comparing `dlt-0.2.6a0/dlt/cli/init_command.py` & `dlt-0.2.6a1/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/cli/pipeline_files.py` & `dlt-0.2.6a1/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/cli/source_detection.py` & `dlt-0.2.6a1/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/cli/telemetry_command.py` & `dlt-0.2.6a1/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/cli/utils.py` & `dlt-0.2.6a1/dlt/cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ast
 import inspect
 import os
 import tempfile
 import time
+import contextlib
 from typing import Any, Callable, Tuple
 
 from dlt.common import git
 from dlt.common.reflection.utils import set_ast_parents
 from dlt.common.storages import FileStorage
 from dlt.common.typing import TFun
 from dlt.common.runtime.telemetry import start_telemetry
@@ -66,20 +67,21 @@
         def _wrap(*f_args: Any, **f_kwargs: Any) -> Any:
             # look for additional arguments
             bound_args = sig.bind(*f_args, **f_kwargs)
             props = {p:bound_args.arguments[p] for p in args if p in bound_args.arguments}
             start_ts = time.time()
 
             def _track(success: bool) -> None:
-                props["elapsed"] = time.time() - start_ts
-                props["success"] = success
-                # resolve runtime config and init telemetry
-                c = resolve_configuration(RunConfiguration())
-                start_telemetry(c)
-                track("command", command, props)
+                with contextlib.suppress(Exception):
+                    props["elapsed"] = time.time() - start_ts
+                    props["success"] = success
+                    # resolve runtime config and init telemetry
+                    c = resolve_configuration(RunConfiguration())
+                    start_telemetry(c)
+                    track("command", command, props)
 
             # some commands should be tracked before execution
             if track_before:
                 _track(True)
                 return f(*f_args, **f_kwargs)
             # some commands we track after, where we can pass the success
             try:
```

### Comparing `dlt-0.2.6a0/dlt/common/arithmetics.py` & `dlt-0.2.6a1/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/accessors.py` & `dlt-0.2.6a1/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/container.py` & `dlt-0.2.6a1/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/exceptions.py` & `dlt-0.2.6a1/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/inject.py` & `dlt-0.2.6a1/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/paths.py` & `dlt-0.2.6a1/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/providers/airflow.py` & `dlt-0.2.6a1/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/providers/context.py` & `dlt-0.2.6a1/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/providers/dictionary.py` & `dlt-0.2.6a1/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/providers/environ.py` & `dlt-0.2.6a1/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/providers/provider.py` & `dlt-0.2.6a1/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/providers/toml.py` & `dlt-0.2.6a1/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/resolve.py` & `dlt-0.2.6a1/dlt/common/configuration/resolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
 def _maybe_parse_native_value(config: TConfiguration, explicit_value: Any, embedded_sections: Tuple[str, ...]) -> Any:
     # use initial value to resolve the whole configuration. if explicit value is a mapping it will be applied field by field later
     if explicit_value and (not isinstance(explicit_value, C_Mapping) or isinstance(explicit_value, BaseConfiguration)):
         # print(f"TRYING TO PARSE NATIVE from {explicit_value}")
         try:
             config.parse_native_representation(explicit_value)
-            # print("----ok")
         except ValueError as v_err:
             # provide generic exception
             raise InvalidNativeValue(type(config), type(explicit_value), embedded_sections, v_err)
         except NotImplementedError:
 
             pass
         # explicit value was consumed
```

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/__init__.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/config_providers_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 
 from typing import List
 from dlt.common.configuration.exceptions import DuplicateConfigProviderException
 from dlt.common.configuration.providers import ConfigProvider, EnvironProvider, ContextProvider, SecretsTomlProvider, ConfigTomlProvider
 from dlt.common.configuration.specs.base_configuration import ContainerInjectableContext, configspec
+from dlt.common.runtime.exec_info import is_running_in_airflow_task
 
 
 @configspec
 class ConfigProvidersContext(ContainerInjectableContext):
     """Injectable list of providers used by the configuration `resolve` module"""
     providers: List[ConfigProvider]
     context_provider: ConfigProvider
@@ -56,34 +57,35 @@
     """Returns a list of configuration providers for an Airflow environment.
 
     This function attempts to import Airflow to determine whether it
     is running in an Airflow environment. If Airflow is not installed,
     an empty list is returned. If Airflow is installed, the function
     returns a list containing the Airflow providers.
     """
-    try:
-        import airflow  # noqa
-        from airflow.models import Variable # noqa
-        from dlt.common.configuration.providers.airflow import (
-            AirflowSecretsTomlProvider,
-            AIRFLOW_SECRETS_TOML_VARIABLE_KEY
-        )
-        from dlt.common.runtime import logger
-    except ImportError:
+    if not is_running_in_airflow_task():
         return []
 
+    from airflow.models import Variable, TaskInstance # noqa
+    from airflow.operators.python import get_current_context  # noqa
+
+    from dlt.common.configuration.providers.airflow import (
+        AirflowSecretsTomlProvider,
+        AIRFLOW_SECRETS_TOML_VARIABLE_KEY
+    )
+
     secrets_toml_var = Variable.get(
         AIRFLOW_SECRETS_TOML_VARIABLE_KEY,
         default_var=None
     )
 
     if secrets_toml_var is not None:
         return [AirflowSecretsTomlProvider()]
     else:
-        logger.warning(
+        ti = get_current_context()["ti"]
+        ti.log.warning(
             f"Airflow variable '{AIRFLOW_SECRETS_TOML_VARIABLE_KEY}' "
             "not found. AirflowSecretsTomlProvider will not be used."
         )
         return []
 
 
 # TODO: implement ConfigProvidersConfiguration and
```

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/exceptions.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/gcp_client_credentials.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/gcp_client_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         return json.dumps(dict(self))
 
     def to_google_credentials(self) -> Any:
         pass
 
     def _from_info_dict(self, info: StrAny) -> None:
         self.update(info)
-        self.__is_resolved__ = not self.is_partial()
+        # self.__is_resolved__ = not self.is_partial()
 
     def __str__(self) -> str:
         return f"{self.project_id}[{self.location}]"
 
 
 @configspec
 class GcpDefaultCredentials(CredentialsWithDefault, GcpCredentialsBase):
@@ -103,14 +103,15 @@
             if isinstance(native_value, ServiceAccountCredentials):
                 # extract credentials
                 service_dict = {
                     "project_id": native_value.project_id,
                     "client_email": native_value.service_account_email,
                     "private_key": native_value  # keep native credentials in private key
                 }
+                self.__is_resolved__ = True
         except ImportError:
             pass
 
         if service_dict is None:
             # check if type is str
             GcpCredentialsBase.parse_native_representation(self, native_value)
             # if not instance of service account credentials then check type and try to parse native value
@@ -169,14 +170,16 @@
                     "project_id": native_value.quota_project_id or "",
                     "client_id": native_value.client_id,
                     "client_secret": native_value.client_secret,
                     "refresh_token": native_value.refresh_token,
                     "scopes": native_value.scopes,
                     "token": native_value.token
                 }
+                # if token is present, we are logged in
+                self.__is_resolved__ = native_value.token is not None
         except ImportError:
             pass
 
         if oauth_dict is None:
             # check if type is str
             GcpCredentialsBase.parse_native_representation(self, native_value)
             # if not instance of oauth2 credentials try to parse native value
@@ -213,42 +216,42 @@
                 self.__is_resolved__ = True
             self.refresh_token = None
 
     def _get_access_token(self) -> TSecretValue:
         try:
             from requests_oauthlib import OAuth2Session
         except ImportError:
-            raise MissingDependencyException("Requests-OAuthlib", ["requests_oauthlib"])
+            raise MissingDependencyException("GcpOAuthCredentials", ["requests_oauthlib"])
 
         google = OAuth2Session(client_id=self.client_id, scope=self.scopes)
         extra = {
             "client_id": self.client_id,
             "client_secret": self.client_secret
         }
         token = google.refresh_token(token_url=self.token_uri, refresh_token=self.refresh_token, **extra)["access_token"]
         return TSecretValue(token)
 
     def _get_refresh_token(self, redirect_url: str) -> Tuple[TSecretValue, TSecretValue]:
         try:
             from google_auth_oauthlib.flow import InstalledAppFlow
         except ImportError:
-            raise MissingDependencyException("Google Auth library", ["google-auth-oauthlib"])
+            raise MissingDependencyException("GcpOAuthCredentials", ["google-auth-oauthlib"])
         flow = InstalledAppFlow.from_client_config(self._installed_dict(redirect_url), self.scopes)
         credentials = flow.run_local_server(port=0)
         return TSecretValue(credentials.refresh_token), TSecretValue(credentials.token)
 
     def to_google_credentials(self) -> Any:
         """
         Will convert the object to a Google oauth2 credentials object
         :returns: Google Credentials object
         """
         try:
             from google.oauth2.credentials import Credentials as GoogleOAuth2Credentials
         except ImportError:
-            raise MissingDependencyException("Google OAuth Library", ["google-auth-oauthlib"])
+            raise MissingDependencyException("GcpOAuthCredentials", ["google-auth-oauthlib"])
 
         credentials = GoogleOAuth2Credentials.from_authorized_user_info(info=dict(self))
         return credentials
 
     def _installed_dict(self, redirect_url: str = "http://localhost") -> StrAny:
         installed_dict = {
             self.client_type: self._info_dict()
```

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/known_sections.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/load_volume_configuration.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/load_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/postgres_credentials.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/postgres_credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from dlt.common.configuration.specs.base_configuration import CredentialsConfiguration, configspec
 
 
 @configspec
 class ConnectionStringCredentials(CredentialsConfiguration):
     drivername: str = None
     database: str = None
-    password: TSecretValue = None
+    password: Optional[TSecretValue] = None
     username: str = None
-    host: str = None
-    port: int = None
+    host: Optional[str] = None
+    port: Optional[int] = None
     query: Optional[Dict[str, str]] = None
 
     __config_gen_annotations__: ClassVar[List[str]] = ["port"]
 
     def parse_native_representation(self, native_value: Any) -> None:
         if not isinstance(native_value, str):
             raise InvalidConnectionString(self.__class__, native_value, self.drivername)
@@ -25,21 +25,19 @@
             url = make_url(native_value)
             # update only values that are not None
             self.update(
                 {k: v for k,v in url._asdict().items() if v is not None}
             )
             if self.query is not None:
                 self.query = dict(self.query)
-            self.__is_resolved__ = not self.is_partial()
+            # self.__is_resolved__ = not self.is_partial()
         except Exception:
             raise InvalidConnectionString(self.__class__, native_value, self.drivername)
 
     def on_resolved(self) -> None:
-        if self.database:
-            self.database = self.database
         if self.password:
             self.password = TSecretValue(self.password.strip())
 
     def to_native_representation(self) -> str:
         return self.to_url().render_as_string(hide_password=False)
 
     def to_url(self) -> URL:
@@ -59,18 +57,22 @@
 
     def parse_native_representation(self, native_value: Any) -> None:
         super().parse_native_representation(native_value)
         self.connect_timeout = int(self.query.get("connect_timeout", self.connect_timeout))
 
     def on_resolved(self) -> None:
         self.database = self.database.lower()
-        self.password = TSecretValue(self.password.strip())
+        if self.password:
+            self.password = TSecretValue(self.password.strip())
 
     def to_url(self) -> URL:
         url = super().to_url()
         url.update_query_pairs([("connect_timeout", str(self.connect_timeout))])
         return url
 
 
 @configspec
 class RedshiftCredentials(PostgresCredentials):
     port: int = 5439
+    password: TSecretValue = None
+    username: str = None
+    host: str = None
```

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/run_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 @configspec
 class RunConfiguration(BaseConfiguration):
     pipeline_name: Optional[str] = None
     sentry_dsn: Optional[str] = None  # keep None to disable Sentry
     slack_incoming_hook: Optional[TSecretStrValue] = None
-    prometheus_port: Optional[int] = None  # keep None to disable Prometheus
     dlthub_telemetry: bool = True  # enable or disable dlthub telemetry
     dlthub_telemetry_segment_write_key: str = "a1F2gc6cNYw2plyAt02sZouZcsRjG7TD"
     log_format: str = '{asctime}|[{levelname:<21}]|{process}|{name}|{filename}|{funcName}:{lineno}|{message}'
     log_level: str = "WARNING"
     request_timeout: Tuple[int, int] = (15, 300)  # default request timeout for all http clients
     config_files_storage_path: str = "/run/config/"
```

### Comparing `dlt-0.2.6a0/dlt/common/configuration/specs/schema_volume_configuration.py` & `dlt-0.2.6a1/dlt/common/configuration/specs/schema_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/configuration/utils.py` & `dlt-0.2.6a1/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/data_types/type_helpers.py` & `dlt-0.2.6a1/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/data_writers/buffered.py` & `dlt-0.2.6a1/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/data_writers/escape.py` & `dlt-0.2.6a1/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/data_writers/exceptions.py` & `dlt-0.2.6a1/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/data_writers/writers.py` & `dlt-0.2.6a1/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/destination/capabilities.py` & `dlt-0.2.6a1/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/destination/reference.py` & `dlt-0.2.6a1/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/exceptions.py` & `dlt-0.2.6a1/dlt/common/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, AnyStr, Sequence
+from typing import Any, AnyStr, Sequence, Optional
 
 
 class DltException(Exception):
     def __reduce__(self) -> Any:
         """Enables exceptions with parametrized constructor to be pickled"""
         return type(self).__new__, (type(self), *self.args), self.__dict__
 
@@ -50,24 +50,14 @@
 class SignalReceivedException(KeyboardInterrupt, TerminalException):
     """Raises when signal comes. Derives from `BaseException` to not be caught in regular exception handlers."""
     def __init__(self, signal_code: int) -> None:
         self.signal_code = signal_code
         super().__init__(f"Signal {signal_code} received")
 
 
-class TimeRangeExhaustedException(DltException):
-    """
-    Raised when backfilling complete and no more time ranges can be generated
-    """
-    def __init__(self, start_ts: float, end_ts: float) -> None:
-        self.start_ts = start_ts
-        self.end_ts = end_ts
-        super().__init__(f"Timerange ({start_ts} to {end_ts}> exhausted")
-
-
 class DictValidationException(DltException):
     def __init__(self, msg: str, path: str, field: str = None, value: Any = None) -> None:
         self.path = path
         self.field = field
         self.value = value
         super().__init__(msg)
 
@@ -150,15 +140,15 @@
     def __init__(self, pipeline_name: str, msg: str) -> None:
         """Base class for all pipeline exceptions. Should not be raised."""
         self.pipeline_name = pipeline_name
         super().__init__(msg)
 
 
 class PipelineStateNotAvailable(PipelineException):
-    def __init__(self, source_name: str) -> None:
+    def __init__(self, source_name: Optional[str] = None) -> None:
         if source_name:
             msg = f"The source {source_name} requested the access to pipeline state but no pipeline is active right now."
         else:
             msg = "The resource you called requested the access to pipeline state but no pipeline is active right now."
         msg += " Call dlt.pipeline(...) before you call the @dlt.source or  @dlt.resource decorated function."
         self.source_name = source_name
         super().__init__(None, msg)
```

### Comparing `dlt-0.2.6a0/dlt/common/git.py` & `dlt-0.2.6a1/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/json/__init__.py` & `dlt-0.2.6a1/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/json/_orjson.py` & `dlt-0.2.6a1/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/json/_simplejson.py` & `dlt-0.2.6a1/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/configuration.py` & `dlt-0.2.6a1/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/json/__init__.py` & `dlt-0.2.6a1/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/json/relational.py` & `dlt-0.2.6a1/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/naming/direct.py` & `dlt-0.2.6a1/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.2.6a1/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.2.6a1/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/naming/naming.py` & `dlt-0.2.6a1/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.2.6a1/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/normalizers/utils.py` & `dlt-0.2.6a1/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/pipeline.py` & `dlt-0.2.6a1/dlt/common/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from dlt.common.configuration.paths import get_dlt_home_dir
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.destination.reference import DestinationReference, TDestinationReferenceArg
 from dlt.common.exceptions import DestinationHasFailedJobs, PipelineStateNotAvailable, SourceSectionNotAvailable
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TWriteDisposition
 from dlt.common.storages.load_storage import LoadPackageInfo
-from dlt.common.typing import DictStrAny
+from dlt.common.typing import DictStrAny, REPattern
+from dlt.common.jsonpath import delete_matches, TAnyJsonPath
 
 
 class ExtractInfo(NamedTuple):
     """A tuple holding information on extracted data items. Returned by pipeline `extract` method."""
     def asdict(self) -> DictStrAny:
         return {}
 
@@ -138,22 +139,24 @@
 
 class SupportsPipeline(Protocol):
     """A protocol with core pipeline operations that lets high level abstractions ie. sources to access pipeline methods and properties"""
     pipeline_name: str
     """Name of the pipeline"""
     destination: DestinationReference
     """The destination reference which is ModuleType. `destination.__name__` returns the name string"""
-    dataset_name: str = None
+    dataset_name: str
     """Name of the dataset to which pipeline will be loaded to"""
     runtime_config: RunConfiguration
     """A configuration of runtime options like logging level and format and various tracing options"""
     working_dir: str
     """A working directory of the pipeline"""
     pipeline_salt: str
     """A configurable pipeline secret to be used as a salt or a seed for encryption key"""
+    first_run: bool
+    """Indicates a first run of the pipeline, where run ends with successful loading of the data"""
 
     @property
     def state(self) -> TPipelineState:
         """Returns dictionary with pipeline state"""
 
     def set_local_state_val(self, key: str, value: Any) -> None:
         """Sets value in local state. Local state is not synchronized with destination."""
@@ -257,14 +260,41 @@
             return initial_default, False
         else:
             # get unmanaged state that is read only
             # TODO: make sure that state if up to date by syncing the pipeline earlier
             return proxy.pipeline().state, False
 
 
+def sources_state(pipeline_state_: Optional[TPipelineState] = None, /) -> DictStrAny:
+    global _last_full_state
+
+    # # get the source name from the section context
+    # source_section: str = None
+    # with contextlib.suppress(ContextDefaultCannotBeCreated):
+    #     sections_context = container[ConfigSectionContext]
+    #     with contextlib.suppress(ValueError):
+    #         source_section = sections_context.source_section()
+
+    # if not source_section:
+    #     raise SourceSectionNotAvailable()
+
+    if pipeline_state_ is None:
+        state, _ = pipeline_state(Container())
+    else:
+        state = pipeline_state_
+    if state is None:
+        raise PipelineStateNotAvailable()
+
+    sources_state_: DictStrAny = state.setdefault(known_sections.SOURCES, {})  # type: ignore
+
+    # allow inspection of last returned full state
+    _last_full_state = state
+    return sources_state_
+
+
 def source_state() -> DictStrAny:
     """Returns a dictionary with the source state. Such state is preserved across pipeline runs and may be used to implement incremental loads.
 
     ### Summary
     The state is a python dictionary-like object that is available within the `@dlt.source` and `@dlt.resource` decorated functions and may be read and written to.
     The data within the state is loaded into destination together with any other extracted data and made automatically available to the source/resource extractor functions when they are run next time.
     When using the state:
@@ -305,43 +335,62 @@
         sections_context = container[ConfigSectionContext]
         with contextlib.suppress(ValueError):
             source_section = sections_context.source_section()
 
     if not source_section:
         raise SourceSectionNotAvailable()
 
-    state, _ = pipeline_state(container)
-    if state is None:
-        raise PipelineStateNotAvailable(source_section)
+    try:
+        state = sources_state()
+    except PipelineStateNotAvailable as e:
+        # Reraise with source section
+        raise PipelineStateNotAvailable(source_section) from e
 
-    source_state: DictStrAny = state.setdefault(known_sections.SOURCES, {})  # type: ignore
-    if source_section:
-        source_state = source_state.setdefault(source_section, {})
+    return state.setdefault(source_section, {})  # type: ignore[no-any-return]
 
-    # allow inspection of last returned full state
-    _last_full_state = state
-    return source_state
 
 _last_full_state: TPipelineState = None
 
 
-def _resource_state(resource_name: str) -> DictStrAny:
+def _delete_source_state_keys(key: TAnyJsonPath, source_state_: Optional[DictStrAny] = None, /) -> None:
+    """Remove one or more key from the source state.
+    The `key` can be any number of keys and/or json paths to be removed.
+    """
+    state_ = source_state() if source_state_ is None else source_state_
+    delete_matches(key, state_)
+
+
+def _resource_state(resource_name: str, source_state_: Optional[DictStrAny] = None, /) -> DictStrAny:
     """Alpha version of the resource state, the signature will change.
     Returns resource-scoped state.
     """
-    return source_state().setdefault('resources', {}).setdefault(resource_name, {})  # type: ignore
+    state_ = source_state() if source_state_ is None else source_state_
+    return state_.setdefault('resources', {}).setdefault(resource_name, {})  # type: ignore
+
 
+def _reset_resource_state(resource_name: str, source_state_: Optional[DictStrAny] = None, /) -> None:
+    """Alpha version of the resource state. Resets the resource state
 
-def _reset_resource_state(resource_name: str) -> None:
-    """Alpha version of the resource state. Resets the resource state"""
-    state_ = source_state()
+    Args:
+        resource_name: The resource key to reset
+        state: Optional source state dictionary to operate on. Use when working outside source context.
+    """
+    state_ = source_state() if source_state_ is None else source_state_
     if "resources" in state_ and resource_name in state_["resources"]:
         state_["resources"].pop(resource_name)
 
 
+def _get_matching_resources(pattern: REPattern, source_state_: Optional[DictStrAny] = None, /) -> List[str]:
+    """Get all resource names in state matching the regex pattern"""
+    state_ = source_state() if source_state_ is None else source_state_
+    if "resources" not in state_:
+        return []
+    return [key for key in state_["resources"] if pattern.match(key)]
+
+
 def get_dlt_pipelines_dir() -> str:
     """ Gets default directory where pipelines' data will be stored
         1. in user home directory ~/.dlt/pipelines/
         2. if current user is root in /var/dlt/pipelines
         3. if current user does not have a home directory in /tmp/dlt/pipelines
     """
     return os.path.join(get_dlt_home_dir(), "pipelines")
```

### Comparing `dlt-0.2.6a0/dlt/common/reflection/spec.py` & `dlt-0.2.6a1/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/reflection/utils.py` & `dlt-0.2.6a1/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/runners/init.py` & `dlt-0.2.6a1/dlt/common/runtime/init.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-import threading
-
-from dlt.common import logger
-from dlt.common.runtime.logger import init_logging
-from dlt.common.runtime.telemetry import start_telemetry
-from dlt.common.runtime.signals import register_signals
 from dlt.common.configuration.specs import RunConfiguration
 
-# signals and telemetry should be initialized only once
+# telemetry should be initialized only once
 _INITIALIZED = False
 _RUN_CONFIGURATION: RunConfiguration = None
 
 
-def initialize_runner(config: RunConfiguration) -> None:
+def initialize_runtime(config: RunConfiguration) -> None:
+    from dlt.common.runtime.logger import init_logging
+    from dlt.common.runtime.telemetry import start_telemetry
+
     global _INITIALIZED, _RUN_CONFIGURATION
 
     # initialize or re-initialize logging with new settings
     init_logging(config)
 
     # initialize only once
     if not _INITIALIZED:
         start_telemetry(config)
-
-        if threading.current_thread() is threading.main_thread():
-            register_signals()
-        else:
-            logger.info("Running in daemon thread, signals not enabled")
-
         _INITIALIZED = True
 
     # store last config
     _RUN_CONFIGURATION = config
```

### Comparing `dlt-0.2.6a0/dlt/common/runners/runnable.py` & `dlt-0.2.6a1/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/runners/stdout.py` & `dlt-0.2.6a1/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/runners/synth_pickle.py` & `dlt-0.2.6a1/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/runners/venv.py` & `dlt-0.2.6a1/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/runtime/exec_info.py` & `dlt-0.2.6a1/dlt/common/runtime/exec_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import io
 import os
+import contextlib
 
-from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.typing import StrStr, StrAny, Literal, List
 from dlt.common.utils import filter_env_vars
 from dlt.version import __version__
 
 
 TExecInfoNames = Literal["kubernetes", "docker", "codespaces", "github_actions", "airflow", "notebook", "colab"]
 # if one of these environment variables is set, we assume to be running in CI env
@@ -67,24 +68,38 @@
         return "COLAB_RELEASE_TAG" in os.environ or "google.colab" in str(get_ipython())  # type: ignore
     except NameError:
         return False
 
 
 def airflow_info() -> StrAny:
     try:
-        from airflow.operators.python import get_current_context
-        get_current_context()
-        return {"AIRFLOW_TASK": True}
+        with contextlib.redirect_stdout(io.StringIO()), contextlib.redirect_stderr(io.StringIO()):
+            from airflow.operators.python import get_current_context
+
+            get_current_context()
+            return {"AIRFLOW_TASK": True}
     except Exception:
         return None
 
 
-def dlt_version_info(config: RunConfiguration) -> StrStr:
+def is_running_in_airflow_task() -> bool:
+    try:
+        with contextlib.redirect_stdout(io.StringIO()), contextlib.redirect_stderr(io.StringIO()):
+            from airflow.operators.python import get_current_context
+
+            context = get_current_context()
+            return context is not None and 'ti' in context
+    except Exception:
+        return False
+
+
+
+def dlt_version_info(pipeline_name: str) -> StrStr:
     """Gets dlt version info including commit and image version available in docker"""
-    version_info = {"dlt_version": __version__, "pipeline_name": config.pipeline_name}
+    version_info = {"dlt_version": __version__, "pipeline_name": pipeline_name}
     # extract envs with build info
     version_info.update(filter_env_vars(["COMMIT_SHA", "IMAGE_VERSION"]))
 
     return version_info
 
 
 def kube_pod_info() -> StrStr:
```

### Comparing `dlt-0.2.6a0/dlt/common/runtime/prometheus.py` & `dlt-0.2.6a1/dlt/common/runtime/prometheus.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.runtime import logger
 from dlt.common.runtime.exec_info import dlt_version_info
 from dlt.common.typing import DictStrAny, StrAny
 
 
-def init_prometheus(config: RunConfiguration) -> None:
-        from prometheus_client import start_http_server, Info
+# def init_prometheus(config: RunConfiguration) -> None:
+#         from prometheus_client import start_http_server, Info
 
-        logger.info(f"Starting prometheus server port {config.prometheus_port}")
-        start_http_server(config.prometheus_port)
-        # collect info
-        Info("runs_component_name", "Name of the executing component").info(dlt_version_info(config))  # type: ignore
+#         logger.info(f"Starting prometheus server port {config.prometheus_port}")
+#         start_http_server(config.prometheus_port)
+#         # collect info
+#         Info("runs_component_name", "Name of the executing component").info(dlt_version_info(config.pipeline_name))  # type: ignore
 
 
 def get_metrics_from_prometheus(gauges: Iterable[MetricWrapperBase]) -> StrAny:
     metrics: DictStrAny = {}
     for g in gauges:
         name = g._name
         if g._is_parent():
```

### Comparing `dlt-0.2.6a0/dlt/common/runtime/segment.py` & `dlt-0.2.6a1/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/runtime/sentry.py` & `dlt-0.2.6a1/dlt/common/runtime/sentry.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from dlt.common.typing import DictStrAny, Any, StrAny
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.runtime.exec_info import dlt_version_info, kube_pod_info, github_info
 
 
 def init_sentry(config: RunConfiguration) -> None:
-    version = dlt_version_info(config)
+    version = dlt_version_info(config.pipeline_name)
     sys_ver = version["dlt_version"]
     release = sys_ver + "_" + version.get("commit_sha", "")
     _SentryHttpTransport.timeout = config.request_timeout[0]
     # TODO: ignore certain loggers ie. dbt loggers
     # https://docs.sentry.io/platforms/python/guides/logging/
     sentry_sdk.init(
         config.sentry_dsn,
```

### Comparing `dlt-0.2.6a0/dlt/common/runtime/signals.py` & `dlt-0.2.6a1/dlt/common/runtime/signals.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+import threading
 import signal
 from contextlib import contextmanager
 from threading import Event
 from typing import Any, TYPE_CHECKING, Iterator
 
 from dlt.common.exceptions import SignalReceivedException
 
 _received_signal: int = 0
-_raise_immediately: bool = False
-_original_sigint_handler = signal.getsignal(signal.SIGINT)
-_original_sigterm_handler = signal.getsignal(signal.SIGTERM)
 exit_event = Event()
 
 
 def signal_receiver(sig: int, frame: Any) -> None:
     if not TYPE_CHECKING:
         from dlt.common.runtime import logger
     else:
@@ -28,45 +26,43 @@
 
     _received_signal = sig
     # awake all threads sleeping on event
     exit_event.set()
 
     logger.info("Sleeping threads signalled")
 
-    if _raise_immediately and _received_signal == signal.SIGINT:
-        raise_if_signalled()
-
 
 def raise_if_signalled() -> None:
     if _received_signal:
         raise SignalReceivedException(_received_signal)
 
 
-def register_signals() -> None:
-    signal.signal(signal.SIGINT, signal_receiver)
-    signal.signal(signal.SIGTERM, signal_receiver)
-
-
-def restore_signals() -> None:
-    signal.signal(signal.SIGINT, _original_sigint_handler)
-    signal.signal(signal.SIGTERM, _original_sigterm_handler)
-
-
 def sleep(sleep_seconds: float) -> None:
     """A signal-aware version of sleep function. Will raise SignalReceivedException if signal was received during sleep period."""
     # do not allow sleeping if signal was received
     raise_if_signalled()
     # sleep or wait for signal
     exit_event.wait(sleep_seconds)
     # if signal then raise
     raise_if_signalled()
 
 
 @contextmanager
-def raise_immediately() -> Iterator[None]:
-    global _raise_immediately
+def delayed_signals() -> Iterator[None]:
+    """Will delay signalling until `raise_if_signalled` is used or signalled `sleep`"""
 
-    try:
-        _raise_immediately = True
+    if threading.current_thread() is threading.main_thread():
+        original_sigint_handler = signal.getsignal(signal.SIGINT)
+        original_sigterm_handler = signal.getsignal(signal.SIGTERM)
+        try:
+            signal.signal(signal.SIGINT, signal_receiver)
+            signal.signal(signal.SIGTERM, signal_receiver)
+            yield
+        finally:
+            global _received_signal
+
+            _received_signal = 0
+            signal.signal(signal.SIGINT, original_sigint_handler)
+            signal.signal(signal.SIGTERM, original_sigterm_handler)
+    else:
+        print("Running in daemon thread, signals not enabled")
         yield
-    finally:
-        _raise_immediately = False
```

### Comparing `dlt-0.2.6a0/dlt/common/runtime/slack.py` & `dlt-0.2.6a1/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/runtime/telemetry.py` & `dlt-0.2.6a1/dlt/common/runtime/telemetry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-from typing import Iterable, Sequence, TypedDict, NamedTuple
-
-
 from dlt.common.configuration.specs import RunConfiguration
-from dlt.common.runtime.prometheus import init_prometheus
 from dlt.common.runtime.segment import init_segment, disable_segment
 
 from dlt.common.runtime.sentry import init_sentry, disable_sentry
-from dlt.common.typing import DictStrAny, StrAny
 
 
 _TELEMETRY_ENABLED = False
 
 
 def start_telemetry(config: RunConfiguration) -> None:
     # enable telemetry only once
@@ -18,26 +13,22 @@
     global _TELEMETRY_ENABLED
     if _TELEMETRY_ENABLED:
         return
 
     if config.sentry_dsn:
         init_sentry(config)
 
-    if config.prometheus_port:
-        init_prometheus(config)
-
     if config.dlthub_telemetry:
         init_segment(config)
 
     _TELEMETRY_ENABLED = True
 
 
 def stop_telemetry() -> None:
     global _TELEMETRY_ENABLED
     if not _TELEMETRY_ENABLED:
         return
 
     disable_sentry()
     disable_segment()
-    # prometheus cannot be stopped
 
     _TELEMETRY_ENABLED = False
```

### Comparing `dlt-0.2.6a0/dlt/common/schema/detections.py` & `dlt-0.2.6a1/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/schema/exceptions.py` & `dlt-0.2.6a1/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/schema/schema.py` & `dlt-0.2.6a1/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/schema/typing.py` & `dlt-0.2.6a1/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/schema/utils.py` & `dlt-0.2.6a1/dlt/common/schema/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import base64
 import hashlib
 
 from copy import deepcopy
-from typing import Dict, List, Sequence, Tuple, Type, Any, cast
+from typing import Dict, List, Sequence, Tuple, Type, Any, cast, Union, Iterable, Optional
 
 from dlt.common import json
 from dlt.common.data_types import TDataType
 from dlt.common.exceptions import DictValidationException
 from dlt.common.normalizers import default_normalizers
 from dlt.common.normalizers.naming import NamingConvention
 from dlt.common.typing import DictStrAny, REPattern
@@ -142,20 +142,32 @@
             return True
         else:
             return False
 
     return validator
 
 
-def compile_simple_regex(r: TSimpleRegex) -> REPattern:
+def _prepare_simple_regex(r: TSimpleRegex) -> str:
     if r.startswith(SIMPLE_REGEX_PREFIX):
-        return re.compile(r[3:])
+        return r[3:]
     else:
         # exact matches
-        return re.compile("^" + re.escape(r) + "$")
+        return "^" + re.escape(r) + "$"
+
+
+def compile_simple_regex(r: TSimpleRegex) -> REPattern:
+    return re.compile(_prepare_simple_regex(r))
+
+
+def compile_simple_regexes(r: Iterable[TSimpleRegex]) -> REPattern:
+    """Compile multiple patterns as one"""
+    pattern = '|'.join(f"({_prepare_simple_regex(p)})" for p in r)
+    if not pattern:  # Don't create an empty pattern that matches everything
+        raise ValueError("Cannot create a regex pattern from empty sequence")
+    return re.compile(pattern)
 
 
 def validate_stored_schema(stored_schema: TStoredSchema) -> None:
     # use lambda to verify only non extra fields
     validate_dict(TStoredSchema, stored_schema, ".", lambda k: not k.startswith("x-"), simple_regex_validator)
     # check child parent relationships
     for table_name, table in stored_schema["tables"].items():
@@ -426,14 +438,27 @@
             if candidate.get("parent") == name:
                 _child(candidate)
 
     _child(tables[table_name])
     return chain
 
 
+def group_tables_by_resource(tables: TSchemaTables, pattern: Optional[REPattern] = None) -> Dict[str, List[TTableSchema]]:
+    """Create a dict of resources and their associated tables and descendant tables
+    If `pattern` is supplied, the result is filtered to only resource names matching the pattern.
+    """
+    result: Dict[str, List[TTableSchema]] = {}
+    for table in tables.values():
+        resource = table.get('resource')
+        if resource and (pattern is None or pattern.match(resource)):
+            resource_tables = result.setdefault(resource, [])
+            resource_tables.extend(get_child_tables(tables, table['name']))
+    return result
+
+
 def version_table() -> TTableSchema:
     table = new_table(VERSION_TABLE_NAME, columns=[
             add_missing_hints({
                 "name": "version",
                 "data_type": "bigint",
                 "nullable": False,
             }),
```

### Comparing `dlt-0.2.6a0/dlt/common/storages/data_item_storage.py` & `dlt-0.2.6a1/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/storages/exceptions.py` & `dlt-0.2.6a1/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/storages/file_storage.py` & `dlt-0.2.6a1/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/storages/live_schema_storage.py` & `dlt-0.2.6a1/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/storages/load_storage.py` & `dlt-0.2.6a1/dlt/common/storages/load_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,17 @@
 
     def delete_completed_package(self, load_id: str) -> None:
         package_path = self.get_completed_package_path(load_id)
         if not self.storage.has_folder(package_path):
             raise LoadPackageNotFound(load_id)
         self.storage.delete_folder(package_path, recursively=True)
 
+    def wipe_normalized_packages(self) -> None:
+        self.storage.delete_folder(self.NORMALIZED_FOLDER, recursively=True)
+
     def get_package_path(self, load_id: str) -> str:
         return join(LoadStorage.NORMALIZED_FOLDER, load_id)
 
     def get_completed_package_path(self, load_id: str) -> str:
         return join(LoadStorage.LOADED_FOLDER, load_id)
 
     def job_elapsed_time_seconds(self, file_path: str, now_ts: float = None) -> float:
```

### Comparing `dlt-0.2.6a0/dlt/common/storages/normalize_storage.py` & `dlt-0.2.6a1/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/storages/schema_storage.py` & `dlt-0.2.6a1/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/storages/versioned_storage.py` & `dlt-0.2.6a1/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/time.py` & `dlt-0.2.6a1/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/typing.py` & `dlt-0.2.6a1/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/utils.py` & `dlt-0.2.6a1/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/validation.py` & `dlt-0.2.6a1/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/common/wei.py` & `dlt-0.2.6a1/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/bigquery/__init__.py` & `dlt-0.2.6a1/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/bigquery/bigquery.py` & `dlt-0.2.6a1/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/bigquery/sql_client.py` & `dlt-0.2.6a1/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/duckdb/__init__.py` & `dlt-0.2.6a1/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/duckdb/configuration.py` & `dlt-0.2.6a1/dlt/destinations/duckdb/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             # check if database was passed as explicit connection
             import duckdb
             if isinstance(native_value, duckdb.DuckDBPyConnection):
                 self._conn = native_value
                 self._conn_owner = False
                 self._conn_borrows = 0
                 self.database = ":external:"
+                self.__is_resolved__ = not self.is_partial()
                 return
         except ImportError:
             pass
         try:
             super().parse_native_representation(native_value)
         except InvalidConnectionString:
             if native_value == ":pipeline:" or is_valid_filepath(native_value, platform="auto"):
```

### Comparing `dlt-0.2.6a0/dlt/destinations/duckdb/duck.py` & `dlt-0.2.6a1/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/duckdb/sql_client.py` & `dlt-0.2.6a1/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/dummy/__init__.py` & `dlt-0.2.6a1/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/dummy/configuration.py` & `dlt-0.2.6a1/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/dummy/dummy.py` & `dlt-0.2.6a1/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/exceptions.py` & `dlt-0.2.6a1/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/insert_job_client.py` & `dlt-0.2.6a1/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/job_client_impl.py` & `dlt-0.2.6a1/dlt/destinations/job_client_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import abstractmethod
 import base64
 import binascii
 import contextlib
 from copy import copy
 import datetime  # noqa: 251
 from types import TracebackType
-from typing import Any, ClassVar, List, NamedTuple, Optional, Sequence, Tuple, Type, Iterable
+from typing import Any, ClassVar, List, NamedTuple, Optional, Sequence, Tuple, Type, Iterable, Iterator
 import zlib
 
 from dlt.common import json, pendulum, logger
 from dlt.common.data_types import TDataType
 from dlt.common.schema.typing import COLUMN_HINTS, LOADS_TABLE_NAME, VERSION_TABLE_NAME, TColumnSchemaBase, TTableSchema
 from dlt.common.schema.utils import add_missing_hints
 from dlt.common.storages import FileStorage
@@ -86,23 +86,34 @@
         with self.sql_client.with_staging_dataset(staging):
             super().update_storage_schema(staging, only_tables, expected_update)
             applied_update: TSchemaTables = {}
             schema_info = self.get_schema_by_hash(self.schema.stored_version_hash)
             if schema_info is None:
                 logger.info(f"Schema with hash {self.schema.stored_version_hash} not found in the storage. upgrading")
 
-                if self.capabilities.supports_ddl_transactions:
-                    with self.sql_client.begin_transaction():
-                        applied_update = self._execute_schema_update_sql(only_tables)
-                else:
+                with self._ddl_transaction():
                     applied_update = self._execute_schema_update_sql(only_tables)
             else:
                 logger.info(f"Schema with hash {self.schema.stored_version_hash} inserted at {schema_info.inserted_at} found in storage, no upgrade required")
             return applied_update
 
+    def drop_tables(self, *tables: str, staging: bool = False) -> None:
+        with self.sql_client.with_staging_dataset(staging):
+            with self._ddl_transaction():
+                self.sql_client.drop_tables(*tables)
+                self._replace_schema_in_storage(self.schema)
+
+    @contextlib.contextmanager
+    def _ddl_transaction(self) -> Iterator[None]:
+        if self.capabilities.supports_ddl_transactions:
+            with self.sql_client.begin_transaction():
+                yield
+        else:
+            yield
+
     def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return SqlMergeJob.from_table_chain(table_chain, self.sql_client)
 
     def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
         """Starts SqlLoadJob for files ending with .sql or returns None to let derived classes to handle their specific jobs"""
         if SqlLoadJob.is_sql_job(file_path):
             # execute sql load job
@@ -287,14 +298,24 @@
             pass
 
         # make utc datetime
         inserted_at = pendulum.instance(row[4])
 
         return StorageSchemaInfo(row[0], row[1], row[2], row[3], inserted_at, schema_str)
 
+    def _replace_schema_in_storage(self, schema: Schema) -> None:
+        """
+        Save the given schema in storage and remove all previous versions with the same name
+        """
+        name = self.sql_client.make_qualified_table_name(VERSION_TABLE_NAME)
+        self.sql_client.execute_sql(
+            f"DELETE FROM {name} WHERE schema_name = %s;", schema.name
+        )
+        self._update_schema_in_storage(schema)
+
     def _update_schema_in_storage(self, schema: Schema) -> None:
         now_ts = str(pendulum.now())
         # get schema string or zip
         schema_str = json.dumps(schema.to_dict())
         # TODO: not all databases store data as utf-8 but this exception is mostly for redshift
         schema_bytes = schema_str.encode("utf-8")
         if len(schema_bytes) > self.capabilities.max_text_data_type_length:
```

### Comparing `dlt-0.2.6a0/dlt/destinations/job_impl.py` & `dlt-0.2.6a1/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/postgres/__init__.py` & `dlt-0.2.6a1/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/postgres/postgres.py` & `dlt-0.2.6a1/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/postgres/sql_client.py` & `dlt-0.2.6a1/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/redshift/README.md` & `dlt-0.2.6a1/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/redshift/__init__.py` & `dlt-0.2.6a1/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/redshift/redshift.py` & `dlt-0.2.6a1/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/sql_client.py` & `dlt-0.2.6a1/dlt/destinations/sql_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,21 @@
     def drop_dataset(self) -> None:
         pass
 
     def truncate_tables(self, *tables: str) -> None:
         sql = ";\n".join(f"TRUNCATE TABLE {self.make_qualified_table_name(t)}" for t in tables)
         self.execute_sql(sql)
 
+    def drop_tables(self, *tables: str) -> None:
+        if not tables:
+            return
+        clauses = (f"DROP TABLE IF EXISTS {self.make_qualified_table_name(table)}" for table in tables)
+        sql = ";\n".join(clauses)
+        self.execute_sql(sql)
+
     @abstractmethod
     def execute_sql(self, sql: AnyStr, *args: Any, **kwargs: Any) -> Optional[Sequence[Sequence[Any]]]:
         pass
 
     @abstractmethod
     def execute_query(self, query: AnyStr, *args: Any, **kwargs: Any) -> ContextManager[DBApiCursor]:
         pass
```

### Comparing `dlt-0.2.6a0/dlt/destinations/sql_merge_job.py` & `dlt-0.2.6a1/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/destinations/typing.py` & `dlt-0.2.6a1/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/extract/decorators.py` & `dlt-0.2.6a1/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/extract/exceptions.py` & `dlt-0.2.6a1/dlt/extract/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,7 +229,12 @@
         self.typ = _typ
         super().__init__(f"First parameter to the source {source_name} is a class {_typ.__name__}. Do not decorate classes with @dlt.source. Instead implement __call__ in your class and pass instance of such class to dlt.source() directly")
 
 
 class SourceSchemaNotAvailable(DltSourceException):
     def __init__(self) -> None:
         super().__init__("Current source schema is available only when called from a function decorated with dlt.source or dlt.resource")
+
+
+class IncrementalUnboundError(DltResourceException):
+    def __init__(self, cursor_path: str) -> None:
+        super().__init__("", f"The incremental definition with cursor path {cursor_path} is used without being bound to the resource. This most often happens when you create dynamic resource from a generator function that uses incremental. See https://dlthub.com/docs/general-usage/incremental-loading#incremental-loading-with-last-value for an example.")
```

### Comparing `dlt-0.2.6a0/dlt/extract/extract.py` & `dlt-0.2.6a1/dlt/extract/extract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import contextlib
 import os
 from typing import ClassVar, List
+
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.resolve import inject_section
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.pipeline import _reset_resource_state
 
 from dlt.common.runtime import signals
-from dlt.common.schema import Schema
-
+from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.utils import uniq_id
 from dlt.common.typing import TDataItems, TDataItem
-from dlt.common.schema import utils, TSchemaUpdate
+from dlt.common.schema import Schema, utils, TSchemaUpdate
 from dlt.common.storages import NormalizeStorage, DataItemStorage
 from dlt.common.configuration.specs import NormalizeVolumeConfiguration, known_sections
+
 from dlt.extract.decorators import SourceSchemaInjectableContext
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints
-
-
 from dlt.extract.pipe import PipeIterator
 from dlt.extract.source import DltResource, DltSource
 from dlt.extract.typing import TableNameMeta
 
 
 class ExtractorStorage(DataItemStorage, NormalizeStorage):
     EXTRACT_FOLDER: ClassVar[str] = "extract"
@@ -53,95 +52,127 @@
         template = NormalizeStorage.build_extracted_file_stem(schema_name, table_name, "%s")
         return self.storage.make_full_path(os.path.join(self._get_extract_path(load_id), template))
 
     def _get_extract_path(self, extract_id: str) -> str:
         return os.path.join(ExtractorStorage.EXTRACT_FOLDER, extract_id)
 
 
-def extract(extract_id: str, source: DltSource, storage: ExtractorStorage, *, max_parallel_items: int = None, workers: int = None, futures_poll_interval: float = None) -> TSchemaUpdate:
-    # TODO: add metrics: number of items processed, also per resource and table
+def extract(
+    extract_id: str,
+    source: DltSource,
+    storage: ExtractorStorage,
+    collector: Collector = NULL_COLLECTOR,
+    *,
+    max_parallel_items: int = None,
+    workers: int = None,
+    futures_poll_interval: float = None
+) -> TSchemaUpdate:
+
     dynamic_tables: TSchemaUpdate = {}
     schema = source.schema
 
-    def _write_item(table_name: str, item: TDataItems) -> None:
-        # normalize table name before writing so the name match the name in schema
-        # note: normalize function should be cached so there's almost no penalty on frequent calling
-        # note: column schema is not required for jsonl writer used here
-        storage.write_data_item(extract_id, schema.name, schema.naming.normalize_identifier(table_name), item, None)
-
-    def _write_dynamic_table(resource: DltResource, item: TDataItem) -> None:
-        table_name = resource._table_name_hint_fun(item)
-        existing_table = dynamic_tables.get(table_name)
-        if existing_table is None:
-            dynamic_tables[table_name] = [resource.table_schema(item)]
-        else:
-            # quick check if deep table merge is required
-            if resource._table_has_other_dynamic_hints:
-                new_table = resource.table_schema(item)
-                # this merges into existing table in place
-                utils.merge_tables(existing_table[0], new_table)
-            else:
-                # if there are no other dynamic hints besides name then we just leave the existing partial table
-                pass
-        # write to storage with inferred table name
-        _write_item(table_name, item)
-
-    def _write_static_table(resource: DltResource, table_name: str) -> None:
-        existing_table = dynamic_tables.get(table_name)
-        if existing_table is None:
-            static_table = resource.table_schema()
-            static_table["name"] = table_name
-            dynamic_tables[table_name] = [static_table]
-
-    # yield from all selected pipes
-    with PipeIterator.from_pipes(source.resources.selected_pipes, max_parallel_items=max_parallel_items, workers=workers, futures_poll_interval=futures_poll_interval) as pipes:
-        for pipe_item in pipes:
-            # TODO: many resources may be returned. if that happens the item meta must be present with table name and this name must match one of resources
-            # TDataItemMeta(table_name, requires_resource, write_disposition, columns, parent etc.)
-            signals.raise_if_signalled()
-            # if meta contains table name
-            resource = source.resources.find_by_pipe(pipe_item.pipe)
-            if isinstance(pipe_item.meta, TableNameMeta):
-                table_name = pipe_item.meta.table_name
-                _write_static_table(resource, table_name)
-                _write_item(table_name, pipe_item.item)
+    with collector(f"Extract {source.name}"):
+
+        def _write_item(table_name: str, item: TDataItems) -> None:
+            # normalize table name before writing so the name match the name in schema
+            # note: normalize function should be cached so there's almost no penalty on frequent calling
+            # note: column schema is not required for jsonl writer used here
+            table_name = schema.naming.normalize_identifier(table_name)
+            collector.update(table_name)
+            storage.write_data_item(extract_id, schema.name, table_name, item, None)
+
+        def _write_dynamic_table(resource: DltResource, item: TDataItem) -> None:
+            table_name = resource._table_name_hint_fun(item)
+            existing_table = dynamic_tables.get(table_name)
+            if existing_table is None:
+                dynamic_tables[table_name] = [resource.table_schema(item)]
             else:
-                # get partial table from table template
-                if resource._table_name_hint_fun:
-                    if isinstance(pipe_item.item, List):
-                        for item in pipe_item.item:
-                            _write_dynamic_table(resource, item)
-                    else:
-                        _write_dynamic_table(resource, pipe_item.item)
+                # quick check if deep table merge is required
+                if resource._table_has_other_dynamic_hints:
+                    new_table = resource.table_schema(item)
+                    # this merges into existing table in place
+                    utils.merge_tables(existing_table[0], new_table)
                 else:
-                    # write item belonging to table with static name
-                    table_name = resource.table_name
+                    # if there are no other dynamic hints besides name then we just leave the existing partial table
+                    pass
+            # write to storage with inferred table name
+            _write_item(table_name, item)
+
+        def _write_static_table(resource: DltResource, table_name: str) -> None:
+            existing_table = dynamic_tables.get(table_name)
+            if existing_table is None:
+                static_table = resource.table_schema()
+                static_table["name"] = table_name
+                dynamic_tables[table_name] = [static_table]
+
+        # yield from all selected pipes
+        with PipeIterator.from_pipes(source.resources.selected_pipes, max_parallel_items=max_parallel_items, workers=workers, futures_poll_interval=futures_poll_interval) as pipes:
+            left_gens = total_gens = len(pipes._sources)
+            collector.update("Resources", 0, total_gens)
+            for pipe_item in pipes:
+
+                curr_gens = len(pipes._sources)
+                if left_gens > curr_gens:
+                    delta = left_gens - curr_gens
+                    left_gens -= delta
+                    collector.update("Resources", delta)
+
+                signals.raise_if_signalled()
+
+                # TODO: many resources may be returned. if that happens the item meta must be present with table name and this name must match one of resources
+                # if meta contains table name
+                resource = source.resources.find_by_pipe(pipe_item.pipe)
+                if isinstance(pipe_item.meta, TableNameMeta):
+                    table_name = pipe_item.meta.table_name
                     _write_static_table(resource, table_name)
                     _write_item(table_name, pipe_item.item)
+                else:
+                    # get partial table from table template
+                    if resource._table_name_hint_fun:
+                        if isinstance(pipe_item.item, List):
+                            for item in pipe_item.item:
+                                _write_dynamic_table(resource, item)
+                        else:
+                            _write_dynamic_table(resource, pipe_item.item)
+                    else:
+                        # write item belonging to table with static name
+                        table_name = resource.table_name
+                        _write_static_table(resource, table_name)
+                        _write_item(table_name, pipe_item.item)
+            if left_gens > 0:
+                # go to 100%
+                collector.update("Resources", left_gens)
 
-    # flush all buffered writers
-    storage.close_writers(extract_id)
+        # flush all buffered writers
+        storage.close_writers(extract_id)
 
     # returns set of partial tables
     return dynamic_tables
 
 
-def extract_with_schema(storage: ExtractorStorage, source: DltSource, schema: Schema, max_parallel_items: int, workers: int) -> str:
+def extract_with_schema(
+    storage: ExtractorStorage,
+    source: DltSource,
+    schema: Schema,
+    collector: Collector,
+    max_parallel_items: int,
+    workers: int
+) -> str:
     # generate extract_id to be able to commit all the sources together later
     extract_id = storage.create_extract_id()
     with Container().injectable_context(SourceSchemaInjectableContext(schema)):
         # inject the config section with the current source name
         with inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, source.section, source.name))):
             # reset resource states
             for resource in source.resources.extracted.values():
                 with contextlib.suppress(DataItemRequiredForDynamicTableHints):
                     if resource.write_disposition == "replace":
                         _reset_resource_state(resource._name)
 
-            extractor = extract(extract_id, source, storage, max_parallel_items=max_parallel_items, workers=workers)
+            extractor = extract(extract_id, source, storage, collector, max_parallel_items=max_parallel_items, workers=workers)
             # source iterates
             # TODO: implement a real check if source is exhausted. most of the resources should be not
             source.exhausted = True
             # iterate over all items in the pipeline and update the schema if dynamic table hints were present
             for _, partials in extractor.items():
                 for partial in partials:
                     schema.update_schema(schema.normalize_table_identifiers(partial))
```

### Comparing `dlt-0.2.6a0/dlt/extract/incremental.py` & `dlt-0.2.6a1/dlt/extract/incremental.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Generic, TypeVar, Any, Optional, Callable, List, TypedDict, get_origin, Sequence
 import inspect
 from functools import wraps
 
-from jsonpath_ng import parse as jsonpath_parse, JSONPath
-
 import dlt
 from dlt.common.json import json
-from dlt.common.typing import DictStrAny, TDataItem, TDataItems, TFun, extract_inner_type, is_optional_type
+from dlt.common.jsonpath import compile_path, find_values, JSONPath
+from dlt.common.typing import TDataItem, TDataItems, TFun, extract_inner_type, is_optional_type
 from dlt.common.schema.typing import TColumnKey
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.pipeline import _resource_state
 from dlt.common.utils import digest128
-from dlt.extract.exceptions import PipeException
+from dlt.extract.exceptions import IncrementalUnboundError, PipeException
 from dlt.extract.pipe import Pipe
 from dlt.extract.utils import resolve_column_value
 from dlt.extract.typing import FilterItem, SupportsPipe, TTableHintTemplate
 
 
 TCursorValue = TypeVar("TCursorValue", bound=Any)
 LastValueFunc = Callable[[Sequence[TCursorValue]], Any]
@@ -83,15 +82,15 @@
             cursor_path: str = dlt.config.value,
             initial_value: Optional[TCursorValue]=None,
             last_value_func: Optional[LastValueFunc[TCursorValue]]=max,
             primary_key: Optional[TTableHintTemplate[TColumnKey]] = None
     ) -> None:
         self.cursor_path = cursor_path
         if self.cursor_path:
-            self.cursor_path_p: JSONPath = jsonpath_parse(cursor_path)
+            self.cursor_path_p: JSONPath = compile_path(cursor_path)
         self.last_value_func = last_value_func
         self.initial_value = initial_value
         """Initial value of last_value"""
         self.start_value: Any = initial_value
         """Value of last_value at the beginning of current pipeline run"""
         self.resource_name: Optional[str] = None
         self.primary_key: Optional[TTableHintTemplate[TColumnKey]] = primary_key
@@ -107,15 +106,15 @@
         i.resource_name = resource_name
         return i
 
     def copy(self) -> "Incremental[TCursorValue]":
         return self.__class__(self.cursor_path, initial_value=self.initial_value, last_value_func=self.last_value_func, primary_key=self.primary_key)
 
     def on_resolved(self) -> None:
-        self.cursor_path_p = jsonpath_parse(self.cursor_path)
+        self.cursor_path_p = compile_path(self.cursor_path)
 
     def parse_native_representation(self, native_value: Any) -> None:
         if isinstance(native_value, Incremental):
             self.cursor_path = native_value.cursor_path
             self.initial_value = native_value.initial_value
             self.last_value_func = native_value.last_value_func
             self.cursor_path_p = self.cursor_path_p
@@ -123,14 +122,16 @@
         else:  # TODO: Maybe check if callable(getattr(native_value, '__lt__', None))
             # Passing bare value `incremental=44` gets parsed as initial_value
             self.initial_value = native_value
         self.__is_resolved__ = not self.is_partial()
 
     def get_state(self) -> IncrementalColumnState:
         """Returns an Incremental state for a particular cursor column"""
+        if not self.resource_name:
+            raise IncrementalUnboundError(self.cursor_path)
         self._cached_state = Incremental._get_state(self.resource_name, self.cursor_path)
         if len(self._cached_state) == 0:
             # set the default like this, setdefault evaluates the default no matter if it is needed or not. and our default is heavy
             self._cached_state.update(
                 {
                     "initial_value": self.initial_value,
                     "last_value": self.initial_value,
@@ -161,21 +162,21 @@
         except KeyError as k_err:
             raise IncrementalPrimaryKeyMissing(self.resource_name, k_err.args[0], row)
 
     def transform(self, row: TDataItem) -> bool:
         if row is None:
             return True
 
-        row_values = self.cursor_path_p.find(row)
-        if len(row_values) == 0:
+        row_values = find_values(self.cursor_path_p, row)
+        if not row_values:
             raise IncrementalCursorPathMissing(self.resource_name, self.cursor_path, row)
 
         incremental_state = self._cached_state
         last_value = incremental_state['last_value']
-        row_value = row_values[0].value  # For now the value needs to match deserialized presentation from state
+        row_value = row_values[0]  # For now the value needs to match deserialized presentation from state
         check_values = (row_value,) + ((last_value, ) if last_value is not None else ())
         new_value = self.last_value_func(check_values)
         if last_value == new_value:
             # we store row id for all records with the current "last_value" in state and use it to deduplicate
             if self.last_value_func((row_value, )) == last_value:
                 unique_value = self.unique_value(row)
                 # if unique value exists then use it to deduplicate
```

### Comparing `dlt-0.2.6a0/dlt/extract/pipe.py` & `dlt-0.2.6a1/dlt/extract/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,16 +261,20 @@
     def bind_gen(self, *args: Any, **kwargs: Any) -> Any:
         """Finds and wraps with `args` + `kwargs` the callable generating step in the resource pipe and then replaces the pipe gen with the wrapped one"""
         try:
             gen = self._wrap_gen(*args, **kwargs)
             self.replace_gen(gen)
             return gen
         except InvalidResourceDataTypeFunctionNotAGenerator:
-            # call regular function to check what is inside
-            _data = self.gen(*args, **kwargs)  # type: ignore
+            try:
+                # call regular function to check what is inside
+                _data = self.gen(*args, **kwargs)  # type: ignore
+            except Exception as ev_ex:
+                # break chaining
+                raise ev_ex from None
             # accept if pipe or object holding pipe is returned
             # TODO: use a protocol (but protocols are slow)
             if isinstance(_data, Pipe) or hasattr(_data, "_pipe"):
                 return _data
             raise
 
     def _wrap_gen(self, *args: Any, **kwargs: Any) -> Any:
@@ -658,14 +662,15 @@
     def _get_source_item(self) -> ResolvablePipeItem:
         # no more sources to iterate
         if len(self._sources) == 0:
             return None
 
         # get items from last added iterator, this makes the overall Pipe as close to FIFO as possible
         gen, step, pipe, meta = self._sources[-1]
+        # print(f"got {pipe.name} {pipe._pipe_id}")
         # TODO: count items coming of the generator and stop the generator if reached. that allows for sampling the beginning of a stream
         # _counts(id(gen)).setdefault(0) + 1
         try:
             item = next(gen)
             # full pipe item may be returned, this is used by ForkPipe step
             # to redirect execution of an item to another pipe
             if isinstance(item, ResolvablePipeItem):
```

### Comparing `dlt-0.2.6a0/dlt/extract/schema.py` & `dlt-0.2.6a1/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/extract/source.py` & `dlt-0.2.6a1/dlt/extract/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from dlt.common.schema.typing import TColumnName
 from dlt.common.typing import AnyFun, StrAny, TDataItem, TDataItems, NoneType
 from dlt.common.configuration.container import Container
 from dlt.common.pipeline import PipelineContext, StateInjectableContext, SupportsPipelineRun, _resource_state, source_state, pipeline_state
 from dlt.common.utils import flatten_list_or_items, get_callable_name, multi_context_manager, uniq_id
 
 from dlt.extract.typing import DataItemWithMeta, ItemTransformFunc, ItemTransformFunctionWithMeta, TableNameMeta, FilterItem, MapItem, YieldMapItem
-from dlt.extract.pipe import Pipe, ManagedPipeIterator
+from dlt.extract.pipe import Pipe, ManagedPipeIterator, TPipeStep
 from dlt.extract.schema import DltResourceSchema, TTableSchemaTemplate
 from dlt.extract.incremental import Incremental, IncrementalResourceWrapper
 from dlt.extract.exceptions import (
     InvalidTransformerDataTypeGeneratorFunctionRequired, InvalidParentResourceDataType, InvalidParentResourceIsAFunction, InvalidResourceDataType, InvalidResourceDataTypeFunctionNotAGenerator, InvalidResourceDataTypeIsNone, InvalidTransformerGeneratorFunction,
     DataItemRequiredForDynamicTableHints, InvalidResourceDataTypeAsync, InvalidResourceDataTypeBasic,
     InvalidResourceDataTypeMultiplePipes, ParametrizedResourceUnbound, ResourceNameMissing, ResourceNotATransformer, ResourcesNotFoundError, SourceExhausted, DeletingResourcesNotSupported)
 
@@ -208,14 +208,46 @@
         """
         if insert_at is None:
             self._pipe.append_step(FilterItem(item_filter))
         else:
             self._pipe.insert_step(FilterItem(item_filter), insert_at)
         return self
 
+    def add_limit(self, max_items: int) -> "DltResource":  # noqa: A003
+        """Adds a limit `max_items` to the resource pipe
+
+        This mutates the encapsulated generator to stop after `max_items` items are yielded. This is useful for testing and debugging. It is
+        a no-op for transformers. Those should be limited by their input data.
+
+        Args:
+            max_items (int): The maximum number of items to yield
+        Returns:
+            "DltResource": returns self
+        """
+        def _gen_wrap(gen: TPipeStep) -> TPipeStep:
+            """Wrap a generator to take the first `max_items` records"""
+            nonlocal max_items
+            count = 0
+            if inspect.isfunction(gen):
+                gen = gen()
+            try:
+                for i in gen:  # type: ignore # TODO: help me fix this later
+                    yield i
+                    count += 1
+                    if count == max_items:
+                        return
+            finally:
+                if inspect.isgenerator(gen):
+                    gen.close()
+            return
+        # transformers should be limited by their input, so we only limit non-transformers
+        if not self.is_transformer:
+            self._pipe.replace_gen(_gen_wrap(self._pipe.gen))
+        return self
+
     def add_step(self, item_transform: ItemTransformFunctionWithMeta[TDataItems], insert_at: int = None) -> "DltResource":  # noqa: A003
         if insert_at is None:
             self._pipe.append_step(item_transform)
         else:
             self._pipe.insert_step(item_transform, insert_at)
         return self
 
@@ -570,14 +602,30 @@
         return schema
 
     def with_resources(self, *resource_names: str) -> "DltSource":
         """A convenience method to select one of more resources to be loaded. Returns a source with the specified resources selected."""
         self._resources.select(*resource_names)
         return self
 
+
+    def add_limit(self, max_items: int) -> "DltSource":  # noqa: A003
+        """Adds a limit `max_items` yielded from all selected resources in the source that are not transformers.
+
+        This is useful for testing, debugging and generating sample datasets for experimentation. You can easily get your test dataset in a few minutes, when otherwise
+        you'd need to wait hours for the full loading to complete.
+
+        Args:
+            max_items (int): The maximum number of items to yield
+        Returns:
+            "DltSource": returns self
+        """
+        for resource in self.resources.selected.values():
+            resource.add_limit(max_items)
+        return self
+
     @property
     def run(self) -> SupportsPipelineRun:
         """A convenience method that will call `run` run on the currently active `dlt` pipeline. If pipeline instance is not found, one with default settings will be created."""
         self_run: SupportsPipelineRun = makefun.partial(Container()[PipelineContext].pipeline().run, *(), data=self)
         return self_run
 
     @property
```

### Comparing `dlt-0.2.6a0/dlt/extract/typing.py` & `dlt-0.2.6a1/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/extract/utils.py` & `dlt-0.2.6a1/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/helpers/dbt/__init__.py` & `dlt-0.2.6a1/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/helpers/dbt/configuration.py` & `dlt-0.2.6a1/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.2.6a1/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/helpers/dbt/exceptions.py` & `dlt-0.2.6a1/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/helpers/dbt/profiles.yml` & `dlt-0.2.6a1/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/helpers/dbt/runner.py` & `dlt-0.2.6a1/dlt/helpers/dbt/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import os
 from subprocess import CalledProcessError
 import giturlparse
-from typing import Any, ClassVar, Optional, Sequence
-from prometheus_client import REGISTRY, Gauge, CollectorRegistry, Info
+from typing import Sequence
 
 import dlt
 from dlt.common import logger
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.specs import CredentialsConfiguration
 from dlt.common.configuration.utils import add_config_to_env
 from dlt.common.runners import Venv
 from dlt.common.runners.stdout import iter_stdout_with_result
-from dlt.common.typing import DictStrStr, StrAny, TSecretValue
+from dlt.common.typing import StrAny, TSecretValue
 from dlt.common.runtime.logger import is_json_logging
-from dlt.common.runtime.prometheus import get_logging_extras
 from dlt.common.storages import FileStorage
 from dlt.common.git import git_custom_key_command, ensure_remote_head, force_clone_repo
 from dlt.common.utils import with_custom_environ
 
 from dlt.helpers.dbt.configuration import DBTRunnerConfiguration
 from dlt.helpers.dbt.exceptions import IncrementalSchemaOutOfSyncError, PrerequisitesException, DBTNodeResult, DBTProcessingError
 
@@ -27,48 +25,33 @@
 
     The created wrapper minimizes the required effort to run `dbt` packages on datasets created with `dlt`. It clones the package repo and keeps it up to data,
     shares the `dlt` destination credentials with `dbt` and allows the isolated execution with `venv` parameter.
     The wrapper creates a `dbt` profile from a passed `dlt` credentials and executes the transformations in `source_dataset_name` schema. Additional configuration is
     passed via DBTRunnerConfiguration instance
     """
 
-    model_elapsed_gauge: ClassVar[Gauge] = None
-    model_exec_info: ClassVar[Info] = None
-
     def __init__(self,
         venv: Venv,
         credentials: CredentialsConfiguration,
         working_dir: str,
         source_dataset_name: str,
-        config: DBTRunnerConfiguration,
-        collector: CollectorRegistry = REGISTRY,
+        config: DBTRunnerConfiguration
     ) -> None:
         self.venv = venv
         self.credentials = credentials
         self.working_dir = working_dir
         self.source_dataset_name = source_dataset_name
         self.config = config
 
         self.package_path: str = None
         # set if package is in repo
         self.repo_storage: FileStorage = None
         self.cloned_package_name: str = None
 
         self._setup_location()
-        try:
-            self._create_gauges(collector)
-        except ValueError as v:
-            # ignore re-creation of gauges
-            if "Duplicated" not in str(v):
-                raise
-
-    @staticmethod
-    def _create_gauges(registry: CollectorRegistry) -> None:
-        DBTPackageRunner.model_elapsed_gauge = Gauge("dbtrunner_model_elapsed_seconds", "Last model processing time", ["model"], registry=registry)
-        DBTPackageRunner.model_exec_info = Info("dbtrunner_model_status", "Last execution status of the model", registry=registry)
 
     def _setup_location(self) -> None:
         # set the package location
         url = giturlparse.parse(self.config.package_location, check_domain=False)
         if not url.valid:
             self.package_path = self.config.package_location
         else:
@@ -89,26 +72,19 @@
             package_vars.update(additional_vars)
         return package_vars
 
     def _log_dbt_run_results(self, results: Sequence[DBTNodeResult]) -> None:
         if not results:
             return
 
-        info: DictStrStr = {}
         for res in results:
             if res.status == "error":
                 logger.error(f"Model {res.model_name} error! Error: {res.message}")
             else:
                 logger.info(f"Model {res.model_name} {res.status} in {res.time} seconds with {res.message}")
-            DBTPackageRunner.model_elapsed_gauge.labels(res.model_name).set(res.time)
-            info[res.model_name] = res.message
-
-        # log execution
-        DBTPackageRunner.model_exec_info.info(info)
-        logger.metrics("stop", "dbt models", extra=get_logging_extras([DBTPackageRunner.model_elapsed_gauge, DBTPackageRunner.model_exec_info]))
 
     def ensure_newest_package(self) -> None:
         """Clones or brings the dbt package at `package_location` up to date."""
         from git import GitError
 
         with git_custom_key_command(self.config.package_repository_ssh_key) as ssh_command:
             try:
@@ -290,8 +266,8 @@
     package_repository_branch: str = None,
     package_repository_ssh_key: TSecretValue = TSecretValue(""),  # noqa
     package_profiles_dir: str = None,
     package_profile_name: str = None,
     auto_full_refresh_when_out_of_sync: bool = None,
     config: DBTRunnerConfiguration = None
     ) -> DBTPackageRunner:
-    return DBTPackageRunner(venv, credentials, working_dir, dataset_name, config, REGISTRY)
+    return DBTPackageRunner(venv, credentials, working_dir, dataset_name, config)
```

### Comparing `dlt-0.2.6a0/dlt/helpers/pandas.py` & `dlt-0.2.6a1/dlt/helpers/pandas.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/helpers/parquet.py` & `dlt-0.2.6a1/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/helpers/streamlit.py` & `dlt-0.2.6a1/dlt/helpers/streamlit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Dict
+from typing import Dict, List
 import humanize
 
 
 from dlt.common import pendulum
 from dlt.common.typing import AnyFun
 from dlt.common.schema.typing import LOADS_TABLE_NAME, VERSION_TABLE_NAME
 from dlt.common.configuration.exceptions import ConfigFieldMissingException
@@ -222,16 +222,23 @@
     st.title(f"Available tables in {schema.name} schema")
 
     for table in schema.data_tables():
         table_name = table["name"]
         st.header(table_name)
         if "description" in table:
             st.text(table["description"])
+        table_hints: List[str] = []
         if "parent" in table:
-            st.text("Parent table: " + table["parent"])
+            table_hints.append("parent: **%s**" % table["parent"])
+        if "resource" in table:
+            table_hints.append("resource: **%s**" % table["resource"])
+        if "write_disposition" in table:
+            table_hints.append("write disposition: **%s**" % table["write_disposition"])
+
+        st.markdown(" | ".join(table_hints))
 
         # table schema contains various hints (like clustering or partition options) that we do not want to show in basic view
         essentials_f = lambda c: {k:v for k, v in c.items() if k in ["name", "data_type", "nullable"]}
 
         st.table(map(essentials_f, table["columns"].values()))
         # add a button that when pressed will show the full content of a table
         if st.button("SHOW DATA", key=table_name):
```

### Comparing `dlt-0.2.6a0/dlt/load/configuration.py` & `dlt-0.2.6a1/dlt/load/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,13 +17,11 @@
     _load_storage_config: LoadVolumeConfiguration = None
 
     if TYPE_CHECKING:
         def __init__(
             self,
             pool_type: TPoolType = None,
             workers: int = None,
-            exit_on_exception: bool = None,
-            is_single_run: bool = None,
             raise_on_failed_jobs: bool = False,
             _load_storage_config: LoadVolumeConfiguration = None
         ) -> None:
             ...
```

### Comparing `dlt-0.2.6a0/dlt/load/exceptions.py` & `dlt-0.2.6a1/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/load/load.py` & `dlt-0.2.6a1/dlt/load/load.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,66 @@
+from functools import reduce
+import datetime  # noqa: 251
 from typing import Dict, List, Optional, Tuple
 from multiprocessing.pool import ThreadPool
-from prometheus_client import REGISTRY, Counter, Gauge, CollectorRegistry, Summary
 
 from dlt.common import sleep, logger
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
+from dlt.common.pipeline import LoadInfo, SupportsPipeline
 from dlt.common.schema.utils import get_child_tables, get_top_level_table, get_write_disposition
-from dlt.common.storages.load_storage import ParsedLoadJobFileName, TJobState
+from dlt.common.storages.load_storage import LoadPackageInfo, ParsedLoadJobFileName, TJobState
 from dlt.common.typing import StrAny
 from dlt.common.runners import TRunMetrics, Runnable, workermethod
+from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.runtime.logger import pretty_format_exception
 from dlt.common.exceptions import TerminalValueError
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TTableSchema, TWriteDisposition
 from dlt.common.storages import LoadStorage
-from dlt.common.runtime.prometheus import get_logging_extras, set_gauge_all_labels
-from dlt.common.destination.reference import FollowupJob, JobClientBase, DestinationReference, LoadJob, NewLoadJob, TLoadJobState, DestinationClientConfiguration
+from dlt.common.destination.reference import DestinationClientDwhConfiguration, FollowupJob, JobClientBase, DestinationReference, LoadJob, NewLoadJob, TLoadJobState, DestinationClientConfiguration
 
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.exceptions import DestinationTerminalException, DestinationTransientException, LoadJobUnknownTableException
 
 from dlt.load.configuration import LoaderConfiguration
 from dlt.load.exceptions import LoadClientJobFailed, LoadClientJobRetry, LoadClientUnsupportedWriteDisposition, LoadClientUnsupportedFileFormats
 
 
 class Load(Runnable[ThreadPool]):
 
-    load_counter: Counter = None
-    job_gauge: Gauge = None
-    job_counter: Counter = None
-    job_wait_summary: Summary = None
-
     @with_config(spec=LoaderConfiguration, sections=(known_sections.LOAD,))
     def __init__(
         self,
         destination: DestinationReference,
-        collector: CollectorRegistry = REGISTRY,
+        collector: Collector = NULL_COLLECTOR,
         is_storage_owner: bool = False,
         config: LoaderConfiguration = config.value,
         initial_client_config: DestinationClientConfiguration = config.value
     ) -> None:
         self.config = config
+        self.collector = collector
         self.initial_client_config = initial_client_config
         self.destination = destination
         self.capabilities = destination.capabilities()
         self.pool: ThreadPool = None
         self.load_storage: LoadStorage = self.create_storage(is_storage_owner)
-        self._processed_load_ids: Dict[str, StrAny] = {}
-        try:
-            Load.create_gauges(collector)
-        except ValueError as v:
-            # ignore re-creation of gauges
-            if "Duplicated" not in str(v):
-                raise
+        self._processed_load_ids: Dict[str, int] = {}
+
 
     def create_storage(self, is_storage_owner: bool) -> LoadStorage:
         load_storage = LoadStorage(
             is_storage_owner,
             self.capabilities.preferred_loader_file_format,
             self.capabilities.supported_loader_file_formats,
             config=self.config._load_storage_config
         )
         return load_storage
 
     @staticmethod
-    def create_gauges(registry: CollectorRegistry) -> None:
-        Load.load_counter = Counter("loader_load_package_counter", "Counts load package processed", registry=registry)
-        Load.job_gauge = Gauge("loader_last_package_jobs_counter", "Counts jobs in last package per state", ["state"], registry=registry)
-        Load.job_counter = Counter("loader_jobs_counter", "Counts jobs per job state", ["state"], registry=registry)
-        Load.job_wait_summary = Summary("loader_jobs_wait_seconds", "Counts jobs total wait until completion", registry=registry)
-
-    @staticmethod
     def get_load_table(schema: Schema, file_name: str) -> TTableSchema:
         table_name = LoadStorage.parse_job_file_name(file_name).table_name
         try:
             table = schema.get_table(table_name)
             # add write disposition if not specified - in child tables
             if "write_disposition" not in table:
                 table["write_disposition"] = get_write_disposition(schema.tables, table_name)
@@ -144,26 +130,23 @@
                 job = EmptyLoadJob.from_file_path(file_path, "failed", pretty_format_exception())
                 # proceed to appending job, do not reraise
             except (DestinationTransientException, Exception):
                 # raise on all temporary exceptions, typically network / server problems
                 raise
             jobs.append(job)
 
-        self.job_gauge.labels("retrieved").inc()
-        self.job_counter.labels("retrieved").inc()
-        logger.metrics("progress", "retrieve jobs", extra=get_logging_extras([self.job_gauge.labels("retrieved"), self.job_counter.labels("retrieved")]))
         return len(jobs), jobs
 
-    def get_jobs_info(self, load_id: str, schema: Schema, disposition: TWriteDisposition = None) -> List[ParsedLoadJobFileName]:
-        merge_jobs_info: List[ParsedLoadJobFileName] = []
+    def get_new_jobs_info(self, load_id: str, schema: Schema, disposition: TWriteDisposition = None) -> List[ParsedLoadJobFileName]:
+        jobs_info: List[ParsedLoadJobFileName] = []
         new_job_files = self.load_storage.list_new_jobs(load_id)
         for job_file in new_job_files:
             if not disposition or self.get_load_table(schema, job_file)["write_disposition"] == disposition:
-                merge_jobs_info.append(LoadStorage.parse_job_file_name(job_file))
-        return merge_jobs_info
+                jobs_info.append(LoadStorage.parse_job_file_name(job_file))
+        return jobs_info
 
     def create_merge_job(self, load_id: str, schema: Schema, top_merged_table: TTableSchema, starting_job: LoadJob) -> NewLoadJob:
         # returns ordered list of tables from parent to child leaf tables
         table_chain: List[TTableSchema] = []
         # make sure all the jobs for the table chain is completed
         for table in get_child_tables(schema.tables, top_merged_table["name"]):
             table_jobs = self.load_storage.list_jobs_for_table(load_id, table["name"])
@@ -194,23 +177,22 @@
     def complete_jobs(self, load_id: str, jobs: List[LoadJob], schema: Schema) -> List[LoadJob]:
         remaining_jobs: List[LoadJob] = []
         logger.info(f"Will complete {len(jobs)} for {load_id}")
         for ii in range(len(jobs)):
             job = jobs[ii]
             logger.debug(f"Checking state for job {job.job_id()}")
             state: TLoadJobState = job.state()
-            final_location: str = None
             if state == "running":
                 # ask again
                 logger.debug(f"job {job.job_id()} still running")
                 remaining_jobs.append(job)
             elif state == "failed":
                 # try to get exception message from job
                 failed_message = job.exception()
-                final_location = self.load_storage.fail_job(load_id, job.file_name(), failed_message)
+                self.load_storage.fail_job(load_id, job.file_name(), failed_message)
                 logger.error(f"Job for {job.job_id()} failed terminally in load {load_id} with message {failed_message}")
             elif state == "retry":
                 # try to get exception message from job
                 retry_message = job.exception()
                 # move back to new folder to try again
                 self.load_storage.retry_job(load_id, job.file_name())
                 logger.warning(f"Job for {job.job_id()} retried in load {load_id} with message {retry_message}")
@@ -224,123 +206,143 @@
                     self.load_storage.add_new_job(load_id, followup_job.new_file_path(), job_state=folder)
                     logger.info(f"Job {job.job_id()} CREATED a new FOLLOWUP JOB {followup_job.new_file_path()} placed in {folder}")
                     # if followup job is not "running" place it in current queue to be finalized
                     if not followup_job.state() == "running":
                         remaining_jobs.append(followup_job)
                 # move to completed folder after followup jobs are created
                 # in case of exception when creating followup job, the loader will retry operation and try to complete again
-                final_location = self.load_storage.complete_job(load_id, job.file_name())
+                self.load_storage.complete_job(load_id, job.file_name())
                 logger.info(f"Job for {job.job_id()} completed in load {load_id}")
 
             if state in ["failed", "completed"]:
-                self.job_gauge.labels(state).inc()
-                self.job_counter.labels(state).inc()
-                self.job_wait_summary.observe(self.load_storage.job_elapsed_time_seconds(final_location))
+                self.collector.update("Jobs")
+                if state == "failed":
+                    self.collector.update("Jobs", 1, message="WARNING: Some of the jobs failed!", label="Failed")
 
-        logger.metrics("progress", "jobs", extra=get_logging_extras([self.job_counter, self.job_gauge, self.job_wait_summary]))
         return remaining_jobs
 
     def complete_package(self, load_id: str, schema: Schema, aborted: bool = False) -> None:
         # do not commit load id for aborted packages
         if not aborted:
             with self.destination.client(schema, self.initial_client_config) as job_client:
-                # TODO: this script should be executed as a job (and contain also code to merge/upsert data and drop temp tables)
-                # TODO: post loading jobs
                 job_client.complete_load(load_id)
         self.load_storage.complete_load_package(load_id, aborted)
         logger.info(f"All jobs completed, archiving package {load_id} with aborted set to {aborted}")
-        self.load_counter.inc()
-        metrics = get_logging_extras([self.load_counter])
-        self._processed_load_ids[load_id] = metrics
-        logger.metrics("stop", "jobs", extra=metrics)
+        self._processed_load_ids[load_id] = 1
 
-    def load_single_package(self, load_id: str) -> None:
-        logger.info(f"Loading schema from load package in {load_id}")
-        schema = self.load_storage.load_package_schema(load_id)
-        logger.info(f"Loaded schema name {schema.name} and version {schema.stored_version}")
+    def load_single_package(self, load_id: str, schema: Schema) -> None:
         # initialize analytical storage ie. create dataset required by passed schema
         job_client: JobClientBase
         with self.destination.client(schema, self.initial_client_config) as job_client:
             expected_update = self.load_storage.begin_schema_update(load_id)
             if expected_update is not None:
                 # update the default dataset
                 logger.info(f"Client for {job_client.config.destination_name} will start initialize storage")
                 job_client.initialize_storage()
                 logger.info(f"Client for {job_client.config.destination_name} will update schema to package schema")
-                all_jobs = self.get_jobs_info(load_id, schema)
+                all_jobs = self.get_new_jobs_info(load_id, schema)
                 all_tables = [job.table_name for job in all_jobs]
                 dlt_tables = [t["name"] for t in schema.dlt_tables()]
                 # only update tables that are present in the load package
                 applied_update = job_client.update_storage_schema(only_tables=set(all_tables+dlt_tables), expected_update=expected_update)
                 # update the staging dataset
-                merge_jobs = self.get_jobs_info(load_id, schema, "merge")
+                merge_jobs = self.get_new_jobs_info(load_id, schema, "merge")
                 if merge_jobs:
                     logger.info(f"Client for {job_client.config.destination_name} will start initialize STAGING storage")
                     job_client.initialize_storage(staging=True)
                     logger.info(f"Client for {job_client.config.destination_name} will UPDATE STAGING SCHEMA to package schema")
                     merge_tables = [job.table_name for job in merge_jobs]
                     job_client.update_storage_schema(staging=True, only_tables=set(merge_tables+dlt_tables), expected_update=expected_update)
                     logger.info(f"Client for {job_client.config.destination_name} will TRUNCATE STAGING TABLES: {merge_tables}")
                     job_client.initialize_storage(staging=True, truncate_tables=merge_tables)
                 self.load_storage.commit_schema_update(load_id, applied_update)
             # spool or retrieve unfinished jobs
             jobs_count, jobs = self.retrieve_jobs(job_client, load_id)
+
         if not jobs:
             # jobs count is a total number of jobs including those that could not be initialized
             jobs_count, jobs = self.spool_new_jobs(load_id, schema)
-            if jobs_count > 0:
-                # this is a new  load package
-                # TODO: this is wrong, we must check completed and failed jobs to say that
-                set_gauge_all_labels(self.job_gauge, 0)
-                self.job_gauge.labels("running").inc(len(jobs))
-                self.job_counter.labels("running").inc(len(jobs))
-                logger.metrics("progress", "jobs",
-                                extra=get_logging_extras([self.job_counter.labels("running"), self.job_gauge.labels("running")])
-            )
         # if there are no existing or new jobs we complete the package
         if jobs_count == 0:
             self.complete_package(load_id, schema, False)
-        else:
-            while True:
-                try:
-                    remaining_jobs = self.complete_jobs(load_id, jobs, schema)
-                    if len(remaining_jobs) == 0:
-                        # get package status
-                        package_info = self.load_storage.get_load_package_info(load_id)
-                        # possibly raise on failed jobs
-                        if self.config.raise_on_failed_jobs:
-                            if package_info.jobs["failed_jobs"]:
-                                failed_job = package_info.jobs["failed_jobs"][0]
-                                raise LoadClientJobFailed(load_id, failed_job.job_file_info.job_id(), failed_job.failed_message)
-                        # possibly raise on too many retires
-                        if self.config.raise_on_max_retries:
-                            for new_job in package_info.jobs["new_jobs"]:
-                                r_c = new_job.job_file_info.retry_count
-                                if r_c > 0 and r_c % self.config.raise_on_max_retries == 0:
-                                    raise LoadClientJobRetry(load_id, new_job.job_file_info.job_id(), r_c, self.config.raise_on_max_retries)
-                        break
-                    # process remaining jobs again
-                    jobs = remaining_jobs
-                    # this will raise on signal
-                    sleep(1)
-                except LoadClientJobFailed:
-                    # the package is completed and skipped
-                    self.complete_package(load_id, schema, True)
-                    raise
+            return
+        # update counter we only care about the jobs that are scheduled to be loaded
+        package_info = self.load_storage.get_load_package_info(load_id)
+        total_jobs = reduce(lambda p, c: p + len(c), package_info.jobs.values(), 0)
+        no_failed_jobs = len(package_info.jobs["failed_jobs"])
+        no_completed_jobs = len(package_info.jobs["completed_jobs"]) + no_failed_jobs
+        self.collector.update("Jobs", no_completed_jobs, total_jobs)
+        if no_failed_jobs > 0:
+            self.collector.update("Jobs", no_failed_jobs, message="WARNING: Some of the jobs failed!", label="Failed")
+        # loop until all jobs are processed
+        while True:
+            try:
+                remaining_jobs = self.complete_jobs(load_id, jobs, schema)
+                if len(remaining_jobs) == 0:
+                    # get package status
+                    package_info = self.load_storage.get_load_package_info(load_id)
+                    # possibly raise on failed jobs
+                    if self.config.raise_on_failed_jobs:
+                        if package_info.jobs["failed_jobs"]:
+                            failed_job = package_info.jobs["failed_jobs"][0]
+                            raise LoadClientJobFailed(load_id, failed_job.job_file_info.job_id(), failed_job.failed_message)
+                    # possibly raise on too many retires
+                    if self.config.raise_on_max_retries:
+                        for new_job in package_info.jobs["new_jobs"]:
+                            r_c = new_job.job_file_info.retry_count
+                            if r_c > 0 and r_c % self.config.raise_on_max_retries == 0:
+                                raise LoadClientJobRetry(load_id, new_job.job_file_info.job_id(), r_c, self.config.raise_on_max_retries)
+                    break
+                # process remaining jobs again
+                jobs = remaining_jobs
+                # this will raise on signal
+                sleep(1)
+            except LoadClientJobFailed:
+                # the package is completed and skipped
+                self.complete_package(load_id, schema, True)
+                raise
 
     def run(self, pool: ThreadPool) -> TRunMetrics:
         # store pool
         self.pool = pool
 
         logger.info("Running file loading")
         # get list of loads and order by name ASC to execute schema updates
         loads = self.load_storage.list_packages()
         logger.info(f"Found {len(loads)} load packages")
         if len(loads) == 0:
-            return TRunMetrics(True, False, 0)
+            return TRunMetrics(True, 0)
 
-        # get top job id and mark as being processed
-        # TODO: another place where tracing must be refactored
+        # load the schema from the package
         load_id = loads[0]
+        logger.info(f"Loading schema from load package in {load_id}")
+        schema = self.load_storage.load_package_schema(load_id)
+        logger.info(f"Loaded schema name {schema.name} and version {schema.stored_version}")
+
+        # get top load id and mark as being processed
+        # TODO: another place where tracing must be refactored
         self._processed_load_ids[load_id] = None
-        self.load_single_package(load_id)
-        return TRunMetrics(False, False, len(self.load_storage.list_packages()))
+        with self.collector(f"Load {schema.name} in {load_id}"):
+            self.load_single_package(load_id, schema)
+        return TRunMetrics(False, len(self.load_storage.list_packages()))
+
+    def get_load_info(self, pipeline: SupportsPipeline, started_at: datetime.datetime = None) -> LoadInfo:
+        # TODO: Load must provide a clear interface to get last loads and metrics
+        # TODO: LoadInfo should hold many datasets
+        load_ids = list(self._processed_load_ids.keys())
+        load_packages: List[LoadPackageInfo] = []
+        for load_id in load_ids:
+            load_packages.append(self.load_storage.get_load_package_info(load_id))
+        dataset_name = None
+        if isinstance(self.initial_client_config, DestinationClientDwhConfiguration):
+            dataset_name = self.initial_client_config.dataset_name
+
+        return LoadInfo(
+            pipeline,
+            self.initial_client_config.destination_name,
+            str(self.initial_client_config.credentials),
+            dataset_name,
+            list(load_ids),
+            load_packages,
+            started_at,
+            pipeline.first_run
+        )
```

### Comparing `dlt-0.2.6a0/dlt/normalize/configuration.py` & `dlt-0.2.6a1/dlt/normalize/configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,12 @@
     _load_storage_config: LoadVolumeConfiguration
 
     if TYPE_CHECKING:
         def __init__(
             self,
             pool_type: TPoolType = None,
             workers: int = None,
-            exit_on_exception: bool = None,
-            is_single_run: bool = None,
             _schema_storage_config: SchemaVolumeConfiguration = None,
             _normalize_storage_config: NormalizeVolumeConfiguration = None,
             _load_storage_config: LoadVolumeConfiguration = None
         ) -> None:
             ...
```

### Comparing `dlt-0.2.6a0/dlt/normalize/normalize.py` & `dlt-0.2.6a1/dlt/normalize/normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,55 @@
 import os
-from itertools import chain
 from typing import Any, Callable, List, Dict, Sequence, Tuple
 from multiprocessing.pool import AsyncResult, Pool as ProcessPool
-from prometheus_client import Counter, CollectorRegistry, REGISTRY, Gauge
 
 from dlt.common import pendulum, json, logger, sleep
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.specs import LoadVolumeConfiguration, NormalizeVolumeConfiguration
 from dlt.common.destination import DestinationCapabilitiesContext, TLoaderFileFormat
 from dlt.common.json import custom_pua_decode
 from dlt.common.runners import TRunMetrics, Runnable
 from dlt.common.runtime import signals
+from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.schema.typing import TStoredSchema, TTableSchemaColumns
 from dlt.common.schema.utils import merge_schema_updates
 from dlt.common.storages.exceptions import SchemaNotFoundError
 from dlt.common.storages import NormalizeStorage, SchemaStorage, LoadStorage
-from dlt.common.runtime.prometheus import get_logging_extras
 from dlt.common.typing import TDataItem
 from dlt.common.schema import TSchemaUpdate, Schema
 from dlt.common.schema.exceptions import CannotCoerceColumnException
 from dlt.common.utils import chunks
 
 from dlt.normalize.configuration import NormalizeConfiguration
 
 # normalize worker wrapping function (map_parallel, map_single) return type
-TMapFuncRV = Tuple[int, Sequence[TSchemaUpdate]]  # (total items processed, total schema updates)
+TMapFuncRV = Sequence[TSchemaUpdate]
 # normalize worker wrapping function signature
 TMapFuncType = Callable[[Schema, str, Sequence[str]], TMapFuncRV]  # input parameters: (schema name, load_id, list of files to process)
 # tuple returned by the worker
 TWorkerRV = Tuple[List[TSchemaUpdate], int, List[str]]
 
 
 class Normalize(Runnable[ProcessPool]):
 
-    # make our gauges static
-    item_counter: Counter = None
-    item_gauge: Gauge = None
-    schema_version_gauge: Gauge = None
-    load_package_counter: Counter = None
-
     @with_config(spec=NormalizeConfiguration, sections=(known_sections.NORMALIZE,))
-    def __init__(self, collector: CollectorRegistry = REGISTRY, schema_storage: SchemaStorage = None, config: NormalizeConfiguration = config.value) -> None:
+    def __init__(self, collector: Collector = NULL_COLLECTOR, schema_storage: SchemaStorage = None, config: NormalizeConfiguration = config.value) -> None:
         self.config = config
+        self.collector = collector
         self.pool: ProcessPool = None
         self.normalize_storage: NormalizeStorage = None
         self.load_storage: LoadStorage = None
         self.schema_storage: SchemaStorage = None
 
         # setup storages
         self.create_storages(config.destination_capabilities.preferred_loader_file_format)
         # create schema storage with give type
         self.schema_storage = schema_storage or SchemaStorage(self.config._schema_storage_config, makedirs=True)
-        try:
-            self.create_gauges(collector)
-        except ValueError as v:
-            # ignore re-creation of gauges
-            if "Duplicated" not in str(v):
-                raise
-
-    @staticmethod
-    def create_gauges(registry: CollectorRegistry) -> None:
-        Normalize.item_counter = Counter("normalize_item_count", "Items processed in normalize", ["schema"], registry=registry)
-        Normalize.item_gauge = Gauge("normalize_last_items", "Number of items processed in last run", ["schema"], registry=registry)
-        Normalize.schema_version_gauge = Gauge("normalize_schema_version", "Current schema version", ["schema"], registry=registry)
-        Normalize.load_package_counter = Counter("normalize_load_packages_created_count", "Count of load package created", ["schema"], registry=registry)
 
     def create_storages(self, loader_file_format: TLoaderFileFormat) -> None:
         # pass initial normalize storage config embedded in normalize config
         self.normalize_storage = NormalizeStorage(True, config=self.config._normalize_storage_config)
         # normalize saves in preferred format but can read all supported formats
         self.load_storage = LoadStorage(True, loader_file_format, LoadStorage.ALL_SUPPORTED_FILE_FORMATS, config=self.config._load_storage_config)
 
@@ -198,15 +178,14 @@
         schema_dict: TStoredSchema = schema.to_dict()
         config_tuple = (self.normalize_storage.config, self.load_storage.config, self.config.destination_capabilities, schema_dict)
         param_chunk = [[*config_tuple, load_id, files] for files in chunk_files]
         tasks: List[Tuple[AsyncResult[TWorkerRV], List[Any]]] = []
 
         # return stats
         schema_updates: List[TSchemaUpdate] = []
-        total_items_processed = 0
 
         # push all tasks to queue
         for params in param_chunk:
             pending: AsyncResult[TWorkerRV] = self.pool.apply_async(Normalize.w_normalize_files, params)
             tasks.append((pending, params))
 
         while len(tasks) > 0:
@@ -217,15 +196,17 @@
                 if pending.ready():
                     if pending.successful():
                         result: TWorkerRV = pending.get()
                         try:
                             # gather schema from all manifests, validate consistency and combine
                             self.update_schema(schema, result[0])
                             schema_updates.extend(result[0])
-                            total_items_processed += result[1]
+                            # update metrics
+                            self.collector.update("Files", len(result[2]))
+                            self.collector.update("Items", result[1])
                         except CannotCoerceColumnException as exc:
                             # schema conflicts resulting from parallel executing
                             logger.warning(f"Parallel schema update conflict, retrying task ({str(exc)}")
                             # delete all files produced by the task
                             for file in result[2]:
                                 os.remove(file)
                             # schedule the task again
@@ -237,36 +218,35 @@
                         # remove finished tasks
                         tasks.remove(task)
                     else:
                         # raise the exception
                         pending.get()
                         raise AssertionError("unreachable code: pending.get must raise")
 
-        return total_items_processed, schema_updates
+        return schema_updates
 
     def map_single(self, schema: Schema, load_id: str, files: Sequence[str]) -> TMapFuncRV:
         result = Normalize.w_normalize_files(
             self.normalize_storage.config,
             self.load_storage.config,
             self.config.destination_capabilities,
             schema.to_dict(),
             load_id,
             files
         )
-
         self.update_schema(schema, result[0])
-        return result[1], result[0]
+        self.collector.update("Files", len(result[2]))
+        self.collector.update("Items", result[1])
+        return result[0]
 
     def spool_files(self, schema_name: str, load_id: str, map_f: TMapFuncType, files: Sequence[str]) -> None:
         schema = Normalize.load_or_create_schema(self.schema_storage, schema_name)
 
         # process files in parallel or in single thread, depending on map_f
-        total_items, schema_updates = map_f(schema, load_id, files)
-        logger.info(f"In schema {schema_name} {total_items} processed with {len(schema_updates)} schema updates")
-        self.schema_version_gauge.labels(schema_name).set(schema.version)
+        schema_updates = map_f(schema, load_id, files)
         # logger.metrics("Normalize metrics", extra=get_logging_extras([self.schema_version_gauge.labels(schema_name)]))
         if len(schema_updates) > 0:
             logger.info(f"Saving schema {schema_name} with version {schema.version}, writing manifest files")
             # schema is updated, save it to schema volume
             self.schema_storage.save_schema(schema)
         # save schema to temp load folder
         self.load_storage.save_temp_schema(schema, load_id)
@@ -276,27 +256,20 @@
         signals.raise_if_signalled()
         logger.info("Committing storage, do not kill this process")
         # rename temp folder to processing
         self.load_storage.commit_temp_load_package(load_id)
         # delete item files to complete commit
         for file in files:
                 self.normalize_storage.storage.delete(file)
-        # for item_file in chain.from_iterable(chunk_files):  # flatten chunks
-        #     self.normalize_storage.storage.delete(item_file)
         # log and update metrics
         logger.info(f"Chunk {load_id} processed")
-        self.load_package_counter.labels(schema_name).inc()
-        self.item_counter.labels(schema_name).inc(total_items)
-        self.item_gauge.labels(schema_name).set(total_items)
-        logger.metrics("stop", "schema items", extra=get_logging_extras(
-            [self.load_package_counter.labels(schema_name), self.item_counter.labels(schema_name), self.item_gauge.labels(schema_name)]))
 
-    def spool_schema_files(self, schema_name: str, files: Sequence[str]) -> str:
+    def spool_schema_files(self, load_id: str, schema_name: str, files: Sequence[str]) -> str:
         # normalized files will go here before being atomically renamed
-        load_id = str(pendulum.now().timestamp())
+
         self.load_storage.create_temp_load_package(load_id)
         logger.info(f"Created temp load folder {load_id} on loading volume")
 
         # if pool is not present use map_single method to run normalization in single process
         map_parallel_f = self.map_parallel if self.pool else self.map_single
         try:
             # process parallel
@@ -314,14 +287,19 @@
         # keep the pool in class instance
         self.pool = pool
         logger.info("Running file normalizing")
         # list files and group by schema name, list must be sorted for group by to actually work
         files = self.normalize_storage.list_files_to_normalize_sorted()
         logger.info(f"Found {len(files)} files")
         if len(files) == 0:
-            return TRunMetrics(True, False, 0)
+            return TRunMetrics(True, 0)
         # group files by schema
-        for schema_name, files_in_schema in self.normalize_storage.group_by_schema(files):
-            logger.info(f"Found files in schema {schema_name}")
-            self.spool_schema_files(schema_name, list(files_in_schema))
+        for schema_name, files_iter in self.normalize_storage.group_by_schema(files):
+            schema_files = list(files_iter)
+            load_id = str(pendulum.now().timestamp())
+            logger.info(f"Found {len(schema_files)} files in schema {schema_name} load_id {load_id}")
+            with self.collector(f"Normalize {schema_name} in {load_id}"):
+                self.collector.update("Files", 0, len(schema_files))
+                self.collector.update("Items", 0)
+                self.spool_schema_files(load_id, schema_name, schema_files)
         # return info on still pending files (if extractor saved something in the meantime)
-        return TRunMetrics(False, False, len(self.normalize_storage.list_files_to_normalize_sorted()))
+        return TRunMetrics(False, len(self.normalize_storage.list_files_to_normalize_sorted()))
```

### Comparing `dlt-0.2.6a0/dlt/pipeline/README.md` & `dlt-0.2.6a1/dlt/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/pipeline/__init__.py` & `dlt-0.2.6a1/dlt/pipeline/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.inject import get_orig_args, last_config
 from dlt.common.destination.reference import DestinationReference, TDestinationReferenceArg
 from dlt.common.pipeline import LoadInfo, PipelineContext, get_dlt_pipelines_dir
 
 from dlt.pipeline.configuration import PipelineConfiguration, ensure_correct_pipeline_kwargs
 from dlt.pipeline.pipeline import Pipeline
+from dlt.pipeline.progress import _from_name as collector_from_name, TCollectorArg, _NULL_COLLECTOR
 
 
 @overload
 def pipeline(
     pipeline_name: str = None,
     pipelines_dir: str = None,
     pipeline_salt: TSecretValue = None,
     destination: TDestinationReferenceArg = None,
     dataset_name: str = None,
     import_schema_path: str = None,
     export_schema_path: str = None,
     full_refresh: bool = False,
-    credentials: Any = None
+    credentials: Any = None,
+    progress: TCollectorArg = _NULL_COLLECTOR
 ) -> Pipeline:
     """Creates a new instance of `dlt` pipeline, which moves the data from the source ie. a REST API to a destination ie. database or a data lake.
 
     ### Summary
     The `pipeline` functions allows you to pass the destination name to which the data should be loaded, the name of the dataset and several other options that govern loading of the data.
     The created `Pipeline` object lets you load the data from any source with `run` method or to have more granular control over the loading process with `extract`, `normalize` and `load` methods.
 
@@ -58,14 +60,18 @@
 
         full_refresh (bool, optional): When set to True, each instance of the pipeline with the `pipeline_name` starts from scratch when run and loads the data to a separate dataset.
         The datasets are identified by `dataset_name_` + datetime suffix. Use this setting whenever you experiment with your data to be sure you start fresh on each run. Defaults to False.
 
         credentials (Any, optional): Credentials for the `destination` ie. database connection string or a dictionary with google cloud credentials.
         In most cases should be set to None, which lets `dlt` to use `secrets.toml` or environment variables to infer right credentials values.
 
+        progress(str, Collector): A progress monitor that shows progress bars, console or log messages with current information on sources, resources, data items etc. processed in
+        `extract`, `normalize` and `load` stage. Pass a string with a collector name or configure your own by choosing from `dlt.progress` module.
+        We support most of the progress libraries: try passing `tqdm`, `enlighten` or `alive_progress` or `log` to write to console/log.
+
     ### Returns:
         Pipeline: An instance of `Pipeline` class with. Please check the documentation of `run` method for information on what to do with it.
     """
 
 
 @overload
 def pipeline() -> Pipeline:  # type: ignore
@@ -80,14 +86,15 @@
     pipeline_salt: TSecretValue = None,
     destination: TDestinationReferenceArg = None,
     dataset_name: str = None,
     import_schema_path: str = None,
     export_schema_path: str = None,
     full_refresh: bool = False,
     credentials: Any = None,
+    progress: TCollectorArg = _NULL_COLLECTOR,
     **kwargs: Any
 ) -> Pipeline:
     ensure_correct_pipeline_kwargs(pipeline, **kwargs)
     # call without arguments returns current pipeline
     orig_args = get_orig_args(**kwargs)  # original (*args, **kwargs)
     # is any of the arguments different from defaults
     has_arguments = bool(orig_args[0]) or any(orig_args[1].values())
@@ -101,25 +108,27 @@
             pass
 
     # if working_dir not provided use temp folder
     if not pipelines_dir:
         pipelines_dir = get_dlt_pipelines_dir()
 
     destination = DestinationReference.from_name(destination or kwargs["destination_name"])
+    progress = collector_from_name(progress)
     # create new pipeline instance
     p = Pipeline(
         pipeline_name,
         pipelines_dir,
         pipeline_salt,
         destination,
         dataset_name,
         credentials,
         import_schema_path,
         export_schema_path,
         full_refresh,
+        progress,
         False,
         last_config(**kwargs),
         kwargs["runtime"])
     # set it as current pipeline
     Container()[PipelineContext].activate(p)
 
     return p
@@ -127,22 +136,24 @@
 
 @with_config(spec=PipelineConfiguration, auto_pipeline_section=True)
 def attach(
     pipeline_name: str = None,
     pipelines_dir: str = None,
     pipeline_salt: TSecretValue = None,
     full_refresh: bool = False,
+    progress: TCollectorArg = _NULL_COLLECTOR,
     **kwargs: Any
 ) -> Pipeline:
     ensure_correct_pipeline_kwargs(attach, **kwargs)
     # if working_dir not provided use temp folder
     if not pipelines_dir:
         pipelines_dir = get_dlt_pipelines_dir()
+    progress = collector_from_name(progress)
     # create new pipeline instance
-    p = Pipeline(pipeline_name, pipelines_dir, pipeline_salt, None, None, None, None, None, full_refresh, True, last_config(**kwargs), kwargs["runtime"])
+    p = Pipeline(pipeline_name, pipelines_dir, pipeline_salt, None, None, None, None, None, full_refresh, progress, True, last_config(**kwargs), kwargs["runtime"])
     # set it as current pipeline
     Container()[PipelineContext].activate(p)
     return p
 
 
 def run(
     data: Any,
@@ -151,15 +162,15 @@
     dataset_name: str = None,
     credentials: Any = None,
     table_name: str = None,
     write_disposition: TWriteDisposition = None,
     columns: Sequence[TColumnSchema] = None,
     schema: Schema = None
 ) -> LoadInfo:
-    """Loads the data from `data` argument into the destination specified in `destination` and dataset specified in `dataset_name`.
+    """Loads the data in `data` argument into the destination specified in `destination` and dataset specified in `dataset_name`.
 
     ### Summary
     This method will `extract` the data from the `data` argument, infer the schema, `normalize` the data into a load package (ie. jsonl or PARQUET files representing tables) and then `load` such packages into the `destination`.
 
     The data may be supplied in several forms:
     * a `list` or `Iterable` of any JSON-serializable objects ie. `dlt.run([1, 2, 3], table_name="numbers")`
     * any `Iterator` or a function that yield (`Generator`) ie. `dlt.run(range(1, 10), table_name="range")`
@@ -178,25 +189,24 @@
 
         destination (str | DestinationReference, optional): A name of the destination to which dlt will load the data, or a destination module imported from `dlt.destination`.
         If not provided, the value passed to `dlt.pipeline` will be used.
 
         dataset_name (str, optional):A name of the dataset to which the data will be loaded. A dataset is a logical group of tables ie. `schema` in relational databases or folder grouping many files.
         If not provided, the value passed to `dlt.pipeline` will be used. If not provided at all then defaults to the `pipeline_name`
 
-
         credentials (Any, optional): Credentials for the `destination` ie. database connection string or a dictionary with google cloud credentials.
         In most cases should be set to None, which lets `dlt` to use `secrets.toml` or environment variables to infer right credentials values.
 
         table_name (str, optional): The name of the table to which the data should be loaded within the `dataset`. This argument is required for a `data` that is a list/Iterable or Iterator without `__name__` attribute.
         The behavior of this argument depends on the type of the `data`:
         * generator functions: the function name is used as table name, `table_name` overrides this default
         * `@dlt.resource`: resource contains the full table schema and that includes the table name. `table_name` will override this property. Use with care!
         * `@dlt.source`: source contains several resources each with a table schema. `table_name` will override all table names within the source and load the data into single table.
 
-        write_disposition (Literal["skip", "append", "replace"], optional): Controls how to write data to a table. `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. . Defaults to "append".
+        write_disposition (Literal["skip", "append", "replace", "merge"], optional): Controls how to write data to a table. `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
         Please note that in case of `dlt.resource` the table schema value will be overwritten and in case of `dlt.source`, the values in all resources will be overwritten.
 
         columns (Sequence[TColumnSchema], optional): A list of column schemas. Typed dictionary describing column names, data types, write disposition and performance hints that gives you full control over the created table schema.
 
         schema (Schema, optional): An explicit `Schema` object in which all table schemas will be grouped. By default `dlt` takes the schema from the source (if passed in `data` argument) or creates a default one itself.
 
     ### Raises:
```

### Comparing `dlt-0.2.6a0/dlt/pipeline/configuration.py` & `dlt-0.2.6a1/dlt/pipeline/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     """Enables the `run` method of the `Pipeline` object to restore the pipeline state and schemas from the destination"""
     enable_runtime_trace: bool = True
     """Enables the tracing. Tracing saves the execution trace locally and is required by `dlt deploy`."""
     use_single_dataset: bool = True
     """Stores all schemas in single dataset. When False, each schema will get a separate dataset with `{dataset_name}_{schema_name}"""
     full_refresh: bool = False
     """When set to True, each instance of the pipeline with the `pipeline_name` starts from scratch when run and loads the data to a separate dataset."""
+    progress: Optional[str] = None
     runtime: RunConfiguration
 
     def on_resolved(self) -> None:
         if not self.pipeline_name:
             self.pipeline_name = self.runtime.pipeline_name
         else:
             self.runtime.pipeline_name = self.pipeline_name
```

### Comparing `dlt-0.2.6a0/dlt/pipeline/dbt.py` & `dlt-0.2.6a1/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/pipeline/exceptions.py` & `dlt-0.2.6a1/dlt/pipeline/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any
 from dlt.common.exceptions import PipelineException
 from dlt.common.pipeline import SupportsPipeline
-from dlt.common.runners import TRunMetrics
 from dlt.pipeline.typing import TPipelineStep
 
 
 class InvalidPipelineName(PipelineException, ValueError):
     def __init__(self, pipeline_name: str, details: str) -> None:
         super().__init__(pipeline_name, f"The pipeline name {pipeline_name} contains invalid characters. The pipeline name is used to create a pipeline working directory and must be a valid directory name. The actual error is: {details}")
 
@@ -28,22 +27,30 @@
 
 class SqlClientNotAvailable(PipelineException):
     def __init__(self, pipeline_name: str,destination_name: str) -> None:
         super().__init__(pipeline_name, f"SQL Client not available for destination {destination_name} in pipeline {pipeline_name}")
 
 
 class PipelineStepFailed(PipelineException):
-    def __init__(self, pipeline: SupportsPipeline, step: TPipelineStep, exception: BaseException, run_metrics: TRunMetrics, step_info: Any = None) -> None:
+    def __init__(self, pipeline: SupportsPipeline, step: TPipelineStep, exception: BaseException, step_info: Any = None) -> None:
         self.pipeline = pipeline
         self.step = step
         self.exception = exception
-        self.run_metrics = run_metrics
         self.step_info = step_info
         super().__init__(pipeline.pipeline_name, f"Pipeline execution failed at stage {step} with exception:\n\n{type(exception)}\n{exception}")
 
 
 class PipelineStateEngineNoUpgradePathException(PipelineException):
     def __init__(self, pipeline_name: str, init_engine: int, from_engine: int, to_engine: int) -> None:
         self.init_engine = init_engine
         self.from_engine = from_engine
         self.to_engine = to_engine
         super().__init__(pipeline_name, f"No engine upgrade path for state in pipeline {pipeline_name} from {init_engine} to {to_engine}, stopped at {from_engine}")
+
+
+class PipelineHasPendingDataException(PipelineException):
+    def __init__(self, pipeline_name: str, pipelines_dir: str) -> None:
+        msg = (
+            f" Operation failed because pipeline with name {pipeline_name} in working directory {pipelines_dir} contains pending extracted files or load packages. "
+            "Use `dlt pipeline sync` to reset the local state then run this operation again."
+        )
+        super().__init__(pipeline_name, msg)
```

### Comparing `dlt-0.2.6a0/dlt/pipeline/pipeline.py` & `dlt-0.2.6a1/dlt/pipeline/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import contextlib
 import os
 import datetime  # noqa: 251
 from contextlib import contextmanager
 from functools import wraps
 from collections.abc import Sequence as C_Sequence
-from typing import Any, Callable, ClassVar, Dict, List, Iterator, Mapping, Optional, Sequence, Tuple, cast, get_type_hints, ContextManager
+from typing import Any, Callable, ClassVar, List, Iterator, Mapping, Optional, Sequence, Tuple, cast, get_type_hints, ContextManager
 
 from dlt import version
 from dlt.common import json, logger, pendulum
 from dlt.common.configuration import inject_section, known_sections
 from dlt.common.configuration.specs import RunConfiguration, NormalizeVolumeConfiguration, SchemaVolumeConfiguration, LoadVolumeConfiguration
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ConfigFieldMissingException, ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.normalizers import default_normalizers, import_normalizers
-from dlt.common.runners.runnable import Runnable
-from dlt.common.runtime import signals
+from dlt.common.runtime import signals, initialize_runtime
 from dlt.common.schema.exceptions import InvalidDatasetName
 from dlt.common.schema.typing import TColumnSchema, TSchemaTables, TWriteDisposition
 from dlt.common.storages.load_storage import LoadJobInfo, LoadPackageInfo, LoadStorage
 from dlt.common.typing import TFun, TSecretValue
-from dlt.common.runners import pool_runner as runner, initialize_runner
-from dlt.common.runners.configuration import PoolRunnerConfiguration
-from dlt.common.storages import LiveSchemaStorage, NormalizeStorage
+from dlt.common.runners import pool_runner as runner
+from dlt.common.storages import LiveSchemaStorage, NormalizeStorage, SchemaStorage
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import DestinationReference, JobClientBase, DestinationClientConfiguration, DestinationClientDwhConfiguration, TDestinationReferenceArg
 from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
 from dlt.common.schema import Schema
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.utils import is_interactive
 
@@ -41,28 +39,29 @@
 from dlt.normalize.configuration import NormalizeConfiguration
 from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.load.configuration import LoaderConfiguration
 from dlt.load import Load
 
 from dlt.pipeline.configuration import PipelineConfiguration
+from dlt.pipeline.progress import _Collector, _NULL_COLLECTOR
 from dlt.pipeline.exceptions import CannotRestorePipelineException, InvalidPipelineName, PipelineConfigMissing, PipelineStepFailed, SqlClientNotAvailable
 from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace, load_trace, merge_traces, start_trace, start_trace_step, end_trace_step, end_trace
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline.state_sync import STATE_ENGINE_VERSION, load_state_from_destination, merge_state_if_changed, migrate_state, state_resource, json_encode_state, json_decode_state
 
 
 def with_state_sync(may_extract_state: bool = False) -> Callable[[TFun], TFun]:
 
     def decorator(f: TFun) -> TFun:
         @wraps(f)
         def _wrap(self: "Pipeline", *args: Any, **kwargs: Any) -> Any:
             # backup and restore state
             should_extract_state = may_extract_state and self.config.restore_from_destination
-            with self._managed_state(extract_state=should_extract_state) as state:
+            with self.managed_state(extract_state=should_extract_state) as state:
                 # add the state to container as a context
                 with self._container.injectable_context(StateInjectableContext(state=state)):
                     return f(self, *args, **kwargs)
 
         return _wrap  # type: ignore
 
     return decorator
@@ -164,55 +163,58 @@
     destination: DestinationReference = None
     """The destination reference which is ModuleType. `destination.__name__` returns the name string"""
     dataset_name: str = None
     """Name of the dataset to which pipeline will be loaded to"""
     credentials: Any = None
     is_active: bool = False
     """Tells if instance is currently active and available via dlt.pipeline()"""
+    collector: _Collector
     config: PipelineConfiguration
     runtime_config: RunConfiguration
 
     def __init__(
             self,
             pipeline_name: str,
             pipelines_dir: str,
             pipeline_salt: TSecretValue,
             destination: DestinationReference,
             dataset_name: str,
             credentials: Any,
             import_schema_path: str,
             export_schema_path: str,
             full_refresh: bool,
+            progress: _Collector,
             must_attach_to_local_pipeline: bool,
             config: PipelineConfiguration,
             runtime: RunConfiguration
         ) -> None:
         """Initializes the Pipeline class which implements `dlt` pipeline. Please use `pipeline` function in `dlt` module to create a new Pipeline instance."""
 
         self.pipeline_salt = pipeline_salt
         self.config = config
         self.runtime_config = runtime
         self.full_refresh = full_refresh
+        self.collector = progress or _NULL_COLLECTOR
 
         self._container = Container()
         self._pipeline_instance_id = self._create_pipeline_instance_id()
         self._pipeline_storage: FileStorage = None
         self._schema_storage: LiveSchemaStorage = None
         self._schema_storage_config: SchemaVolumeConfiguration = None
         self._normalize_storage_config: NormalizeVolumeConfiguration = None
         self._load_storage_config: LoadVolumeConfiguration = None
         self._trace: PipelineTrace = None
         self._last_trace: PipelineTrace = None
         self._state_restored: bool = False
 
-        initialize_runner(self.runtime_config)
+        initialize_runtime(self.runtime_config)
         # initialize pipeline working dir
         self._init_working_dir(pipeline_name, pipelines_dir)
 
-        with self._managed_state() as state:
+        with self.managed_state() as state:
             # set the pipeline properties from state
             self._state_to_props(state)
             # we overwrite the state with the values from init
             self._set_destination(destination)  # changing the destination could be dangerous if pipeline has not loaded items
             self._set_dataset_name(dataset_name)
             self.credentials = credentials
             self._configure(import_schema_path, export_schema_path, must_attach_to_local_pipeline)
@@ -228,14 +230,15 @@
             self.pipeline_salt,
             self.destination,
             self.dataset_name,
             self.credentials,
             self._schema_storage.config.import_schema_path,
             self._schema_storage.config.export_schema_path,
             self.full_refresh,
+            self.collector,
             False,
             self.config,
             self.runtime_config
         )
 
     @with_runtime_trace
     @with_schemas_sync  # this must precede with_state_sync
@@ -271,15 +274,15 @@
                 # commit extract ids
                 # TODO: if we fail here we should probably wipe out the whole extract folder
                 for extract_id in extract_ids:
                     storage.commit_extract_files(extract_id)
                 return ExtractInfo()
         except Exception as exc:
             # TODO: provide metrics from extractor
-            raise PipelineStepFailed(self, "extract", exc, runner.LAST_RUN_METRICS, ExtractInfo()) from exc
+            raise PipelineStepFailed(self, "extract", exc, ExtractInfo()) from exc
 
     @with_runtime_trace
     @with_schemas_sync
     @with_config_section((known_sections.NORMALIZE,))
     def normalize(self, workers: int = 1) -> NormalizeInfo:
         """Normalizes the data prepared with `extract` method, infers the schema and creates load packages for the `load` method. Requires `destination` to be known."""
         if is_interactive() and workers > 1:
@@ -288,32 +291,30 @@
         if not self.default_schema_name:
             return None
 
         # make sure destination capabilities are available
         self._get_destination_capabilities()
         # create default normalize config
         normalize_config = NormalizeConfiguration(
-            is_single_run=True,
-            exit_on_exception=True,
             workers=workers,
             pool_type="none" if workers == 1 else "process",
             _schema_storage_config=self._schema_storage_config,
             _normalize_storage_config=self._normalize_storage_config,
             _load_storage_config=self._load_storage_config
         )
         # run with destination context
         with self._maybe_destination_capabilities():
             # shares schema storage with the pipeline so we do not need to install
-            normalize = Normalize(config=normalize_config, schema_storage=self._schema_storage)
+            normalize = Normalize(collector=self.collector, config=normalize_config, schema_storage=self._schema_storage)
             try:
-                self._run_step_in_pool("normalize", normalize, normalize.config)
+                with signals.delayed_signals():
+                    runner.run_pool(normalize.config, normalize)
                 return NormalizeInfo()
-            except PipelineStepFailed as pip_ex:
-                pip_ex.step_info = NormalizeInfo()
-                raise
+            except Exception as n_ex:
+                raise PipelineStepFailed(self, "normalize", n_ex, Normalize()) from n_ex
 
     @with_runtime_trace
     @with_schemas_sync
     @with_state_sync()
     @with_config_section((known_sections.LOAD,))
     def load(
         self,
@@ -334,31 +335,29 @@
         # check if any schema is present, if not then no data was extracted
         if not self.default_schema_name:
             return None
 
         # make sure that destination is set and client is importable and can be instantiated
         client = self._get_destination_client(self.default_schema)
 
-        # create initial loader config and the loader
+        # create default loader config and the loader
         load_config = LoaderConfiguration(
-            is_single_run=True,
-            exit_on_exception=True,
             workers=workers,
             raise_on_failed_jobs=raise_on_failed_jobs,
             _load_storage_config=self._load_storage_config
         )
-        load = Load(self.destination, is_storage_owner=False, config=load_config, initial_client_config=client.config)
+        load = Load(self.destination, collector=self.collector, is_storage_owner=False, config=load_config, initial_client_config=client.config)
         try:
-            self._run_step_in_pool("load", load, load.config)
+            with signals.delayed_signals():
+                runner.run_pool(load.config, load)
             info = self._get_load_info(load)
             self.first_run = False
             return info
-        except PipelineStepFailed as pipex:
-            pipex.step_info = self._get_load_info(load)
-            raise
+        except Exception as l_ex:
+            raise PipelineStepFailed(self, "load", l_ex, self._get_load_info(load)) from l_ex
 
     @with_runtime_trace
     @with_config_section(("run",))
     def run(
         self,
         data: Any = None,
         *,
@@ -538,15 +537,20 @@
 
     @property
     def has_data(self) -> bool:
         """Tells if the pipeline contains any data: schemas, extracted files, load packages or loaded packages in the destination"""
         return not self.first_run or bool(self.schema_names) or len(self.list_extracted_resources()) > 0 or len(self.list_normalized_load_packages()) > 0
 
     @property
-    def schemas(self) -> Mapping[str, Schema]:
+    def has_pending_data(self) -> bool:
+        """Tells if the pipeline contains any extracted files or pending load packages"""
+        return bool(self.list_normalized_load_packages() or self.list_extracted_resources())
+
+    @property
+    def schemas(self) -> SchemaStorage:
         return self._schema_storage
 
     @property
     def default_schema(self) -> Schema:
         return self.schemas[self.default_schema_name]
 
     @property
@@ -769,17 +773,15 @@
 
         return sources
 
     def _extract_source(self, storage: ExtractorStorage, source: DltSource, max_parallel_items: int, workers: int) -> str:
         # discover the schema from source
         source_schema = source.schema
 
-        # make CTRL-C working while running user code
-        with signals.raise_immediately():
-            extract_id = extract_with_schema(storage, source, source_schema, max_parallel_items, workers)
+        extract_id = extract_with_schema(storage, source, source_schema, self.collector, max_parallel_items, workers)
 
         # if source schema does not exist in the pipeline
         if source_schema.name not in self._schema_storage:
             # save schema into the pipeline
             self._schema_storage.save_schema(source_schema)
 
         # and set as default if this is first schema in pipeline
@@ -795,49 +797,14 @@
         # get the current schema and merge tables from source_schema
         # note we are not merging props like max nesting or column propagation
         for table in source_schema.data_tables():
             pipeline_schema.update_schema(pipeline_schema.normalize_table_identifiers(table))
 
         return extract_id
 
-    def _run_step_in_pool(self, step: TPipelineStep, runnable: Runnable[Any], config: PoolRunnerConfiguration) -> int:
-        # TODO: remove runner altogether. it does not fit into current architecture
-        try:
-            ec = runner.run_pool(config, runnable)
-            # in any other case we raise if runner exited with status failed
-            if runner.LAST_RUN_METRICS.has_failed:
-                raise PipelineStepFailed(self, step, runner.LAST_RUN_EXCEPTION, runner.LAST_RUN_METRICS)
-            return ec
-        except Exception as r_ex:
-            # if EXIT_ON_EXCEPTION flag is set, exception will bubble up directly
-            raise PipelineStepFailed(self, step, runner.LAST_RUN_EXCEPTION, runner.LAST_RUN_METRICS) from r_ex
-        # finally:
-        #     signals.raise_if_signalled()
-
-    # def _run_f_in_pool(self, run_f: Callable[..., Any], config: PoolRunnerConfiguration) -> int:
-
-    #     def _run(_: Any) -> TRunMetrics:
-    #         rv = run_f()
-    #         if isinstance(rv, TRunMetrics):
-    #             return rv
-    #         if isinstance(rv, int):
-    #             pending = rv
-    #         else:
-    #             pending = 1
-    #         return TRunMetrics(False, False, int(pending))
-
-    #     # run the fun
-    #     ec = runner.run_pool(config, _run)
-    #     # ec > 0 - signalled
-    #     # -1 - runner was not able to start
-
-    #     if runner.LAST_RUN_METRICS is not None and runner.LAST_RUN_METRICS.has_failed:
-    #         raise runner.last_run_exception
-    #     return ec
-
     def _get_destination_client_initial_config(self, credentials: Any = None) -> DestinationClientConfiguration:
         if not self.destination:
             raise PipelineConfigMissing(
                 self.pipeline_name,
                 "destination",
                 "load",
                 "Please provide `destination` argument to `pipeline`, `run` or `load` method directly or via .dlt config.toml file or environment variable."
@@ -957,38 +924,18 @@
     def _inject_schema(self, schema: Schema) -> None:
         """Injects a schema into the pipeline. Existing schema will be overwritten"""
         self._schema_storage.save_schema(schema)
         if not self.default_schema_name:
             self._set_default_schema_name(schema)
 
     def _get_load_info(self, load: Load) -> LoadInfo:
-        # TODO: Load must provide a clear interface to get last loads and metrics
-        # TODO: LoadInfo should hold many datasets
-        load_ids = load._processed_load_ids
-        load_packages: List[LoadPackageInfo] = []
-        load_storage = self._get_load_storage()
-        for load_id in load_ids:
-            load_packages.append(load_storage.get_load_package_info(load_id))
-        dataset_name = None
-        if isinstance(load.initial_client_config, DestinationClientDwhConfiguration):
-            dataset_name = load.initial_client_config.dataset_name
         started_at: datetime.datetime = None
         if self._trace:
             started_at = self._trace.started_at
-
-        return LoadInfo(
-            self,
-            load.initial_client_config.destination_name,
-            str(load.initial_client_config.credentials),
-            dataset_name,
-            list(load_ids.keys()),
-            load_packages,
-            started_at,
-            self.first_run
-        )
+        return load.get_load_info(self, started_at)
 
     def _get_state(self) -> TPipelineState:
         try:
             state = json_decode_state(self._pipeline_storage.load(Pipeline.STATE_FILE))
             return migrate_state(self.pipeline_name, state, state["_state_engine_version"], STATE_ENGINE_VERSION)
         except FileNotFoundError:
             return {
@@ -1068,15 +1015,15 @@
                             self._schema_storage.load_schema(schema_name)
                     else:
                         logger.info(f"The schema {schema_name} was restored from the destination {self.destination.__name__}:{job_client.sql_client.dataset_name}")
                         restored_schemas.append(Schema.from_dict(json.loads(schema_info.schema)))
         return restored_schemas
 
     @contextmanager
-    def _managed_state(self, *, extract_state: bool = False) -> Iterator[TPipelineState]:
+    def managed_state(self, *, extract_state: bool = False) -> Iterator[TPipelineState]:
         # load or restore state
         state = self._get_state()
         # TODO: we should backup schemas here
         try:
             yield state
         except Exception:
             backup_state = self._get_state()
@@ -1143,14 +1090,14 @@
         self._pipeline_storage.save(Pipeline.STATE_FILE, json_encode_state(state))
 
     def _extract_state(self, state: TPipelineState) -> TPipelineState:
         # this will extract the state into current load package and update the schema with the _dlt_pipeline_state table
         # note: the schema will be persisted because the schema saving decorator is over the state manager decorator for extract
         state_source = DltSource("pipeline_state", self.pipeline_name, self.default_schema, [state_resource(state)])
         storage = ExtractorStorage(self._normalize_storage_config)
-        extract_id = extract_with_schema(storage, state_source, self.default_schema, 1, 1)
+        extract_id = extract_with_schema(storage, state_source, self.default_schema, _NULL_COLLECTOR, 1, 1)
         storage.commit_extract_files(extract_id)
         return state
 
     def __getstate__(self) -> Any:
         # pickle only the SupportsPipeline protocol fields
         return {"pipeline_name": self.pipeline_name}
```

### Comparing `dlt-0.2.6a0/dlt/pipeline/state_sync.py` & `dlt-0.2.6a1/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/pipeline/trace.py` & `dlt-0.2.6a1/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/pipeline/track.py` & `dlt-0.2.6a1/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/reflection/names.py` & `dlt-0.2.6a1/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/reflection/script_inspector.py` & `dlt-0.2.6a1/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/reflection/script_visitor.py` & `dlt-0.2.6a1/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/sources/helpers/requests/__init__.py` & `dlt-0.2.6a1/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/sources/helpers/requests/retry.py` & `dlt-0.2.6a1/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/sources/helpers/requests/session.py` & `dlt-0.2.6a1/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/sources/helpers/transform.py` & `dlt-0.2.6a1/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/dlt/version.py` & `dlt-0.2.6a1/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a0/pyproject.toml` & `dlt-0.2.6a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.2.6a0"
+version = "0.2.6a1"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -24,15 +24,14 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = ">=2.26.0"
 pendulum = ">=2.1.2"
 simplejson = ">=3.17.5"
 PyYAML = ">=5.4.1"
 json-logging = "1.4.1rc0"
-prometheus-client = ">=0.11.0"
 semver = ">=2.13.0"
 sentry-sdk = ">=1.4.3"
 hexbytes = ">=0.2.2"
 cachetools = ">=5.2.0"
 tzdata = ">=2022.1"
 tomlkit = ">=0.11.3"
 asyncstdlib = ">=3.10.5"
@@ -45,17 +44,19 @@
 setuptools = ">=65.6.0"
 humanize = ">=4.4.0"
 astunparse = ">=1.6.3"
 cron-descriptor = ">=1.2.32"
 pipdeptree = ">=2.3.3"
 gitpython = ">=3.1.29"
 pytz = ">=2022.6"
-tqdm = ">=4.64.1"
 giturlparse = ">=0.10.0"
 orjson = {version = "^3.8.6", markers="platform_python_implementation != 'PyPy'"}
+tenacity = "^8.2.2"
+jsonpath-ng = "^1.5.3"
+deprecated = "^1.2.13"
 
 psycopg2-binary = {version = ">=2.9.1", optional = true}
 # use this dependency as the current version of psycopg2cffi does not have sql module
 # psycopg2cffi = {git = "https://github.com/chtd/psycopg2cffi.git", optional = true, markers="platform_python_implementation == 'PyPy'"}
 psycopg2cffi = {version = ">=2.9.0", optional = true, markers="platform_python_implementation == 'PyPy'"}
 
 grpcio = {version = ">=1.50.0", optional = true}
@@ -64,17 +65,16 @@
 
 duckdb = {version = ">=0.6.1,<0.8.0", optional = true}
 
 dbt-core = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-redshift = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-bigquery = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-duckdb = {version = ">=1.3.0,<1.5.0", optional = true}
-tenacity = "^8.2.2"
-jsonpath-ng = "^1.5.3"
-deprecated = "^1.2.13"
+psutil = "^5.9.5"
+
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 mypy = "1.2.0"
 flake8 = "^5.0.0"
 bandit = "^1.7.0"
@@ -109,14 +109,17 @@
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.10.0"
 types-click = "^7.1.8"
 pandas = "^1.5.3"
 sqlfluff = "^1.4.5"
 google-auth-oauthlib = "^1.0.0"
 types-deprecated = "^1.2.9.2"
+tqdm = "^4.65.0"
+enlighten = "^1.11.2"
+alive-progress = "^3.1.1"
 
 [tool.poetry.group.airflow]
 optional = true
 
 [tool.poetry.group.airflow.dependencies]
 apache-airflow = "^2.5.3"
```

### Comparing `dlt-0.2.6a0/PKG-INFO` & `dlt-0.2.6a1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.2.6a0
+Version: 0.2.6a1
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -49,49 +49,62 @@
 Requires-Dist: json-logging (==1.4.1rc0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: makefun (>=1.15.0)
 Requires-Dist: orjson (>=3.8.6,<4.0.0); platform_python_implementation != "PyPy"
 Requires-Dist: pathvalidate (>=2.5.2)
 Requires-Dist: pendulum (>=2.1.2)
 Requires-Dist: pipdeptree (>=2.3.3)
-Requires-Dist: prometheus-client (>=0.11.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1); extra == "postgres" or extra == "redshift"
 Requires-Dist: psycopg2cffi (>=2.9.0); (platform_python_implementation == "PyPy") and (extra == "postgres" or extra == "redshift")
 Requires-Dist: pyarrow (>=8.0.0); extra == "gcp" or extra == "bigquery"
 Requires-Dist: pytz (>=2022.6)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: requirements-parser (>=0.5.0)
 Requires-Dist: semver (>=2.13.0)
 Requires-Dist: sentry-sdk (>=1.4.3)
 Requires-Dist: setuptools (>=65.6.0)
 Requires-Dist: simplejson (>=3.17.5)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tomlkit (>=0.11.3)
-Requires-Dist: tqdm (>=4.64.1)
 Requires-Dist: typing-extensions (>=4.0.0)
 Requires-Dist: tzdata (>=2022.1)
 Project-URL: Repository, https://github.com/dlt-hub/dlt
 Description-Content-Type: text/markdown
 
-![](https://github.com/dlt-hub/dlt/raw/devel/docs/DLT-Pacman-Big.gif)
-
+<h1 align="center">
+    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>
+</h1>
 <p align="center">
+Be it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.
+</p>
 
-[![PyPI version](https://badge.fury.io/py/dlt.svg)](https://pypi.org/project/dlt/)
-[![LINT Badge](https://github.com/dlt-hub/dlt/actions/workflows/lint.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/lint.yml)
-[![TEST COMMON Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_common.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_common.yml)
-[![TEST DESTINATIONS Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_destinations.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_destinations.yml)
-[![TEST BIGQUERY Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_destination_bigquery.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_destination_bigquery.yml)
-[![TEST DBT Badge](https://github.com/dlt-hub/dlt/actions/workflows/test_dbt_runner.yml/badge.svg)](https://github.com/dlt-hub/dlt/actions/workflows/test_dbt_runner.yml)
+<div align="center">
+  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">
+    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />
+  </a>
+  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">
+    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">
+  </a>
+  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">
+    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">
+  </a>
+</div>
 
-</p>
+## Installation
+
+dlt supports Python 3.8+.
 
-# data load tool (dlt)
+```bash
+pip install dlt
+```
+
+## Quick Start
 
-**[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**
+Load chess game data from chess.com API and save it in DuckDB:
 
 ```python
 import dlt
 from chess import chess # a utility function that grabs data from the chess.com API
 
 # create a dlt pipeline that will load chess game data to the DuckDB destination
 pipeline = dlt.pipeline(
@@ -103,101 +116,48 @@
 # use chess.com API to grab data about a few players
 data = chess(['magnuscarlsen', 'rpragchess'], start_month='2022/11', end_month='2022/12')
 
 # extract, normalize, and load the data
 pipeline.run(data)
 ```
 
-**data load tool (dlt)** is an open source Python library that makes data loading easy
-
-- Automatically turn the JSON returned by any API into a live dataset stored wherever you want it
-- `pip install dlt` and then include `import dlt` to use it in your Python loading script
-- The **dlt** library is licensed under the Apache License 2.0, so you can use it for free forever
-
-Read more about it on the [dlt Docs](https://dlthub.com/docs)
-
-# semantic versioning
-
-`dlt` will follow the semantic versioning with [`MAJOR.MINOR.PATCH`](https://peps.python.org/pep-0440/#semantic-versioning) pattern. Currently we do **pre-release versioning** with major version being 0.
-
-- `minor` version change means breaking changes
-- `patch` version change means new features that should be backward compatible
-- any suffix change ie. `a10` -> `a11` is a patch
-
-# development
-
-`dlt` uses `poetry` to manage, build and version the package. It also uses `make` to automate tasks. To start
-
-```sh
-make install-poetry  # will install poetry, to be run outside virtualenv
-```
-
-then
+Try it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**
 
-```sh
-make dev  # will install all deps including dev
-```
-
-Executing `poetry shell` and working in it is very convenient at this moment.
-
-## python version
-
-Use python 3.8 for development which is the lowest supported version for `dlt`. You'll need `distutils` and `venv`:
-
-```shell
-sudo apt-get install python3.8
-sudo apt-get install python3.8-distutils
-sudo apt install python3.8-venv
-```
-
-You may also use `pyenv` as [poetry](https://python-poetry.org/docs/managing-environments/) suggests.
-
-## bumping version
+## Features
 
-Please use `poetry version prerelease` to bump patch and then `make build-library` to apply changes. The source of the version is `pyproject.toml` and we use poetry to manage it.
+- **Automatic Schema:** Data structure inspection and schema creation for the destination.
+- **Data Normalization:** Consistent and verified data before loading.
+- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.
+- **Scalable:** Adapts to growing data needs in production.
+- **Easy Maintenance:** Clear data pipeline structure for updates.
+- **Rapid Exploration:** Quickly explore and gain insights from new data sources.
+- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.
+- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.
+- **Incremental Loading:** Load only new or changed data and avoid loading old records again.
+- **Open Source:** Free and Apache 2.0 Licensed.
 
-## testing and linting
+## Ready to use Pipelines and Destinations
 
-`dlt` uses `mypy` and `flake8` with several plugins for linting. We do not reorder imports or reformat code.
+Explore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
 
-`pytest` is used as test harness. `make test-common` will run tests of common components and does not require any external resources.
+## Documentation
 
-### testing destinations
+For detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).
 
-To test destinations use `make test`. You will need following external resources
+## Examples
 
-1. `BigQuery` project
-2. `Redshift` cluster
-3. `Postgres` instance. You can find a docker compose for postgres instance [here](tests/load/postgres/docker-compose.yml). When run the instance is configured to work with the tests.
+You can find examples for various use cases in the [examples](docs/examples) folder.
 
-```shell
-cd tests/load/postgres/
-docker-compose up --build -d
-```
-
-See `tests/.example.env` for the expected environment variables and command line example to run the tests. Then create `tests/.env` from it. You configure the tests as you would configure the dlt pipeline.
-We'll provide you with access to the resources above if you wish to test locally.
-
-To test local destinations (`duckdb` and `postgres`) run `make test-local`. You can run this tests without additional credentials (just copy `.example.env` into `.env`)
-
-## publishing
-
-1. Make sure that you are on `devel` branch and you have the newest code that passed all tests on CI.
-2. Verify the current version with `poetry version`
-3. You'll need `pypi` access token and use `poetry config pypi-token.pypi your-api-token` then
-
-```
-make publish-library
-```
+## Get Involved
 
-4. Make a release on github, use version and git tag as release name
+The dlt project is quickly growing, and we're excited to have you join our community! Here's how you can get involved:
 
-## contributing
+- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)
+- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.
+- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.
+- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.
+- **Improve documentation**: Help us enhance the dlt documentation.
 
-To contribute via pull request:
+## License
 
-1. Create an issue with your idea for a feature etc.
-2. Write your code and tests
-3. Lint your code with `make lint`. Test the common modules with `make test-common`
-4. If you work on a destination code then contact us to get access to test destinations
-5. Create a pull request
+DLT is released under the [Apache 2.0 License](LICENSE.txt).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

