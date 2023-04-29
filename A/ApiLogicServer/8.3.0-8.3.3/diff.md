# Comparing `tmp/ApiLogicServer-8.3.0.tar.gz` & `tmp/ApiLogicServer-8.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ApiLogicServer-8.3.0.tar", last modified: Thu Apr 27 02:31:19 2023, max compression
+gzip compressed data, was "ApiLogicServer-8.3.3.tar", last modified: Sat Apr 29 22:01:05 2023, max compression
```

## Comparing `ApiLogicServer-8.3.0.tar` & `ApiLogicServer-8.3.3.tar`

### file list

```diff
@@ -1,762 +1,766 @@
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.975350 ApiLogicServer-8.3.0/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.780486 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/
--rw-r--r--   0 val        (502) staff       (20)    15305 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    53720 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/SOURCES.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/dependency_links.txt
--rw-r--r--   0 val        (502) staff       (20)       66 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/entry_points.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/not-zip-safe
--rw-r--r--   0 val        (502) staff       (20)      585 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/requires.txt
--rw-r--r--   0 val        (502) staff       (20)       21 2023-04-27 02:31:19.000000 ApiLogicServer-8.3.0/ApiLogicServer.egg-info/top_level.txt
--rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/LICENSE
--rw-r--r--   0 val        (502) staff       (20)      732 2023-04-23 23:14:50.000000 ApiLogicServer-8.3.0/MANIFEST.in
--rw-r--r--   0 val        (502) staff       (20)    15305 2023-04-27 02:31:19.975074 ApiLogicServer-8.3.0/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    14316 2023-04-27 02:26:34.000000 ApiLogicServer-8.3.0/README.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.782317 ApiLogicServer-8.3.0/api_logic_server_cli/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    59835 2023-04-27 02:26:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/api_logic_server.py
--rw-r--r--   0 val        (502) staff       (20)      120 2023-04-27 00:54:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/api_logic_server_info.yaml
--rw-r--r--   0 val        (502) staff       (20)    33430 2023-03-10 20:22:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/cli.py
--rw-r--r--   0 val        (502) staff       (20)     1001 2023-04-02 18:24:38.000000 ApiLogicServer-8.3.0/api_logic_server_cli/cli_args_base.py
--rw-r--r--   0 val        (502) staff       (20)     3184 2023-04-02 23:08:24.000000 ApiLogicServer-8.3.0/api_logic_server_cli/cli_args_project.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.785729 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-26 18:43:59.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-11-10 15:34:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.790357 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      173 2022-11-10 15:35:23.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      189 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2601 2022-11-18 17:28:18.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3049 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     5300 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     7174 2023-02-10 20:33:17.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    13492 2023-03-16 03:50:38.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    21342 2023-02-05 16:19:42.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    35378 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     4053 2023-01-18 01:12:07.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    20087 2023-02-05 19:25:01.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    37019 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2274 2023-02-26 20:50:53.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     2617 2023-03-12 04:54:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     5290 2023-02-05 02:48:17.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
--rw-r--r--   0 val        (502) staff       (20)    11423 2023-03-16 03:50:23.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py
--rw-r--r--   0 val        (502) staff       (20)    34401 2023-02-05 02:48:22.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/model_creation_services.py
--rw-r--r--   0 val        (502) staff       (20)     6127 2023-01-18 01:12:06.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.792257 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store
--rwxrwxrwx   0 val        (502) staff       (20)    15430 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.792420 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
--rwxrwxrwx   0 val        (502) staff       (20)  1145966 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
--rwxrwxrwx   0 val        (502) staff       (20)     3870 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
--rwxrwxrwx   0 val        (502) staff       (20)      692 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
--rwxrwxrwx   0 val        (502) staff       (20)     5347 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
--rwxrwxrwx   0 val        (502) staff       (20)     9664 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
--rwxrwxrwx   0 val        (502) staff       (20)      492 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
--rwxrwxrwx   0 val        (502) staff       (20)       67 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.773537 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.794801 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
--rwxrwxrwx   0 val        (502) staff       (20)    86781 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
--rwxrwxrwx   0 val        (502) staff       (20)   166928 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
--rwxrwxrwx   0 val        (502) staff       (20)      211 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
--rwxrwxrwx   0 val        (502) staff       (20)      516 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.856172 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
--rwxrwxrwx   0 val        (502) staff       (20)     1576 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     3197 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9011 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    21905 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7103 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1004 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     2792 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7546 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    17381 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    33520 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    71153 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    14043 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    36857 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5595 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    14138 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6135 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    14288 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2280 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5953 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4407 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10552 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2156 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5783 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    11957 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    24504 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13356 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4187 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10856 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7001 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    17447 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3591 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8746 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9475 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3140 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7634 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4056 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9168 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8184 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    18882 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9104 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    14317 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    32894 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3152 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8052 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8662 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    20172 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4982 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13442 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6569 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    15183 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2002 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2974 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1967 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5172 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5948 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    10454 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    23458 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     3229 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4128 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10303 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    17096 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    31009 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7760 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    18142 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9800 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    21207 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3420 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8828 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3820 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10430 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    41393 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   145206 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5605 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13185 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8412 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    19971 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9916 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    22155 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    16602 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4681 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11819 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3710 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9146 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1924 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4864 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11830 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3092 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8217 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2417 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7472 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    16988 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2342 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6267 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)  3310604 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      576 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20) 10838575 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    35620 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   121512 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    17547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    39845 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2594 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6567 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    18754 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    38065 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7008 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2693 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6865 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3378 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8159 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2709 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6645 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4619 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10592 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4203 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10608 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2559 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6522 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5926 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    96741 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1840 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5116 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    19497 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3725 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9025 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3288 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8254 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2026 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5528 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    26650 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9201 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    21765 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11826 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    34921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   119930 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4669 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4316 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10868 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    11414 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    24817 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2622 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)     7016 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5259 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    13615 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7391 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    17258 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1986 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4960 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3230 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8177 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)  1384276 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
--rwxrwxrwx   0 val        (502) staff       (20)     3014 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)  5552838 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.860277 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
--rwxrwxrwx   0 val        (502) staff       (20)    72504 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.866214 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.866774 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/
--rw-r--r--   0 val        (502) staff       (20)       55 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
--rw-r--r--   0 val        (502) staff       (20)      389 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.867252 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
--rw-r--r--   0 val        (502) staff       (20)      742 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
--rw-r--r--   0 val        (502) staff       (20)      276 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.867395 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
--rw-r--r--   0 val        (502) staff       (20)      124 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.773843 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.773891 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.867702 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 val        (502) staff       (20)      483 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 val        (502) staff       (20)      727 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 val        (502) staff       (20)      938 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.868091 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
--rw-r--r--   0 val        (502) staff       (20)       64 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
--rw-r--r--   0 val        (502) staff       (20)      662 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
--rw-r--r--   0 val        (502) staff       (20)     3669 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
--rw-r--r--   0 val        (502) staff       (20)       68 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
--rw-r--r--   0 val        (502) staff       (20)      556 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/create_admin.sh
--rw-r--r--   0 val        (502) staff       (20)      624 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/fab_config.py
--rw-r--r--   0 val        (502) staff       (20)     2683 2023-02-05 02:49:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/home.js
--rw-r--r--   0 val        (502) staff       (20)     3121 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js
--rw-r--r--   0 val        (502) staff       (20)    35694 2023-02-05 19:24:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/ui_admin_creator.py
--rw-r--r--   0 val        (502) staff       (20)     2252 2023-03-12 01:14:25.000000 ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/uri_info.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.882951 ApiLogicServer-8.3.0/api_logic_server_cli/database/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-22 22:39:55.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)  1067008 2022-10-11 15:13:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite
--rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    45056 2023-01-19 01:03:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/authentication.sqlite
--rw-r--r--   0 val        (502) staff       (20)   413696 2022-12-26 21:41:55.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/classicmodels.sqlite
--rw-r--r--   0 val        (502) staff       (20)      122 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)    16384 2023-03-07 00:17:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/new.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/nw-gold-plus.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-03-19 18:51:02.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)   496640 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/nw.sqlite
--rw-r--r--   0 val        (502) staff       (20)    32768 2023-03-08 04:23:41.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests.sqlite
--rw-r--r--   0 val        (502) staff       (20)       53 2023-03-08 15:53:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests.yml
--rw-r--r--   0 val        (502) staff       (20)       23 2023-04-06 03:07:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests_nw.yml
--rw-r--r--   0 val        (502) staff       (20)       25 2023-04-06 03:06:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests_nw_1.yml
--rw-r--r--   0 val        (502) staff       (20)       21 2023-03-14 16:06:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests_typical.yml
--rw-r--r--   0 val        (502) staff       (20)    16384 2022-12-31 01:13:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/database/todos.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.903399 ApiLogicServer-8.3.0/api_logic_server_cli/docs/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1251 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/API-Customize.md
--rw-r--r--   0 val        (502) staff       (20)     2647 2022-12-29 01:51:24.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/API.md
--rw-r--r--   0 val        (502) staff       (20)     3222 2022-12-21 16:33:05.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Admin-Customization.md
--rw-r--r--   0 val        (502) staff       (20)    18275 2023-03-10 04:52:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Admin-Tour.md
--rw-r--r--   0 val        (502) staff       (20)      384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Architecture-What-Is.md
--rw-r--r--   0 val        (502) staff       (20)    12713 2022-11-22 02:48:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Architecture.md
--rw-r--r--   0 val        (502) staff       (20)    61944 2022-10-11 03:42:54.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Behave-Logic-Report.md
--rw-r--r--   0 val        (502) staff       (20)     3838 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Behave.md
--rw-r--r--   0 val        (502) staff       (20)     1994 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Create-ApiLogicProject.md
--rw-r--r--   0 val        (502) staff       (20)     5319 2022-12-21 20:29:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Classes.md
--rw-r--r--   0 val        (502) staff       (20)     2660 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Customization.md
--rw-r--r--   0 val        (502) staff       (20)     1114 2023-01-27 04:14:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Examples.md
--rw-r--r--   0 val        (502) staff       (20)      970 2022-10-03 02:15:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Keys.md
--rw-r--r--   0 val        (502) staff       (20)     3898 2023-01-06 02:59:38.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Multi.md
--rw-r--r--   0 val        (502) staff       (20)    13193 2023-03-12 01:14:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Database-Connectivity.md
--rw-r--r--   0 val        (502) staff       (20)     1241 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Execute.md
--rw-r--r--   0 val        (502) staff       (20)     3273 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-Frameworks.md
--rw-r--r--   0 val        (502) staff       (20)      527 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-Low-Code.md
--rw-r--r--   0 val        (502) staff       (20)     7036 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-RETE.md
--rw-r--r--   0 val        (502) staff       (20)     1851 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/IDE-Customize.md
--rw-r--r--   0 val        (502) staff       (20)     7532 2023-01-20 15:50:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/IDE-Execute.md
--rw-r--r--   0 val        (502) staff       (20)     6368 2023-02-04 01:50:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Eval-x.md
--rw-r--r--   0 val        (502) staff       (20)     8093 2023-01-09 21:17:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Eval.md
--rw-r--r--   0 val        (502) staff       (20)     3390 2023-02-03 23:28:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Express-x.md
--rw-r--r--   0 val        (502) staff       (20)     3539 2022-08-23 15:56:25.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Express.md
--rw-r--r--   0 val        (502) staff       (20)      566 2022-11-30 17:57:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-psycopg2.md
--rw-r--r--   0 val        (502) staff       (20)      977 2022-11-17 04:40:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-pyodbc.md
--rw-r--r--   0 val        (502) staff       (20)     7135 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install.md
--rw-r--r--   0 val        (502) staff       (20)    13448 2023-02-05 02:54:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Internals-CLI.md
--rw-r--r--   0 val        (502) staff       (20)     6504 2022-12-01 16:51:37.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Internals.md
--rw-r--r--   0 val        (502) staff       (20)     3258 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Operation.md
--rw-r--r--   0 val        (502) staff       (20)    14729 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)    10325 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Why.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic.md
--rw-r--r--   0 val        (502) staff       (20)     4205 2022-08-28 15:23:33.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Manage-GitHub.md
--rw-r--r--   0 val        (502) staff       (20)     3796 2022-12-28 03:43:06.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Builders.md
--rw-r--r--   0 val        (502) staff       (20)     1957 2022-12-22 04:40:03.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-DevOps.md
--rw-r--r--   0 val        (502) staff       (20)     1930 2023-01-31 22:36:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Env.md
--rw-r--r--   0 val        (502) staff       (20)     4936 2022-11-24 20:38:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Execution.md
--rw-r--r--   0 val        (502) staff       (20)     2446 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Rebuild.md
--rw-r--r--   0 val        (502) staff       (20)     2104 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Structure.md
--rw-r--r--   0 val        (502) staff       (20)      773 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Sample-Database.md
--rw-r--r--   0 val        (502) staff       (20)     2227 2023-02-14 23:54:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Activation.md
--rw-------   0 val        (502) staff       (20)     1585 2023-01-21 01:47:08.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authentication-Provider.md
--rw-------   0 val        (502) staff       (20)     1470 2023-01-21 02:17:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authentication.md
--rw-r--r--   0 val        (502) staff       (20)     1922 2023-01-06 17:06:26.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authorization.md
--rw-r--r--   0 val        (502) staff       (20)     5277 2023-01-21 01:31:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Overview.md
--rw-r--r--   0 val        (502) staff       (20)      155 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech--Notes.md
--rw-r--r--   0 val        (502) staff       (20)      237 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-4GL.md
--rw-r--r--   0 val        (502) staff       (20)     7081 2022-11-24 00:40:19.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-CodeSpaces.md
--rw-r--r--   0 val        (502) staff       (20)     3053 2022-12-06 21:43:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md
--rw-r--r--   0 val        (502) staff       (20)     3174 2022-12-06 18:38:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)     5693 2022-12-05 19:50:10.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference.md
--rw-r--r--   0 val        (502) staff       (20)     3385 2022-11-07 18:45:42.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Docker.md
--rw-r--r--   0 val        (502) staff       (20)      815 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Install-Python.md
--rw-r--r--   0 val        (502) staff       (20)     1049 2022-10-03 16:52:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Proven.md
--rw-r--r--   0 val        (502) staff       (20)     2679 2022-12-07 04:30:27.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Python-311.md
--rw-r--r--   0 val        (502) staff       (20)     3728 2023-01-12 06:40:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Python.md
--rw-r--r--   0 val        (502) staff       (20)     3019 2022-10-21 23:29:01.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-m1.md
--rw-r--r--   0 val        (502) staff       (20)     1644 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-mkdocs-material.md
--rw-r--r--   0 val        (502) staff       (20)    12291 2022-10-08 18:23:10.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Troubleshooting.md
--rw-r--r--   0 val        (502) staff       (20)    15277 2023-04-27 02:31:04.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)     6697 2022-12-02 18:42:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Working-With-Docker.md
--rw-r--r--   0 val        (502) staff       (20)     4031 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.903819 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-08-30 03:14:41.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.904412 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/
--rw-r--r--   0 val        (502) staff       (20)     2362 2022-08-29 00:06:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/bulb-icon.svg
--rw-r--r--   0 val        (502) staff       (20)     3482 2022-08-30 03:46:01.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/lightbulb.svg
--rw-r--r--   0 val        (502) staff       (20)    15440 2023-02-06 03:49:29.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/index.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.904763 ApiLogicServer-8.3.0/api_logic_server_cli/docs/stylesheets/
--rw-r--r--   0 val        (502) staff       (20)      634 2022-08-30 03:44:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/docs/stylesheets/extra.css
--rw-r--r--   0 val        (502) staff       (20)    11824 2023-02-11 04:16:18.000000 ApiLogicServer-8.3.0/api_logic_server_cli/extended_builder.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.906796 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/
--rw-r--r--   0 val        (502) staff       (20)     1431 2023-02-05 02:48:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
--rw-r--r--   0 val        (502) staff       (20)     1956 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/configZZ.py
--rw-r--r--   0 val        (502) staff       (20)       63 2022-10-01 16:17:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/db_typesZZ.txt
--rw-r--r--   0 val        (502) staff       (20)    12053 2023-02-05 02:48:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/modelsZZ.py
--rw-r--r--   0 val        (502) staff       (20)      888 2023-04-23 22:57:22.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/nw_virtual_attrs.py
--rw-r--r--   0 val        (502) staff       (20)      870 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
--rw-r--r--   0 val        (502) staff       (20)     1006 2023-04-21 23:18:04.000000 ApiLogicServer-8.3.0/api_logic_server_cli/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.911444 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-04-26 02:43:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.912474 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      444 2023-02-05 02:50:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 21:44:41.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-01-08 18:52:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      106 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.912741 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:37.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.914735 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1306 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1196 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1205 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1116 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run.xml
--rw-r--r--   0 val        (502) staff       (20)     2433 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.915174 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     6518 2023-04-13 16:38:20.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      437 2023-04-13 04:29:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.916445 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     2053 2023-04-26 02:48:17.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/customize_api.py
--rw-r--r--   0 val        (502) staff       (20)      316 2023-01-23 01:07:06.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/expose_api_models.py
--rw-r--r--   0 val        (502) staff       (20)      521 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/json_encoder.py
--rw-r--r--   0 val        (502) staff       (20)     2527 2023-04-26 02:40:27.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/readme_customize_api.md
--rw-r--r--   0 val        (502) staff       (20)    18289 2023-04-22 14:56:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api_logic_server_run.py
--rw-r--r--   0 val        (502) staff       (20)     3131 2023-03-03 16:08:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.917436 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.918970 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/
--rw-r--r--   0 val        (502) staff       (20)     2101 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/env.py
--rw-r--r--   0 val        (502) staff       (20)     1967 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/readme.md
--rw-r--r--   0 val        (502) staff       (20)      494 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.919361 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/versions/
--rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
--rw-r--r--   0 val        (502) staff       (20)     3027 2023-02-09 15:42:27.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic.ini
--rw-r--r--   0 val        (502) staff       (20)      537 2023-01-28 17:53:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/bind_databases.py
--rw-r--r--   0 val        (502) staff       (20)      469 2023-01-23 01:14:38.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)      139 2022-12-21 03:23:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/default.env
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.919722 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.921036 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/
--rw-r--r--   0 val        (502) staff       (20)     2381 2023-02-26 22:13:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
--rw-r--r--   0 val        (502) staff       (20)     3643 2023-02-25 03:16:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
--rw-r--r--   0 val        (502) staff       (20)      331 2023-04-02 15:52:20.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     2079 2023-04-02 16:35:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
--rw-r--r--   0 val        (502) staff       (20)      876 2023-01-07 21:19:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
--rw-r--r--   0 val        (502) staff       (20)     1475 2023-04-21 23:01:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.922139 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logic/
--rw-r--r--   0 val        (502) staff       (20)      592 2023-04-26 02:47:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)     5953 2023-04-27 00:49:20.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
--rw-r--r--   0 val        (502) staff       (20)      568 2023-03-04 03:52:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/mypy.ini
--rw-r--r--   0 val        (502) staff       (20)     3820 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py
--rw-r--r--   0 val        (502) staff       (20)     6894 2023-04-27 00:54:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)      801 2022-10-19 20:24:10.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/run.ps1
--rwxr-xr-x   0 val        (502) staff       (20)     1040 2022-11-09 16:08:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/run.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.922829 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-12-15 01:50:41.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.923535 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-18 05:06:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-12-14 21:51:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.925711 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      173 2022-12-14 21:55:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      928 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1803 2022-12-18 03:38:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      820 2022-12-16 14:20:29.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1392 2022-12-14 22:25:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1024 2022-12-16 15:01:05.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1619 2022-12-15 17:24:50.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      580 2022-12-19 03:03:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.926325 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.926631 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1493 2022-12-19 03:13:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     4355 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)     2907 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.775495 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.927682 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1215 2022-12-19 03:24:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     2262 2022-12-19 00:39:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      839 2022-12-18 03:49:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.927945 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
--rw-r--r--   0 val        (502) staff       (20)     2165 2023-02-15 02:24:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)      587 2023-01-23 01:02:25.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.928739 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/
--rw-r--r--   0 val        (502) staff       (20)     1403 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
--rw-r--r--   0 val        (502) staff       (20)     1156 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
--rw-r--r--   0 val        (502) staff       (20)     1364 2023-01-12 23:29:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.929581 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.929855 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     4665 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3425 2023-03-03 16:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/authentication.py
--rw-r--r--   0 val        (502) staff       (20)     6004 2023-03-03 16:56:55.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/authorization.py
--rw-r--r--   0 val        (502) staff       (20)     1705 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.930378 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/templates/
--rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/templates/index.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.930634 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.931218 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     9969 2022-11-29 03:36:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
--rw-r--r--   0 val        (502) staff       (20)     1026 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.931396 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      414 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.931760 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      416 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     1518 2023-02-11 17:50:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.932472 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
--rw-r--r--   0 val        (502) staff       (20)      147 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
--rw-r--r--   0 val        (502) staff       (20)    65295 2022-10-11 03:42:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.933277 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/basic/
--rw-r--r--   0 val        (502) staff       (20)      735 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/basic/server_test.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.933874 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 20:09:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.934310 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)     6671 2023-03-19 18:44:09.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
--rw-r--r--   0 val        (502) staff       (20)     2750 2023-02-05 02:50:52.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/home.js
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.934619 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-26 23:48:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.936701 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
--rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.938129 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/
--rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.938284 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/templates/
--rw-r--r--   0 val        (502) staff       (20)       26 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/templates/content.html
--rw-r--r--   0 val        (502) staff       (20)     9076 2023-03-24 00:43:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/util.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.939792 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/
--rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-03-10 20:26:13.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/py.py
--rw-r--r--   0 val        (502) staff       (20)      738 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
--rw-r--r--   0 val        (502) staff       (20)      579 2023-03-03 02:36:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
--rw-r--r--   0 val        (502) staff       (20)      900 2023-02-05 02:50:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
--rw-r--r--   0 val        (502) staff       (20)      698 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
--rw-r--r--   0 val        (502) staff       (20)      893 2023-02-05 02:50:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.940341 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.940575 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/api/
--rw-r--r--   0 val        (502) staff       (20)     8711 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.941426 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/
--rw-r--r--   0 val        (502) staff       (20)     2662 2023-04-24 23:31:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)      312 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/db_debug.py
--rw-r--r--   0 val        (502) staff       (20)        0 2022-11-16 19:24:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)       29 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.941687 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/logic/
--rw-r--r--   0 val        (502) staff       (20)    10650 2023-04-23 00:10:12.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)      305 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.941991 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/security/
--rw-r--r--   0 val        (502) staff       (20)     1158 2023-02-14 15:54:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.942239 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.942342 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.943075 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      187 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
--rw-r--r--   0 val        (502) staff       (20)      285 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
--rw-r--r--   0 val        (502) staff       (20)     1281 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
--rw-r--r--   0 val        (502) staff       (20)      473 2023-04-23 23:42:07.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.944594 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      450 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     2130 2023-01-14 03:27:19.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
--rw-r--r--   0 val        (502) staff       (20)    16642 2023-02-16 04:52:22.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
--rw-r--r--   0 val        (502) staff       (20)     4722 2023-04-23 23:41:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.944950 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
--rw-r--r--   0 val        (502) staff       (20)     4356 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.947665 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
--rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     5794 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     2568 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
--rw-r--r--   0 val        (502) staff       (20)     8481 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
--rw-r--r--   0 val        (502) staff       (20)     8445 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
--rw-r--r--   0 val        (502) staff       (20)     2561 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.948338 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.949990 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/
--rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
--rw-r--r--   0 val        (502) staff       (20)    16926 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
--rw-r--r--   0 val        (502) staff       (20)      840 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
--rw-r--r--   0 val        (502) staff       (20)     1381 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
--rw-r--r--   0 val        (502) staff       (20)      831 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
--rw-r--r--   0 val        (502) staff       (20)     8405 2023-03-10 20:26:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
--rw-r--r--   0 val        (502) staff       (20)    13497 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
--rw-r--r--   0 val        (502) staff       (20)     1543 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.950173 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/
--rw-r--r--   0 val        (502) staff       (20)     8196 2022-11-11 23:20:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.951135 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)    17259 2023-04-24 23:38:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     3443 2023-02-05 02:51:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
--rw-r--r--   0 val        (502) staff       (20)     8798 2022-12-30 19:58:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.951407 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-11 23:17:05.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.953186 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/
--rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.954941 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
--rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.955125 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw_no_cust/
--rw-r--r--   0 val        (502) staff       (20)     5431 2023-02-05 02:51:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.956541 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:04:24.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.958105 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      446 2023-02-05 02:55:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 02:52:45.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      215 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.958369 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:05:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.960784 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:30:57.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1141 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml
--rw-r--r--   0 val        (502) staff       (20)     1162 2023-02-14 05:07:31.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml
--rw-r--r--   0 val        (502) staff       (20)     1174 2023-02-14 05:17:54.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1148 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml
--rw-r--r--   0 val        (502) staff       (20)     1160 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml
--rw-r--r--   0 val        (502) staff       (20)     1142 2023-02-14 05:16:08.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml
--rw-r--r--   0 val        (502) staff       (20)     1204 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1386 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.961315 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     5986 2023-04-13 16:51:25.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      100 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.962889 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-27 01:16:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.963858 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1238 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3435 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3970 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3439 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     5965 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.963995 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
--rw-r--r--   0 val        (502) staff       (20)     2895 2023-02-28 05:23:15.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
--rw-r--r--   0 val        (502) staff       (20)     2058 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.965403 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.965656 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     8571 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
--rw-r--r--   0 val        (502) staff       (20)    11838 2023-01-28 17:14:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
--rw-r--r--   0 val        (502) staff       (20)     1452 2023-02-27 23:00:55.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
--rw-r--r--   0 val        (502) staff       (20)     3530 2023-02-28 05:20:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
--rw-r--r--   0 val        (502) staff       (20)     7699 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
--rw-r--r--   0 val        (502) staff       (20)    21134 2023-04-14 00:57:12.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-04-02 02:53:45.000000 ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/sample_db.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.967172 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)      369 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
--rw-r--r--   0 val        (502) staff       (20)        0 2023-01-03 23:29:33.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.968964 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      175 2023-01-03 23:29:48.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      191 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     8054 2022-11-17 03:31:49.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    14080 2023-02-17 01:02:20.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    21696 2023-03-12 04:54:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     1755 2023-02-01 19:08:47.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    53944 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
--rw-r--r--   0 val        (502) staff       (20)       54 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.970082 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)     1850 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
--rw-r--r--   0 val        (502) staff       (20)     2593 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
--rw-r--r--   0 val        (502) staff       (20)     3865 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.970470 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      183 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      203 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)       87 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
--rw-r--r--   0 val        (502) staff       (20)     1399 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)      196 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.971398 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.972559 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      195 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      215 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    32358 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    74447 2023-04-06 14:36:23.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    58988 2023-04-06 14:31:39.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
--rw-r--r--   0 val        (502) staff       (20)     3252 2022-11-18 19:19:33.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.973099 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
--rw-r--r--   0 val        (502) staff       (20)    33384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
--rw-r--r--   0 val        (502) staff       (20)      440 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
--rwxr-xr-x   0 val        (502) staff       (20)    17212 2023-03-12 01:12:46.000000 ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-27 02:31:19.974759 ApiLogicServer-8.3.0/api_logic_server_cli/templates/
--rw-r--r--   0 val        (502) staff       (20)    14864 2023-03-29 21:47:30.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     1221 2023-03-29 20:25:21.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/app_fiddle.md
--rw-r--r--   0 val        (502) staff       (20)     3322 2023-04-13 17:12:40.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/app_fiddle.txt
--rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/index.html
--rw-r--r--   0 val        (502) staff       (20)      900 2023-01-19 01:43:35.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/login_endpoint.txt
--rw-r--r--   0 val        (502) staff       (20)      205 2023-01-19 01:44:07.000000 ApiLogicServer-8.3.0/api_logic_server_cli/templates/login_endpoint_imports.txt
--rw-r--r--   0 val        (502) staff       (20)       38 2023-04-27 02:31:19.975387 ApiLogicServer-8.3.0/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)     3521 2023-04-26 19:16:06.000000 ApiLogicServer-8.3.0/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.776017 ApiLogicServer-8.3.3/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.566931 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/
+-rw-r--r--   0 val        (502) staff       (20)    14774 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    53981 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/SOURCES.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/dependency_links.txt
+-rw-r--r--   0 val        (502) staff       (20)       66 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/entry_points.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/not-zip-safe
+-rw-r--r--   0 val        (502) staff       (20)      585 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/requires.txt
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-04-29 22:01:05.000000 ApiLogicServer-8.3.3/ApiLogicServer.egg-info/top_level.txt
+-rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/LICENSE
+-rw-r--r--   0 val        (502) staff       (20)      732 2023-04-23 23:14:50.000000 ApiLogicServer-8.3.3/MANIFEST.in
+-rw-r--r--   0 val        (502) staff       (20)    14774 2023-04-29 22:01:05.775639 ApiLogicServer-8.3.3/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    13785 2023-04-29 22:00:12.000000 ApiLogicServer-8.3.3/README.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.569055 ApiLogicServer-8.3.3/api_logic_server_cli/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)    59911 2023-04-29 19:56:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/api_logic_server.py
+-rw-r--r--   0 val        (502) staff       (20)      131 2023-04-29 21:44:24.000000 ApiLogicServer-8.3.3/api_logic_server_cli/api_logic_server_info.yaml
+-rw-r--r--   0 val        (502) staff       (20)    33430 2023-03-10 20:22:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/cli.py
+-rw-r--r--   0 val        (502) staff       (20)     1001 2023-04-02 18:24:38.000000 ApiLogicServer-8.3.3/api_logic_server_cli/cli_args_base.py
+-rw-r--r--   0 val        (502) staff       (20)     3184 2023-04-02 23:08:24.000000 ApiLogicServer-8.3.3/api_logic_server_cli/cli_args_project.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.572547 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-26 18:43:59.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-11-10 15:34:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.577545 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      173 2022-11-10 15:35:23.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      189 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2601 2022-11-18 17:28:18.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3049 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5300 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     7174 2023-02-10 20:33:17.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    13492 2023-03-16 03:50:38.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    21342 2023-02-05 16:19:42.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    35378 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     4053 2023-01-18 01:12:07.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    20087 2023-02-05 19:25:01.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    37019 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2274 2023-02-26 20:50:53.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2617 2023-03-12 04:54:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5290 2023-02-05 02:48:17.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
+-rw-r--r--   0 val        (502) staff       (20)    11423 2023-03-16 03:50:23.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/api_logic_server_utils.py
+-rw-r--r--   0 val        (502) staff       (20)    34401 2023-02-05 02:48:22.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/model_creation_services.py
+-rw-r--r--   0 val        (502) staff       (20)     6127 2023-01-18 01:12:06.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.579977 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store
+-rwxrwxrwx   0 val        (502) staff       (20)    15430 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.580135 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
+-rwxrwxrwx   0 val        (502) staff       (20)  1145966 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
+-rwxrwxrwx   0 val        (502) staff       (20)     3870 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
+-rwxrwxrwx   0 val        (502) staff       (20)      692 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
+-rwxrwxrwx   0 val        (502) staff       (20)     5347 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
+-rwxrwxrwx   0 val        (502) staff       (20)     9664 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
+-rwxrwxrwx   0 val        (502) staff       (20)      492 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
+-rwxrwxrwx   0 val        (502) staff       (20)       67 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.559148 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.582444 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
+-rwxrwxrwx   0 val        (502) staff       (20)    86781 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
+-rwxrwxrwx   0 val        (502) staff       (20)   166928 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
+-rwxrwxrwx   0 val        (502) staff       (20)      211 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
+-rwxrwxrwx   0 val        (502) staff       (20)      516 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.658366 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
+-rwxrwxrwx   0 val        (502) staff       (20)     1576 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     3197 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9011 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    21905 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7103 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1004 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     2792 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7546 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    17381 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    33520 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    71153 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    14043 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    36857 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5595 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    14138 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6135 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    14288 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2280 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5953 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4407 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10552 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2156 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5783 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    11957 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    24504 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13356 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4187 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10856 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7001 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    17447 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3591 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8746 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9475 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3140 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7634 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4056 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9168 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8184 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    18882 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9104 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    14317 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    32894 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3152 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8052 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8662 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    20172 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4982 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13442 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6569 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    15183 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2002 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2974 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1967 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5172 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5948 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    10454 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    23458 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     3229 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4128 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10303 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    17096 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    31009 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7760 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    18142 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9800 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    21207 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3420 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8828 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3820 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10430 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    41393 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   145206 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5605 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13185 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8412 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    19971 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9916 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    22155 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    16602 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4681 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11819 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3710 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9146 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1924 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4864 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11830 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3092 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8217 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2417 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7472 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    16988 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2342 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6267 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)  3310604 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      576 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20) 10838575 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    35620 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   121512 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    17547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    39845 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2594 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6567 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    18754 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    38065 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7008 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2693 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6865 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3378 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8159 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2709 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6645 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4619 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10592 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4203 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10608 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2559 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6522 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5926 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    96741 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1840 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5116 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    19497 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3725 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9025 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3288 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8254 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2026 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5528 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    26650 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9201 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    21765 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11826 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    34921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   119930 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4669 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4316 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10868 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    11414 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    24817 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2622 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)     7016 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5259 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    13615 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7391 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    17258 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1986 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4960 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3230 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8177 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)  1384276 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
+-rwxrwxrwx   0 val        (502) staff       (20)     3014 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)  5552838 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.662765 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
+-rwxrwxrwx   0 val        (502) staff       (20)    72504 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.667416 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.668102 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/
+-rw-r--r--   0 val        (502) staff       (20)       55 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
+-rw-r--r--   0 val        (502) staff       (20)      389 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.668635 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
+-rw-r--r--   0 val        (502) staff       (20)      742 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)      276 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.668797 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
+-rw-r--r--   0 val        (502) staff       (20)      124 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.559458 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.559499 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.669150 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 val        (502) staff       (20)      483 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 val        (502) staff       (20)      727 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 val        (502) staff       (20)      938 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.669474 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
+-rw-r--r--   0 val        (502) staff       (20)       64 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
+-rw-r--r--   0 val        (502) staff       (20)      662 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
+-rw-r--r--   0 val        (502) staff       (20)     3669 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
+-rw-r--r--   0 val        (502) staff       (20)       68 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
+-rw-r--r--   0 val        (502) staff       (20)      556 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/create_admin.sh
+-rw-r--r--   0 val        (502) staff       (20)      624 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/fab_config.py
+-rw-r--r--   0 val        (502) staff       (20)     2683 2023-02-05 02:49:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/home.js
+-rw-r--r--   0 val        (502) staff       (20)     3121 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/react_admin_component.js
+-rw-r--r--   0 val        (502) staff       (20)    35694 2023-02-05 19:24:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/ui_admin_creator.py
+-rw-r--r--   0 val        (502) staff       (20)     2252 2023-03-12 01:14:25.000000 ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/uri_info.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.685328 ApiLogicServer-8.3.3/api_logic_server_cli/database/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-22 22:39:55.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)  1067008 2022-10-11 15:13:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/Chinook_Sqlite.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)    45056 2023-01-19 01:03:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/authentication.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   413696 2022-12-26 21:41:55.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/classicmodels.sqlite
+-rw-r--r--   0 val        (502) staff       (20)      122 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)    16384 2023-03-07 00:17:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/new.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/nw-gold-plus.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-03-19 18:51:02.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   496640 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/nw.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    32768 2023-03-08 04:23:41.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       53 2023-03-08 15:53:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests.yml
+-rw-r--r--   0 val        (502) staff       (20)       23 2023-04-06 03:07:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests_nw.yml
+-rw-r--r--   0 val        (502) staff       (20)       25 2023-04-06 03:06:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests_nw_1.yml
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-03-14 16:06:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests_typical.yml
+-rw-r--r--   0 val        (502) staff       (20)    16384 2022-12-31 01:13:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/database/todos.sqlite
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.703214 ApiLogicServer-8.3.3/api_logic_server_cli/docs/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1251 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/API-Customize.md
+-rw-r--r--   0 val        (502) staff       (20)     2647 2022-12-29 01:51:24.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/API.md
+-rw-r--r--   0 val        (502) staff       (20)     3222 2022-12-21 16:33:05.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Admin-Customization.md
+-rw-r--r--   0 val        (502) staff       (20)    18275 2023-03-10 04:52:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Admin-Tour.md
+-rw-r--r--   0 val        (502) staff       (20)      384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Architecture-What-Is.md
+-rw-r--r--   0 val        (502) staff       (20)    12713 2022-11-22 02:48:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Architecture.md
+-rw-r--r--   0 val        (502) staff       (20)    61944 2022-10-11 03:42:54.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Behave-Logic-Report.md
+-rw-r--r--   0 val        (502) staff       (20)     3838 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Behave.md
+-rw-r--r--   0 val        (502) staff       (20)     1994 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Create-ApiLogicProject.md
+-rw-r--r--   0 val        (502) staff       (20)     5319 2022-12-21 20:29:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Classes.md
+-rw-r--r--   0 val        (502) staff       (20)     2660 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Customization.md
+-rw-r--r--   0 val        (502) staff       (20)     1114 2023-01-27 04:14:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Examples.md
+-rw-r--r--   0 val        (502) staff       (20)      970 2022-10-03 02:15:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Keys.md
+-rw-r--r--   0 val        (502) staff       (20)     3898 2023-01-06 02:59:38.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Multi.md
+-rw-r--r--   0 val        (502) staff       (20)    13193 2023-03-12 01:14:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Database-Connectivity.md
+-rw-r--r--   0 val        (502) staff       (20)     1241 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Execute.md
+-rw-r--r--   0 val        (502) staff       (20)     3273 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-Frameworks.md
+-rw-r--r--   0 val        (502) staff       (20)      527 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-Low-Code.md
+-rw-r--r--   0 val        (502) staff       (20)     7036 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-RETE.md
+-rw-r--r--   0 val        (502) staff       (20)     1851 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/IDE-Customize.md
+-rw-r--r--   0 val        (502) staff       (20)     7532 2023-01-20 15:50:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/IDE-Execute.md
+-rw-r--r--   0 val        (502) staff       (20)     6368 2023-02-04 01:50:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Eval-x.md
+-rw-r--r--   0 val        (502) staff       (20)     8093 2023-01-09 21:17:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Eval.md
+-rw-r--r--   0 val        (502) staff       (20)     3390 2023-02-03 23:28:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Express-x.md
+-rw-r--r--   0 val        (502) staff       (20)     3539 2022-08-23 15:56:25.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Express.md
+-rw-r--r--   0 val        (502) staff       (20)      566 2022-11-30 17:57:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-psycopg2.md
+-rw-r--r--   0 val        (502) staff       (20)      977 2022-11-17 04:40:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-pyodbc.md
+-rw-r--r--   0 val        (502) staff       (20)     7135 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install.md
+-rw-r--r--   0 val        (502) staff       (20)    13448 2023-02-05 02:54:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Internals-CLI.md
+-rw-r--r--   0 val        (502) staff       (20)     6504 2022-12-01 16:51:37.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Internals.md
+-rw-r--r--   0 val        (502) staff       (20)     3258 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Operation.md
+-rw-r--r--   0 val        (502) staff       (20)    14729 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)    10325 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Why.md
+-rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic.md
+-rw-r--r--   0 val        (502) staff       (20)     4205 2022-08-28 15:23:33.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Manage-GitHub.md
+-rw-r--r--   0 val        (502) staff       (20)     3796 2022-12-28 03:43:06.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Builders.md
+-rw-r--r--   0 val        (502) staff       (20)     1957 2022-12-22 04:40:03.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-DevOps.md
+-rw-r--r--   0 val        (502) staff       (20)     1930 2023-01-31 22:36:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Env.md
+-rw-r--r--   0 val        (502) staff       (20)     4936 2022-11-24 20:38:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Execution.md
+-rw-r--r--   0 val        (502) staff       (20)     2446 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Rebuild.md
+-rw-r--r--   0 val        (502) staff       (20)     2104 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Structure.md
+-rw-r--r--   0 val        (502) staff       (20)      773 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Sample-Database.md
+-rw-r--r--   0 val        (502) staff       (20)     2227 2023-02-14 23:54:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Activation.md
+-rw-------   0 val        (502) staff       (20)     1585 2023-01-21 01:47:08.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authentication-Provider.md
+-rw-------   0 val        (502) staff       (20)     1470 2023-01-21 02:17:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authentication.md
+-rw-r--r--   0 val        (502) staff       (20)     1922 2023-01-06 17:06:26.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authorization.md
+-rw-r--r--   0 val        (502) staff       (20)     5277 2023-01-21 01:31:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Overview.md
+-rw-r--r--   0 val        (502) staff       (20)      155 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech--Notes.md
+-rw-r--r--   0 val        (502) staff       (20)      237 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-4GL.md
+-rw-r--r--   0 val        (502) staff       (20)     7081 2022-11-24 00:40:19.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-CodeSpaces.md
+-rw-r--r--   0 val        (502) staff       (20)     3053 2022-12-06 21:43:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md
+-rw-r--r--   0 val        (502) staff       (20)     3174 2022-12-06 18:38:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)     5693 2022-12-05 19:50:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference.md
+-rw-r--r--   0 val        (502) staff       (20)     3385 2022-11-07 18:45:42.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Docker.md
+-rw-r--r--   0 val        (502) staff       (20)      815 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Install-Python.md
+-rw-r--r--   0 val        (502) staff       (20)     1049 2022-10-03 16:52:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Proven.md
+-rw-r--r--   0 val        (502) staff       (20)     2679 2022-12-07 04:30:27.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Python-311.md
+-rw-r--r--   0 val        (502) staff       (20)     3728 2023-01-12 06:40:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Python.md
+-rw-r--r--   0 val        (502) staff       (20)     3019 2022-10-21 23:29:01.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-m1.md
+-rw-r--r--   0 val        (502) staff       (20)     1644 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-mkdocs-material.md
+-rw-r--r--   0 val        (502) staff       (20)    12291 2022-10-08 18:23:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Troubleshooting.md
+-rw-r--r--   0 val        (502) staff       (20)    15277 2023-04-27 02:31:04.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tutorial.md
+-rw-r--r--   0 val        (502) staff       (20)     6697 2022-12-02 18:42:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Working-With-Docker.md
+-rw-r--r--   0 val        (502) staff       (20)     4031 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.703499 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-08-30 03:14:41.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.703978 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/
+-rw-r--r--   0 val        (502) staff       (20)     2362 2022-08-29 00:06:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/bulb-icon.svg
+-rw-r--r--   0 val        (502) staff       (20)     3482 2022-08-30 03:46:01.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/lightbulb.svg
+-rw-r--r--   0 val        (502) staff       (20)    15440 2023-02-06 03:49:29.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/index.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.704175 ApiLogicServer-8.3.3/api_logic_server_cli/docs/stylesheets/
+-rw-r--r--   0 val        (502) staff       (20)      634 2022-08-30 03:44:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/docs/stylesheets/extra.css
+-rw-r--r--   0 val        (502) staff       (20)    11824 2023-02-11 04:16:18.000000 ApiLogicServer-8.3.3/api_logic_server_cli/extended_builder.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.705870 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/
+-rw-r--r--   0 val        (502) staff       (20)     1431 2023-02-05 02:48:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
+-rw-r--r--   0 val        (502) staff       (20)     1956 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/configZZ.py
+-rw-r--r--   0 val        (502) staff       (20)       63 2022-10-01 16:17:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/db_typesZZ.txt
+-rw-r--r--   0 val        (502) staff       (20)    12053 2023-02-05 02:48:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/modelsZZ.py
+-rw-r--r--   0 val        (502) staff       (20)      888 2023-04-23 22:57:22.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/nw_virtual_attrs.py
+-rw-r--r--   0 val        (502) staff       (20)      870 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
+-rw-r--r--   0 val        (502) staff       (20)     1006 2023-04-21 23:18:04.000000 ApiLogicServer-8.3.3/api_logic_server_cli/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.709620 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-04-26 02:43:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.710522 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      444 2023-02-05 02:50:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 21:44:41.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-01-08 18:52:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      106 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.710816 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:37.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.712859 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1127 2023-04-29 02:28:50.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml
+-rw-r--r--   0 val        (502) staff       (20)     1306 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1196 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1205 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1193 2023-04-29 01:03:03.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml
+-rw-r--r--   0 val        (502) staff       (20)     2444 2023-04-29 01:03:22.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.713433 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     6518 2023-04-13 16:38:20.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      437 2023-04-13 04:29:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.714628 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     2053 2023-04-26 02:48:17.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/customize_api.py
+-rw-r--r--   0 val        (502) staff       (20)      316 2023-01-23 01:07:06.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/expose_api_models.py
+-rw-r--r--   0 val        (502) staff       (20)      521 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/json_encoder.py
+-rw-r--r--   0 val        (502) staff       (20)     2689 2023-04-29 21:17:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/readme_customize_api.md
+-rw-r--r--   0 val        (502) staff       (20)    18920 2023-04-29 18:24:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api_logic_server_run.py
+-rw-r--r--   0 val        (502) staff       (20)     3131 2023-03-03 16:08:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.715529 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.716256 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/
+-rw-r--r--   0 val        (502) staff       (20)     2101 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/env.py
+-rw-r--r--   0 val        (502) staff       (20)     1967 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/readme.md
+-rw-r--r--   0 val        (502) staff       (20)      494 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.716400 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/versions/
+-rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     3027 2023-02-09 15:42:27.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic.ini
+-rw-r--r--   0 val        (502) staff       (20)      537 2023-01-28 17:53:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/bind_databases.py
+-rw-r--r--   0 val        (502) staff       (20)      469 2023-01-23 01:14:38.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)      139 2022-12-21 03:23:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/default.env
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.716580 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.717759 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/
+-rw-r--r--   0 val        (502) staff       (20)     2381 2023-02-26 22:13:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     3643 2023-02-25 03:16:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
+-rw-r--r--   0 val        (502) staff       (20)      331 2023-04-02 15:52:20.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     2079 2023-04-02 16:35:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
+-rw-r--r--   0 val        (502) staff       (20)      876 2023-01-07 21:19:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
+-rw-r--r--   0 val        (502) staff       (20)     1475 2023-04-21 23:01:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.718322 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/
+-rw-r--r--   0 val        (502) staff       (20)      592 2023-04-26 02:47:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)     5953 2023-04-27 00:49:20.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
+-rw-r--r--   0 val        (502) staff       (20)      568 2023-03-04 03:52:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/mypy.ini
+-rw-r--r--   0 val        (502) staff       (20)     3820 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py
+-rw-r--r--   0 val        (502) staff       (20)     7133 2023-04-29 21:44:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)      801 2022-10-19 20:24:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/run.ps1
+-rwxr-xr-x   0 val        (502) staff       (20)     1040 2022-11-09 16:08:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/run.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.719092 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-12-15 01:50:41.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.719768 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-18 05:06:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-12-14 21:51:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.722043 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      173 2022-12-14 21:55:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      928 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1803 2022-12-18 03:38:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      820 2022-12-16 14:20:29.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1392 2022-12-14 22:25:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1024 2022-12-16 15:01:05.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1619 2022-12-15 17:24:50.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      580 2022-12-19 03:03:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.722817 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.723085 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1493 2022-12-19 03:13:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     4355 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)     2907 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.561468 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.723867 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1215 2022-12-19 03:24:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2262 2022-12-19 00:39:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      839 2022-12-18 03:49:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.724095 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
+-rw-r--r--   0 val        (502) staff       (20)     2165 2023-02-15 02:24:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)      587 2023-01-23 01:02:25.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.724775 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/
+-rw-r--r--   0 val        (502) staff       (20)     1403 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
+-rw-r--r--   0 val        (502) staff       (20)     1156 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
+-rw-r--r--   0 val        (502) staff       (20)     1364 2023-01-12 23:29:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.725821 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.726100 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     4665 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3425 2023-03-03 16:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/authentication.py
+-rw-r--r--   0 val        (502) staff       (20)     6004 2023-03-03 16:56:55.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/authorization.py
+-rw-r--r--   0 val        (502) staff       (20)     1705 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.726381 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/templates/
+-rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/templates/index.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.726567 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.727351 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     9969 2022-11-29 03:36:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
+-rw-r--r--   0 val        (502) staff       (20)     1026 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.727611 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      414 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.728091 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      416 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     1518 2023-02-11 17:50:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.728953 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
+-rw-r--r--   0 val        (502) staff       (20)      147 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
+-rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
+-rw-r--r--   0 val        (502) staff       (20)    65295 2022-10-11 03:42:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.729936 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)      735 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/basic/server_test.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.730546 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 20:09:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.731029 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)     6671 2023-03-19 18:44:09.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
+-rw-r--r--   0 val        (502) staff       (20)     2750 2023-02-05 02:50:52.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/home.js
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.731325 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-26 23:48:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.733319 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.734717 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.734883 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/templates/
+-rw-r--r--   0 val        (502) staff       (20)       26 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/templates/content.html
+-rw-r--r--   0 val        (502) staff       (20)     9076 2023-03-24 00:43:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/util.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.737074 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/
+-rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-03-10 20:26:13.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/py.py
+-rw-r--r--   0 val        (502) staff       (20)      738 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
+-rw-r--r--   0 val        (502) staff       (20)      579 2023-03-03 02:36:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-02-05 02:50:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
+-rw-r--r--   0 val        (502) staff       (20)      698 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
+-rw-r--r--   0 val        (502) staff       (20)      893 2023-02-05 02:50:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.737885 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.738499 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/
+-rw-r--r--   0 val        (502) staff       (20)     8711 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/customize_api.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.739429 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/multi-table-example/
+-rw-r--r--   0 val        (502) staff       (20)    34142 2023-04-29 21:00:10.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
+-rw-r--r--   0 val        (502) staff       (20)      650 2023-04-29 21:02:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.740268 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/
+-rw-r--r--   0 val        (502) staff       (20)     2662 2023-04-24 23:31:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)      312 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/db_debug.py
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-11-16 19:24:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       29 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.740526 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/logic/
+-rw-r--r--   0 val        (502) staff       (20)    10650 2023-04-23 00:10:12.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)      241 2023-04-29 21:06:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.740820 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/security/
+-rw-r--r--   0 val        (502) staff       (20)     1158 2023-02-14 15:54:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.741157 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.741255 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.741827 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      187 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
+-rw-r--r--   0 val        (502) staff       (20)      285 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
+-rw-r--r--   0 val        (502) staff       (20)     1281 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
+-rw-r--r--   0 val        (502) staff       (20)      473 2023-04-23 23:42:07.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.742845 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      450 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     2130 2023-01-14 03:27:19.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
+-rw-r--r--   0 val        (502) staff       (20)    16642 2023-02-16 04:52:22.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
+-rw-r--r--   0 val        (502) staff       (20)     4722 2023-04-23 23:41:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.743111 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
+-rw-r--r--   0 val        (502) staff       (20)     4356 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.744937 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     5794 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     2568 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
+-rw-r--r--   0 val        (502) staff       (20)     8481 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
+-rw-r--r--   0 val        (502) staff       (20)     8445 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
+-rw-r--r--   0 val        (502) staff       (20)     2561 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.745723 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.747602 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
+-rw-r--r--   0 val        (502) staff       (20)    16926 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
+-rw-r--r--   0 val        (502) staff       (20)      840 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
+-rw-r--r--   0 val        (502) staff       (20)     1381 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
+-rw-r--r--   0 val        (502) staff       (20)      831 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
+-rw-r--r--   0 val        (502) staff       (20)     8405 2023-03-10 20:26:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
+-rw-r--r--   0 val        (502) staff       (20)    13497 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
+-rw-r--r--   0 val        (502) staff       (20)     1543 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.747785 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/
+-rw-r--r--   0 val        (502) staff       (20)     8196 2022-11-11 23:20:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.748769 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)    17259 2023-04-24 23:38:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     3443 2023-02-05 02:51:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
+-rw-r--r--   0 val        (502) staff       (20)     8798 2022-12-30 19:58:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.749175 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-11 23:17:05.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.750904 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.752387 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.752574 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw_no_cust/
+-rw-r--r--   0 val        (502) staff       (20)     5431 2023-02-05 02:51:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.754309 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:04:24.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.755904 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      446 2023-02-05 02:55:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 02:52:45.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      215 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.756150 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:05:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.758823 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:30:57.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1141 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml
+-rw-r--r--   0 val        (502) staff       (20)     1162 2023-02-14 05:07:31.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml
+-rw-r--r--   0 val        (502) staff       (20)     1174 2023-02-14 05:17:54.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1148 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml
+-rw-r--r--   0 val        (502) staff       (20)     1160 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml
+-rw-r--r--   0 val        (502) staff       (20)     1142 2023-02-14 05:16:08.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml
+-rw-r--r--   0 val        (502) staff       (20)     1204 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1386 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.759488 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     5986 2023-04-13 16:51:25.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      100 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.761554 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-27 01:16:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.762950 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1238 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3435 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3970 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3439 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5965 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.763099 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
+-rw-r--r--   0 val        (502) staff       (20)     2895 2023-02-28 05:23:15.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
+-rw-r--r--   0 val        (502) staff       (20)     2058 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.764738 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.765018 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     8571 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)    11838 2023-01-28 17:14:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
+-rw-r--r--   0 val        (502) staff       (20)     1452 2023-02-27 23:00:55.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)     3530 2023-02-28 05:20:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     7699 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
+-rw-r--r--   0 val        (502) staff       (20)    21134 2023-04-14 00:57:12.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-04-02 02:53:45.000000 ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/sample_db.sqlite
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.766602 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)      369 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-01-03 23:29:33.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.768327 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      175 2023-01-03 23:29:48.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      191 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     8054 2022-11-17 03:31:49.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    14080 2023-02-17 01:02:20.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    21445 2023-04-29 17:29:36.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1755 2023-02-01 19:08:47.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    53944 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
+-rw-r--r--   0 val        (502) staff       (20)       54 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.769702 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)     1850 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
+-rw-r--r--   0 val        (502) staff       (20)     2593 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
+-rw-r--r--   0 val        (502) staff       (20)     3865 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.770127 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      183 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      203 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)       87 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
+-rw-r--r--   0 val        (502) staff       (20)     1399 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)      196 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.771042 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.772280 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      195 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      215 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    32358 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    74447 2023-04-06 14:36:23.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    58988 2023-04-06 14:31:39.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
+-rw-r--r--   0 val        (502) staff       (20)     3252 2022-11-18 19:19:33.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.772893 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
+-rw-r--r--   0 val        (502) staff       (20)    33384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
+-rw-r--r--   0 val        (502) staff       (20)      440 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
+-rwxr-xr-x   0 val        (502) staff       (20)    17236 2023-04-29 17:29:32.000000 ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-29 22:01:05.775255 ApiLogicServer-8.3.3/api_logic_server_cli/templates/
+-rw-r--r--   0 val        (502) staff       (20)    14864 2023-03-29 21:47:30.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     1221 2023-03-29 20:25:21.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/app_fiddle.md
+-rw-r--r--   0 val        (502) staff       (20)     3322 2023-04-13 17:12:40.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/app_fiddle.txt
+-rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/index.html
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-01-19 01:43:35.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/login_endpoint.txt
+-rw-r--r--   0 val        (502) staff       (20)      205 2023-01-19 01:44:07.000000 ApiLogicServer-8.3.3/api_logic_server_cli/templates/login_endpoint_imports.txt
+-rw-r--r--   0 val        (502) staff       (20)       38 2023-04-29 22:01:05.776079 ApiLogicServer-8.3.3/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)     3521 2023-04-26 19:16:06.000000 ApiLogicServer-8.3.3/setup.py
```

### Comparing `ApiLogicServer-8.3.0/ApiLogicServer.egg-info/PKG-INFO` & `ApiLogicServer-8.3.3/ApiLogicServer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 8.3.0
+Version: 8.3.3
 Summary: Create JSON:API and Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/ApiLogicServer
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://valhuber.github.io/ApiLogicServer/
 Platform: any
@@ -263,48 +263,37 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+04/29/2023 - 08.03.03: restore missing debug info for open database failures
+
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
-04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships (Issue 65)
-
-03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4 
-
-03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3
+03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4
 
 02/15/2023 - 08.00.01: Declarative Authorization and Authentication
 
 01/05/2023 - 07.00.00: Multi-db, sqlite test dbs, tests run, security prototype, env config
 
-12/21/2022 - 06.05.00: devops, env db uri, api endpoint names, git-push-new-project
-
-12/08/2022 - 06.04.05: Clarify creating docker repo, IP info, logic comments, nested result example
-
 11/22/2022 - 06.03.06: Image, Chkbox, Dialects, run.sh, SQL/Server url change, stop endpoint, Chinook Sqlite
 
 10/02/2022 - 06.02.00: Option infer_primary_key, Oct1 SRA (issue 49), cleanup db/api setup, restore postgres dvr
 
 09/15/2022 - 06.01.00: Multi-app Projects
 
 08/28/2022 - 06.00.01: Admin App show_when, cascade add. Simplify Codespaces swagger url & use default config
 
 06/12/2022 - 05.02.22: No pyodbc by default, model customizations simplified, better logging
 
-05/30/2022 - 05.02.16: Python 3.10, Dockerfile include, start info
-
 05/04/2022 - 05.02.03: alembic for database migrations, admin-merge.yaml
 
 04/27/2022 - 05.01.02: copy_children, with support for nesting (children and grandchildren, etc.)
 
 03/27/2022 - 05.00.06: Introducing [Behave test framework](https://apilogicserver.github.io/Docs/Logic-Tutorial/), LogicBank bugfix
 
 12/26/2021 - 04.00.05: Introducing the Admin app, with Readme Tutorial
 
-11/13/2021 - 03.50.01: rebuild-from-database/model, improved relationship support 
-
-09/15/2021 - 03.00.09: auto-create .devcontainer for vscode, configure network, python & debug
```

### Comparing `ApiLogicServer-8.3.0/ApiLogicServer.egg-info/SOURCES.txt` & `ApiLogicServer-8.3.3/ApiLogicServer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -421,18 +421,19 @@
 api_logic_server_cli/project_prototype/run.sh
 api_logic_server_cli/project_prototype/util.py
 api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
 api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
 api_logic_server_cli/project_prototype/.devcontainer/setup.sh
 api_logic_server_cli/project_prototype/.idea/.DS_Store
 api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
+api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml
 api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
 api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
 api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
-api_logic_server_cli/project_prototype/.idea/runConfigurations/run.xml
+api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml
 api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
 api_logic_server_cli/project_prototype/.vscode/launch.json
 api_logic_server_cli/project_prototype/.vscode/settings.json
 api_logic_server_cli/project_prototype/api/__init__.py
 api_logic_server_cli/project_prototype/api/customize_api.py
 api_logic_server_cli/project_prototype/api/expose_api_models.py
 api_logic_server_cli/project_prototype/api/json_encoder.py
@@ -519,14 +520,16 @@
 api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
 api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
 api_logic_server_cli/project_prototype/venv_setup/venv.ps1
 api_logic_server_cli/project_prototype/venv_setup/venv.sh
 api_logic_server_cli/project_prototype_nw/.DS_Store
 api_logic_server_cli/project_prototype_nw/readme.md
 api_logic_server_cli/project_prototype_nw/api/customize_api.py
+api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
+api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
 api_logic_server_cli/project_prototype_nw/database/customize_models.py
 api_logic_server_cli/project_prototype_nw/database/db_debug.py
 api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
 api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
 api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
 api_logic_server_cli/project_prototype_nw/security/declare_security.py
 api_logic_server_cli/project_prototype_nw/test/__init__.py
```

### Comparing `ApiLogicServer-8.3.0/ApiLogicServer.egg-info/requires.txt` & `ApiLogicServer-8.3.3/ApiLogicServer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/LICENSE` & `ApiLogicServer-8.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/MANIFEST.in` & `ApiLogicServer-8.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/PKG-INFO` & `ApiLogicServer-8.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 8.3.0
+Version: 8.3.3
 Summary: Create JSON:API and Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/ApiLogicServer
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://valhuber.github.io/ApiLogicServer/
 Platform: any
@@ -263,48 +263,37 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+04/29/2023 - 08.03.03: restore missing debug info for open database failures
+
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
-04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships (Issue 65)
-
-03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4 
-
-03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3
+03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4
 
 02/15/2023 - 08.00.01: Declarative Authorization and Authentication
 
 01/05/2023 - 07.00.00: Multi-db, sqlite test dbs, tests run, security prototype, env config
 
-12/21/2022 - 06.05.00: devops, env db uri, api endpoint names, git-push-new-project
-
-12/08/2022 - 06.04.05: Clarify creating docker repo, IP info, logic comments, nested result example
-
 11/22/2022 - 06.03.06: Image, Chkbox, Dialects, run.sh, SQL/Server url change, stop endpoint, Chinook Sqlite
 
 10/02/2022 - 06.02.00: Option infer_primary_key, Oct1 SRA (issue 49), cleanup db/api setup, restore postgres dvr
 
 09/15/2022 - 06.01.00: Multi-app Projects
 
 08/28/2022 - 06.00.01: Admin App show_when, cascade add. Simplify Codespaces swagger url & use default config
 
 06/12/2022 - 05.02.22: No pyodbc by default, model customizations simplified, better logging
 
-05/30/2022 - 05.02.16: Python 3.10, Dockerfile include, start info
-
 05/04/2022 - 05.02.03: alembic for database migrations, admin-merge.yaml
 
 04/27/2022 - 05.01.02: copy_children, with support for nesting (children and grandchildren, etc.)
 
 03/27/2022 - 05.00.06: Introducing [Behave test framework](https://apilogicserver.github.io/Docs/Logic-Tutorial/), LogicBank bugfix
 
 12/26/2021 - 04.00.05: Introducing the Admin app, with Readme Tutorial
 
-11/13/2021 - 03.50.01: rebuild-from-database/model, improved relationship support 
-
-09/15/2021 - 03.00.09: auto-create .devcontainer for vscode, configure network, python & debug
```

### Comparing `ApiLogicServer-8.3.0/README.md` & `ApiLogicServer-8.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -239,48 +239,37 @@
 
 
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+04/29/2023 - 08.03.03: restore missing debug info for open database failures
+
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
 
-04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships (Issue 65)
-
-03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4 
-
-03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3
+03/23/2023 - 08.01.15: table filters, cloud debug additions, issue 59, 62-4
 
 02/15/2023 - 08.00.01: Declarative Authorization and Authentication
 
 01/05/2023 - 07.00.00: Multi-db, sqlite test dbs, tests run, security prototype, env config
 
-12/21/2022 - 06.05.00: devops, env db uri, api endpoint names, git-push-new-project
-
-12/08/2022 - 06.04.05: Clarify creating docker repo, IP info, logic comments, nested result example
-
 11/22/2022 - 06.03.06: Image, Chkbox, Dialects, run.sh, SQL/Server url change, stop endpoint, Chinook Sqlite
 
 10/02/2022 - 06.02.00: Option infer_primary_key, Oct1 SRA (issue 49), cleanup db/api setup, restore postgres dvr
 
 09/15/2022 - 06.01.00: Multi-app Projects
 
 08/28/2022 - 06.00.01: Admin App show_when, cascade add. Simplify Codespaces swagger url & use default config
 
 06/12/2022 - 05.02.22: No pyodbc by default, model customizations simplified, better logging
 
-05/30/2022 - 05.02.16: Python 3.10, Dockerfile include, start info
-
 05/04/2022 - 05.02.03: alembic for database migrations, admin-merge.yaml
 
 04/27/2022 - 05.01.02: copy_children, with support for nesting (children and grandchildren, etc.)
 
 03/27/2022 - 05.00.06: Introducing [Behave test framework](https://apilogicserver.github.io/Docs/Logic-Tutorial/), LogicBank bugfix
 
 12/26/2021 - 04.00.05: Introducing the Admin app, with Readme Tutorial
 
-11/13/2021 - 03.50.01: rebuild-from-database/model, improved relationship support 
-
-09/15/2021 - 03.00.09: auto-create .devcontainer for vscode, configure network, python & debug
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/api_logic_server.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/api_logic_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,18 @@
         * api/expose_api_models.py for a safrs api  - using introspected models.py
     * Special provisions for NW Sample, to show customizations.
     * See end for key module map quick links...
 
 Called from api_logic_server_cli.py, by instantiating the ProjectRun object.
 '''
 
-__version__ = "08.03.00"
+__version__ = "08.03.03"
 recent_changes = \
     f'\n\nRecent Changes:\n' +\
+    "\t04/29/2023 - 08.03.03: connect error reporting, startup logging \n"\
     "\t04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, readme updates, LogicBank 1.8.4 \n"\
     "\t04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65) \n"\
     "\t04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships \n"\
     "\t03/23/2023 - 08.01.15: cloud debug additions, issue 59, 62-4, table filters \n"\
     "\t03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3 \n"\
     "\t02/15/2023 - 08.00.01: Declarative Authorization and Authentication, Werkzeug==2.2.3 \n"\
     "\t01/10/2023 - 07.00.04: Portable projects, server_proxy  \n"\
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/cli.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/cli.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/cli_args_base.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/cli_args_base.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/cli_args_project.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/cli_args_project.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/api_logic_server_utils.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/model_creation_services.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/model_creation_services.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/create_admin.sh` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/create_admin.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/fab_config.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/fab_config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/home.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/templates/react_admin_component.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/ui_admin_creator.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/ui_admin_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/create_from_model/uri_info.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/create_from_model/uri_info.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/Chinook_Sqlite.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/authentication.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/authentication.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/classicmodels.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/classicmodels.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/new.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/new.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/nw-gold-plus.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/nw-gold-plus.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/nw-gold.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/nw-gold.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/nw.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/nw.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/table_filters_tests.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/table_filters_tests.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/database/todos.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/database/todos.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/API-Customize.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/API-Customize.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/API.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/API.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Admin-Customization.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Admin-Customization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Admin-Tour.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Admin-Tour.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Architecture.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Architecture.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Behave-Logic-Report.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Behave-Logic-Report.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Behave.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Behave.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Create-ApiLogicProject.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Create-ApiLogicProject.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Classes.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Classes.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Customization.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Customization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Examples.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Examples.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Keys.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Keys.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Data-Model-Multi.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Data-Model-Multi.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Database-Connectivity.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Database-Connectivity.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Execute.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Execute.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-Frameworks.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-Frameworks.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-Low-Code.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-Low-Code.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/FAQ-RETE.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/FAQ-RETE.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/IDE-Customize.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/IDE-Customize.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/IDE-Execute.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/IDE-Execute.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Eval-x.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Eval-x.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Eval.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Eval.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Express-x.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Express-x.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-Express.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-Express.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-psycopg2.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-psycopg2.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install-pyodbc.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install-pyodbc.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Install.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Install.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Internals-CLI.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Internals-CLI.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Internals.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Internals.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Operation.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Operation.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Tutorial.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic-Why.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic-Why.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Logic.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Logic.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Manage-GitHub.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Manage-GitHub.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Builders.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Builders.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-DevOps.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-DevOps.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Env.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Env.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Execution.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Execution.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Rebuild.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Rebuild.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Project-Structure.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Project-Structure.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Sample-Database.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Sample-Database.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Activation.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Activation.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authentication-Provider.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authentication-Provider.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authentication.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authentication.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Authorization.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Authorization.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Security-Overview.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Security-Overview.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-CodeSpaces.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-CodeSpaces.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Conference.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Conference.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Docker.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Docker.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Install-Python.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Install-Python.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Proven.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Proven.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Python-311.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Python-311.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-Python.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-Python.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-m1.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-m1.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tech-mkdocs-material.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tech-mkdocs-material.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Troubleshooting.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Troubleshooting.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Tutorial.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Tutorial.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Working-With-Docker.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Working-With-Docker.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/bulb-icon.svg` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/bulb-icon.svg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/assets/images/lightbulb.svg` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/assets/images/lightbulb.svg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/index.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/index.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/docs/stylesheets/extra.css` & `ApiLogicServer-8.3.3/api_logic_server_cli/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/extended_builder.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/extended_builder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/Todo_modelsZZ.py.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/Todo_modelsZZ.py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/configZZ.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/configZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/modelsZZ.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/modelsZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/nw_virtual_attrs.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/nw_virtual_attrs.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/logging.yml` & `ApiLogicServer-8.3.3/api_logic_server_cli/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml`

 * *Files 6% similar despite different names*

#### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml`

```diff
@@ -1,23 +1,23 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component name="ProjectRunConfigurationManager">
-  <configuration default="false" name="run" type="PythonConfigurationType" factoryName="Python">
-    <module name="ApiLogicProject"/>
+  <configuration default="false" name="Execute classicmodels" type="PythonConfigurationType" factoryName="Python">
+    <module name="tutorial"/>
     <option name="INTERPRETER_OPTIONS" value=""/>
     <option name="PARENT_ENVS" value="true"/>
     <envs>
       <env name="PYTHONUNBUFFERED" value="1"/>
     </envs>
-    <option name="SDK_HOME" value=""/>
-    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
-    <option name="IS_MODULE_SDK" value="true"/>
+    <option name="SDK_HOME" value="$PROJECT_DIR$/../venv/bin/python"/>
+    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/classicmodels"/>
+    <option name="IS_MODULE_SDK" value="false"/>
     <option name="ADD_CONTENT_ROOTS" value="true"/>
     <option name="ADD_SOURCE_ROOTS" value="true"/>
     <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
-    <option name="SCRIPT_NAME" value="$PROJECT_DIR$/api_logic_server_run.py"/>
+    <option name="SCRIPT_NAME" value="api_logic_server_run.py"/>
     <option name="PARAMETERS" value=""/>
     <option name="SHOW_COMMAND_LINE" value="false"/>
     <option name="EMULATE_TERMINAL" value="false"/>
     <option name="MODULE_MODE" value="false"/>
     <option name="REDIRECT_INPUT" value="false"/>
     <option name="INPUT_FILE" value=""/>
     <method v="2"/>
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml`

 * *Files 2% similar despite different names*

#### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component name="ProjectRunConfigurationManager">
-  <configuration default="false" name="run docker" type="PythonConfigurationType" factoryName="Python">
+  <configuration default="false" name="ApiLogicServer docker" type="PythonConfigurationType" factoryName="Python">
     <module name="py-ApiLogicProject"/>
     <option name="INTERPRETER_OPTIONS" value=""/>
     <option name="PARENT_ENVS" value="true"/>
     <envs>
       <env name="PYTHONUNBUFFERED" value="1"/>
     </envs>
     <option name="SDK_HOME" value="docker://apilogicserver/api_logic_server:latest/python"/>
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/.vscode/launch.json` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/customize_api.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/customize_api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/json_encoder.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api/readme_customize_api.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api/readme_customize_api.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-This describes how to add endpoints; for more information, [see here](https://apilogicserver.github.io/Docs/API-Customize).
+Without customization, your API supports multi-table retrieval.  For more information, [see here](https://apilogicserver.github.io/Docs/API-Multi-Table).
+
+This describes how to *add new endpoints*.  For more information, [see here](https://apilogicserver.github.io/Docs/API-Customize).
 
 &nbsp;
 
 ## Examples      
 Examples from tutorial project:
 * Examples drawn from [tutorial project](https://github.com/ApiLogicServer/demo/blob/main/api/customize_api.py)
 * Use Shift + "." to view in project mode
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/api_logic_server_run.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/api_logic_server_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,25 @@
 
     See Main Code (at end).
         Use log messages to understand API and Logic activation.
 
 ==============================================================================
 """
 
-import os, logging, logging.config, sys, yaml  # failure here means venv probably not set
+import traceback
+try:
+    import os, logging, logging.config, sys, yaml  # failure here means venv probably not set
+except:
+    track = traceback.format_exc()
+    print(" ")
+    print(track)
+    print("venv probably not set")
+    print("Please see https://apilogicserver.github.io/Docs/Project-Env/ \n")
+    exit(1)
+
 from flask_sqlalchemy import SQLAlchemy
 import json
 from pathlib import Path
 
 def is_docker() -> bool:
     """ running docker?  dir exists: /home/api_logic_server """
     path = '/home/api_logic_server'
@@ -52,14 +62,17 @@
 http_type = "http"
 
 current_path = os.path.abspath(os.path.dirname(__file__))
 sys.path.append(current_path)
 project_dir = str(current_path)
 os.chdir(project_dir)  # so admin app can find images, code
 import util as util
+logic_logger_activate_debug = False
+""" True prints all rules on startup """
+
 
 
 # ==================================
 #       LOGGING SETUP
 # ================================== 
 
 current_path = os.path.abspath(os.path.dirname(__file__))
@@ -274,14 +287,16 @@
 # ==========================================================
 
 def create_app(swagger_host: str = "localhost", swagger_port: str = "5656"):
     """ Creates flask_app, Opens Database, Activates API and Logic """ 
 
     from sqlalchemy import exc as sa_exc
 
+    global logic_logger_activate_debug
+
     with warnings.catch_warnings():
 
         flask_app = Flask("API Logic Server", template_folder='ui/templates')  # templates to load ui/admin/admin.yaml
 
         setup_logging(flask_app)        
         safrs_log_level = safrs.log.getEffectiveLevel()
         db_logger = logging.getLogger('sqlalchemy')
@@ -328,16 +343,21 @@
             from api import expose_api_models, customize_api
 
             import database.models
             app_logger.info("Data Model Loaded, customizing...")
             from database import customize_models
 
             from logic import declare_logic
+            logic_logger = logging.getLogger('logic_logger')
+            logic_logger_level = logic_logger.getEffectiveLevel()
+            if logic_logger_activate_debug == False:
+                logic_logger.setLevel(logging.INFO)
             app_logger.info("")
             LogicBank.activate(session=session, activator=declare_logic.declare_logic, constraint_event=constraint_handler)
+            logic_logger.setLevel(logic_logger_level)
             app_logger.info("Declare   Logic complete - logic/declare_logic.py (rules + code)"
                 + f' -- {len(database.models.metadata.tables)} tables loaded\n')  # db opened 1st access
             
             method_decorators : list = []
             expose_api_models.expose_models(safrs_api, method_decorators)
             app_logger.info(f'Declare   API - api/expose_api_models, endpoint for each table on {swagger_host}:{swagger_port}, customizing...')
             customize_api.expose_services(flask_app, safrs_api, project_dir, swagger_host=swagger_host, PORT=port)  # custom services
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/config.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/env.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic/readme.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/alembic.ini` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/alembic.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/database/bind_databases.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/database/bind_databases.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/docker/build_image.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logging.yml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logic/declare_logic.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/declare_logic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/mypy.ini` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/mypy.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/readme.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,110 @@
-# Readme - API Logic Project
-
-This API Logic Project was created by the API Logic Server with the `ApiLogicServer create` command.  
-
-Edit / extend this readme as desired.
-
-&nbsp;&nbsp;
-
 # Setup and Run
 
-To run your project, the system requires various runtime systems for data access, api, and logic.  These are [included with API Logic Server](https://apilogicserver.github.io/Docs/Architecture-What-Is/).  So, to run your project:
+To run your project, the system requires various runtime systems for data access, api, and logic.  These are included with API Logic Server ([architecture doc here](https://apilogicserver.github.io/Docs/Architecture-What-Is/)).  So, to run your project ([instructions here](#setup-instructions)):
 
-1.  __Establish your Python Environment__ to activate these runtime systems
-    * Choose the __either__ the _Local Install_ __or__ the _Docker_ approach below, then 
+1.  __Establish your Python Environment__ to activate these runtime system
 2. __Run__
 
-For instructions, [see here](#setup-instructions).
-
 &nbsp;
 
-# Project Structure
-This project was created with the directory structure shown below.
+# Key Customization Files
+
+Your project is ready to run, but it's likely you'll want to customize it - declare logic, new endpoints, etc.
+
+The ___Key Customization Files___ listed in the table below are created as stubs, intended for you to add customizations that extend
+the created API, Logic and Web App.
 
-The ___Key Customization Files___ in the table are created as stubs, intended for you to add customizations that extend
-the created API, Logic and Web App.  Since they are separate files, the project can be
+* Since they are separate files, the project can be
 [rebuilt](https://apilogicserver.github.io/Docs/Project-Rebuild/) (e.g., synchronized with a revised schema), preserving your customizations.
 
-Please see the ```nw``` sample for examples of typical customizations.  You can open it in GitHub (use Shift + "." to view in project mode) - [click here](https://github.com/ApiLogicServer/demo).
+Please see the `nw` sample for examples of typical customizations.  You can open it in GitHub (use Shift + "." to view in project mode) - [click here](https://github.com/ApiLogicServer/demo).
 
 | Directory | Usage                         | Key Customization File             | Typical Customization                                                                 |
 |:-------------- |:------------------------------|:-----------------------------------|:--------------------------------------------------------------------------------------|
 | ```api``` | JSON:API                      | ```api/customize_api.py```         | Add new end points / services                                                         |
 | ```database``` | SQLAlchemy Data Model Classes | ```database/customize_models.py``` | Add derived attributes, and relationships missing in the schema                       |
 | ```logic``` | Transactional Logic           | ```logic/declare_logic.py```       | Declare multi-table derivations, constraints, and events such as send mail / messages |
 | ```ui``` | Admin App                     | ```ui/admin/admin.yaml```          | Control field display - order, captions etc.                                          |
 | ```security``` | Authentication, Authorization   | ```security/declare_security.py```          | Control login, role-based row access         |
 | ```tests``` | Behave Test Suite              | ```tests/api_logic_server_behave/features```          | Declare and implement [Behave Tests](https://apilogicserver.github.io/Docs/Behave/)                                          |
 
 &nbsp;
 
 # Project Information
 
+This API Logic Project was created with the `ApiLogicServer create` command.
+For information on Managing API Logic Projects, [click here](https://apilogicserver.github.io/Docs/Project-Structure).
+
 | About                    | Info                               |
 |:-------------------------|:-----------------------------------|
 | Created                  | creation-date                      |
 | API Logic Server Version | api_logic_server_version           |
 | Created in directory     | api_logic_server_project_directory |
 | API Name                 | api_logic_server_api_name          |
+| Execution begins with    | `api_logic_server_run.py`          |
+
+&nbsp;
+
+# Setup Instructions
+
+Setup your Python environment, according to whether you did a *local install*, or *Docker*.  Choose the appropriate section, then run.
+
+&nbsp;
+
+## Establish Your Python Environment - Local Install
+
+You `requirements.txt` has already been created, so...
+
+```bash title="Install API Logic Server in a Virtual Environment"
+python -m venv venv                        # may require python3 -m venv venv
+venv\Scripts\activate                      # mac/linux: source venv/bin/activate
+python -m pip install -r requirements.txt  # accept "new Virtual environment"
+```
+
+Notes:
+
+* See also the `venv_setup` directory in this API Logic Project.
+
+* If using SqlServer, install `pyodbc`.  Not required for docker-based projects.  For local installs, see the [Quick Start](https://apilogicserver.github.io/Docs/Install-pyodbc/).
+
+&nbsp;
+
+## Establish Your Python Environment - Docker
+
+Your runtime systems are part of Dev Container, which you probably activated when you [opened the project](https://apilogicserver.github.io/Docs/IDE-Execute/).  
+ * If you did not accept the "Open in Container" option when you started VSCode, use __View > Command Palette > Remote-Containers: Reopen in Container__.
+
+&nbsp;
+
+## Run
+
+To run your project
+
+![Start Project](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/nutshell/project-executable.png?raw=true)
+
+As shown above:
+
+1. Use the pre-supplied Run Configuration
+2. Click the url in the console to start the Admin App
+    * Use it to explore your data (shown below)
+    * And your API (via Swagger)
+
+![Admin App](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/ui-admin/run-admin-app.png?raw=true)
 
 
 &nbsp;
 
-# Key Technologies
+# Appendix: Key Technologies
 
 API Logic Server is based on the projects shown below.
 Consult their documentation for important information.
 
+&nbsp;
+
 ### SARFS JSON:API Server
 
 [SAFRS: Python OpenAPI & JSON:API Framework](https://github.com/thomaxxl/safrs)
 
 SAFRS is an acronym for SqlAlchemy Flask-Restful Swagger.
 The purpose of this framework is to help python developers create
 a self-documenting JSON API for sqlalchemy database objects and relationships.
@@ -70,88 +116,45 @@
 Class and method descriptions and examples can be provided
 in yaml syntax in the code comments.
 
 The description is parsed and shown in the swagger web interface.
 The result is an easy-to-use
 swagger/OpenAPI and JSON:API compliant API implementation.
 
-### LogicBank
+&nbsp;
 
+### LogicBank
 [Transaction Logic for SQLAlchemy Object Models](https://apilogicserver.github.io/Docs/Logic-Why/)
 
 Use Logic Bank to govern SQLAlchemy update transaction logic - 
 multi-table derivations, constraints, and actions such as sending mail or messages. Logic consists of _both:_
 
 *   **Rules - 40X** more concise using a spreadsheet-like paradigm, and
 
 *   **Python - control and extensibility,** using standard tools and techniques
 
 Logic Bank is based on SQLAlchemy - it handles `before_flush` events to enforce your logic.
 Your logic therefore applies to any SQLAlchemy-based access - JSON:Api, Admin App, etc.
 
+&nbsp;
 
 ### SQLAlchemy
 
 [Object Relational Mapping for Python](https://docs.sqlalchemy.org/en/13/).
 
 SQLAlchemy provides Python-friendly database access for Python.
 
 It is used by JSON:Api, Logic Bank, and the Admin App.
 
 SQLAlchemy processing is based on Python `model` classes,
 created automatically by API Logic Server from your database,
 and saved in the `database` directory.
 
+&nbsp;
 
 ### Admin App
 
 This generated project also contains a React Admin app:
 * Multi-page - including page transitions to "drill down"
 * Multi-table - master / details (with tab sheets)
 * Intelligent layout - favorite fields first, predictive joins, etc
-* Logic Aware - updates are monitored by business logic
-
-
-&nbsp;
-
-# Setup Instructions
-
-&nbsp;
-
-## Establish Your Python Environment - Local Install
-
-You `requirements.txt` has already been created, so...
-
-```bash title="Install API Logic Server in a Virtual Environment"
-python -m venv venv                        # may require python3 -m venv venv
-venv\Scripts\activate                      # mac/linux: source venv/bin/activate
-python -m pip install -r requirements.txt  # accept "new Virtual environment"
-```
-
-Notes:
-
-* See also the `venv_setup` directory in this API Logic Project.
-
-* If using SqlServer, install `pyodbc`.  Not required for docker-based projects.  For local installs, see the [Quick Start](https://apilogicserver.github.io/Docs/Install-pyodbc/).
-
-&nbsp;
-
-## Establish Your Python Environment - Docker
-
-Your runtime systems are part of Dev Container, which you probably activated when you [opened the project](https://apilogicserver.github.io/Docs/IDE-Execute/).  If you did not accept the "Open in Container" option when you started VSCode, use __View > Command Palette > Remote-Containers: Reopen in Container__.
-
-&nbsp;
-
-## Run
-
-To run your project
-
-![Start Project](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/nutshell/project-executable.png?raw=true)
-
-As shown above:
-
-1. Use the pre-supplied Run Configuration
-2. Click the url in the console to start the Admin App
-    * Use it to explore your data (shown below)
-    * And your API (via Swagger)
-
-![Admin App](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/ui-admin/run-admin-app.png?raw=true)
+* Logic Aware - updates are monitored by business logic
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/run.ps1` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/run.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/run.sh` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/run.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/declare_security.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/notes_temp/token.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/authentication.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/authentication.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/authorization.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/authorization.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/security/system/custom_swagger.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/templates/index.html` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/test/basic/server_test.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/admin/home.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/util.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/util.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/py.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/venv_setup/venv.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/api/customize_api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/database/customize_models.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/database/customize_models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype_nw_no_cust/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml`

 * *Files 8% similar despite different names*

#### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component name="ProjectRunConfigurationManager">
-  <configuration default="false" name="Execute classicmodels" type="PythonConfigurationType" factoryName="Python">
+  <configuration default="false" name="Execute todo" type="PythonConfigurationType" factoryName="Python">
     <module name="tutorial"/>
     <option name="INTERPRETER_OPTIONS" value=""/>
     <option name="PARENT_ENVS" value="true"/>
     <envs>
       <env name="PYTHONUNBUFFERED" value="1"/>
     </envs>
     <option name="SDK_HOME" value="$PROJECT_DIR$/../venv/bin/python"/>
-    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/classicmodels"/>
+    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/todo"/>
     <option name="IS_MODULE_SDK" value="false"/>
     <option name="ADD_CONTENT_ROOTS" value="true"/>
     <option name="ADD_SOURCE_ROOTS" value="true"/>
     <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
     <option name="SCRIPT_NAME" value="api_logic_server_run.py"/>
     <option name="PARAMETERS" value=""/>
     <option name="SHOW_COMMAND_LINE" value="false"/>
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml`

 * *Files 4% similar despite different names*

#### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml`

```diff
@@ -1,23 +1,23 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component name="ProjectRunConfigurationManager">
-  <configuration default="false" name="Execute todo" type="PythonConfigurationType" factoryName="Python">
-    <module name="tutorial"/>
+  <configuration default="false" name="ApiLogicServer" type="PythonConfigurationType" factoryName="Python">
+    <module name="ApiLogicProject"/>
     <option name="INTERPRETER_OPTIONS" value=""/>
     <option name="PARENT_ENVS" value="true"/>
     <envs>
       <env name="PYTHONUNBUFFERED" value="1"/>
     </envs>
-    <option name="SDK_HOME" value="$PROJECT_DIR$/../venv/bin/python"/>
-    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/todo"/>
-    <option name="IS_MODULE_SDK" value="false"/>
+    <option name="SDK_HOME" value=""/>
+    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+    <option name="IS_MODULE_SDK" value="true"/>
     <option name="ADD_CONTENT_ROOTS" value="true"/>
     <option name="ADD_SOURCE_ROOTS" value="true"/>
     <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
-    <option name="SCRIPT_NAME" value="api_logic_server_run.py"/>
+    <option name="SCRIPT_NAME" value="$PROJECT_DIR$/api_logic_server_run.py"/>
     <option name="PARAMETERS" value=""/>
     <option name="SHOW_COMMAND_LINE" value="false"/>
     <option name="EMULATE_TERMINAL" value="false"/>
     <option name="MODULE_MODE" value="false"/>
     <option name="REDIRECT_INPUT" value="false"/>
     <option name="INPUT_FILE" value=""/>
     <method v="2"/>
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/.vscode/launch.json` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/readme.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/project_tutorial/sample_db.sqlite` & `ApiLogicServer-8.3.3/api_logic_server_cli/project_tutorial/sample_db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x0e270d64 (Sun Mar 12 01:12:46 2023 UTC)
-files sz: 17212
+moddate:  0xfc534d64 (Sat Apr 29 17:29:32 2023 UTC)
+files sz: 17236
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x970064005a00640164026c015a01640164026c025a02640164026c035a
@@ -1620,40 +1620,35 @@
          code
             0x97007401000000000000000000007c006a010000000000000000a60100
             00ab0100000000000000007d017405000000000000000000007c01a60100
             00ab0100000000000000007d027c006a030000000000000000721a7c006a
             030000000000000000a00400000000000000000000000000000000000000
             006401a6010000ab0100000000000000006e0164027d0309007c02a00500
             000000000000000000000000000000000000007c01a6010000ab01000000
-            000000000001006ecb23000100740d000000000000000000006a07000000
+            000000000001006e8023000100740d000000000000000000006a07000000
             0000000000a6000000ab0000000000000000007d04741000000000000000
             000000a00900000000000000000000000000000000000000007c04a60100
             00ab0100000000000000000100741000000000000000000000a009000000
             000000000000000000000000000000000064037c006a0100000000000000
             009b0064049d03a6010000ab010000000000000000010074100000000000
             0000000000a00900000000000000000000000000000000000000006405a6
-            010000ab0100000000000000000100741500000000000000000000a60000
-            00ab0000000000000000000100741000000000000000000000a009000000
-            000000000000000000000000000000000064037c006a0100000000000000
-            009b0064069d03a6010000ab010000000000000000010074100000000000
-            0000000000a00900000000000000000000000000000000000000006407a6
-            010000ab01000000000000000001007417000000000000000000006408a6
-            010000ab010000000000000000010059006e0378035900770164097c006a
-            010000000000000000760072157c01a00c00000000000000000000000000
-            00000000000000640aa6010000ab0100000000000000000100741b000000
-            00000000000000a6000000ab0000000000000000007d05741d0000000000
-            00000000007c027c006a0f00000000000000007c006a1000000000000000
-            007c006a1100000000000000007c006a1200000000000000007c006a1300
-            000000000000007c006a140000000000000000a6070000ab070000000000
-            0000007d067c066a1500000000000000007c006a1400000000000000005f
-            1500000000000000007c06a0160000000000000000000000000000000000
-            0000007c05a6010000ab01000000000000000001007c05a0170000000000
+            010000ab01000000000000000001007415000000000000000000006406a6
+            010000ab010000000000000000010059006e0378035900770164077c006a
+            010000000000000000760072157c01a00b00000000000000000000000000
+            000000000000006408a6010000ab01000000000000000001007419000000
+            00000000000000a6000000ab0000000000000000007d05741b0000000000
+            00000000007c027c006a0e00000000000000007c006a0f00000000000000
+            007c006a1000000000000000007c006a1100000000000000007c006a1200
+            000000000000007c006a130000000000000000a6070000ab070000000000
+            0000007d067c066a1400000000000000007c006a1300000000000000005f
+            1400000000000000007c06a0150000000000000000000000000000000000
+            0000007c05a6010000ab01000000000000000001007c05a0160000000000
             000000000000000000000000000000a6000000ab0000000000000000007d
-            077431000000000000000000007c077c00a6020000ab0200000000000000
-            007d077c077433000000000000000000007c066a1a0000000000000000a6
+            07742f000000000000000000007c077c00a6020000ab0200000000000000
+            007d077c077431000000000000000000007c066a190000000000000000a6
             010000ab01000000000000000066025300
          248           0 RESUME                   0
          
          253           2 LOAD_GLOBAL              1 (NULL + create_engine)
                       14 LOAD_FAST                0 (args)
                       16 LOAD_ATTR                1 (url)
                       26 PRECALL                  1
@@ -1683,183 +1678,157 @@
          
          259         144 LOAD_FAST                2 (metadata)
                      146 LOAD_METHOD              5 (reflect)
                      168 LOAD_FAST                1 (engine)
                      170 PRECALL                  1
                      174 CALL                     1
                      184 POP_TOP
-                     186 JUMP_FORWARD           203 (to 594)
+                     186 JUMP_FORWARD           128 (to 444)
                  >>  188 PUSH_EXC_INFO
          
          260         190 POP_TOP
          
          261         192 LOAD_GLOBAL             13 (NULL + traceback)
                      204 LOAD_ATTR                7 (format_exc)
                      214 PRECALL                  0
                      218 CALL                     0
                      228 STORE_FAST               4 (track)
          
          262         230 LOAD_GLOBAL             16 (log)
-                     242 LOAD_METHOD              9 (debug)
+                     242 LOAD_METHOD              9 (info)
                      264 LOAD_FAST                4 (track)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 POP_TOP
          
          263         282 LOAD_GLOBAL             16 (log)
-                     294 LOAD_METHOD              9 (debug)
+                     294 LOAD_METHOD              9 (info)
                      316 LOAD_CONST               3 ('\n***** Database failed to open: ')
                      318 LOAD_FAST                0 (args)
                      320 LOAD_ATTR                1 (url)
                      330 FORMAT_VALUE             0
                      332 LOAD_CONST               4 (' *****\n')
                      334 BUILD_STRING             3
                      336 PRECALL                  1
                      340 CALL                     1
                      350 POP_TOP
          
-         264         352 LOAD_GLOBAL             16 (log)
-                     364 LOAD_METHOD              9 (debug)
-                     386 LOAD_CONST               5 ('.. Here are some examples:\n')
+         266         352 LOAD_GLOBAL             16 (log)
+                     364 LOAD_METHOD              9 (info)
+                     386 LOAD_CONST               5 ('\n...see https://apilogicserver.github.io/Docs/Troubleshooting/#database-failed-to-open \n\n')
                      388 PRECALL                  1
                      392 CALL                     1
                      402 POP_TOP
          
-         265         404 LOAD_GLOBAL             21 (NULL + print_uri_info)
-                     416 PRECALL                  0
-                     420 CALL                     0
-                     430 POP_TOP
-         
-         266         432 LOAD_GLOBAL             16 (log)
-                     444 LOAD_METHOD              9 (debug)
-                     466 LOAD_CONST               3 ('\n***** Database failed to open: ')
-                     468 LOAD_FAST                0 (args)
-                     470 LOAD_ATTR                1 (url)
-                     480 FORMAT_VALUE             0
-                     482 LOAD_CONST               6 (' -- see examples above *****\n')
-                     484 BUILD_STRING             3
-                     486 PRECALL                  1
-                     490 CALL                     1
-                     500 POP_TOP
-         
-         267         502 LOAD_GLOBAL             16 (log)
-                     514 LOAD_METHOD              9 (debug)
-                     536 LOAD_CONST               7 ('\n...see https://apilogicserver.github.io/Docs/Troubleshooting/')
-                     538 PRECALL                  1
-                     542 CALL                     1
-                     552 POP_TOP
-         
-         268         554 LOAD_GLOBAL             23 (NULL + exit)
-                     566 LOAD_CONST               8 (1)
-                     568 PRECALL                  1
-                     572 CALL                     1
-                     582 POP_TOP
-                     584 POP_EXCEPT
-                     586 JUMP_FORWARD             3 (to 594)
-                 >>  588 COPY                     3
-                     590 POP_EXCEPT
-                     592 RERAISE                  1
-         
-         269     >>  594 LOAD_CONST               9 ('sqlite')
-                     596 LOAD_FAST                0 (args)
-                     598 LOAD_ATTR                1 (url)
-                     608 CONTAINS_OP              0
-                     610 POP_JUMP_FORWARD_IF_FALSE    21 (to 654)
-         
-         271         612 LOAD_FAST                1 (engine)
-                     614 LOAD_METHOD             12 (execute)
-                     636 LOAD_CONST              10 ('PRAGMA journal_mode = OFF')
-                     638 PRECALL                  1
-                     642 CALL                     1
-                     652 POP_TOP
-         
-         273     >>  654 LOAD_GLOBAL             27 (NULL + StringIO)
-                     666 PRECALL                  0
-                     670 CALL                     0
-                     680 STORE_FAST               5 (capture)
-         
-         275         682 LOAD_GLOBAL             29 (NULL + CodeGenerator)
-                     694 LOAD_FAST                2 (metadata)
-                     696 LOAD_FAST                0 (args)
-                     698 LOAD_ATTR               15 (noindexes)
-                     708 LOAD_FAST                0 (args)
-                     710 LOAD_ATTR               16 (noconstraints)
-         
-         276         720 LOAD_FAST                0 (args)
-                     722 LOAD_ATTR               17 (nojoined)
-                     732 LOAD_FAST                0 (args)
-                     734 LOAD_ATTR               18 (noinflect)
-                     744 LOAD_FAST                0 (args)
-                     746 LOAD_ATTR               19 (noclasses)
-                     756 LOAD_FAST                0 (args)
-                     758 LOAD_ATTR               20 (model_creation_services)
-         
-         275         768 PRECALL                  7
-                     772 CALL                     7
-                     782 STORE_FAST               6 (generator)
-         
-         277         784 LOAD_FAST                6 (generator)
-                     786 LOAD_ATTR               21 (metadata)
-                     796 LOAD_FAST                0 (args)
-                     798 LOAD_ATTR               20 (model_creation_services)
-                     808 STORE_ATTR              21 (metadata)
-         
-         278         818 LOAD_FAST                6 (generator)
-                     820 LOAD_METHOD             22 (render)
-                     842 LOAD_FAST                5 (capture)
-                     844 PRECALL                  1
-                     848 CALL                     1
-                     858 POP_TOP
-         
-         279         860 LOAD_FAST                5 (capture)
-                     862 LOAD_METHOD             23 (getvalue)
-                     884 PRECALL                  0
-                     888 CALL                     0
-                     898 STORE_FAST               7 (models_py)
-         
-         280         900 LOAD_GLOBAL             49 (NULL + fix_generated)
-                     912 LOAD_FAST                7 (models_py)
-                     914 LOAD_FAST                0 (args)
-                     916 PRECALL                  2
-                     920 CALL                     2
-                     930 STORE_FAST               7 (models_py)
-         
-         281         932 LOAD_FAST                7 (models_py)
-                     934 LOAD_GLOBAL             51 (NULL + len)
-                     946 LOAD_FAST                6 (generator)
-                     948 LOAD_ATTR               26 (models)
-                     958 PRECALL                  1
-                     962 CALL                     1
-                     972 BUILD_TUPLE              2
-                     974 RETURN_VALUE
+         268         404 LOAD_GLOBAL             21 (NULL + exit)
+                     416 LOAD_CONST               6 (1)
+                     418 PRECALL                  1
+                     422 CALL                     1
+                     432 POP_TOP
+                     434 POP_EXCEPT
+                     436 JUMP_FORWARD             3 (to 444)
+                 >>  438 COPY                     3
+                     440 POP_EXCEPT
+                     442 RERAISE                  1
+         
+         269     >>  444 LOAD_CONST               7 ('sqlite')
+                     446 LOAD_FAST                0 (args)
+                     448 LOAD_ATTR                1 (url)
+                     458 CONTAINS_OP              0
+                     460 POP_JUMP_FORWARD_IF_FALSE    21 (to 504)
+         
+         271         462 LOAD_FAST                1 (engine)
+                     464 LOAD_METHOD             11 (execute)
+                     486 LOAD_CONST               8 ('PRAGMA journal_mode = OFF')
+                     488 PRECALL                  1
+                     492 CALL                     1
+                     502 POP_TOP
+         
+         273     >>  504 LOAD_GLOBAL             25 (NULL + StringIO)
+                     516 PRECALL                  0
+                     520 CALL                     0
+                     530 STORE_FAST               5 (capture)
+         
+         275         532 LOAD_GLOBAL             27 (NULL + CodeGenerator)
+                     544 LOAD_FAST                2 (metadata)
+                     546 LOAD_FAST                0 (args)
+                     548 LOAD_ATTR               14 (noindexes)
+                     558 LOAD_FAST                0 (args)
+                     560 LOAD_ATTR               15 (noconstraints)
+         
+         276         570 LOAD_FAST                0 (args)
+                     572 LOAD_ATTR               16 (nojoined)
+                     582 LOAD_FAST                0 (args)
+                     584 LOAD_ATTR               17 (noinflect)
+                     594 LOAD_FAST                0 (args)
+                     596 LOAD_ATTR               18 (noclasses)
+                     606 LOAD_FAST                0 (args)
+                     608 LOAD_ATTR               19 (model_creation_services)
+         
+         275         618 PRECALL                  7
+                     622 CALL                     7
+                     632 STORE_FAST               6 (generator)
+         
+         277         634 LOAD_FAST                6 (generator)
+                     636 LOAD_ATTR               20 (metadata)
+                     646 LOAD_FAST                0 (args)
+                     648 LOAD_ATTR               19 (model_creation_services)
+                     658 STORE_ATTR              20 (metadata)
+         
+         278         668 LOAD_FAST                6 (generator)
+                     670 LOAD_METHOD             21 (render)
+                     692 LOAD_FAST                5 (capture)
+                     694 PRECALL                  1
+                     698 CALL                     1
+                     708 POP_TOP
+         
+         279         710 LOAD_FAST                5 (capture)
+                     712 LOAD_METHOD             22 (getvalue)
+                     734 PRECALL                  0
+                     738 CALL                     0
+                     748 STORE_FAST               7 (models_py)
+         
+         280         750 LOAD_GLOBAL             47 (NULL + fix_generated)
+                     762 LOAD_FAST                7 (models_py)
+                     764 LOAD_FAST                0 (args)
+                     766 PRECALL                  2
+                     770 CALL                     2
+                     780 STORE_FAST               7 (models_py)
+         
+         281         782 LOAD_FAST                7 (models_py)
+                     784 LOAD_GLOBAL             49 (NULL + len)
+                     796 LOAD_FAST                6 (generator)
+                     798 LOAD_ATTR               25 (models)
+                     808 PRECALL                  1
+                     812 CALL                     1
+                     822 BUILD_TUPLE              2
+                     824 RETURN_VALUE
          ExceptionTable:
            144 to 184 -> 188 [0]
-           188 to 582 -> 588 [1] lasti
+           188 to 432 -> 438 [1] lasti
          consts
             ' called by ApiLogicServer CLI > ModelCreationServices > create_models_py\n\n    returns str to be written to models.py\n    '
             ','
             None
             '\n***** Database failed to open: '
             ' *****\n'
-            '.. Here are some examples:\n'
-            ' -- see examples above *****\n'
-            '\n...see https://apilogicserver.github.io/Docs/Troubleshooting/'
+            '\n...see https://apilogicserver.github.io/Docs/Troubleshooting/#database-failed-to-open \n\n'
             1
             'sqlite'
             'PRAGMA journal_mode = OFF'
-         names      ('create_engine', 'url', 'MetaData', 'tables', 'split', 'reflect', 'traceback', 'format_exc', 'log', 'debug', 'print_uri_info', 'exit', 'execute', 'StringIO', 'CodeGenerator', 'noindexes', 'noconstraints', 'nojoined', 'noinflect', 'noclasses', 'model_creation_services', 'metadata', 'render', 'getvalue', 'fix_generated', 'len', 'models')
+         names      ('create_engine', 'url', 'MetaData', 'tables', 'split', 'reflect', 'traceback', 'format_exc', 'log', 'info', 'exit', 'execute', 'StringIO', 'CodeGenerator', 'noindexes', 'noconstraints', 'nojoined', 'noinflect', 'noclasses', 'model_creation_services', 'metadata', 'render', 'getvalue', 'fix_generated', 'len', 'models')
          varnames   ('args', 'engine', 'metadata', 'tables', 'track', 'capture', 'generator', 'models_py')
          freevars   ()
          cellvars   ()
          filename   '/Users/val/dev/ApiLogicServer/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py'
          name       'create_models_memstring'
          firstlineno 248
          lnotab
-            0x020528021e01460102022e01020126013401460134011c014601340128
-            0112022a021c02260130ff100222012a0128012001
+            0x020528021e01460102022e0102012601340146033402280112022a021c
+            02260130ff100222012a0128012001
       'DB App'
       '*'
       ('origins',)
       ('SQLALCHEMY_TRACK_MODIFICATIONS', 'MAX_PAGE_LIMIT')
       True
       ('SQLALCHEMY_DATABASE_URI', 'DEBUG', 'JSON_AS_ASCII')
       'models.py'
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py` & `ApiLogicServer-8.3.3/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,20 +255,20 @@
     metadata = MetaData(engine)
     tables = args.tables.split(",") if args.tables else None
     try:
         # metadata.reflect(engine, args.schema, not args.noviews, tables)  # load metadata - this opens the db
         metadata.reflect(engine)
     except:
         track = traceback.format_exc()
-        log.debug(track)
-        log.debug(f'\n***** Database failed to open: {args.url} *****\n')
-        log.debug(f'.. Here are some examples:\n')
-        print_uri_info()
-        log.debug(f'\n***** Database failed to open: {args.url} -- see examples above *****\n')
-        log.debug(f'\n...see https://apilogicserver.github.io/Docs/Troubleshooting/')
+        log.info(track)
+        log.info(f'\n***** Database failed to open: {args.url} *****\n')
+        # log.info(f'.. See example above\n')
+        # print_uri_info()
+        log.info(f'\n...see https://apilogicserver.github.io/Docs/Troubleshooting/#database-failed-to-open \n\n')
+        # log.info(f'\n***** Database failed to open: {args.url} -- see examples above *****\n')
         exit(1)
     if "sqlite" in args.url: # db.session.bind.dialect.name == "sqlite":   FIXME review
         # dirty hack for sqlite
         engine.execute("""PRAGMA journal_mode = OFF""")
 
     capture = StringIO()  # generate and return the model
     # outfile = io.open(args.outfile, 'w', encoding='utf-8') if args.outfile else capture # sys.stdout
```

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/templates/admin.yaml` & `ApiLogicServer-8.3.3/api_logic_server_cli/templates/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/templates/app_fiddle.md` & `ApiLogicServer-8.3.3/api_logic_server_cli/templates/app_fiddle.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/templates/app_fiddle.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/templates/app_fiddle.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/templates/index.html` & `ApiLogicServer-8.3.3/api_logic_server_cli/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/api_logic_server_cli/templates/login_endpoint.txt` & `ApiLogicServer-8.3.3/api_logic_server_cli/templates/login_endpoint.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.0/setup.py` & `ApiLogicServer-8.3.3/setup.py`

 * *Files identical despite different names*

