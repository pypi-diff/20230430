# Comparing `tmp/qwak_core-0.0.36.tar.gz` & `tmp/qwak_core-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.36.tar", max compression
+gzip compressed data, was "qwak_core-0.0.37.tar", max compression
```

## Comparing `qwak_core-0.0.36.tar` & `qwak_core-0.0.37.tar`

### file list

```diff
@@ -1,535 +1,543 @@
--rw-r--r--   0        0        0      264 2023-04-27 13:49:23.740425 qwak_core-0.0.36/README.md
--rw-r--r--   0        0        0        0 2023-04-27 13:50:26.540478 qwak_core-0.0.36/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-04-27 13:50:26.564478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-04-27 13:50:07.536461 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.564478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-04-27 13:50:26.560478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-04-27 13:50:07.192461 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.560478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-04-27 13:50:26.560478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-04-27 13:50:07.364462 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.564478 qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-04-27 13:50:26.552478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-04-27 13:50:06.680461 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-04-27 13:50:26.556478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-27 13:50:26.556478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-04-27 13:50:06.852461 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.556478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-04-27 13:50:26.556478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-04-27 13:50:07.024461 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.560478 qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-04-27 13:50:26.540478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-04-27 13:50:06.508461 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-04-27 13:50:26.540478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-04-27 13:50:26.544478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-04-27 13:50:07.708462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.544478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-04-27 13:50:26.548478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-04-27 13:50:08.048462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.548478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-04-27 13:50:26.548478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-04-27 13:50:08.224462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-04-27 13:50:26.552478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-04-27 13:50:26.544478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-04-27 13:50:07.876462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.544478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-04-27 13:50:26.552478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-04-27 13:50:08.396462 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.552478 qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-04-27 13:50:26.592478 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-04-27 13:50:10.864464 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.596478 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-04-27 13:50:26.596478 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-04-27 13:50:11.064464 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-04-27 13:50:26.596478 qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-04-27 13:50:26.668478 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-04-27 13:50:15.828469 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.672478 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-04-27 13:50:26.672478 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-04-27 13:50:16.004469 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-04-27 13:50:26.672478 qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-04-27 13:50:26.676478 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-04-27 13:50:16.880469 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-04-27 13:50:26.676478 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-04-27 13:50:26.676478 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-04-27 13:50:16.708469 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.676478 qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-04-27 13:50:26.680478 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-04-27 13:50:17.056470 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.680478 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-04-27 13:50:26.680478 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-04-27 13:50:17.228470 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-04-27 13:50:26.680478 qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-04-27 13:50:26.740478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-04-27 13:50:22.216474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.744478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-04-27 13:50:26.736478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-04-27 13:50:21.860474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.740478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-04-27 13:50:26.740478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-04-27 13:50:22.040474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.740478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-04-27 13:50:26.732478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-04-27 13:50:21.508473 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-04-27 13:50:26.736478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-04-27 13:50:26.736478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-04-27 13:50:21.684474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.736478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-04-27 13:50:26.748478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-04-27 13:50:22.740475 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.752478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-04-27 13:50:26.748478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-04-27 13:50:22.568474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.748478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-04-27 13:50:26.744478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-04-27 13:50:22.392474 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.744478 qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-04-27 13:50:26.788478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-04-27 13:50:25.912477 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.788478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-04-27 13:50:26.784478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-04-27 13:50:25.548477 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.784478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-04-27 13:50:26.788478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-04-27 13:50:25.732477 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-04-27 13:50:26.788478 qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-04-27 13:50:26.708478 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-04-27 13:50:19.012471 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-04-27 13:50:26.708478 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-04-27 13:50:26.704478 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-04-27 13:50:18.836471 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.708478 qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-04-27 13:50:26.696478 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-04-27 13:50:18.484471 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.696478 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-04-27 13:50:26.700478 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-04-27 13:50:18.656471 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.700478 qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-04-27 13:50:26.700478 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-04-27 13:50:19.188471 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-04-27 13:50:26.700478 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-04-27 13:50:26.704478 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-04-27 13:50:19.568472 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-04-27 13:50:26.704478 qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-04-27 13:50:26.712478 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-04-27 13:50:19.936472 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.716478 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-04-27 13:50:26.716478 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-27 13:50:20.108472 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-27 13:50:26.716478 qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-04-27 13:50:26.688478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-04-27 13:50:17.960470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.692478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-04-27 13:50:26.692478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-04-27 13:50:18.132470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-04-27 13:50:26.692478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-04-27 13:50:26.684478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-04-27 13:50:17.600470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.688478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-04-27 13:50:26.684478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-04-27 13:50:17.416470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.684478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-04-27 13:50:26.688478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-04-27 13:50:17.784470 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-04-27 13:50:26.688478 qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-04-27 13:50:26.584478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-04-27 13:50:09.976464 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.584478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-27 13:50:26.584478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-04-27 13:50:10.152464 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.588478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-04-27 13:50:26.588478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-04-27 13:50:10.328464 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-04-27 13:50:26.588478 qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-04-27 13:50:26.652478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-04-27 13:50:14.784468 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.652478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-04-27 13:50:26.648478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-04-27 13:50:14.612468 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-04-27 13:50:26.648478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-04-27 13:50:26.632478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-04-27 13:50:13.212466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.632478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-04-27 13:50:26.628478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-04-27 13:50:13.040466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.632478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-04-27 13:50:26.624478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-04-27 13:50:12.496466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.624478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-04-27 13:50:26.628478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-04-27 13:50:12.868466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-04-27 13:50:26.628478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-04-27 13:50:26.632478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-04-27 13:50:13.388466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.636478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-04-27 13:50:26.636478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-04-27 13:50:13.564467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-04-27 13:50:26.636478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-04-27 13:50:26.624478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-04-27 13:50:12.684466 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.624478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-04-27 13:50:26.636478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-04-27 13:50:13.736467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.640478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-04-27 13:50:26.652478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-04-27 13:50:26.092477 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.652478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-04-27 13:50:26.656478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-04-27 13:50:26.272477 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-04-27 13:50:26.656478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-04-27 13:50:26.656478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-04-27 13:50:15.308468 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.660478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-04-27 13:50:26.660478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-04-27 13:50:15.480468 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-04-27 13:50:26.660478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-04-27 13:50:26.660478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-04-27 13:50:15.652469 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.664478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-04-27 13:50:26.664478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-04-27 13:50:16.360469 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.668478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-04-27 13:50:26.664478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-04-27 13:50:16.180469 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-04-27 13:50:26.664478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-04-27 13:50:26.668478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-04-27 13:50:16.532469 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.668478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-04-27 13:50:26.640478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-04-27 13:50:13.916467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.640478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-04-27 13:50:26.640478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-04-27 13:50:14.088467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.644478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-04-27 13:50:26.644478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-04-27 13:50:14.264467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-04-27 13:50:26.644478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-04-27 13:50:26.648478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-04-27 13:50:14.440467 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.648478 qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-04-27 13:50:26.752478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-04-27 13:50:22.912475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.752478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-04-27 13:50:26.752478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-04-27 13:50:23.084475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-27 13:50:26.756478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-04-27 13:50:26.756478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-04-27 13:50:23.256475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.756478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-04-27 13:50:26.756478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-04-27 13:50:23.436475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-27 13:50:26.760478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-04-27 13:50:26.760478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-04-27 13:50:23.616475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-04-27 13:50:26.760478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-04-27 13:50:26.760478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-04-27 13:50:23.788475 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.764478 qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-04-27 13:50:26.720478 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-04-27 13:50:20.280472 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.720478 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-04-27 13:50:26.720478 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-27 13:50:20.452473 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-27 13:50:26.720478 qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-04-27 13:50:26.604478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-04-27 13:50:11.776465 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.608478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-27 13:50:26.608478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-04-27 13:50:11.952465 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.612478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-04-27 13:50:26.612478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-04-27 13:50:12.128466 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-04-27 13:50:26.616478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-04-27 13:50:26.616478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-04-27 13:50:12.300466 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.620478 qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-04-27 13:50:26.692478 qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-04-27 13:50:18.304471 qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-04-27 13:50:26.696478 qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-04-27 13:50:26.764478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-04-27 13:50:23.964475 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.764478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-04-27 13:50:26.768478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-04-27 13:50:24.136476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.768478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-04-27 13:50:26.768478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-04-27 13:50:24.312476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.768478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-04-27 13:50:26.772478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-04-27 13:50:24.488476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.772478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-27 13:50:26.772478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-04-27 13:50:24.664476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.772478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-04-27 13:50:26.776478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-04-27 13:50:24.856476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-04-27 13:50:26.776478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-04-27 13:50:26.776478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-04-27 13:50:25.028476 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.780478 qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-04-27 13:50:26.724478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-04-27 13:50:20.800473 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.724478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-04-27 13:50:26.732478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-04-27 13:50:21.332473 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.732478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-04-27 13:50:26.728478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-04-27 13:50:20.980473 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-04-27 13:50:26.728478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-04-27 13:50:26.728478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-04-27 13:50:21.156473 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.728478 qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-04-27 13:50:26.712478 qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-04-27 13:50:19.760472 qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-04-27 13:50:26.712478 qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-04-27 13:50:26.580478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-04-27 13:50:11.424465 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-04-27 13:50:26.580478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-04-27 13:50:26.576478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-04-27 13:50:11.244465 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.576478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-04-27 13:50:26.580478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-04-27 13:50:11.604465 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-04-27 13:50:26.584478 qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-04-27 13:50:26.708478 qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-04-27 13:50:19.376472 qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-04-27 13:50:26.712478 qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-04-27 13:50:26.724478 qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-04-27 13:50:20.624473 qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-04-27 13:50:26.724478 qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-04-27 13:50:26.576478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-04-27 13:50:09.276463 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.576478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-04-27 13:50:26.572478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-04-27 13:50:09.100463 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-04-27 13:50:26.572478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-04-27 13:50:26.564478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-04-27 13:50:08.568462 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.568478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-04-27 13:50:26.568478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-04-27 13:50:08.744463 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.568478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-04-27 13:50:26.572478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-04-27 13:50:08.924463 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-04-27 13:50:26.572478 qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-04-27 13:50:26.780478 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-04-27 13:50:25.376477 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-04-27 13:50:26.784478 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-04-27 13:50:26.780478 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-04-27 13:50:25.204476 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.780478 qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-04-27 13:50:26.588478 qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-04-27 13:50:10.496464 qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.592478 qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3001 2023-04-27 13:50:26.592478 qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2574 2023-04-27 13:50:10.668464 qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-27 13:50:26.592478 qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     1906 2023-04-27 13:50:28.260479 qwak_core-0.0.36/pyproject.toml
--rw-r--r--   0        0        0      447 2023-04-27 13:50:28.260479 qwak_core-0.0.36/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5478 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0       77 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-04-27 13:49:23.744425 qwak_core-0.0.36/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4255 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     2585 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     2006 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2961 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1730 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     8808 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     5933 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      829 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/schema.py
--rw-r--r--   0        0        0     2964 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/schema_entities.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak/testing/fixtures.py
--rw-r--r--   0        0        0       46 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-04-27 13:49:23.748425 qwak_core-0.0.36/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5776 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-04-27 13:49:23.752425 qwak_core-0.0.36/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 qwak_core-0.0.36/setup.py
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-04-30 08:23:55.964205 qwak_core-0.0.37/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 08:25:06.992573 qwak_core-0.0.37/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-04-30 08:25:07.016573 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-04-30 08:24:46.848468 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.020573 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-04-30 08:25:07.012573 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-04-30 08:24:46.476466 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.016573 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-04-30 08:25:07.016573 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-04-30 08:24:46.660467 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.016573 qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-04-30 08:25:07.008573 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-04-30 08:24:45.920463 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-04-30 08:25:07.008573 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-30 08:25:07.008573 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-04-30 08:24:46.104464 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.008573 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-04-30 08:25:07.012573 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-04-30 08:24:46.292465 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.012573 qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-04-30 08:25:06.992573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-04-30 08:24:45.732462 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-04-30 08:25:06.996573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-04-30 08:25:06.996573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-04-30 08:24:47.036469 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:06.996573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-04-30 08:25:07.000573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-04-30 08:24:47.412471 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.000573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-04-30 08:25:07.004573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-04-30 08:24:47.604472 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-04-30 08:25:07.004573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-04-30 08:25:06.996573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-04-30 08:24:47.224470 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.000573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-04-30 08:25:07.004573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-04-30 08:24:47.792473 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.004573 qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-04-30 08:25:07.048573 qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-04-30 08:24:50.412487 qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.048573 qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-04-30 08:25:07.052573 qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-04-30 08:24:50.600488 qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-04-30 08:25:07.052573 qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-04-30 08:25:07.120573 qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-04-30 08:24:55.700514 qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.120573 qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-04-30 08:25:07.120573 qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-04-30 08:24:55.884515 qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-04-30 08:25:07.120573 qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-04-30 08:25:07.124573 qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-04-30 08:24:56.816520 qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-04-30 08:25:07.124573 qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-04-30 08:25:07.124573 qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-04-30 08:24:56.632519 qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.124573 qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-04-30 08:25:07.128574 qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-04-30 08:24:56.996521 qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.128574 qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-04-30 08:25:07.128574 qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-04-30 08:24:57.180522 qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-04-30 08:25:07.132573 qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-04-30 08:25:07.192574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-04-30 08:25:02.400549 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.192574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-04-30 08:25:07.188574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-04-30 08:25:02.028547 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.188574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-04-30 08:25:07.188574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-04-30 08:25:02.212548 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.192574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-04-30 08:25:07.184574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-04-30 08:25:01.656545 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-04-30 08:25:07.184574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-04-30 08:25:07.184574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-04-30 08:25:01.844546 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.188574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-04-30 08:25:07.200574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-04-30 08:25:02.952552 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.200574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-04-30 08:25:07.196574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-04-30 08:25:02.768551 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.196574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-04-30 08:25:07.192574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-04-30 08:25:02.584550 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.196574 qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-04-30 08:25:07.240574 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-04-30 08:25:06.340569 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.240574 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-04-30 08:25:07.232574 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-04-30 08:25:05.956567 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.236574 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-04-30 08:25:07.236574 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-04-30 08:25:06.156568 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-04-30 08:25:07.236574 qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-04-30 08:25:07.156574 qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-04-30 08:24:59.056532 qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-04-30 08:25:07.156574 qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-04-30 08:25:07.156574 qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-04-30 08:24:58.872531 qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.156574 qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-04-30 08:25:07.144574 qwak_core-0.0.37/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-04-30 08:24:58.500529 qwak_core-0.0.37/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.148573 qwak_core-0.0.37/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-04-30 08:25:07.148573 qwak_core-0.0.37/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-04-30 08:24:58.684530 qwak_core-0.0.37/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.148573 qwak_core-0.0.37/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-04-30 08:25:07.148573 qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-04-30 08:24:59.240532 qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-04-30 08:25:07.152573 qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-04-30 08:25:07.152573 qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-04-30 08:24:59.636535 qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-04-30 08:25:07.152573 qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-04-30 08:25:07.164574 qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-04-30 08:25:00.016537 qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.164574 qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-04-30 08:25:07.164574 qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-30 08:25:00.196537 qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-30 08:25:07.168574 qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-04-30 08:25:07.140574 qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-04-30 08:24:57.944526 qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.140574 qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-04-30 08:25:07.140574 qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-04-30 08:24:58.128527 qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-04-30 08:25:07.140574 qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-04-30 08:25:07.132573 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-04-30 08:24:57.564524 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.136573 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-04-30 08:25:07.132573 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-04-30 08:24:57.376523 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.132573 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-04-30 08:25:07.136573 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-04-30 08:24:57.756525 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-04-30 08:25:07.136573 qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-04-30 08:25:07.036573 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-04-30 08:24:49.472482 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.040573 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-30 08:25:07.040573 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-04-30 08:24:49.660483 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.040573 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-04-30 08:25:07.044573 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-04-30 08:24:49.848484 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-04-30 08:25:07.044573 qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-04-30 08:25:07.100573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-04-30 08:24:54.592508 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.100573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-04-30 08:25:07.096573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-04-30 08:24:54.408507 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-04-30 08:25:07.096573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-04-30 08:25:07.080573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-04-30 08:24:52.912500 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.080573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-04-30 08:25:07.076573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-04-30 08:24:52.728499 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.076573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-04-30 08:25:07.068573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-04-30 08:24:52.144496 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.072573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-04-30 08:25:07.072573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-04-30 08:24:52.540498 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-04-30 08:25:07.076573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-04-30 08:25:07.080573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-04-30 08:24:53.100501 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.080573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-04-30 08:25:07.084573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-04-30 08:24:53.284502 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-04-30 08:25:07.084573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-04-30 08:25:07.072573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-04-30 08:24:52.344497 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.072573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-04-30 08:25:07.084573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-04-30 08:24:53.468502 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.088573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-04-30 08:25:07.100573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-04-30 08:25:06.532570 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.100573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-04-30 08:25:07.104573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-04-30 08:25:06.720571 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-04-30 08:25:07.104573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-04-30 08:25:07.104573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-04-30 08:24:55.148511 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.108573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-04-30 08:25:07.108573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-04-30 08:24:55.332512 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-04-30 08:25:07.108573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-04-30 08:25:07.108573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-04-30 08:24:55.516513 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.112573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-04-30 08:25:07.112573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-04-30 08:24:56.264517 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.116573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-04-30 08:25:07.112573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-04-30 08:24:56.072516 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-04-30 08:25:07.112573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-04-30 08:25:07.116573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-04-30 08:24:56.448518 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.116573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-04-30 08:25:07.088573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-04-30 08:24:53.656504 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.088573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-04-30 08:25:07.088573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-04-30 08:24:53.848504 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.092573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-04-30 08:25:07.092573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-04-30 08:24:54.036506 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-04-30 08:25:07.092573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-04-30 08:25:07.096573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-04-30 08:24:54.224506 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.096573 qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-04-30 08:25:07.200574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-04-30 08:25:03.136553 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.200574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-04-30 08:25:07.204574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-04-30 08:25:03.320554 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-30 08:25:07.204574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-04-30 08:25:07.204574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-04-30 08:25:03.508555 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.204574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-04-30 08:25:07.208574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-04-30 08:25:03.700556 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-30 08:25:07.208574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-04-30 08:25:07.208574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-04-30 08:25:03.896557 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-04-30 08:25:07.212574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-04-30 08:25:07.212574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-04-30 08:25:04.080558 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.212574 qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-04-30 08:25:07.168574 qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-04-30 08:25:00.376538 qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.168574 qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-04-30 08:25:07.168574 qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-30 08:25:00.556539 qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-30 08:25:07.172574 qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-04-30 08:25:07.056573 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-04-30 08:24:51.376492 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.056573 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-30 08:25:07.060573 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-04-30 08:24:51.564493 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.060573 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-04-30 08:25:07.064573 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-04-30 08:24:51.764494 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-04-30 08:25:07.064573 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-04-30 08:25:07.068573 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-04-30 08:24:51.952495 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.068573 qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-04-30 08:25:07.144574 qwak_core-0.0.37/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-04-30 08:24:58.312528 qwak_core-0.0.37/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-04-30 08:25:07.144574 qwak_core-0.0.37/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-04-30 08:25:07.212574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-04-30 08:25:04.268559 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.216574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-04-30 08:25:07.216574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-04-30 08:25:04.452560 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.216574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-04-30 08:25:07.216574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-04-30 08:25:04.640560 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.220574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-04-30 08:25:07.220574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-04-30 08:25:04.828561 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.220574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-30 08:25:07.224574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-04-30 08:25:05.016563 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.224574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-04-30 08:25:07.224574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-04-30 08:25:05.220564 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-04-30 08:25:07.228574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-04-30 08:25:07.228574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-04-30 08:25:05.404564 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.228574 qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-04-30 08:25:07.176574 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-04-30 08:25:00.916541 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.176574 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-04-30 08:25:07.180574 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-04-30 08:25:01.468544 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.180574 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-04-30 08:25:07.176574 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-04-30 08:25:01.100542 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-04-30 08:25:07.176574 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-04-30 08:25:07.180574 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-04-30 08:25:01.284543 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.180574 qwak_core-0.0.37/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-04-30 08:25:07.160574 qwak_core-0.0.37/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-04-30 08:24:59.832536 qwak_core-0.0.37/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-04-30 08:25:07.164574 qwak_core-0.0.37/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-04-30 08:25:07.032573 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-04-30 08:24:50.996490 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-04-30 08:25:07.036573 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-04-30 08:25:07.032573 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-04-30 08:24:50.788488 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.032573 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-04-30 08:25:07.036573 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-04-30 08:24:51.184491 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-04-30 08:25:07.036573 qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-04-30 08:25:07.160574 qwak_core-0.0.37/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-04-30 08:24:59.432533 qwak_core-0.0.37/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-04-30 08:25:07.160574 qwak_core-0.0.37/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-04-30 08:25:07.172574 qwak_core-0.0.37/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-04-30 08:25:00.732540 qwak_core-0.0.37/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-04-30 08:25:07.172574 qwak_core-0.0.37/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-04-30 08:25:07.028573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-04-30 08:24:48.724478 qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.028573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-04-30 08:25:07.028573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-04-30 08:24:48.540477 qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-04-30 08:25:07.028573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-04-30 08:25:07.020573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-04-30 08:24:47.976474 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.020573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-04-30 08:25:07.020573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-04-30 08:24:48.164475 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.024573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-04-30 08:25:07.024573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-04-30 08:24:48.352476 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-04-30 08:25:07.024573 qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-04-30 08:25:07.232574 qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-04-30 08:25:05.776566 qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-04-30 08:25:07.232574 qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-04-30 08:25:07.228574 qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-04-30 08:25:05.592565 qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.232574 qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-04-30 08:25:07.044573 qwak_core-0.0.37/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-04-30 08:24:50.040485 qwak_core-0.0.37/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.044573 qwak_core-0.0.37/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3001 2023-04-30 08:25:07.048573 qwak_core-0.0.37/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2574 2023-04-30 08:24:50.224486 qwak_core-0.0.37/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-30 08:25:07.048573 qwak_core-0.0.37/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2485 2023-04-30 08:25:08.844582 qwak_core-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-04-30 08:25:08.844582 qwak_core-0.0.37/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0       77 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4255 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     2585 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1201 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-04-30 08:23:55.964205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     2006 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2961 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1730 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    27897 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     8808 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     6127 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      829 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/schema.py
+-rw-r--r--   0        0        0     2964 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0       46 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-04-30 08:23:55.968205 qwak_core-0.0.37/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5776 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-30 08:23:55.972205 qwak_core-0.0.37/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 qwak_core-0.0.37/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.37/PKG-INFO
```

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.37/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.37/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/pyproject.toml` & `qwak_core-0.0.37/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.36"
+version = "0.0.37"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
-    {include = "qwak"},
-    {include = "_qwak_proto"},
-    {include = "qwak_services_mock"},
+    { include = "qwak" },
+    { include = "_qwak_proto" },
+    { include = "qwak_services_mock" },
 ]
 include = ["./qwak/**/*", "./_qwak_proto/**/*", "./qwak_services_mock/**/*"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -31,35 +31,42 @@
 protobuf = ">=3.10,<4"
 dependency-injector = ">=4.0"
 requests = "*"
 python-jose = "*"
 PyYAML = "*"
 marshmallow-dataclass = "^8.5.8"
 typeguard = "^2"
+pyarrow = { version = ">=6.0.0", optional = true }
+pyathena = { version = ">=2.2.0,!=2.18.0", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.2.2"
 black = "23.1.0"
 flake8 = "5.0.0"
-bandit = {version = "^1.7.5", extras=["toml"]}
+bandit = { version = "^1.7.5", extras = ["toml"] }
 coverage = "7.2.1"
-typing_extensions ="4.4.0"
+typing_extensions = "4.4.0"
 bump2version = "1.0.1"
 grpcio-tools = ">=1.47.0"
 mypy-protobuf = "^3.0.0"
 pytest-lazy-fixture = "^0.6.3"
 changelog-cli = "*"
-pandas = [ # Inference dependencies
-    {version="<1.4", python=">=3.7.1,<3.8"},
-    {version=">=1.4.3,<2.0.0", python=">=3.8,<3.10"}
+testcontainers = "^3.6.1"
+sqlalchemy = "==1.4.16"
+sqlalchemy-utils = "<=0.36.5,>=0.36.2"
+trino = "^0.319.0"
+pandas = [
+    { version = "<1.4", python = ">=3.7.1,<3.8" },
+    { version = ">=1.4.0", python = ">=3.8,<3.10" }
 ]
 
 
 [tool.poetry.extras]
+feature-store = ["pyarrow", "pyathena"]
 
 [tool.black]
 extend-exclude = '''
 (
      .*_pb2.py
     | .*_pb2_grpc.py
 )'''
@@ -70,10 +77,17 @@
 ]
 markers = [
     "integration: marks tests as slow (deselect with '-m \"not integration\"')",
 ]
 
 [tool.bandit]
 
+[tool.poe.tasks]
+generate = { cmd = "./scripts/gen-proto.sh" }
+clean = { cmd = "rm -rf dist ./**/__pycache__", help = "Clean build artifacts" }
+install = "poetry install"
+validate = { cmd = "pre-commit run  --all-files", help = "Check lint on all files" }
+test = { cmd = "pytest --disable-warnings tests", help = "Run tests" }
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qwak_core-0.0.36/qwak/automations/__init__.py` & `qwak_core-0.0.37/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/automations/automation_executions.py` & `qwak_core-0.0.37/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/automations/automations.py` & `qwak_core-0.0.37/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.37/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.37/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.37/qwak/clients/administration/eco_system/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Dict, List, Optional, Set
 
 import grpc
-from _qwak_proto.qwak.administration.v0.environments.configuration_pb2 import (
-    QwakEnvironmentConfiguration,
-)
 from _qwak_proto.qwak.ecosystem.v0.ecosystem_pb2 import (
+    EnvironmentDetails,
     UserContextAccountDetails,
     UserContextEnvironmentDetails,
 )
 from _qwak_proto.qwak.ecosystem.v0.ecosystem_runtime_service_pb2 import (
     GetAuthenticatedUserContextRequest,
     GetAuthenticatedUserContextResponse,
     GetCloudCredentialsRequest,
@@ -102,15 +100,15 @@
     def get_environments(self) -> Dict[str, UserContextEnvironmentDetails]:
         account = self.get_account_details()
 
         return account.environment_by_id
 
     def get_environment_configuration(
         self, environment_name: Optional[str] = None
-    ) -> QwakEnvironmentConfiguration:
+    ) -> EnvironmentDetails:
         account_details = self.get_account_details()
         if environment_name:
             matching_envs = self.get_envs_by_names(account_details, {environment_name})
             if not matching_envs:
                 available_environments_names = self.get_available_envs_names(
                     account_details
                 )
@@ -119,15 +117,15 @@
                     f"environments are: {', '.join(available_environments_names)}"
                 )
             return matching_envs[0].configuration
 
         else:
             return account_details.environment_by_id[
                 account_details.default_environment_id
-            ].configuration
+            ]
 
     def get_environment_model_api(self, environment_name: Optional[str] = None) -> str:
         return self.get_environment_configuration(environment_name).model_api_url
 
     @staticmethod
     def get_available_envs_names(
         account_details: UserContextAccountDetails,
```

### Comparing `qwak_core-0.0.36/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.37/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.37/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/alert_management/client.py` & `qwak_core-0.0.37/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/analytics/client.py` & `qwak_core-0.0.37/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/audience/client.py` & `qwak_core-0.0.37/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/automation_management/client.py` & `qwak_core-0.0.37/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.37/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.37/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.37/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.37/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/build_management/client.py` & `qwak_core-0.0.37/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.37/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.37/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/deployment/client.py` & `qwak_core-0.0.37/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.37/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.37/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.37/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.37/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.37/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/logging_client/client.py` & `qwak_core-0.0.37/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/model_management/client.py` & `qwak_core-0.0.37/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/project/client.py` & `qwak_core-0.0.37/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/secret_service/client.py` & `qwak_core-0.0.37/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.37/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.37/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.37/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.37/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.37/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.37/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.37/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.37/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.37/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.37/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.37/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/feature_store/online/client.py` & `qwak_core-0.0.37/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/const.py` & `qwak_core-0.0.37/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.37/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.37/qwak/inner/di_configuration/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,7 +176,14 @@
 
     def get_models_api(self):
         """
         Get the account Models API address
         :return: Models API address
         """
         return self._get_claims()[self.QWAK_MODELS_API]
+
+    def get_environment_id(self):
+        """
+        Get the account Models API address
+        :return: Models API address
+        """
+        return self._get_claims()[self.QWAK_PARTNER_ID]
```

### Comparing `qwak_core-0.0.36/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.37/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.37/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/singleton_meta.py` & `qwak_core-0.0.37/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/tool/auth.py` & `qwak_core-0.0.37/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.37/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.37/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.37/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.37/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/adapters/__init__.py` & `qwak_core-0.0.37/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.37/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.37/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.37/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.37/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.37/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/base.py` & `qwak_core-0.0.37/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/decorators/api.py` & `qwak_core-0.0.37/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.37/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/experiment_tracking.py` & `qwak_core-0.0.37/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/schema.py` & `qwak_core-0.0.37/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model/schema_entities.py` & `qwak_core-0.0.37/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.37/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.37/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.37/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.37/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.37/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.37/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/qwak_client/client.py` & `qwak_core-0.0.37/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.37/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/qwak_client/models/model.py` & `qwak_core-0.0.37/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.37/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.37/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.37/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/qwak_services_mock/services_mock.py` & `qwak_core-0.0.37/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.36/setup.py` & `qwak_core-0.0.37/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -69,18 +69,21 @@
  'qwak.clients.logging_client',
  'qwak.clients.model_management',
  'qwak.clients.project',
  'qwak.clients.secret_service',
  'qwak.clients.user_application_instance',
  'qwak.exceptions',
  'qwak.feature_store',
+ 'qwak.feature_store._common',
  'qwak.feature_store.data_sources',
  'qwak.feature_store.data_sources.batch_sources',
  'qwak.feature_store.entities',
  'qwak.feature_store.feature_sets',
+ 'qwak.feature_store.offline',
+ 'qwak.feature_store.offline.athena',
  'qwak.feature_store.online',
  'qwak.inner',
  'qwak.inner.di_configuration',
  'qwak.inner.runtime_di',
  'qwak.inner.tool',
  'qwak.inner.tool.grpc',
  'qwak.inner.tool.run_config',
@@ -112,25 +115,29 @@
  'grpcio>=1.32.0',
  'marshmallow-dataclass>=8.5.8,<9.0.0',
  'protobuf>=3.10,<4',
  'python-jose',
  'requests',
  'typeguard>=2,<3']
 
+extras_require = \
+{'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
+
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.36',
+    'version': '0.0.37',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.7.1,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `qwak_core-0.0.36/PKG-INFO` & `qwak_core-0.0.37/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.36
+Version: 0.0.37
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,19 +13,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Provides-Extra: feature-store
 Requires-Dist: PyYAML
 Requires-Dist: dependency-injector (>=4.0)
 Requires-Dist: grpcio (>=1.32.0)
 Requires-Dist: marshmallow-dataclass (>=8.5.8,<9.0.0)
 Requires-Dist: protobuf (>=3.10,<4)
+Requires-Dist: pyarrow (>=6.0.0) ; extra == "feature-store"
+Requires-Dist: pyathena (>=2.2.0,!=2.18.0) ; extra == "feature-store"
 Requires-Dist: python-jose
 Requires-Dist: requests
 Requires-Dist: typeguard (>=2,<3)
 Project-URL: Home page, https://www.qwak.com/
 Description-Content-Type: text/markdown
 
 # Qwak Core
```

