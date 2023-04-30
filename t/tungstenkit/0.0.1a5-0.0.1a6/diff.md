# Comparing `tmp/tungstenkit-0.0.1a5.tar.gz` & `tmp/tungstenkit-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tungstenkit-0.0.1a5.tar", max compression
+gzip compressed data, was "tungstenkit-0.0.1a6.tar", max compression
```

## Comparing `tungstenkit-0.0.1a5.tar` & `tungstenkit-0.0.1a6.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0     4086 2023-04-28 23:29:56.390539 tungstenkit-0.0.1a5/README.md
--rw-r--r--   0        0        0     3063 2023-04-28 23:31:19.538575 tungstenkit-0.0.1a5/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-11 17:07:01.860571 tungstenkit-0.0.1a5/tungstenkit/__init__.py
--rw-r--r--   0        0        0        0 2023-02-17 08:39:48.957419 tungstenkit-0.0.1a5/tungstenkit/_internal/__init__.py
--rw-r--r--   0        0        0       58 2023-02-17 08:39:48.957863 tungstenkit-0.0.1a5/tungstenkit/_internal/build/__init__.py
--rw-r--r--   0        0        0    13058 2023-04-28 23:27:15.780413 tungstenkit-0.0.1a5/tungstenkit/_internal/build/build_context.py
--rw-r--r--   0        0        0      223 2023-04-26 21:31:10.277468 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/__init__.py
--rw-r--r--   0        0        0     6665 2023-04-26 21:31:10.277684 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_dockerfile.py
--rw-r--r--   0        0        0      385 2023-02-17 08:39:48.959447 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/__init__.py
--rw-r--r--   0        0        0      483 2023-04-09 10:35:04.753993 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/base_image.py
--rw-r--r--   0        0        0      238 2023-02-17 08:39:48.959971 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/conda_image.py
--rw-r--r--   0        0        0     2552 2023-04-26 21:31:10.278022 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/cuda_image.py
--rw-r--r--   0        0        0      369 2023-02-17 08:39:48.960423 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/custom_image.py
--rw-r--r--   0        0        0     1622 2023-04-26 21:31:10.278341 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/python_image.py
--rw-r--r--   0        0        0      574 2023-04-09 10:35:04.754747 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/shared.py
--rw-r--r--   0        0        0      652 2023-04-26 21:31:10.278501 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/model_dockerfile.py
--rw-r--r--   0        0        0     7737 2023-04-26 21:31:10.278850 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/__init__.py
--rw-r--r--   0        0        0     1008 2023-04-09 10:35:04.755489 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/__init__.py
--rw-r--r--   0        0        0     3604 2023-03-30 23:07:07.733066 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/base_collection.py
--rw-r--r--   0        0        0     1593 2023-04-09 10:35:04.755732 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/common.py
--rw-r--r--   0        0        0     4315 2023-04-26 21:31:10.279190 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/tf_collection.py
--rw-r--r--   0        0        0     6509 2023-04-26 21:31:10.279501 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/torch_collection.py
--rw-r--r--   0        0        0      723 2023-02-17 08:39:48.962919 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/pip_requirement.py
--rw-r--r--   0        0        0      924 2023-04-09 10:35:04.756528 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/requirements_txt.py
--rw-r--r--   0        0        0      257 2023-04-26 21:31:10.279771 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/task_dockerfile_writer.py
--rw-r--r--   0        0        0     1373 2023-04-09 10:35:04.757025 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/template_args.py
--rw-r--r--   0        0        0      345 2023-02-17 08:39:48.964092 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/base.j2
--rw-r--r--   0        0        0      951 2023-02-17 08:39:48.964269 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/install_conda.j2
--rw-r--r--   0        0        0      834 2023-03-30 23:07:07.735005 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/install_python.j2
--rw-r--r--   0        0        0      824 2023-04-09 10:35:04.757393 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/setup_tungsten.j2
--rw-r--r--   0        0        0     1905 2023-04-09 10:35:04.757672 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/setup_user.j2
--rw-r--r--   0        0        0     1218 2023-04-28 23:31:24.056305 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/tungstenkit/pyproject.toml
--rw-r--r--   0        0        0     2152 2023-04-26 21:31:10.280640 tungstenkit-0.0.1a5/tungstenkit/_internal/build/model.py
--rw-r--r--   0        0        0        0 2023-02-17 08:39:48.966251 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/__init__.py
--rw-r--r--   0        0        0     2653 2023-04-26 21:31:10.280844 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/callbacks.py
--rw-r--r--   0        0        0     2280 2023-04-28 23:27:15.781189 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/login_command.py
--rw-r--r--   0        0        0     1428 2023-04-26 21:31:10.281426 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/main.py
--rw-r--r--   0        0        0    12392 2023-04-28 23:27:15.782080 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/model_commands.py
--rw-r--r--   0        0        0      653 2023-04-26 21:31:10.281918 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/options.py
--rw-r--r--   0        0        0      144 2023-04-09 22:57:33.217617 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/__init__.py
--rw-r--r--   0        0        0      146 2023-04-09 10:35:04.759933 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/__init__.py
--rw-r--r--   0        0        0      565 2023-04-26 21:31:10.282274 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/__init__.py
--rw-r--r--   0        0        0       78 2023-04-09 10:35:04.760862 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/common.py
--rw-r--r--   0        0        0       97 2023-04-09 10:35:04.761036 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/datapoint.py
--rw-r--r--   0        0        0      423 2023-04-09 10:35:04.761184 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/dataset.py
--rw-r--r--   0        0        0      124 2023-04-26 21:31:10.282618 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/instance.py
--rw-r--r--   0        0        0     1138 2023-04-26 21:31:10.283727 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/model.py
--rw-r--r--   0        0        0      101 2023-04-09 10:35:04.761619 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/namespace.py
--rw-r--r--   0        0        0      174 2023-04-09 10:35:04.761763 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/project.py
--rw-r--r--   0        0        0      698 2023-04-17 13:32:38.408872 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/storage.py
--rw-r--r--   0        0        0       85 2023-04-09 10:35:04.762055 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/token.py
--rw-r--r--   0        0        0      256 2023-04-09 10:35:04.762195 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/user.py
--rw-r--r--   0        0        0    16927 2023-04-26 21:31:10.284175 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/tungsten_api_client.py
--rw-r--r--   0        0        0     9376 2023-04-27 00:19:46.503001 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/tungsten_client.py
--rw-r--r--   0        0        0      178 2023-04-09 22:56:23.933893 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/__init__.py
--rw-r--r--   0        0        0      574 2023-04-09 22:44:42.545013 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/schemas.py
--rw-r--r--   0        0        0     4453 2023-04-26 21:31:10.285036 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/tungsten_model_api_client.py
--rw-r--r--   0        0        0     4000 2023-04-11 16:43:31.229639 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/tungsten_model_client.py
--rw-r--r--   0        0        0     4074 2023-04-28 23:27:15.782456 tungstenkit-0.0.1a5/tungstenkit/_internal/configs.py
--rw-r--r--   0        0        0     2111 2023-04-28 23:27:15.782804 tungstenkit-0.0.1a5/tungstenkit/_internal/constants.py
--rw-r--r--   0        0        0     4887 2023-04-26 21:31:10.286049 tungstenkit-0.0.1a5/tungstenkit/_internal/containerized_services.py
--rw-r--r--   0        0        0      132 2023-04-26 22:02:15.494035 tungstenkit-0.0.1a5/tungstenkit/_internal/contexts.py
--rw-r--r--   0        0        0     9936 2023-04-28 23:27:15.784185 tungstenkit-0.0.1a5/tungstenkit/_internal/io.py
--rw-r--r--   0        0        0     6498 2023-04-11 17:20:16.148322 tungstenkit-0.0.1a5/tungstenkit/_internal/io_schema.py
--rw-r--r--   0        0        0       94 2023-04-09 10:35:04.764738 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/__init__.py
--rw-r--r--   0        0        0     6745 2023-04-26 21:31:10.287336 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_blob_store.py
--rw-r--r--   0        0        0     9003 2023-04-26 21:31:10.287658 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_model.py
--rw-r--r--   0        0        0    14814 2023-04-26 21:31:10.288022 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_model_store.py
--rw-r--r--   0        0        0     3014 2023-04-26 21:31:10.288307 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_store.py
--rw-r--r--   0        0        0     2955 2023-04-26 23:19:48.588616 tungstenkit-0.0.1a5/tungstenkit/_internal/logging.py
--rw-r--r--   0        0        0    10513 2023-04-28 23:27:15.785158 tungstenkit-0.0.1a5/tungstenkit/_internal/model.py
--rw-r--r--   0        0        0        0 2023-02-17 08:39:49.007358 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/__init__.py
--rw-r--r--   0        0        0       67 2023-03-06 16:17:19.313885 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/__init__.py
--rw-r--r--   0        0        0     5083 2023-04-26 21:40:01.486422 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/404.html
--rw-r--r--   0        0        0      401 2023-04-26 21:40:00.038750 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/9J0J94uaBN6r2ZngrgX1w/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-04-26 21:40:00.038529 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/9J0J94uaBN6r2ZngrgX1w/_ssgManifest.js
--rw-r--r--   0        0        0  1564405 2023-04-26 21:40:00.044383 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/370-54e89ea530a46e74.js
--rw-r--r--   0        0        0    78390 2023-04-26 21:40:00.039266 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js
--rw-r--r--   0        0        0   452205 2023-04-26 21:40:00.041443 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js
--rw-r--r--   0        0        0   141074 2023-04-26 21:40:00.039764 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js
--rw-r--r--   0        0        0    90428 2023-04-26 21:40:00.041155 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js
--rw-r--r--   0        0        0   142467 2023-04-26 21:40:00.042918 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_app-a5d327f8245a7cb7.js
--rw-r--r--   0        0        0      250 2023-04-26 21:40:00.042591 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
--rw-r--r--   0        0        0    32188 2023-04-26 21:40:00.042788 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/index-d22c2e2ad4a0676a.js
--rw-r--r--   0        0        0    91460 2023-04-26 21:40:00.040708 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3853 2023-04-26 21:40:00.041574 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/webpack-b98be2d55f37c35c.js
--rw-r--r--   0        0        0     1914 2023-04-26 21:40:00.041630 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/6c93262152699231.css
--rw-r--r--   0        0        0    39283 2023-04-26 21:40:00.042000 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css
--rw-r--r--   0        0        0   256670 2023-04-26 21:40:00.061924 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/favicon.ico
--rw-r--r--   0        0        0    27067 2023-04-26 21:40:01.469688 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/index.html
--rw-r--r--   0        0        0     2956 2023-04-26 21:40:00.060165 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/logo.svg
--rw-r--r--   0        0        0     1375 2023-04-26 21:40:00.060165 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/next.svg
--rw-r--r--   0        0        0     1138 2023-04-26 21:40:00.060279 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/thirteen.svg
--rw-r--r--   0        0        0    27505 2023-04-26 21:40:00.060754 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/tungstenWithoutText.png
--rw-r--r--   0        0        0    18388 2023-04-26 21:40:00.060785 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/tungsten_greyed_out_logo.png
--rw-r--r--   0        0        0      629 2023-04-26 21:40:00.060638 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/vercel.svg
--rw-r--r--   0        0        0     3255 2023-04-18 14:30:25.906560 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/schemas.py
--rw-r--r--   0        0        0     5725 2023-04-17 13:32:38.450673 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/server.py
--rw-r--r--   0        0        0      156 2023-04-10 03:44:40.979762 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/__init__.py
--rw-r--r--   0        0        0     7170 2023-04-18 14:30:25.907462 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/example_service.py
--rw-r--r--   0        0        0     5594 2023-04-17 13:32:38.451856 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/file_service.py
--rw-r--r--   0        0        0    12106 2023-04-17 13:32:38.452749 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/prediction_service.py
--rw-r--r--   0        0        0        0 2023-02-17 08:39:49.007650 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/__init__.py
--rw-r--r--   0        0        0       32 2023-04-26 21:31:10.290945 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/__main__.py
--rw-r--r--   0        0        0     2885 2023-04-28 03:17:20.449371 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/cli.py
--rw-r--r--   0        0        0     3546 2023-04-26 21:31:10.291554 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/config.py
--rw-r--r--   0        0        0      144 2023-04-09 18:07:13.836271 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/enums.py
--rw-r--r--   0        0        0       70 2023-04-09 10:35:04.768748 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/__init__.py
--rw-r--r--   0        0        0      772 2023-04-09 10:35:04.768945 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/abstract_event_bus.py
--rw-r--r--   0        0        0      125 2023-04-09 10:35:04.769155 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/event.py
--rw-r--r--   0        0        0      337 2023-04-09 18:14:24.800665 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/factory.py
--rw-r--r--   0        0        0      511 2023-04-09 10:35:04.769485 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/local_event_bus.py
--rw-r--r--   0        0        0       78 2023-04-09 10:35:04.769721 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/__init__.py
--rw-r--r--   0        0        0      209 2023-04-09 10:35:04.769876 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/abstract_file_uploader.py
--rw-r--r--   0        0        0        7 2023-04-09 10:35:04.770021 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/azure_file_uploader.py
--rw-r--r--   0        0        0      602 2023-04-09 10:35:04.770162 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/factory.py
--rw-r--r--   0        0        0      675 2023-04-26 21:31:10.292540 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/in_memory_file_uploader.py
--rw-r--r--   0        0        0     1839 2023-04-26 21:31:10.292849 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/local_fs_file_uploader.py
--rw-r--r--   0        0        0        7 2023-04-09 10:35:04.770768 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/s3_file_uploader.py
--rw-r--r--   0        0        0        7 2023-02-17 08:39:49.008624 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/grpc_server.py
--rw-r--r--   0        0        0     5544 2023-04-26 21:31:10.293182 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/http_server.py
--rw-r--r--   0        0        0      563 2023-04-28 23:27:15.786706 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/ids.py
--rw-r--r--   0        0        0      184 2023-04-09 10:35:04.771472 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/__init__.py
--rw-r--r--   0        0        0      526 2023-04-09 10:35:04.771700 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/abstract_input_queue.py
--rw-r--r--   0        0        0      348 2023-04-09 18:14:24.863856 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/factory.py
--rw-r--r--   0        0        0     3215 2023-04-28 23:27:15.787098 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/local_input_queue.py
--rw-r--r--   0        0        0      131 2023-04-09 10:35:04.772211 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/shared.py
--rw-r--r--   0        0        0       69 2023-04-09 10:35:04.772454 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/__init__.py
--rw-r--r--   0        0        0    11275 2023-04-26 22:31:57.812867 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/subproc.py
--rw-r--r--   0        0        0     9827 2023-04-28 23:27:15.787490 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/worker.py
--rw-r--r--   0        0        0      248 2023-04-09 10:35:04.773162 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/__init__.py
--rw-r--r--   0        0        0     1487 2023-04-28 23:27:15.788210 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/abstract_result_cache.py
--rw-r--r--   0        0        0      396 2023-04-09 18:14:24.863983 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/factory.py
--rw-r--r--   0        0        0    10448 2023-04-28 23:27:15.788639 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/local_result_cache.py
--rw-r--r--   0        0        0      474 2023-04-09 10:35:04.774049 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/shared.py
--rw-r--r--   0        0        0     1365 2023-04-09 10:35:04.774342 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/schema.py
--rw-r--r--   0        0        0      503 2023-03-15 00:25:51.895356 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/server_exceptions.py
--rw-r--r--   0        0        0        0 2023-02-17 08:39:49.016050 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/task_server/__init__.py
--rw-r--r--   0        0        0     9316 2023-02-17 08:39:49.016381 tungstenkit-0.0.1a5/tungstenkit/_internal/task.py
--rw-r--r--   0        0        0        0 2023-02-17 08:39:49.019727 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1472 2023-04-09 10:35:04.774544 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/avatar.py
--rw-r--r--   0        0        0     2996 2023-04-26 23:35:59.492013 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/console.py
--rw-r--r--   0        0        0      937 2023-04-26 21:31:10.295291 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/context.py
--rw-r--r--   0        0        0    15016 2023-04-26 23:33:26.063956 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/docker.py
--rw-r--r--   0        0        0     2068 2023-04-26 21:31:10.295914 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/file.py
--rw-r--r--   0        0        0     6213 2023-04-28 23:27:15.789532 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/imports.py
--rw-r--r--   0        0        0     1700 2023-04-17 13:32:38.460136 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/json.py
--rw-r--r--   0        0        0     2910 2023-04-17 13:32:38.461086 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/markdown.py
--rw-r--r--   0        0        0      551 2023-03-31 00:24:18.313560 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/pydantic.py
--rw-r--r--   0        0        0     1241 2023-04-26 21:31:10.296085 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/regex.py
--rw-r--r--   0        0        0    12774 2023-04-26 21:31:10.296375 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/requests.py
--rw-r--r--   0        0        0     2037 2023-03-30 23:07:07.750471 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/serialize.py
--rw-r--r--   0        0        0      676 2023-03-31 00:17:55.349782 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/string.py
--rw-r--r--   0        0        0      648 2023-02-17 08:39:49.021077 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/typing.py
--rw-r--r--   0        0        0     1946 2023-04-26 21:31:10.296913 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/uri.py
--rw-r--r--   0        0        0     6332 2023-04-26 21:31:10.297213 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/version.py
--rw-r--r--   0        0        0      353 2023-02-17 08:39:49.021416 tungstenkit-0.0.1a5/tungstenkit/_versions.py
--rw-r--r--   0        0        0     2171 2023-04-26 21:31:10.297501 tungstenkit-0.0.1a5/tungstenkit/exceptions.py
--rw-r--r--   0        0        0      166 2023-04-28 23:27:15.790414 tungstenkit-0.0.1a5/tungstenkit/io.py
--rw-r--r--   0        0        0      171 2023-02-17 08:39:49.021956 tungstenkit-0.0.1a5/tungstenkit/model.py
--rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 tungstenkit-0.0.1a5/PKG-INFO
+-rw-r--r--   0        0        0     4086 2023-04-28 23:29:56.390539 tungstenkit-0.0.1a6/README.md
+-rw-r--r--   0        0        0     3034 2023-04-30 20:26:37.411748 tungstenkit-0.0.1a6/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-11 17:07:01.860571 tungstenkit-0.0.1a6/tungstenkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:48.957419 tungstenkit-0.0.1a6/tungstenkit/_internal/__init__.py
+-rw-r--r--   0        0        0       58 2023-02-17 08:39:48.957863 tungstenkit-0.0.1a6/tungstenkit/_internal/build/__init__.py
+-rw-r--r--   0        0        0    13058 2023-04-28 23:27:15.780413 tungstenkit-0.0.1a6/tungstenkit/_internal/build/build_context.py
+-rw-r--r--   0        0        0      223 2023-04-26 21:31:10.277468 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/__init__.py
+-rw-r--r--   0        0        0     6665 2023-04-26 21:31:10.277684 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_dockerfile.py
+-rw-r--r--   0        0        0      385 2023-02-17 08:39:48.959447 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/__init__.py
+-rw-r--r--   0        0        0      483 2023-04-09 10:35:04.753993 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/base_image.py
+-rw-r--r--   0        0        0      238 2023-02-17 08:39:48.959971 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/conda_image.py
+-rw-r--r--   0        0        0     2552 2023-04-26 21:31:10.278022 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/cuda_image.py
+-rw-r--r--   0        0        0      369 2023-02-17 08:39:48.960423 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/custom_image.py
+-rw-r--r--   0        0        0     1622 2023-04-26 21:31:10.278341 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/python_image.py
+-rw-r--r--   0        0        0      574 2023-04-09 10:35:04.754747 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/shared.py
+-rw-r--r--   0        0        0      652 2023-04-26 21:31:10.278501 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/model_dockerfile.py
+-rw-r--r--   0        0        0     7737 2023-04-26 21:31:10.278850 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/__init__.py
+-rw-r--r--   0        0        0     1008 2023-04-09 10:35:04.755489 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/__init__.py
+-rw-r--r--   0        0        0     3604 2023-03-30 23:07:07.733066 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/base_collection.py
+-rw-r--r--   0        0        0     1593 2023-04-09 10:35:04.755732 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/common.py
+-rw-r--r--   0        0        0     4315 2023-04-26 21:31:10.279190 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/tf_collection.py
+-rw-r--r--   0        0        0     6509 2023-04-26 21:31:10.279501 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/torch_collection.py
+-rw-r--r--   0        0        0      723 2023-02-17 08:39:48.962919 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/pip_requirement.py
+-rw-r--r--   0        0        0      924 2023-04-09 10:35:04.756528 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/requirements_txt.py
+-rw-r--r--   0        0        0      257 2023-04-26 21:31:10.279771 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/task_dockerfile_writer.py
+-rw-r--r--   0        0        0     1373 2023-04-09 10:35:04.757025 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/template_args.py
+-rw-r--r--   0        0        0      345 2023-02-17 08:39:48.964092 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/base.j2
+-rw-r--r--   0        0        0      951 2023-02-17 08:39:48.964269 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/install_conda.j2
+-rw-r--r--   0        0        0      834 2023-03-30 23:07:07.735005 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/install_python.j2
+-rw-r--r--   0        0        0      824 2023-04-09 10:35:04.757393 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/setup_tungsten.j2
+-rw-r--r--   0        0        0     1905 2023-04-09 10:35:04.757672 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/setup_user.j2
+-rw-r--r--   0        0        0     1218 2023-04-30 20:26:56.532564 tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/tungstenkit/pyproject.toml
+-rw-r--r--   0        0        0     2152 2023-04-26 21:31:10.280640 tungstenkit-0.0.1a6/tungstenkit/_internal/build/model.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:48.966251 tungstenkit-0.0.1a6/tungstenkit/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     2653 2023-04-26 21:31:10.280844 tungstenkit-0.0.1a6/tungstenkit/_internal/cli/callbacks.py
+-rw-r--r--   0        0        0     2280 2023-04-28 23:27:15.781189 tungstenkit-0.0.1a6/tungstenkit/_internal/cli/login_command.py
+-rw-r--r--   0        0        0     1428 2023-04-26 21:31:10.281426 tungstenkit-0.0.1a6/tungstenkit/_internal/cli/main.py
+-rw-r--r--   0        0        0    12392 2023-04-28 23:27:15.782080 tungstenkit-0.0.1a6/tungstenkit/_internal/cli/model_commands.py
+-rw-r--r--   0        0        0      653 2023-04-26 21:31:10.281918 tungstenkit-0.0.1a6/tungstenkit/_internal/cli/options.py
+-rw-r--r--   0        0        0      144 2023-04-09 22:57:33.217617 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/__init__.py
+-rw-r--r--   0        0        0      146 2023-04-09 10:35:04.759933 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-26 21:31:10.282274 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-09 10:35:04.760862 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/common.py
+-rw-r--r--   0        0        0       97 2023-04-09 10:35:04.761036 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/datapoint.py
+-rw-r--r--   0        0        0      423 2023-04-09 10:35:04.761184 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/dataset.py
+-rw-r--r--   0        0        0      124 2023-04-26 21:31:10.282618 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/instance.py
+-rw-r--r--   0        0        0     1138 2023-04-26 21:31:10.283727 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/model.py
+-rw-r--r--   0        0        0      101 2023-04-09 10:35:04.761619 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/namespace.py
+-rw-r--r--   0        0        0      174 2023-04-09 10:35:04.761763 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/project.py
+-rw-r--r--   0        0        0      698 2023-04-17 13:32:38.408872 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/storage.py
+-rw-r--r--   0        0        0       85 2023-04-09 10:35:04.762055 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/token.py
+-rw-r--r--   0        0        0      256 2023-04-09 10:35:04.762195 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/user.py
+-rw-r--r--   0        0        0    16927 2023-04-26 21:31:10.284175 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/tungsten_api_client.py
+-rw-r--r--   0        0        0     9376 2023-04-27 00:19:46.503001 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/tungsten_client.py
+-rw-r--r--   0        0        0      178 2023-04-09 22:56:23.933893 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten_model/__init__.py
+-rw-r--r--   0        0        0      574 2023-04-09 22:44:42.545013 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten_model/schemas.py
+-rw-r--r--   0        0        0     4453 2023-04-26 21:31:10.285036 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten_model/tungsten_model_api_client.py
+-rw-r--r--   0        0        0     4000 2023-04-11 16:43:31.229639 tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten_model/tungsten_model_client.py
+-rw-r--r--   0        0        0     4074 2023-04-28 23:27:15.782456 tungstenkit-0.0.1a6/tungstenkit/_internal/configs.py
+-rw-r--r--   0        0        0     2111 2023-04-28 23:27:15.782804 tungstenkit-0.0.1a6/tungstenkit/_internal/constants.py
+-rw-r--r--   0        0        0     4887 2023-04-26 21:31:10.286049 tungstenkit-0.0.1a6/tungstenkit/_internal/containerized_services.py
+-rw-r--r--   0        0        0      132 2023-04-26 22:02:15.494035 tungstenkit-0.0.1a6/tungstenkit/_internal/contexts.py
+-rw-r--r--   0        0        0     9844 2023-04-30 19:24:36.136700 tungstenkit-0.0.1a6/tungstenkit/_internal/io.py
+-rw-r--r--   0        0        0     6498 2023-04-11 17:20:16.148322 tungstenkit-0.0.1a6/tungstenkit/_internal/io_schema.py
+-rw-r--r--   0        0        0       94 2023-04-09 10:35:04.764738 tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/__init__.py
+-rw-r--r--   0        0        0     6745 2023-04-26 21:31:10.287336 tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/local_blob_store.py
+-rw-r--r--   0        0        0     9003 2023-04-26 21:31:10.287658 tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/local_model.py
+-rw-r--r--   0        0        0    14814 2023-04-26 21:31:10.288022 tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/local_model_store.py
+-rw-r--r--   0        0        0     3014 2023-04-26 21:31:10.288307 tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/local_store.py
+-rw-r--r--   0        0        0     2955 2023-04-26 23:19:48.588616 tungstenkit-0.0.1a6/tungstenkit/_internal/logging.py
+-rw-r--r--   0        0        0    10509 2023-04-30 20:26:20.800920 tungstenkit-0.0.1a6/tungstenkit/_internal/model.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:49.007358 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/__init__.py
+-rw-r--r--   0        0        0       67 2023-03-06 16:17:19.313885 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/__init__.py
+-rw-r--r--   0        0        0     5083 2023-04-26 21:40:01.486422 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/404.html
+-rw-r--r--   0        0        0      401 2023-04-26 21:40:00.038750 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/9J0J94uaBN6r2ZngrgX1w/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-04-26 21:40:00.038529 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/9J0J94uaBN6r2ZngrgX1w/_ssgManifest.js
+-rw-r--r--   0        0        0  1564405 2023-04-26 21:40:00.044383 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/370-54e89ea530a46e74.js
+-rw-r--r--   0        0        0    78390 2023-04-26 21:40:00.039266 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js
+-rw-r--r--   0        0        0   452205 2023-04-26 21:40:00.041443 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js
+-rw-r--r--   0        0        0   141074 2023-04-26 21:40:00.039764 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js
+-rw-r--r--   0        0        0    90428 2023-04-26 21:40:00.041155 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js
+-rw-r--r--   0        0        0   142467 2023-04-26 21:40:00.042918 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_app-a5d327f8245a7cb7.js
+-rw-r--r--   0        0        0      250 2023-04-26 21:40:00.042591 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
+-rw-r--r--   0        0        0    32188 2023-04-26 21:40:00.042788 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/index-d22c2e2ad4a0676a.js
+-rw-r--r--   0        0        0    91460 2023-04-26 21:40:00.040708 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3853 2023-04-26 21:40:00.041574 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/webpack-b98be2d55f37c35c.js
+-rw-r--r--   0        0        0     1914 2023-04-26 21:40:00.041630 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/6c93262152699231.css
+-rw-r--r--   0        0        0    39283 2023-04-26 21:40:00.042000 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css
+-rw-r--r--   0        0        0   256670 2023-04-26 21:40:00.061924 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/favicon.ico
+-rw-r--r--   0        0        0    27067 2023-04-26 21:40:01.469688 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/index.html
+-rw-r--r--   0        0        0     2956 2023-04-26 21:40:00.060165 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/logo.svg
+-rw-r--r--   0        0        0     1375 2023-04-26 21:40:00.060165 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/next.svg
+-rw-r--r--   0        0        0     1138 2023-04-26 21:40:00.060279 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/thirteen.svg
+-rw-r--r--   0        0        0    27505 2023-04-26 21:40:00.060754 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/tungstenWithoutText.png
+-rw-r--r--   0        0        0    18388 2023-04-26 21:40:00.060785 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/tungsten_greyed_out_logo.png
+-rw-r--r--   0        0        0      629 2023-04-26 21:40:00.060638 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/vercel.svg
+-rw-r--r--   0        0        0     3255 2023-04-18 14:30:25.906560 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/schemas.py
+-rw-r--r--   0        0        0     5725 2023-04-17 13:32:38.450673 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/server.py
+-rw-r--r--   0        0        0      156 2023-04-10 03:44:40.979762 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/services/__init__.py
+-rw-r--r--   0        0        0     7170 2023-04-18 14:30:25.907462 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/services/example_service.py
+-rw-r--r--   0        0        0     5594 2023-04-17 13:32:38.451856 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/services/file_service.py
+-rw-r--r--   0        0        0    12106 2023-04-17 13:32:38.452749 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/services/prediction_service.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:49.007650 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-26 21:31:10.290945 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/__main__.py
+-rw-r--r--   0        0        0     2885 2023-04-28 03:17:20.449371 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/cli.py
+-rw-r--r--   0        0        0     3546 2023-04-26 21:31:10.291554 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/config.py
+-rw-r--r--   0        0        0      144 2023-04-09 18:07:13.836271 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/enums.py
+-rw-r--r--   0        0        0       70 2023-04-09 10:35:04.768748 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/event_buses/__init__.py
+-rw-r--r--   0        0        0      772 2023-04-09 10:35:04.768945 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/event_buses/abstract_event_bus.py
+-rw-r--r--   0        0        0      125 2023-04-09 10:35:04.769155 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/event_buses/event.py
+-rw-r--r--   0        0        0      337 2023-04-09 18:14:24.800665 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/event_buses/factory.py
+-rw-r--r--   0        0        0      511 2023-04-09 10:35:04.769485 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/event_buses/local_event_bus.py
+-rw-r--r--   0        0        0       78 2023-04-09 10:35:04.769721 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-09 10:35:04.769876 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/abstract_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-04-09 10:35:04.770021 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/azure_file_uploader.py
+-rw-r--r--   0        0        0      602 2023-04-09 10:35:04.770162 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/factory.py
+-rw-r--r--   0        0        0      675 2023-04-26 21:31:10.292540 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/in_memory_file_uploader.py
+-rw-r--r--   0        0        0     1839 2023-04-26 21:31:10.292849 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/local_fs_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-04-09 10:35:04.770768 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/s3_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-02-17 08:39:49.008624 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/grpc_server.py
+-rw-r--r--   0        0        0     5544 2023-04-26 21:31:10.293182 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/http_server.py
+-rw-r--r--   0        0        0      563 2023-04-28 23:27:15.786706 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/ids.py
+-rw-r--r--   0        0        0      184 2023-04-09 10:35:04.771472 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/input_queues/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-09 10:35:04.771700 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/input_queues/abstract_input_queue.py
+-rw-r--r--   0        0        0      348 2023-04-09 18:14:24.863856 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/input_queues/factory.py
+-rw-r--r--   0        0        0     3215 2023-04-28 23:27:15.787098 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/input_queues/local_input_queue.py
+-rw-r--r--   0        0        0      131 2023-04-09 10:35:04.772211 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/input_queues/shared.py
+-rw-r--r--   0        0        0       69 2023-04-09 10:35:04.772454 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/prediction_worker/__init__.py
+-rw-r--r--   0        0        0    11227 2023-04-30 20:26:21.862511 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/prediction_worker/subproc.py
+-rw-r--r--   0        0        0     9827 2023-04-28 23:27:15.787490 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/prediction_worker/worker.py
+-rw-r--r--   0        0        0      248 2023-04-09 10:35:04.773162 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/result_caches/__init__.py
+-rw-r--r--   0        0        0     1487 2023-04-28 23:27:15.788210 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/result_caches/abstract_result_cache.py
+-rw-r--r--   0        0        0      396 2023-04-09 18:14:24.863983 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/result_caches/factory.py
+-rw-r--r--   0        0        0    10448 2023-04-28 23:27:15.788639 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/result_caches/local_result_cache.py
+-rw-r--r--   0        0        0      474 2023-04-09 10:35:04.774049 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/result_caches/shared.py
+-rw-r--r--   0        0        0     1365 2023-04-09 10:35:04.774342 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/schema.py
+-rw-r--r--   0        0        0      503 2023-03-15 00:25:51.895356 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/server_exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:49.016050 tungstenkit-0.0.1a6/tungstenkit/_internal/servers/task_server/__init__.py
+-rw-r--r--   0        0        0     9316 2023-02-17 08:39:49.016381 tungstenkit-0.0.1a6/tungstenkit/_internal/task.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:49.019727 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1472 2023-04-09 10:35:04.774544 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2023-04-26 23:35:59.492013 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/console.py
+-rw-r--r--   0        0        0      937 2023-04-26 21:31:10.295291 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/context.py
+-rw-r--r--   0        0        0    15016 2023-04-26 23:33:26.063956 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/docker.py
+-rw-r--r--   0        0        0     2068 2023-04-26 21:31:10.295914 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/file.py
+-rw-r--r--   0        0        0     6213 2023-04-28 23:27:15.789532 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/imports.py
+-rw-r--r--   0        0        0     1700 2023-04-17 13:32:38.460136 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/json.py
+-rw-r--r--   0        0        0     2910 2023-04-17 13:32:38.461086 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/markdown.py
+-rw-r--r--   0        0        0      551 2023-03-31 00:24:18.313560 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/pydantic.py
+-rw-r--r--   0        0        0     1241 2023-04-26 21:31:10.296085 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/regex.py
+-rw-r--r--   0        0        0    12774 2023-04-26 21:31:10.296375 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/requests.py
+-rw-r--r--   0        0        0     2037 2023-03-30 23:07:07.750471 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/serialize.py
+-rw-r--r--   0        0        0      676 2023-03-31 00:17:55.349782 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/string.py
+-rw-r--r--   0        0        0      648 2023-02-17 08:39:49.021077 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/typing.py
+-rw-r--r--   0        0        0     1946 2023-04-26 21:31:10.296913 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/uri.py
+-rw-r--r--   0        0        0     6332 2023-04-26 21:31:10.297213 tungstenkit-0.0.1a6/tungstenkit/_internal/utils/version.py
+-rw-r--r--   0        0        0      353 2023-02-17 08:39:49.021416 tungstenkit-0.0.1a6/tungstenkit/_versions.py
+-rw-r--r--   0        0        0     2184 2023-04-29 21:27:51.323901 tungstenkit-0.0.1a6/tungstenkit/exceptions.py
+-rw-r--r--   0        0        0      166 2023-04-28 23:27:15.790414 tungstenkit-0.0.1a6/tungstenkit/io.py
+-rw-r--r--   0        0        0      171 2023-02-17 08:39:49.021956 tungstenkit-0.0.1a6/tungstenkit/model.py
+-rw-r--r--   0        0        0     7256 1970-01-01 00:00:00.000000 tungstenkit-0.0.1a6/PKG-INFO
```

### Comparing `tungstenkit-0.0.1a5/README.md` & `tungstenkit-0.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/pyproject.toml` & `tungstenkit-0.0.1a6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.0.1a5"
+version = "0.0.1a6"
 description = "Tungstenkit is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models."
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://tungsten-ai.github.io/docs"
 readme = ["README.md"]
 packages = [{include = "tungstenkit"}]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
+    "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development",
+    "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries",
-    "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: User Interfaces",
     "Typing :: Typed",
     "Environment :: Console",
+    "Environment :: Web Environment",
     "Environment :: GPU",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -77,22 +79,18 @@
 flake8 = "^3.7.9"
 pytest = "^7.1.3"
 pytest-cov = "^2.8.1"
 types-pyyaml = "^6.0.12.2"
 types-requests = "^2.28.11.5"
 types-setuptools = "^65.6.0.2"
 twine = "^4.0.2"
-pytest-asyncio = "^0.20.3"
-types-aiofiles = "^22.1.0.4"
 locust = "^2.14.2"
 types-tabulate = "^0.9.0.0"
 types-markdown = "^3.4.2.5"
 pytest-timeout = "^2.1.0"
-bcrypt = "^4.0.1"
-trustme = "^0.9.0"
 jsonschema = "^4.17.3"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 line_length = 99
```

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/build_context.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/build_context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_dockerfile.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/cuda_image.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/cuda_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/python_image.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/python_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/shared.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/base_images/shared.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/model_dockerfile.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/model_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/__init__.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/__init__.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/base_collection.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/base_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/common.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/tf_collection.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/tf_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/torch_collection.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/gpu_packages/torch_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/pip_requirement.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/requirements_txt.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/python/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/template_args.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/template_args.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/install_conda.j2` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/install_conda.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/install_python.j2` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/install_python.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/setup_tungsten.j2` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/setup_tungsten.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/setup_user.j2` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/templates/setup_user.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/tungstenkit/pyproject.toml` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/dockerfile/tungstenkit/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.0.1a5"
+version = "0.0.1a6"
 description = "Tungstenkit is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models."
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://tungsten-ai.github.io/docs"
 packages = [{include = "tungstenkit"}]
 
 [tool.poetry.scripts]
 tungsten = "tungstenkit._internal.cli.main:main"
```

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/build/model.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/build/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/callbacks.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/cli/callbacks.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/login_command.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/cli/login_command.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/main.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/model_commands.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/cli/model_commands.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/options.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/cli/options.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/__init__.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/model.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/storage.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/schemas/storage.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/tungsten_api_client.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/tungsten_api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/tungsten_client.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten/tungsten_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/schemas.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten_model/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/tungsten_model_api_client.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten_model/tungsten_model_api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/tungsten_model_client.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/clients/tungsten_model/tungsten_model_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/configs.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/configs.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/constants.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/containerized_services.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/containerized_services.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/io.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,27 +283,25 @@
     *,
     description: str = None,
     choices: t.Sequence[t.Union[str, int]] = None,
     ge: float = None,
     le: float = None,
     min_length: int = None,
     max_length: int = None,
-    default_factory: t.Callable[[], t.Any] = None,
 ):
     extras: t.Dict[str, t.Any] = dict()
     if choices is not None:
         extras.update(choices=choices)
     return PydanticField(
         default=Undefined if default is Ellipsis else default,
         description=description,
         ge=ge,
         le=le,
         min_length=min_length,
         max_length=max_length,
-        default_factory=default_factory,
         **extras,
     )
 
 
 def _get_uri_scheme(uri_str: str) -> str:
     return furl(uri_str[:50]).scheme
```

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/io_schema.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/io_schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_blob_store.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/local_blob_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_model.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/local_model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_model_store.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/local_model_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_store.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/local_store/local_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/logging.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/model.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     def setup(self) -> t.Any:
         pass
 
     @abc.abstractmethod
     def predict(self, inputs: t.List[InputType]) -> t.Sequence[OutputType]:
         pass
 
-    def predict_for_demo(
+    def predict_demo(
         self, inputs: t.List[InputType]
     ) -> t.Tuple[t.Sequence[OutputType], t.Sequence[t.Union[t.Dict[str, t.Any], io.BaseIO]]]:
         outputs = self.predict(inputs)
         return outputs, outputs
 
     @classmethod
     def _get_model_config(cls) -> ModelConfig:
```

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/404.html` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/404.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/370-54e89ea530a46e74.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/370-54e89ea530a46e74.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_app-a5d327f8245a7cb7.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_app-a5d327f8245a7cb7.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/index-d22c2e2ad4a0676a.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/index-d22c2e2ad4a0676a.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/webpack-b98be2d55f37c35c.js` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/webpack-b98be2d55f37c35c.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/6c93262152699231.css` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/6c93262152699231.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/favicon.ico` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/index.html` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/index.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/logo.svg` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/logo.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/next.svg` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/next.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/thirteen.svg` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/thirteen.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/tungstenWithoutText.png` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/tungstenWithoutText.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/tungsten_greyed_out_logo.png` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/tungsten_greyed_out_logo.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/vercel.svg` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/frontend/vercel.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/schemas.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/server.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/example_service.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/services/example_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/file_service.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/services/file_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/prediction_service.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/demo_server/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/cli.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/cli.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/config.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/config.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/abstract_event_bus.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/event_buses/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/factory.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/factory.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/in_memory_file_uploader.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/in_memory_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/local_fs_file_uploader.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/file_uploaders/local_fs_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/http_server.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/http_server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/ids.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/ids.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/abstract_input_queue.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/input_queues/abstract_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/local_input_queue.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/input_queues/local_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/subproc.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/prediction_worker/subproc.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,18 +168,16 @@
             self._is_running = True
             # Send ACK to the main proc and release lock blocking cancelation
             self._conn_in_subproc.send(None)
 
             # print(f"working dir: {Path('.').resolve()}")
             parsed_inputs = [self._io_classes.input.parse_obj(inp) for inp in inputs]
             if is_demo:
-                fn_name = (
-                    self._model.__class__.__name__ + "." + self._model.predict_for_demo.__name__
-                )
-                tup = self._model.predict_for_demo(parsed_inputs)
+                fn_name = self._model.__class__.__name__ + "." + self._model.predict_demo.__name__
+                tup = self._model.predict_demo(parsed_inputs)
                 try:
                     it = iter(tup)
                 except TypeError:
                     raise exceptions.InvalidOutput(
                         f"Return of '{fn_name}' is not iterable. "
                         "It should return both 'outputs' and 'demo_outputs'."
                     )
```

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/worker.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/prediction_worker/worker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/abstract_result_cache.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/result_caches/abstract_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/local_result_cache.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/result_caches/local_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/schema.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/servers/model_server/schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/task.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/task.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/avatar.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/console.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/console.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/context.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/docker.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/docker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/file.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/file.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/imports.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/imports.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/json.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/json.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/markdown.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/pydantic.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/regex.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/regex.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/requests.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/requests.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/serialize.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/string.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/string.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/typing.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/typing.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/uri.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/version.py` & `tungstenkit-0.0.1a6/tungstenkit/_internal/utils/version.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a5/tungstenkit/exceptions.py` & `tungstenkit-0.0.1a6/tungstenkit/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Optional
 
 
 class TungstenException(Exception):
     """
-    Base class for all Tungsten's errors.
+    Base class for all Tungstenkit's errors.
     Each custom exception should be derived from this class.
     """
 
+    pass
+
 
 # TODO group exceptions
 
 
 class TungstenModelError(TungstenException):
     pass
```

### Comparing `tungstenkit-0.0.1a5/PKG-INFO` & `tungstenkit-0.0.1a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: tungstenkit
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: Tungstenkit is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models.
 Home-page: https://tungsten-ai.github.io/docs
 Author: Tungsten Contributors
 Author-email: foss@tungsten-ai.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
+Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -31,16 +33,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Typing :: Typed
 Requires-Dist: attrs (>=22.1.0,<23.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: cattrs (>=22.1.0,<23.0.0)
```

