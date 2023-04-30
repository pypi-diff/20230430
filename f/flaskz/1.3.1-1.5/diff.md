# Comparing `tmp/flaskz-1.3.1.tar.gz` & `tmp/flaskz-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.3.1.tar", last modified: Thu Mar  2 10:06:21 2023, max compression
+gzip compressed data, was "flaskz-1.5.tar", last modified: Sun Apr 30 16:26:54 2023, max compression
```

## Comparing `flaskz-1.3.1.tar` & `flaskz-1.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.091895 flaskz-1.3.1/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.3.1/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     4629 2023-03-02 10:06:21.092045 flaskz-1.3.1/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     4171 2023-03-02 10:02:03.000000 flaskz-1.3.1/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.3.1/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      704 2023-03-02 10:06:21.092703 flaskz-1.3.1/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.068055 flaskz-1.3.1/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.072710 flaskz-1.3.1/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-03-02 10:05:23.000000 flaskz-1.3.1/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.076478 flaskz-1.3.1/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.3.1/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.3.1/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.078229 flaskz-1.3.1/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)        0 2022-07-29 14:22:02.000000 flaskz-1.3.1/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8509 2022-05-29 14:44:01.000000 flaskz-1.3.1/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)     9509 2022-11-22 03:30:58.000000 flaskz-1.3.1/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.078899 flaskz-1.3.1/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2154 2022-05-16 03:47:40.000000 flaskz-1.3.1/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.082179 flaskz-1.3.1/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     5629 2023-02-27 05:12:35.000000 flaskz-1.3.1/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    23570 2023-02-19 06:39:09.000000 flaskz-1.3.1/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     8341 2023-01-31 11:13:01.000000 flaskz-1.3.1/src/flaskz/models/_model.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     5312 2022-12-03 17:06:08.000000 flaskz-1.3.1/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.3.1/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.084218 flaskz-1.3.1/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    10289 2023-03-02 10:04:06.000000 flaskz-1.3.1/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      958 2021-11-15 11:23:32.000000 flaskz-1.3.1/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3683 2021-11-15 07:26:44.000000 flaskz-1.3.1/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.091378 flaskz-1.3.1/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      253 2022-11-07 02:04:34.000000 flaskz-1.3.1/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      627 2022-11-08 11:34:23.000000 flaskz-1.3.1/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2246 2022-03-15 07:51:52.000000 flaskz-1.3.1/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     5690 2022-03-20 13:31:57.000000 flaskz-1.3.1/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     9558 2023-01-09 07:49:33.000000 flaskz-1.3.1/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      838 2022-05-11 02:41:06.000000 flaskz-1.3.1/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2659 2020-12-03 03:47:20.000000 flaskz-1.3.1/src/flaskz/utils/_magic.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     4470 2023-01-17 03:26:04.000000 flaskz-1.3.1/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     4752 2023-02-13 09:31:20.000000 flaskz-1.3.1/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2573 2021-11-17 08:09:34.000000 flaskz-1.3.1/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     2758 2022-12-13 09:01:00.000000 flaskz-1.3.1/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-03-02 10:06:21.075375 flaskz-1.3.1/src/flaskz.egg-info/
--rwxrwxrwx   0 taozh      (501) staff       (20)     4629 2023-03-02 10:06:21.000000 flaskz-1.3.1/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-03-02 10:06:21.000000 flaskz-1.3.1/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-03-02 10:06:21.000000 flaskz-1.3.1/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-03-02 10:06:21.000000 flaskz-1.3.1/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-03-02 10:06:21.000000 flaskz-1.3.1/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.371591 flaskz-1.5/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.5/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     6014 2023-04-30 16:26:54.371934 flaskz-1.5/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5573 2023-04-30 02:34:26.000000 flaskz-1.5/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.5/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      702 2023-04-30 16:26:54.373355 flaskz-1.5/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.317386 flaskz-1.5/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.322595 flaskz-1.5/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       21 2023-04-25 08:17:23.000000 flaskz-1.5/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.329130 flaskz-1.5/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.5/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.5/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.334334 flaskz-1.5/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.5/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.5/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)     9693 2023-04-26 10:31:33.000000 flaskz-1.5/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.335590 flaskz-1.5/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2148 2023-04-29 08:02:14.000000 flaskz-1.5/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.341339 flaskz-1.5/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5452 2023-04-29 08:02:14.000000 flaskz-1.5/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    26141 2023-04-27 03:54:02.000000 flaskz-1.5/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     8353 2023-04-26 10:19:02.000000 flaskz-1.5/src/flaskz/models/_model.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5969 2023-04-30 02:33:59.000000 flaskz-1.5/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.5/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.346233 flaskz-1.5/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    19354 2023-04-27 11:45:35.000000 flaskz-1.5/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.5/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3816 2023-04-27 11:38:34.000000 flaskz-1.5/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.369687 flaskz-1.5/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      253 2022-11-07 02:04:34.000000 flaskz-1.5/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2099 2023-04-30 03:06:59.000000 flaskz-1.5/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2571 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10388 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.5/src/flaskz/utils/_magic.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5002 2023-04-26 10:29:46.000000 flaskz-1.5/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7682 2023-04-27 03:34:22.000000 flaskz-1.5/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2578 2023-04-26 10:29:46.000000 flaskz-1.5/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     2784 2023-04-24 11:30:26.000000 flaskz-1.5/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-04-30 16:26:54.326104 flaskz-1.5/src/flaskz.egg-info/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6014 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-04-30 16:26:54.000000 flaskz-1.5/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.3.1/LICENSE` & `flaskz-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.3.1/PKG-INFO` & `flaskz-1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.3.1
+Version: 1.5
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,41 +24,56 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.5** `2023/05/01`
+    - [A] 重构`flaskz.rest`路由生成模块*
+        - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
+        - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
+        - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
+        - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
+        - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
+        - 添加`register_model_query_route`函数，可用于生成指定数据模型的全量查询路由
+        - 添加`register_model_query_pss_route`函数，可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
+        - 添加`register_models_query_route`函数，可用于生成多个数据模型的全量查询路由
+    - [A] `ModelMixin.query_pss`方法支持多列排序*
+    - [A] `flaskz.models.init_model`和`flaskz.log.init_log`函数添加对`Class`类型参数的支持
+    - [A] `BaseModelMixin.delete_db`方法添加对`dict`类型参数的支持
+    - [A] `flaskz.utils`添加`cls_to_dict`函数, 用于生成类属性的dict对象
+    - [C] `BaseModelMixin.bulk_delete`方法会删除符合条件的所有数据(此前版本只删除第一个)
 - **1.3.1** `2023/03/02`
-    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决<2.2.3版本的Flask不会将结尾不带`/`的请求重定向到带`/`路由的问题???
+    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决<2.2.3版本的Flask不会将结尾不带`/`的请求重定向到带`/`路由的问题
 - **1.3** `2023/03/01`
     - [A] `init_model_rest_blueprint`函数生成的query路由, 添加对单个数据的查询功能(`[GET]url_prefix/did/`)
     - [A] `init_model_rest_blueprint`函数生成的update路由, 添加URL主键支持(`[PATCH]url_prefix/did/`)
     - [C] `init_model_rest_blueprint`函数生成的delete路由, 结尾添加`/`, 用于支持以`/`结尾的URL删除请求(`[DELETE]url_prefix/did/`)
     - [A] 添加`FLASKZ_DATABASE_ENGINE_KWARGS`参数, 用于自定义engine参数
 - **1.2** `2023/02/01`
     - [A] 添加`FLASKZ_DATABASE_POOL_PRE_PING`参数, 用于设置engine的`pool_pre_ping`参数
     - [A] `init_model`函数添加数据库连接异常处理和重新连接
-    - ~~[C] `init_model_rest_blueprint`函数生成的删除路由URL中的id参数添加`path`类型转换(已移除)~~
+    - ~~[C] `init_model_rest_blueprint`函数生成的删除路由URL中的id参数添加`path`类型转换(v1.3.1已移除)~~
 - **1.1** `2023/01/01`
-    - [F] 修复`BaseModelMixin`的`update_db`和`delete_db`方法在非flask应用或没有flask应用上下文时的操作失败问题
+    - [F] 修复`BaseModelMixin`的`update_db`和`delete_db`方法在非Flask应用或没有Flask应用上下文时的操作失败问题
 - **1.0** `2022/12/01`
-    - [A] 添加`flask.utils.set_timeout`和`flask.utils.set_interval`函数用于延迟和周期性函数执行
-    - [A] `flask.ext.ssh`添加`timeout`参数以设置超时时间(登录&命令执行)
+    - [A] 添加`flaskz.utils.set_timeout`和`flaskz.utils.set_interval`函数用于延迟和周期性函数执行
+    - [A] `flaskz.ext.ssh`添加`timeout`参数以设置超时时间(登录&命令执行)
     - [F] 修复`BaseModelMixin.bulk_delete`方法因某条数据删除失败导致的操作中断和部分删除问题
 - **0.9** `2022/10/01`
     - [A] 添加`flaskz.auth`包, 提供了JWS授权功能
     - [A] 添加`flaskz.ext.ssh`, 提供了ssh相关功能(`pip install paramiko`)
 - **0.8** `2022/08/01`
-    - [A] `BaseModelMixin`和`ModelMixin`模型扩展类添加没有flask上下文环境时的使用支持
+    - [A] `BaseModelMixin`和`ModelMixin`模型扩展类添加没有Flask上下文环境时的使用支持
     - [A] 添加`flaskz.ext`包用于存放扩展工具类, 请注意ext包中的代码依赖的第三方包, 不在flaskz的install_requires中, 需要单独安装
-    - [C] 将`flask.utils.RSACipher`和`flask.utils.AESCipher`类所在的`cypher.py`文件移到了`flaskz.ext`包中
+    - [C] 将`flaskz.utils.RSACipher`和`flaskz.utils.AESCipher`类所在的`cypher.py`文件移到了`flaskz.ext`包中
 - **0.7** `2022/06/01`
-    - [A] 添加`flask.utils.RSACipher`和`flask.utils.AESCipher`类用于加密&解密, 需要安装`pycryptodome`包
-    - [A] 添加`flask.utils.append_url_search_params`函数, 用于向url中添加search参数
+    - [A] 添加`flaskz.utils.RSACipher`和`flaskz.utils.AESCipher`类用于加密&解密, 需要安装`pycryptodome`包
+    - [A] 添加`flaskz.utils.append_url_search_params`函数, 用于向url中添加search参数
 - **0.6** `2022/05/06`
     - [F] 修复当数据模型relationship中设置`lazy=joined`时, 排序引起的`"Can't resolve label reference"`问题
     - [F] 修复`merge_dict`方法, 因使用iteritems导致的bug
     - [F] 修复`forward_request`方法, 因请求没有设置`Content-Type=application/json`, 获取json时引发的`BadRequest('Content-Type was not 'application/json')`异常
     - [F] 修复未调用`init_log`初始化, 调用flaskz_logger时, 引起的`NameError(name '_flaskz_logger' is not defined)`问题
 - **0.3** `2021/11/26`
     - [A] 添加`FLASKZ_LOGGER_DISABLED`参数, 用于控制flaskz_logger的启用和禁用
```

### Comparing `flaskz-1.3.1/setup.cfg` & `flaskz-1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.3.1
+version = 1.5
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.3.1/src/flaskz/auth/_jws.py` & `flaskz-1.5/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.3.1/src/flaskz/ext/cypher.py` & `flaskz-1.5/src/flaskz/ext/cypher.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from Crypto.Util.Padding import pad, unpad
 
 __all__ = ['RSACipher', 'AESCipher']
 
 
 class RSACipher:
     """
-    The rsa utility class
+    The rsa utility class.
 
     The result of the encrypt and sign methods are in base64 format
     """
 
     @staticmethod
     def generate_key(bits=1024, to_base64=True):
         """
@@ -40,15 +40,16 @@
         return private_key, public_key
 
     @staticmethod
     def encrypt(plaintext, public_key):
         """
         Encrypt data with rsa public key.
 
-        encrypt_key = RSACipher.encrypt(public_key, aes_key)
+        Example:
+            encrypt_key = RSACipher.encrypt(public_key, aes_key)
 
         :param plaintext: the data to be encrypted
         :param public_key: rsa public key
 
         :return: ciphertext：the encrypted text(base64 format)
         """
         plaintext = _to_byte(plaintext)
@@ -56,48 +57,51 @@
         return base64.b64encode(cipher.encrypt(plaintext)).decode('utf-8')
 
     @staticmethod
     def decrypt(ciphertext, private_key):
         """
         Decrypt ciphertext with rsa private key.
 
-        aes_key = RSACipher.decrypt(private_key, encrypt_key)
+        Example:
+            aes_key = RSACipher.decrypt(private_key, encrypt_key)
 
         :param ciphertext: the data to be decrypted(base64 format)
         :param private_key: rsa private key
 
         :return: plaintext: the decrypted string
         """
         ciphertext = _to_byte(ciphertext)
         cipher = PKCS1_OAEP.new(RSACipher._import_rsa_key(private_key), hashAlgo=SHA256)
         return cipher.decrypt(base64.b64decode(ciphertext)).decode('utf-8')
 
     @staticmethod
     def sign(text, private_key):
         """
-        Sign the data with the private key
+        Sign the data with the private key.
 
-        signature = RSACipher.sign(private_key, aes_key)
+        Example:
+            signature = RSACipher.sign(private_key, aes_key)
 
         :param text: the text to be signed
         :param private_key: rsa private key
 
         :return: signature: the signature(base64 format)
         """
         text = _to_byte(text)
         signer = PKCS1_v1_5.new(RSACipher._import_rsa_key(private_key))
         signature = signer.sign(SHA256.new(text))
         return base64.b64encode(signature).decode('utf-8')
 
     @staticmethod
     def verify(text, signature, public_key):
         """
-        Verify the signature
+        Verify the signature.
 
-        result = RSACipher.verify(public_key, aes_key, signature)
+        Example:
+            result = RSACipher.verify(public_key, aes_key, signature)
 
         :param text: the raw text
         :param signature: the signature(base64 format)
         :param public_key: rsa public key
 
         :return: result: return True on success, otherwise return False
         """
@@ -113,37 +117,39 @@
         if _is_base64(key):
             key = base64.b64decode(key)
         return RSA.importKey(key)
 
 
 class AESCipher:
     """
-    The aes utility class
+    The aes utility class.
 
-    The result of the encrypt is in base64 format
+    The result of the encrypt is in base64 format.
     """
 
     @staticmethod
     def generate_key():
         """
         Generate a 16-bit random key
 
-        aes_key = AESCipher.generate_key()
+        Example:
+            aes_key = AESCipher.generate_key()
 
         :return: key
         """
         key = ''.join(random.choice(string.digits + string.ascii_letters) for _ in range(16))
         return key
 
     @staticmethod
     def encrypt(plaintext, key, iv=None):
         """
         Encrypt data with aes key and iv.
 
-        encrypt_text = AESCipher.encrypt(data, aes_key)
+        Example:
+            encrypt_text = AESCipher.encrypt(data, aes_key)
 
         :param plaintext: the data to be encrypted
         :param key: the key used to create AES cipher
         :param iv: the iv used to create AES cipher(AES.MODE_CBC), if None, use key as iv.
 
         :return: ciphertext: the encrypted text(base64 format)
         """
@@ -154,15 +160,16 @@
         return base64.b64encode(cipher.encrypt(plaintext)).decode('utf-8')
 
     @staticmethod
     def decrypt(ciphertext, key, iv=None):
         """
         Decrypt ciphertext with aes key and iv.
 
-        decrypt_text = AESCipher.decrypt(encrypt_text, aes_key)
+        Example:
+            decrypt_text = AESCipher.decrypt(encrypt_text, aes_key)
 
         :param ciphertext: the ciphertext to be decrypted(base64 format)
         :param key: the key used to decrypt
         :param iv: the iv used to decrypt, if None, use key as iv.
 
         :return: plaintext: the decrypted string
         """
```

### Comparing `flaskz-1.3.1/src/flaskz/ext/ssh.py` & `flaskz-1.5/src/flaskz/ext/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,33 @@
 from paramiko.ssh_exception import SSHException
 from paramiko.util import retry_on_signal
 
 
 @contextmanager
 def ssh_session(hostname, username, password=None, port=22, **kwargs):
     """
-    with ssh_session(host, username, password, timeout=20) as ssh:
-        ssh.run_command("ls -l")
+    SSH contextmanager.
+
+    Example:
+        with ssh_session(host, username, password, timeout=20) as ssh:
+            ssh.run_command("ls -l")
+
     """
     ssh_client = SSH(hostname=hostname, username=username, password=password, port=port, **kwargs)
     yield ssh_client
     ssh_client.close()
 
 
 class SSH(object):
     def __init__(self, hostname, username, password=None, port=22, **kwargs):
         """
-        ssh = SSH(host, username, password, timeout=20)
+        Create a SSH instance.
+
+        Example:
+            ssh = SSH(host, username, password, timeout=20)
         """
         self._username = username
         self._password = password
 
         self._timeout = kwargs.pop('timeout', 0)
         self.transport = paramiko.Transport(_create_socket(hostname=hostname, port=port, timeout=self._timeout))
         # self.transport = paramiko.Transport((hostname, port))
@@ -55,34 +62,38 @@
             self._channel = self.ssh.invoke_shell(height=100000)
             if self._timeout > 0:
                 self._channel.settimeout(self._timeout)
         return self._channel
 
     def run_command(self, command):
         """
-        Run the command
-        ssh.run_command("ls -l")
+        Run the command.
+
+        Example:
+            ssh.run_command("ls -l")
         """
         command = command.strip()
         self.channel.send(command + '\n')
         output = self._get_output(command)
 
         if self._password and command.lower().startswith('sudo') and 'assword' in output:  # input password
-            pwd_ouput = self.run_command(self._password)
-            if 'assword' in pwd_ouput:
+            pwd_output = self.run_command(self._password)
+            if 'assword' in pwd_output:
                 return output
             return self.run_command(command)
 
         return output
 
     def run_command_list(self, command_list, last_result=False):
         """
-        Run a command list
+        Run a command list.
         By default, returns the list of results , if last_result==True returns the result of the last command
-        ssh.run_command_list(['cd /usr/projects/git/srte',
+
+        Example:
+            ssh.run_command_list(['cd /usr/projects/git/srte',
                       'pwd',
                       'git pull origin master',
                       'wiui@hotmail.com',
                       '11111111'
                       ], True)
         """
         re_list = []
@@ -90,17 +101,19 @@
             re_list.append(self.run_command(command))
         if last_result is True:
             return re_list[-1]
         return re_list
 
     def sftp_get_dir(self, remote_dir, local_dir):
         """
-        Download remote direction to local
-        Return the local files list
-        ssh.sftp_get_dir("/usr/projects/git/srte/src/", "/Users/taozh/Work/Codes/ssh_test/sftp")
+        Download remote direction to local.
+        Return the local files list.
+
+        Example:
+            ssh.sftp_get_dir("/usr/projects/git/srte/src/", "/Users/taozh/Work/Codes/ssh_test/sftp")
         """
         if not self._path_exists(remote_dir):
             return False
         remote_dir = _remove_end_slash(remote_dir)
         local_dir = _remove_end_slash(local_dir)
         if not os.path.exists(local_dir):
             os.mkdir(local_dir)
@@ -113,16 +126,18 @@
             if not os.path.exists(local_filepath):
                 os.makedirs(local_filepath)
             self.sftp.get(f, local_filename)
         return local_files
 
     def listdir(self, path, recursion=False):
         """
-        List all files in the given path
-        ssh.listdir("/usr/projects/git/srte/src/")
+        List all files in the given path.
+
+        Example:
+            ssh.listdir("/usr/projects/git/srte/src/")
         """
         all_files = []
         path = _remove_end_slash(path)
         if path[-1] == '/':
             path = path[0:-1]
         files = self.sftp.listdir_attr(path)
         for f in files:
@@ -172,25 +187,24 @@
                     break
 
         return ''.join(res_list)
 
 
 def _create_socket(hostname, port, timeout=0):
     """
-    Create socket instance
+    Create socket instance.
     If timeout>0, set the timeout of the instance, otherwise use the default timeout(maybe 75s).
+
     :param hostname:
     :param port:
     :param timeout:
     :return:
     """
     reason = "No suitable address family"
-    addrinfos = socket.getaddrinfo(
-        hostname, port, socket.AF_UNSPEC, socket.SOCK_STREAM
-    )
+    addrinfos = socket.getaddrinfo(hostname, port, socket.AF_UNSPEC, socket.SOCK_STREAM)
     for family, socktype, proto, canonname, sockaddr in addrinfos:
         if socktype == socket.SOCK_STREAM:
             sock = socket.socket(family, socket.SOCK_STREAM)
             if timeout > 0:
                 sock.settimeout(timeout)
             now = datetime.now()
             try:
@@ -205,15 +219,15 @@
             "Unable to connect to {}: {}".format(hostname, reason)
         )
     return sock
 
 
 def _clear_redundant(txt, command):
     """
-    Clear the redundant information
+    Clear the redundant information.
     - Welcome info      ex)Welcome to Ubuntu...
     - Last login info   ex)Last login...
     - Path info         ex)[root@localhost ~]...
     - Command info      ex)ls -l
 
     """
     # remove the start command  ex) ls -l
```

### Comparing `flaskz-1.3.1/src/flaskz/log/__init__.py` & `flaskz-1.5/src/flaskz/log/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 
 def init_log(app):
     """
     Initialize system log configuration
     :param app:
     :return:
     """
-    if isinstance(app, Flask):
-        app_config = app.config
-    else:
-        app_config = app
+    app_config = get_app_config_items(app) or {}
     level = logging.getLevelName(app_config.get('FLASKZ_LOGGER_LEVEL'))
     formatter = logging.Formatter(app_config.get('FLASKZ_LOGGER_FORMAT'))
     global _flaskz_logger
     _flaskz_logger = logging.getLogger('flaskz_logger')
     _flaskz_logger.setLevel(level)
     filename = app_config.get('FLASKZ_LOGGER_FILENAME')
 
@@ -61,7 +58,10 @@
 def get_log_data(data):
     return json.dumps(data, default=_log_data_converter)
 
 
 def _log_data_converter(value):
     if isinstance(value, datetime.datetime):
         return value.__str__()
+
+
+from ..utils import get_app_config_items
```

### Comparing `flaskz-1.3.1/src/flaskz/models/__init__.py` & `flaskz-1.5/src/flaskz/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,31 +6,27 @@
 from sqlalchemy import create_engine, event
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine import ExceptionContext
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
 from ..log import flaskz_logger
-from ..utils import Attribute
+from ..utils import Attribute, cls_to_dict
 
 DBSession = sessionmaker(autocommit=False)
 
 ModelBase = declarative_base()
 
 
 def init_model(app):
     """
-    Initialize the database
+    Initialize the database.
     """
     is_app = isinstance(app, Flask)
-    if is_app:
-        app_config = app.config
-    else:
-        app_config = app
-    # app_config = app.config
+    app_config = get_app_config_items(app) or {}
     database_uri = app_config.get('FLASKZ_DATABASE_URI')
 
     # enable sqlite foreign key
     # if database_uri.startswith('sqlite'):
     @event.listens_for(Engine, "connect")
     def set_sqlite_pragma(dbapi_connection, connection_record):
         cursor = dbapi_connection.cursor()
@@ -66,15 +62,15 @@
                 if not context.connection or context.sqlalchemy_exception.connection_invalidated:
                     now = datetime.now().timestamp()
                     last_connect_time = engine_err_info.get('connect_time')
                     if last_connect_time is None or now - last_connect_time > 1:  # interval >1s
                         engine_err_info['connect_time'] = now
                         engine.connect()  # reconnect
 
-    except Exception as e:
+    except Exception:
         flaskz_logger.exception('Connect to database ' + database_uri + ' error\n')
         return
 
     if not is_app:
         return
 
     @app.teardown_appcontext
@@ -100,17 +96,14 @@
                 'end_time': end_time,
                 'duration': (end_time - start_time) * 1000,  # ms
                 'statement': statement,
                 'parameters': parameters,
                 'context': context,
             }))
 
-        # if duration > db_slow_time:
-        #     app_logger.warning('Slow query: %s\nParameters: %s\nDuration: %fms\n' % (statement, parameters, duration))
-
         db_slow_time = app_config.get('FLASKZ_DATABASE_DEBUG_SLOW_TIME', -1)  # set config['FLASKZ_DATABASE_DEBUG_SLOW_TIME'] to enable
         db_access_times = app_config.get('FLASKZ_DATABASE_DEBUG_ACCESS_TIMES', -1)  # set config['FLASKZ_DATABASE_DEBUG_ACCESS_TIMES'] to enable
         if db_slow_time > 0 or db_access_times > 0:
             @app.after_request
             def after_request(response):
                 queries = get_debug_queries()
                 times = len(queries)
@@ -127,7 +120,9 @@
                             flaskz_logger.warning('Slow queries:\n' + ('\n'.join(slow_queries)))
                 return response
 
 
 from ._base import *
 from ._model import *
 from ._util import *
+
+from ..utils import get_app_config_items
```

### Comparing `flaskz-1.3.1/src/flaskz/models/_base.py` & `flaskz-1.5/src/flaskz/models/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 from sqlalchemy import text
 
 from .. import res_status_codes
-from ..utils import find_list, filter_list, is_str, is_dict, ins_to_dict, get_dict_value_by_type
+from ..utils import find_list, filter_list, is_str, is_dict, is_list, ins_to_dict, get_dict_value_by_type
 
 __all__ = ['BaseModelMixin']
 
 
 class BaseModelMixin:
     # -------------------------------------------about model-------------------------------------------
     @classmethod
     def get_class_name(cls):
         """
         Get the name of the model class.
+
+        Example:
+            User.get_class_name() #User
+
         :return:
         """
         return cls.__name__
 
     @classmethod
     def get_columns(cls):
         """
         Get all the columns of the model class.
-        Menu.get_cls_columns()
+
+        Example:
+            User.get_cls_columns()
+
         :return:
         """
         return cls.__table__.columns
 
     @classmethod
     def get_columns_fields(cls):
         """
-        Get all the column fields
+        Get all the column fields.
 
          .. versionadded:: 1.3
 
+        Example:
+            User.get_columns_fields()
+
         :return:
         """
         fields = []
         for col in cls.get_columns():
             fields.append(cls.get_column_field(col))  # col.key
         return fields
 
     @classmethod
     def get_column_field(cls, col):
         """
-        Get the field variable name of the column, default return the key of the column
-        Used to get json fields to create or update data(get_columns_json), or convert data to json(_to_json)
+        Get the field variable name of the column, default return the key of the column.
+        Used to get json fields to create or update data(filter_attrs_by_columns), or convert data to json(_to_json).
 
         If the field name is different from the database column name
         #1 set field in info dict.(recommend)
         system_default = Column('default', Boolean, default=False, info={'field': 'system_default'})
 
         #2 rewrite to get the field name
         system_default = Column('default', Boolean, default=False)
@@ -65,87 +75,96 @@
         if field:
             return field
         return col.key
 
     @classmethod
     def get_column_by_field(cls, field):
         """
-        Get the column of the specified field
+        Get the column of the specified field.
+
+        Example:
+            User.get_column_by_field('name')
+
         :param field:
         :return:
         """
         for col in cls.get_columns():
             if (cls.get_column_field(col)) == field:
                 return col
 
     @classmethod
     def get_primary_column(cls):
         """
-         Get the primary column of the model class.
+        Get the primary column of the model class.
+
+        Example:
+            User.get_primary_column()   # id column
+
         :return:
         """
         return find_list(cls.get_columns(), lambda c: c.primary_key is True)
 
     @classmethod
     def get_primary_key(cls):
         """
-        Get the primary_key of the model class.
+        Get the key of the primary column.
+
+        Example:
+            User.get_primary_key()  # 'id'
+
         :return:
         """
         col = cls.get_primary_column()
         if col is not None:  # must
             return col.key
         return None
 
     @classmethod
     def get_primary_field(cls):
         """
-        Get the primary_key field of the model class.
+        Get the field of the primary column.
+
+        Example:
+            User.get_primary_field()    # 'id'
+
         :return:
         """
         col = cls.get_primary_column()
         if col is not None:  # must
             return cls.get_column_field(col)  # col.key
         return None
 
     @classmethod
     def get_unique_columns(cls):
         """
-        Get the unique column list of the model class
-         Menu.get_cls_unique_columns()
+        Get the unique column list of the model class.
+
+        Example:
+            User.get_unique_columns()
+
         :return:
         """
         return filter_list(cls.get_columns(), lambda col: col.unique is True)
 
     @classmethod
     def get_relationships(cls):
         """
         Get all the relationship list of the model class.
-         Menu.get_cls_relationships()
+
+        Example:
+            User.get_relationships()
+
         :return:
         """
         return cls.__mapper__.relationships
 
     # -------------------------------------------About data-------------------------------------------
     def to_dict(self, option=None):
         """
-        # 过滤
-            -不同的class会有不同的条件过滤-->过滤掉不需要的属性(create_user/password)
-            -过滤条件可以是class上的属性，也可以是传递到方法中的exclude
-                -如果有include--->只返回include中的属性
-                -如果没有include而有exclude--->将exclude中的属性过滤掉
-        *# 如果属性是关系对象/列表，则
-        *#
-        *#
-        *#
-        # 单个对象很容易处理，但是 relationships不好处理
-        # 不同的relationship，cascade不同
-        # relation中可能有嵌套
-        # 有可能两个对象里都有同一个对象
-        Convert model data to dict
+        Convert model data to dict.
 
         ins_to_dict(A, {
             'cascade': 3,  # 如果子项没有cascade，则使用父项-1，如果cascade不大于0，则不对象属性
             'recursion_value': '{...}'
             # 'include': ['a1'],  # 只有include中的字段才会返回，不区分值是否是对象，include的优先级>exclude
             # 'exclude': ['a2'],  # 只有exclude外的字段才会返回，不区分值是否是对象
             # 'getattr_items': lambda ins, item_cascade, option, path_keys: ins.__dict__.items(),
@@ -165,74 +184,102 @@
             #     'exclude': ['n'],
             #     'cascade': 1
             # },
             # "cc.xx": {
             #     'exclude': ['x2']
             # }
         })
+
+        过滤
+            -不同的class会有不同的条件过滤-->过滤掉不需要的属性(create_user/password)
+            -过滤条件可以是class上的属性，也可以是传递到方法中的exclude
+                -如果有include--->只返回include中的属性
+                -如果没有include而有exclude--->将exclude中的属性过滤掉
+        # 如果属性是关系对象/列表，则
+
+
+
+        # 单个对象很容易处理，但是 relationships不好处理
+        # 不同的relationship，cascade不同
+        # relation中可能有嵌套
+        # 有可能两个对象里都有同一个对象
         """
-        cls = self.__class__
         opt = {
             'getattrs': lambda ins, *args, **kwargs: ins.__class__.get_to_dict_attrs(ins, *args, **kwargs),
             'include': lambda ins, key: ins.__class__.to_dict_field_filter(key),
         }
         if option:
             opt.update(option)
         return ins_to_dict(self, opt)
 
     @classmethod
     def get_to_dict_attrs(cls, ins, cascade, *args):
+        """to_dict attr """
         fields = [cls.get_column_field(col) for col in cls.get_columns()]
         if cascade > 0:
             for relationship in cls.get_relationships():
                 lazy = relationship.lazy
                 if lazy != 'dynamic' and lazy != 'noload':
                     fields.append(relationship.key)
         items = {}
         for field in fields:
             items[field] = getattr(ins, field)
         return items
 
     @classmethod
     def to_dict_field_filter(cls, field):
         """
-        to_dict callback.
+        to_dict field filter callback.
         If return false, the field will not be returned.
         :param field:
         :return:
         """
         return True
 
     @classmethod
-    def get_columns_json(cls, data):
+    def filter_attrs_by_columns(cls, data):
         """
-        Get the data corresponding to the column.
-        :param data::
+        Filter out the attributes(dict) corresponding to the columns from the specified data(dict).
+
+        :param data:
         :return:
         """
-        json = {}
+        attrs = {}
         auto_columns = getattr(cls, 'auto_columns', [])
         auto_fields = []
         for col in auto_columns:
             if is_str(col):
                 auto_fields.append(col)
             else:
                 auto_fields.append(cls.get_column_field(col))
 
         for col in cls.get_columns():
             field = cls.get_column_field(col)  # col.key
             if (field in data) and (field not in auto_fields) and (not col.info.get('auto', False)):
                 value = data.get(field)
                 if col.nullable is False:
                     if not (value is None or (is_str(value) and value.strip() == "")):
-                        json[field] = value
+                        attrs[field] = value
                 else:
-                    json[field] = value
+                    attrs[field] = value
+
+        return attrs
+
+    @classmethod
+    def get_columns_json(cls, data):
+        """
+        Get the attributes(dict) corresponding to the column from the specified data(dict).
 
-        return json
+        .. deprecated:: 1.5 please use filter_attrs_by_columns method
+
+        :param data:
+        :return:
+        """
+
+        return cls.filter_attrs_by_columns(data)
 
     # -------------------------------------------add-------------------------------------------
     @classmethod
     def check_add_data(cls, data):
         """
         Check the the added json data.
         --validate the json data
@@ -247,15 +294,18 @@
                 return data
             return res_status_codes.bad_request
         return cls._check_unique(data)
 
     @classmethod
     def add_db(cls, data):
         """
-        Add the data to the db.
+        Add data to the db.
+
+        Example:
+            User.add_db({"name": "taozh", "email": "taozh@focus-ui.com"})
 
         :param data:
         :return:
         """
         instance = create_instance(cls, data)
         with db_session() as session:
             session.add(instance)
@@ -305,16 +355,19 @@
         if exist is not True:
             return exist
         return cls._check_unique(data)
 
     @classmethod
     def update_db(cls, data):
         """
-        Update the data to the db.
-        Only the fields in json will be updated
+        Update the data to the db. The primary key value must be in data.
+        Only the fields in data will be updated.
+
+        Example:
+            User.update_db({"id": 1, "email": "taozh@focus-ui.com"})
 
         :param data:
         :return:
         """
         pk_value = cls._get_pk_value(data)
         if pk_value is None:  # pk value does not exist
             return res_status_codes.db_data_not_found
@@ -325,15 +378,15 @@
                 return res_status_codes.db_data_not_found
             cls._update_ins(instance, data)  # @2022-12-01 change to ensure the updated instance and the setattr action in the same session
         return instance
 
     @classmethod
     def bulk_update(cls, items, with_relationship=False):
         """
-        Perform a bulk update of the given list of mapping dictionaries
+        Perform a bulk update of the given list of mapping dictionaries.
 
         sa version upgrade: https://docs.sqlalchemy.org/en/20/orm/queryguide/dml.html
         :param items:
         :param with_relationship:
         :return:
         """
         if len(items) == 0:
@@ -348,15 +401,15 @@
         else:
             with db_session() as session:
                 session.bulk_update_mappings(cls, items)
 
     @classmethod
     def _update_ins(cls, instance, data):
         if instance:
-            for field in cls.get_columns_json(data):  # Only the fields in json will be updated
+            for field in cls.filter_attrs_by_columns(data):  # Only the fields in json will be updated
                 setattr(instance, field, data.get(field))
             relationships = create_relationships(cls, data)
             for field in relationships:
                 setattr(instance, field, relationships[field])
         return instance
 
     # -------------------------------------------delete-------------------------------------------
@@ -377,77 +430,87 @@
         pk = cls.get_primary_field()
         data = {pk: pk_value}
         return cls._check_exist(data)
 
     @classmethod
     def delete_db(cls, pk_value):
         """
-        Delete data from the db.
+        Delete the specified data with the specified primary key value.
+
+        Example:
+            User.delete_db(1)   # pk
+            User.delete_db({'id': 1})   # dict
 
         :param pk_value:
         :return:
         """
         if pk_value is None:  # Object does not exist
             return res_status_codes.db_data_not_found
         with db_session() as session:  # @2022-12-01 change to ensure the deleted instance and the delete action in the same session
-            instance = session.query(cls).get(pk_value)
+            if is_dict(pk_value):  # @2023-03-27 add
+                instance = session.query(cls).filter_by(**pk_value).limit(1).first()
+            else:
+                instance = session.query(cls).get(pk_value)
             if instance is None:  # Object does not exist
                 return res_status_codes.db_data_not_found
             session.delete(instance)
         return instance
 
     @classmethod
     def bulk_delete(cls, items):
         """
-        Perform a bulk delete of the given list of mapping dictionaries
-
-            Role.bulk_delete([1,2,3])
+        Perform a bulk delete of the given list of mapping dictionaries.
 
         .. versionupdated:: 1.0
 
-        sa version upgrade: https://docs.sqlalchemy.org/en/20/orm/queryguide/dml.html
+        Example:
+            User.bulk_delete([1,2,3])   # pk list
+            User.bulk_delete([{'id': 1}, {'id': 2}, {'id': 3}]) # dict list
+
         :param items:
         :return:
         """
         if len(items) == 0:
             return
         pk = cls.get_primary_field()
         with db_session() as session:
             pk_list = []
             for item in items:
                 if is_dict(item):
-                    instance = session.query(cls).filter_by(**item).limit(1).first()
-                    if instance:
+                    # instance = session.query(cls).filter_by(**item).limit(1).first()
+                    # if instance:
+                    #     pk_list.append(getattr(instance, pk))
+                    for instance in session.query(cls).filter_by(**item):  # @2023-03-27 first to all, ex)delete all items with same name
                         pk_list.append(getattr(instance, pk))
                 else:
                     pk_list.append(item)
             # @2022-11-03: Use 'where' and 'in' to rewrite bulk delete to avoid partial delete scenarios
             if len(pk_list) > 0:
                 session.query(cls).filter(getattr(cls, pk).in_(pk_list)).delete()
 
     # -------------------------------------------query-------------------------------------------
 
     @classmethod
     def query(cls):
         """
-        Return a 'Query' object corresponding to this class
+        Return a 'Query' object corresponding to this class.
 
-        query = TemplateModel.query()
-        print(query.all())
+        Example:
+            query = TemplateModel.query()
+            print(query.all())
 
         :return:
         """
         with db_session(do_commit=False) as session:
             return session.query(cls)
 
     @classmethod
     def get_query_default_order(cls):
         """
-        Get the default order of the query.
-        column key, not field
+        Get the default order of the query.(column key, not field)
 
         get_primary_key-->get_primary_column to fix
         sqlalchemy.exc.CompileError: Can't resolve label reference for ORDER BY / GROUP BY / DISTINCT etc.
             Textual SQL expression 'id' should be explicitly declared as text('id')
         :return:
         """
         return cls.get_primary_column()
@@ -455,14 +518,17 @@
     @classmethod
     def query_by_unique_key(cls, data):
         """
         Query data by the unique values.
         --If exist,returns the instance.
         --Otherwise,returns None
 
+        Example:
+            User.query_by_unique_key(data)
+
         :param data:
         :return:
         """
         cols = cls.get_unique_columns()
         if len(cols) == 0:
             return None
 
@@ -481,83 +547,102 @@
             instance = query.first()
         return instance
 
     @classmethod
     def query_by_pk(cls, pk_value):
         """
         Query by pk value.
+
+        Example:
+            User.query_by_pk(1)
+
         :param pk_value:
         :return:
         """
         with db_session(do_commit=False) as session:
             instance = session.query(cls).get(pk_value)
         return instance
 
     @classmethod
     def query_by(cls, by_dict, return_first=False):
         """
         Query by dict object.
-        -If first is True, return the first row object or None.
         -If first is not True, return the list result of the query.
+        -If first is True, return the first row object or None.
+
+        Example:
+            User.query_by({'name': 'flaskz'})   # list
+            User.query_by({'name': 'flaskz'}, True) # first row
+
         """
         with db_session(do_commit=False) as session:
             if return_first is True:
                 result = session.query(cls).filter_by(**by_dict).limit(1).first()
             else:
                 result = session.query(cls).filter_by(**by_dict).all()
         return result
 
     @classmethod
     def query_all(cls):
         """
         Query all the data of the model class.
+
+        Example:
+            User.query_all()
+
         :return:
         """
         query_order = cls.get_query_default_order()
         with db_session(do_commit=False) as session:
             query = session.query(cls)
             if query_order is not None:
                 query = query.order_by(query_order)
             result = query.all()
         return result
 
     @classmethod
     def query_pss(cls, pss_option):
         """
         Query data by search, pagination and sort condition.
+        Please use flaskz.utils.get_pss to parse option first.
+        pss = page+search+sort
 
         Example:
-        result, result = TemplateModel.query_pss(get_pss(   # use flaskz.utils.get_pss to format condition
-            TemplateModel, {   # FROM templates
-                "search": {                         # WHERE
-                    "like": "t",                    # name like '%t%' OR description like '%t%' (TemplateModel.like_columns = ['name', description])
-                    "age": {                        # AND (age>1 AND age<20)
-                        ">": 1,                     # operator:value, operators)'='/'>'/'<'/'>='/'<='/'BETWEEN'/'LIKE'/'IN'
-                        "<": 20
+            result, result = TemplateModel.query_pss(get_pss(   # use flaskz.utils.get_pss to format condition
+                TemplateModel, {   # FROM templates
+                    "search": {                         # WHERE
+                        "like": "t",                    # name like '%t%' OR description like '%t%' (TemplateModel.like_columns = ['name', description])
+                        "age": {                        # AND (age>1 AND age<20)
+                            ">": 1,                     # operator:value, operators)'='/'>'/'<'/'>='/'<='/'BETWEEN'/'LIKE'/'IN'
+                            "<": 20
+                        },
+                        "email": "taozh@focus-ui.com",  # AND (email='taozh@focus-ui.com')
+                        "_ors": {                       # AND (country='America' OR country='Canada')
+                            "country": "America||Canada"
+                        },
+                        "_ands": {                      # AND (grade>1 AND grade<5)
+                            "grade": {
+                                ">": 1,
+                                "<": 5
+                            }
+                        }
                     },
-                    "email": "taozh@focus-ui.com",  # AND (email='taozh@focus-ui.com')
-                    "_ors": {                       # AND (country='America' OR country='Canada')
-                        "country": "America||Canada"
+                    "sort": {                           # ORDER BY templates.name ASC
+                        "field": "name",
+                        "order": "asc"
                     },
-                    "_ands": {                      # AND (grade>1 AND grade<5)
-                        "grade": {
-                            ">": 1,
-                            "<": 5
-                        }
+                    # "sort":[                          # ORDER BY templates.name ASC, templates.age DESC
+                    #     {"field": "name", "order": "asc"},
+                    #     {field": "age", "order": "desc"}
+                    # ],
+                    "page": {                           # LIMIT ? OFFSET ? (20, 0)
+                        "offset": 0,
+                        "size": 20
                     }
-                },
-                "sort": {                           # ORDER BY templates.name ASC
-                    "field": "name",
-                    "order": "asc"
-                },
-                "page": {                           # LIMIT ? OFFSET ? (20, 0)
-                    "offset": 0,
-                    "size": 20
-                }
-            }))
+                }))
 
         # sql
         SELECT templates.id AS templates_id, templates.name AS templates_name, templates.age AS templates_age, templates.email AS templates_email,
                 templates.country AS templates_country, templates.grade AS templates_grade, templates.description AS templates_description,
                 templates.created_at AS templates_created_at, templates.updated_at AS templates_updated_at
         FROM templates
         WHERE
@@ -569,63 +654,70 @@
 
         :param pss_option:
         :return:
         """
         filter_likes = pss_option.get('filter_likes', [])
         filter_ands = pss_option.get('filter_ands', [])
         filter_ors = pss_option.get('filter_ors', [])
-        # offset = pss_option.get('offset', 0)
-        # limit = pss_option.get('limit', 0)
         offset = max(get_dict_value_by_type(pss_option, 'offset', int, 0), 0)  # @2023-01-09 update, add type check
         limit = max(get_dict_value_by_type(pss_option, 'limit', int, 0), 0)
 
         # pss_json.get('order') or cls.get_query_default_order()
         # bool(pss_json.get('order')) --> Boolean value of this clause is not defined
-        order = pss_option.get('order')
-        if order is None:
-            order = cls.get_query_default_order()
+        orders = pss_option.get('order')
+        if orders is None:
+            orders = [cls.get_query_default_order()]  # default order
+        elif not is_list(orders):  # asc/desc
+            orders = [orders]
+
+        if not is_list(orders):
+            orders = []
 
         with db_session(do_commit=False) as session:
             query = session.query(cls)
             if len(filter_likes) > 0:
                 query = query.filter(text('(' + (' OR '.join(filter_likes)) + ')'))
             if len(filter_ands) > 0:
                 query = query.filter(text('(' + (' AND '.join(filter_ands)) + ')'))
             if len(filter_ors) > 0:
                 query = query.filter(text('(' + (' OR '.join(filter_ors)) + ')'))
             count = query.count()
             if count > 0 and offset < count:
-                query = query.order_by(order).offset(offset)
+                for order in orders:
+                    query = query.order_by(order)
+                query = query.offset(offset)
                 if limit > 0:
                     query = query.limit(limit)
                 items = query.all()
             else:
                 items = []
         return {
             'count': count,
             'data': items
         }
 
     # -------------------------------------------check-------------------------------------------
     @classmethod
     def _get_pk_value(cls, data):
         """
-        Get the primary key value from the json data
+        Get the primary key value from the json data.
+
         :param data:
         :return:
         """
         pk = cls.get_primary_field()
         if pk:
             return data.get(pk)
 
     @classmethod
     def _check_exist(cls, data):
         """
-        Check whether the data exists
-        Return True if exists, else return not found code
+        Check whether the data exists.
+        Return True if exists, else return not found code.
+
         :param data:
         :return:
         """
         pk_value = cls._get_pk_value(data)
         if pk_value is not None and cls.query_by_pk(pk_value):
             return True
         return res_status_codes.db_data_not_found  # used to return to the client
```

### Comparing `flaskz-1.3.1/src/flaskz/models/_model.py` & `flaskz-1.5/src/flaskz/models/_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         return data
 
     @classmethod
     def before_add(cls, data):
         """
         The callback before adding data.
         If the return value is not True, the adding process will be terminated and the result will be returned to the client.
+
         :param data: The data to be added
         :return: True|Error Message
         """
         return True
 
     @classmethod
     def after_add(cls, data, instance, before_result):
@@ -141,16 +142,16 @@
 
         return _op_result(before_result, instance)
 
     # -------------------------------------------delete-------------------------------------------
     @classmethod
     def get_delete_data(cls, pk_value):
         """
-        Return the primary key of the data to be deleted. By default, return the primary key of the client data
-        Rewrite to customize the deleted data
+        Return the primary key of the data to be deleted. By default, return the primary key of the client data.
+        Rewrite to customize the deleted data.
 
         :param pk_value: The primary key of the data to be deleted
         :return:
         """
         return pk_value
 
     @classmethod
@@ -213,29 +214,31 @@
 
         return _op_result(before_result, instance)
 
     # -------------------------------------------query-------------------------------------------
     @classmethod
     def query_all(cls):
         """
-        Override the base query_all method and return success flag
-        Used in router to return query data
+        Override the base query_all method and return success flag.
+        Used in router to return query data.
+
         :return:
         """
         try:
             return True, super().query_all()
         except Exception as e:
             flaskz_logger.exception(e)
             return False, res_status_codes.db_query_err
 
     @classmethod
     def query_pss(cls, pss_option):
         """
-        Override the base query_pss method and return success flag
-        Used in router to return query data
+        Override the base query_pss method and return success flag.
+        Used in router to return query data.
+
         :param pss_option:
         :return:
         """
         try:
             return True, super().query_pss(pss_option)
         except Exception as e:
             flaskz_logger.exception(e)
```

### Comparing `flaskz-1.3.1/src/flaskz/models/_util.py` & `flaskz-1.5/src/flaskz/models/_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,46 +3,51 @@
 from flask import g
 
 from . import DBSession
 from ._base import BaseModelMixin
 from ..utils import get_g_cache, set_g_cache
 
 __all__ = ['create_instance', 'create_relationships',
-           'query_multiple_model',
+           'query_all_models', 'query_multiple_model',
            'append_debug_queries', 'get_debug_queries',
            'get_db_session', 'db_session', 'close_db_session',
            'model_to_dict',
            'is_model_mixin_instance'
            ]
 
 
 def create_instance(model_cls, data, create_relationship=True):
     """
-    Create an instance of the specified model class with the data
+    Create an instance of the specified model class with the data.
+
+    Example:
+        create_instance(User, {"name": "taozh", "email": "taozh@focus-ui.com"})
+
     :param model_cls: The specified model class.
     :param data: The data used to create instance.
     :param create_relationship: If true, the relationships will be created.
     :return:
     """
     if not isinstance(data, dict):
         return None
 
-    col_value_dict = model_cls.get_columns_json(data)
+    col_value_dict = model_cls.filter_attrs_by_columns(data)
     instance = model_cls(**col_value_dict)
 
     if create_relationship is True:
         relationships = create_relationships(model_cls, data)
         for key in relationships:
             setattr(instance, key, relationships[key])
     return instance
 
 
 def create_relationships(model_cls, data):
     """
-    Create the relationship dict of the specified model class with the data
+    Create the relationship dict of the specified model class with the data.
+
     :param model_cls:
     :param data:
     :return:
     """
     relationships = model_cls.get_relationships()
     relationship_map = {}
     for key in relationships.keys():
@@ -59,34 +64,54 @@
 
         if relationship is not None:
             relationship_map[key] = relationship
 
     return relationship_map
 
 
-def query_multiple_model(*cls_list):
+def query_all_models(*models):
     """
-    Query all the data of the multiple specified model class.
-    :param cls_list:
-    :return:If failed, returns the failed tuple, otherwise, returns the the data list.
+    Query all the data of the specified model list.
+
+    .. versionadded:: 1.5
+
+    Example:
+        result = query_all_models(User, Role)
+
+    :param models:
+    :return:
     """
     result = []
-    for cls in cls_list:
-        r = cls.query_all()
+    for model in models:
+        r = model.query_all()
 
         if type(r) is tuple:  # ModelMixin
             if r[0] is not True:  # error
                 return r
             else:
                 result.append(r[1])
         else:
             result.append(r)
     return result
 
 
+def query_multiple_model(*cls_list):
+    """
+    Query all the data of the multiple specified model class.
+
+    Example:
+        result = query_multiple_model(User, Role)
+
+    :param cls_list:
+    :return:If failed, returns the failed tuple, otherwise, returns the the data list.
+    """
+
+    return query_all_models(*cls_list)
+
+
 def append_debug_queries(query):
     if _has_g_context():  # @2022-07-26 add,
         debug_queries = getattr(g, 'z_debug_queries', None)
         if debug_queries is None:
             g.z_debug_queries = debug_queries = []
         debug_queries.append(query)
 
@@ -102,47 +127,50 @@
         return False
     return True
     # return has_request_context() or g is not None
 
 
 def get_db_session():
     """
-    Get the db session from g.
+    Get the db session from g(flask)/ Create a db session.
     If not exist, create a session and return.
+
     :return:
     """
     if _has_g_context():  # @2022-07-26 add, make sure work without flask request
         session = get_g_cache('_flaskz_db_session')
         if session is None:
             session = DBSession()
             set_g_cache('_flaskz_db_session', session)
     else:
         session = DBSession()
     return session
 
 
 def close_db_session():
     """
-    Close the session in the g
+    Close the session in the g.
+
     :return:
     """
     if _has_g_context():  # @2022-07-26 add
         session = get_g_cache('_flaskz_db_session')
         if session is not None:
             session.close()
 
 
 @contextmanager
 def db_session(do_commit=True):
     """
     Database session context manager.
 
-    instance = create_instance(cls, json_data)
-    with db_session() as session:
-        session.add(instance)
+    Example:
+        instance = create_instance(cls, json_data)
+        with db_session() as session:
+            session.add(instance)
 
     :param do_commit: If false, session will not commit,generally used for query operations
     :return:
     """
     session = get_db_session()
     try:
         yield session
@@ -152,15 +180,19 @@
         if do_commit is not False:
             session.rollback()
         raise e
 
 
 def model_to_dict(ins, option=None):
     """
-    Convert model data to json dict
+    Convert model data to dict.
+
+    Example:
+        result = Role.update(request_json)
+        res_data = model_to_dict(result[1], {'cascade': 1})
 
     :param ins:
     :param option:
     :return:
     """
     if isinstance(ins, list):
         data_list = []
@@ -174,12 +206,13 @@
         return ins.to_dict(option)
     else:
         return ins
 
 
 def is_model_mixin_instance(obj):
     """
-    Check if the object is an instance of the BaseModelMixin
+    Check if the object is an instance of the BaseModelMixin.
+
     :param obj:
     :return:
     """
     return isinstance(obj, BaseModelMixin)
```

### Comparing `flaskz-1.3.1/src/flaskz/res_status_codes.py` & `flaskz-1.5/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.3.1/src/flaskz/rest/_mgmt.py` & `flaskz-1.5/src/flaskz/rest/_mgmt.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
     def logging(self, logging):
         self._logging = logging
         return self._logging
 
     @property
     def logging_callback(self):
-        return self._logging
+        return self._logging
```

### Comparing `flaskz-1.3.1/src/flaskz/rest/_util.py` & `flaskz-1.5/src/flaskz/rest/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     model_rest_manager = getattr(current_app, 'model_rest_manager', None)
     if model_rest_manager:
         return getattr(model_rest_manager, callback_name)
 
 
 def rest_login_required():
     """
-     If you decorate a view with this, it will ensure that the current user is
-    logged in and authenticated before calling the actual view.
+    If you decorate a view with this, it will ensure that the current user is logged in and authenticated before calling the actual view.
 
     @sys_mgmt_bp.route('/auth/account/', methods=['GET', 'POST'])
     @rest_login_required()
     def sys_auth_account_query():
         pass
 
     :return:
@@ -44,15 +43,15 @@
         return wrapper
 
     return decorate
 
 
 def rest_permission_required(module, op_permission=None):
     """
-    If you decorate a view with this, it will ensure that the current user
+    If you decorate a view with this, it will ensure that the current user.
     has the module permission and operation permission before calling the actual view.
 
     @sys_mgmt_bp.route('/role/', methods=['GET'])
     @rest_permission_required('role')
     def sys_role_query():
         pass
 
@@ -81,14 +80,15 @@
 
     return decorate
 
 
 def get_rest_log_msg(api_info, req_data, success, res_data):
     """
     Return the log message text.
+
     :param api_info:
     :param req_data:
     :param success:
     :param res_data:
     :return:
     """
     return get_wrap_str(
@@ -96,36 +96,40 @@
         '--Request data:', req_data,
         '--Response result:' + str(success),
         '--Response data:', res_data)
 
 
 def log_operation(*args, **kwargs):
     """
-    Log operation
+    Log operation/action.
+
+    Example:
+        log_operation('users', 'login', success, request_json.get('username'), res_data)
+
     :param args:
     :param kwargs:
     :return:
     """
     logging_callback = get_current_model_rest_manager_callback('logging_callback')
     if logging_callback:
         logging_callback(*args, **kwargs)
 
 
 def gen_route_method(method, url_prefix):
     """
-    Generate endpoint unique function name
+    Generate endpoint unique function name.
     :param method:
     :param url_prefix:
     :return:
     """
 
     def decorator(f):
         def wrap(*args, **kwargs):
             return f(*args, **kwargs)
 
         methods = url_prefix.split('/')
         methods.append(method)
-        methods.insert(0, 'model_rest')
-        wrap.__name__ = '_'.join(filter_list(methods, lambda item: item != ''))
+        methods.insert(0, 'model_route')
+        wrap.__name__ = '_'.join(filter_list(methods, lambda item: item != '')).replace('-', '_')
         return wrap
 
     return decorator
```

### Comparing `flaskz-1.3.1/src/flaskz/utils/_cache.py` & `flaskz-1.5/src/flaskz/utils/_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,37 @@
             'data': data,
         }
     return data
 
 
 def set_app_cache(key, data, expire_minutes=0):
     """
-    Set the current application data cache, such as menu items
+    Set the current application data cache, such as menu items.
+
+    Example:
+        set_app_cache('sys_module_name_mapping', module_name_mapping)
+
     :param expire_minutes:
     :param key:
     :param data:
     :return:
     """
     cache = getattr(current_app, 'z_data_cache', None)
     if cache is None:
         cache = current_app.z_data_cache = {}
     cache[key] = _generate_cache_expire_data(data, expire_minutes)
 
 
 def get_app_cache(key):
     """
     Get the current application data cache by the key.
+
+    Example:
+        module_name_mapping = get_app_cache('sys_module_name_mapping')
+
     :param key:
     :return:
     """
     cache = getattr(current_app, 'z_data_cache', None)
     if cache:
         data = cache.get(key)
         if is_dict(data) and '_zexpires_time' in data:
@@ -48,48 +56,58 @@
 
     return None
 
 
 def clear_app_cache():
     """
     Clear all the current application data caches.
+
     :return:
     """
     cache = getattr(current_app, 'z_data_cache', None)
     if cache:
         cache.clear()
 
 
 def set_g_cache(key, data):
     """
     Set the data cache in g, such as db session.
+
+    Example:
+        set_g_cache('_flaskz_db_session', session)
+
     :param key:
     :param data:
     :return:
     """
     cache = getattr(g, 'z_data_cache', None)
     if cache is None:
         cache = g.z_data_cache = {}
     cache[key] = data
 
 
 def get_g_cache(key):
     """
     Get the g data cache by the key.
+
+    Example:
+        session = get_g_cache('_flaskz_db_session')
+
     :param key:
     :return:
     """
     cache = getattr(g, 'z_data_cache', None)
     if cache:
         return cache.get(key)
     return None
 
 
 def remove_g_cache(key):
     """
     Remove the g data cache.
+
     :param key:
     :return:
     """
     cache = getattr(g, 'z_data_cache', None)
     if cache:
         del cache[key]
```

### Comparing `flaskz-1.3.1/src/flaskz/utils/_cls.py` & `flaskz-1.5/src/flaskz/utils/_cls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from inspect import isfunction
 
-__all__ = ['Attribute', 'ins_to_dict']
+__all__ = ['Attribute', 'cls_to_dict', 'ins_to_dict']
 
 
 class Attribute:
     """
     Used to create attribute object
     obj = AttrCls(**{'a':1,'b':2})
     obj.c = 3
@@ -24,18 +24,53 @@
     def __repr__(self):
         t = []
         for key, value in self.__dict__.items():
             t.append(key + '=' + str(value))
         return 'Attribute(' + ", ".join(t) + ')'
 
 
+def cls_to_dict(cls, option=None):  # @2023-03-15 add, convert class(config) to dictionary
+    """
+    Convert class(config) to dictionary.
+
+     .. versionadded:: 1.5
+
+     Example:
+         cls_to_dict(Config)
+         cls_to_dict(TestConfig)
+
+    :param cls:
+    :param option:
+    :return:
+    """
+    if option is None:
+        option = {}
+    attr_filter = _get_option_filter(option)
+
+    props = {}
+    cls_dir = dir(cls.__class__)
+    for key in dir(cls):
+        if key.startswith('__') or key in cls_dir:
+            continue
+        if _filter_attr(cls, key, attr_filter) is False:
+            continue
+
+        value = getattr(cls, key)
+        if callable(value):
+            continue
+        props[key] = value
+
+    return props
+
+
 def ins_to_dict(ins, option=None):
     """
-    Convert instance object to dictionary
-    ex)
+    Convert instance object to dictionary.
+
+    Example:
     ins_to_dict(A, {
         'cascade': 3,  # 如果子项没有cascade，则使用父项-1，如果cascade不大于0，则不对象属性
         'recursion_value': '{...}'
         # 'include': ['a1'],  # 只有include中的字段才会返回，不区分值是否是对象，include的优先级>exclude
         # 'exclude': ['a2'],  # 只有exclude外的字段才会返回，不区分值是否是对象
         # 'getattrs': lambda ins, item_cascade, option, path_keys: ins.__dict__.items(),
         #
@@ -54,14 +89,15 @@
         #     'exclude': ['n'],
         #     'cascade': 1
         # },
         # "cc.xx": {
         #     'exclude': ['x2']
         # }
     })
+
     :param ins:
     :param option:
     :return:
     """
     if isinstance(ins, list):
         result = []
         for item in ins:
@@ -104,41 +140,19 @@
 
     item_getattrs = _get_option_key(option, path_keys, 'getattrs')
     if item_getattrs:
         attrs = item_getattrs(ins, item_cascade, option, path_keys)
     else:
         attrs = ins.__dict__
 
-    item_include = item_option.get('include', [])
-    item_exclude = item_option.get('exclude', [])
-
-    if isfunction(item_include):
-        has_item_include = 'func'
-    else:
-        has_item_include = len(item_include) > 0
-
-    if isfunction(item_exclude):
-        has_item_exclude = 'func'
-    else:
-        has_item_exclude = len(item_exclude) > 0
-
-    result = {}
-
     # with_none_value = item_option.get('with_none_value', False)
-
+    attr_filter = _get_option_filter(item_option)
+    result = {}
     for key, value in attrs.items():
-
-        if has_item_include is True and key not in item_include:
-            continue
-        elif has_item_include == "func" and item_include(ins, key) is not True:
-            continue
-
-        if has_item_exclude is True and key in item_exclude:
-            continue
-        elif has_item_exclude == "func" and item_exclude(ins, key) is True:
+        if _filter_attr(ins, key, attr_filter) is False:
             continue
 
         _value = None
         if isinstance(value, list):
             _value = []
             _isinstance = False
             for item in value:
@@ -178,7 +192,47 @@
 
     item_key = '.'.join(key_list)
     item_option = option.get(item_key)
     if isinstance(item_option, dict):
         if key in item_option:
             return item_option.get(key)
     return _get_option_key(option, key_list[:-1], key)
+
+
+def _get_option_filter(option):
+    include = option.get('include', [])
+    exclude = option.get('exclude', [])
+
+    if isfunction(include):
+        has_include = 'func'
+    else:
+        has_include = len(include) > 0
+
+    if isfunction(exclude):
+        has_exclude = 'func'
+    else:
+        has_exclude = len(exclude) > 0
+    return {
+        'include': include,
+        'has_include': has_include,
+        'exclude': exclude,
+        'has_exclude': has_exclude,
+    }
+
+
+def _filter_attr(obj, attr, attr_filter):
+    has_include = attr_filter.get('has_include')
+    include = attr_filter.get('include')
+    has_exclude = attr_filter.get('has_exclude')
+    exclude = attr_filter.get('exclude')
+
+    if has_include is True and attr not in include:
+        return False
+    elif has_include == "func" and include(obj, attr) is not True:
+        return False
+
+    if has_exclude is True and attr in exclude:
+        return False
+    elif has_exclude == "func" and exclude(obj, attr) is True:
+        return False
+
+    return True
```

### Comparing `flaskz-1.3.1/src/flaskz/utils/_common.py` & `flaskz-1.5/src/flaskz/utils/_common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections.abc import Mapping
 
 __all__ = [
     'filter_list', 'find_list', 'merge_list', 'each_list', 'get_list',
     'get_dict', 'del_dict_keys', 'get_deep', 'set_deep', 'merge_dict', 'get_ins_mapping', 'get_dict_mapping', 'get_dict_value_by_type',
     'is_list', 'is_dict', 'slice_str',
-    'get_wrap_str', 'is_str',
+    'get_wrap_str', 'is_str', 'str_replace',
     'bulk_append_child'
 ]
 
 
 # -------------------------------------------list-------------------------------------------
 def filter_list(item_list, func, with_index=False):
     """
@@ -213,29 +213,34 @@
         else:
             map_dict[get_deep(item, key)] = item
 
     return map_dict
 
 
 def merge_dict(dct, *merged_dict_list):
-    """ Recursive dict merge. Inspired by :meth:``dict.update()``, instead of
+    """
+    Recursive dict merge. Inspired by :meth:``dict.update()``, instead of
     updating only top-level keys, dict_merge recurses down into dicts nested
     to an arbitrary depth, updating keys. The ``merge_dct`` is merged into
     ``dct``.
+
+    .. versionupdated:: 1.5 - return dct
+
     :param dct: dict onto which the merge is executed
     :param merged_dict_list: dct merged into dct
-    :return: None
+    :return: dct
     """
     for dict_item in merged_dict_list:
-        for k, v in dict_item.items():  # #2022-04-22 dict_item.iteritems-->dict_item.items
+        for k, v in dict_item.items():  # 2022-04-22 dict_item.iteritems-->dict_item.items
             if (k in dct and isinstance(dct[k], dict)
                     and isinstance(dict_item[k], Mapping)):
                 merge_dict(dct[k], dict_item[k])
             else:
                 dct[k] = dict_item[k]
+    return dct  # @2023-04-12 add result
 
 
 def get_dict_value_by_type(obj, key, value_type, default=None, by_instance=False):
     """
     Get the dict value of the specified key, if value is not the instance of the specified type, return default value.
 
     .. versionadded:: 1.2
@@ -260,52 +265,56 @@
             return value
     return default
 
 
 # -------------------------------------------type-------------------------------------------
 def is_str(value, by_instance=False):
     """
-    Check whether the value is string
+    Check whether the value is string.
+
     :param value:
     :param by_instance:
     :return:
     """
     if by_instance is True:
         return isinstance(value, str)
     return type(value) == str
 
 
 def is_list(value, by_instance=False):
     """
-    Check whether the value is list object
+    Check whether the value is list object.
+
     :param value:
     :param by_instance:
     :return:
     """
     if by_instance is True:
         return isinstance(value, list)
     return type(value) == list
 
 
 def is_dict(value, by_instance=False):
     """
-    Check whether the value is dict object
+    Check whether the value is dict object.
+
     :param value:
     :param by_instance:
     :return:
     """
     if by_instance is True:
         return isinstance(value, dict)
     return type(value) == dict
 
 
 # -------------------------------------------str-------------------------------------------
 def get_wrap_str(*items):
     """
-    Use '\n' to join multiple strings
+    Use '\n' to join multiple strings.
+
     :param items:
     :return:
     """
     result = []
     for item in items:
         if item is not None:
             result.append(str(item))
@@ -321,19 +330,50 @@
         return value
     result = value[0:start_len]
     if end_len != 0:
         result = result + ellipsis_str + value[end_len:]
     return result
 
 
+def str_replace(txt, old, new=''):
+    """
+    Return a copy with all occurrences of substring old replaced by new.
+
+    .. versionadded:: 1.5
+
+    Example:
+        str_replace('abca','a','A')             # AbcA
+        str_replace('abca',{'a':'A','b':'B'})   # ABcA
+        str_replace('abca',['a','b'],"*")       # **c*
+
+    :param txt:
+    :param old:
+    :param new:
+    :return:
+    """
+    v_type = type(old)
+    if v_type is dict:
+        for key in old:
+            txt = txt.replace(key, old[key])
+    elif v_type is list:
+        for item in old:
+            txt = txt.replace(item, new)
+    else:
+        txt = txt.replace(old, new)
+    return txt
+
+
 # -------------------------------------------other-------------------------------------------
 def bulk_append_child(items, parent_map, item_parent_key='parent_id', children_key="children", parent_map_key='id'):
     """
-    Append the items to the child list of the matched parent object
-    bulk_append_child(interface_items,device_list, 'device_id', 'interface_list')
+    Append the items to the child list of the matched parent object.
+
+    Example:
+        bulk_append_child(interface_items,device_list, 'device_id', 'interface_list')
+
     :param items:
     :param item_parent_key:
     :param parent_map:
     :param children_key:
     :param parent_map_key:
     :return:
     """
```

### Comparing `flaskz-1.3.1/src/flaskz/utils/_func.py` & `flaskz-1.5/src/flaskz/utils/_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __all__ = ['get_list_args']
 
 
 def get_list_args(params, args):  # @2022-05-11: add
     """
-    Returns a single new list combining keys and args
+    Returns a single new list combining keys and args.
 
     def xxx(names, *args):
         print(get_list_args(names, args))
 
     xxx('a', ['b', 'c'])    -->['a', 'b', 'c']
     xxx('a', 'b', 'c')      -->['a', 'b', 'c']
     xxx(['a', 'b'], 'c')    -->['a', 'b', 'c']
```

### Comparing `flaskz-1.3.1/src/flaskz/utils/_magic.py` & `flaskz-1.5/src/flaskz/utils/_magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 __all__ = ['typed_property', 'init_properties']
 
 
 def typed_property(name, expected_type):
     """
     Example 1:
-    class Person:
-        name = typed_property('name', str)
-        age = typed_property('age', int)
+        class Person:
+            name = typed_property('name', str)
+            age = typed_property('age', int)
 
     Example 2:
-    String = partial(typed_property, expected_type=str)
-    Integer = partial(typed_property, expected_type=int)
-    class Person:
-        name = String('name')
-        age = Integer('age')
+        String = partial(typed_property, expected_type=str)
+        Integer = partial(typed_property, expected_type=int)
+        class Person:
+            name = String('name')
+            age = Integer('age')
 
     :param name:
     :param expected_type:
     :return:
     """
     storage_name = '_' + name
 
@@ -32,41 +32,42 @@
         setattr(self, storage_name, value)
 
     return prop
 
 
 def init_properties(self, extra_kwargs, *args, **kwargs):
     """
-    class A:
-        _fields = ['a', 'b', 'c']
-
-        def __init__(self, *args, **kwargs):
-            init_property(self, False, *args, **kwargs)
-
-
-    class B:
-        _fields = ['a', 'b', 'c']
-
-        def __init__(self, *args, **kwargs):
-            init_property(self, True, *args, **kwargs)  # extended keyword arguments
-
-
-    print(A(1, 2, 3))
-    print(A(1, 2, c=3))
-    print(A(1, b=2, c=3))
-    # print(A(1, 2, 3, e=4))  # TypeError: A got an unexpected keyword argument e
-    # print(A(1, 2, 3, 4))  # TypeError: A takes 3 positional arguments but 4 were given
-    # print(A(1, 2, 3, a=4))  # TypeError: A got an unexpected keyword argument a
-
-    print(B(1, 2, 3))
-    print(B(1, 2, c=3))
-    print(B(1, b=2, c=3))
-    print(B(1, 2, 3, e=4))
-    # print(B(1, 2, 3, 4))  # TypeError: B takes 3 positional arguments but 4 were given
-    # print(B(1, 2, 3, a=4))  # TypeError: B got an unexpected keyword argument a
+    Example:
+        class A:
+            _fields = ['a', 'b', 'c']
+
+            def __init__(self, *args, **kwargs):
+                init_property(self, False, *args, **kwargs)
+
+
+        class B:
+            _fields = ['a', 'b', 'c']
+
+            def __init__(self, *args, **kwargs):
+                init_property(self, True, *args, **kwargs)  # extended keyword arguments
+
+
+        print(A(1, 2, 3))
+        print(A(1, 2, c=3))
+        print(A(1, b=2, c=3))
+        # print(A(1, 2, 3, e=4))  # TypeError: A got an unexpected keyword argument e
+        # print(A(1, 2, 3, 4))  # TypeError: A takes 3 positional arguments but 4 were given
+        # print(A(1, 2, 3, a=4))  # TypeError: A got an unexpected keyword argument a
+
+        print(B(1, 2, 3))
+        print(B(1, 2, c=3))
+        print(B(1, b=2, c=3))
+        print(B(1, 2, 3, e=4))
+        # print(B(1, 2, 3, 4))  # TypeError: B takes 3 positional arguments but 4 were given
+        # print(B(1, 2, 3, a=4))  # TypeError: B got an unexpected keyword argument a
     """
     _fields = getattr(self, '_fields', [])
     filed_len = len(_fields)
     args_len = len(args)
     cls_name = self.__class__.__name__
     if args_len > filed_len:
         raise TypeError(cls_name + ' takes {} positional arguments but {} were given'.format(filed_len, args_len))
```

### Comparing `flaskz-1.3.1/src/flaskz/utils/_request_api.py` & `flaskz-1.5/src/flaskz/utils/_request_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,18 @@
         if key in requests_kwargs:
             req_kwargs[key] = value
     return req_kwargs
 
 
 def api_request(url, method="GET", url_params=None, base_url="", raw_response=False, **kwargs):
     """
-    Request an api
+    Request an api.
+
+    Example
+        api_request('ELASTICSEARCH_URI', url_params={'index': index}, json=query, timeout=10)
 
     :param url:
     :param method:
     :param url_params:
     :param raw_response:
     :param base_url:
     :param kwargs:
@@ -86,15 +89,25 @@
         flaskz_logger.exception('Api request failed:\n' + str(e))
 
     return res_status_codes.api_request_err, result
 
 
 def forward_request(url, payload=None, raw_response=False, error_code=500, **kwargs):
     """
-    Forward the request to other service
+    Forward the request to other service.
+
+    Example:
+        @api_bp.route('/<regex(".*"):path>/', methods=HTTP_METHODS)
+        def remote(path):
+            remote_res = forward_request(base_url + path)
+            res = make_response(remote_res[0], remote_res[1])
+            for k, v in remote_res[2]:
+                if k not in ['Transfer-Encoding']:
+                    res.headers[k] = v
+            return res
 
     :param error_code:
     :param payload:
     :param raw_response:
     :param url: The forward url
     :return:
     """
@@ -123,18 +136,19 @@
     return res.text, res.status_code, res.headers.items()
 
 
 def append_url_search_params(url, params):  # @2022-05-09: add
     """
     Appends a specified key/value pair as a new search parameter.
 
-    append_url_search_params('https://example.com',{'foo':1,'bar':2}) --> 'https://example.com?foo=1&bar=2' # append
-    append_url_search_params('https://example.com?foo=1&bar=2',{'baz':3}) --> 'https://example.com?foo=1&bar=2&baz=3' # append
-    append_url_search_params('https://example.com?foo=1&bar=2',{'bar':3}) --> 'https://example.com?foo=1&bar=3' # replace
-    append_url_search_params('a/b',{'c':3}) --> 'a/b?c=3'
+    Example:
+        append_url_search_params('https://example.com',{'foo':1,'bar':2}) --> 'https://example.com?foo=1&bar=2' # append
+        append_url_search_params('https://example.com?foo=1&bar=2',{'baz':3}) --> 'https://example.com?foo=1&bar=2&baz=3' # append
+        append_url_search_params('https://example.com?foo=1&bar=2',{'bar':3}) --> 'https://example.com?foo=1&bar=3' # replace
+        append_url_search_params('a/b',{'c':3}) --> 'a/b?c=3'
 
     :param url:
     :param params:
     :return:
 
     """
     url_parts = urllib.parse.urlparse(url)
```

### Comparing `flaskz-1.3.1/src/flaskz/utils/_response.py` & `flaskz-1.5/src/flaskz/utils/_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 __all__ = ['create_response', 'get_status_msg', 'ResponseManager']
 
 
 def create_response(success, data, data_wrapped=False):
     """
     Create the response json result.
+
     :param success:
     :param data:
     :param data_wrapped:
     :return:
     """
     if success is True:
         return _create_success_response(data, data_wrapped)
@@ -57,15 +58,16 @@
         'message': str(msg),
     }
 
 
 def get_status_msg(status_code):
     """
     Get the specified message by status_code.
-    Can be used to return internationalized text, Local can be fixed, or get the local from request
+    Can be used to return internationalized text, Local can be fixed, or get the local from request.
+
     :param status_code:
     :return:
     """
     response_callback = get_current_response_manager('get_response_callback')
     if response_callback:
         return response_callback(status_code)
```

### Comparing `flaskz-1.3.1/src/flaskz/utils/_timer.py` & `flaskz-1.5/src/flaskz/utils/_timer.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,44 +38,46 @@
 
 
 def set_interval(interval, function, args=None, kwargs=None, immediately=False, daemon=True):
     """
     Execute a function periodically at a specified time interval(milliseconds).
     The result of the function execution is False, then the loop is interrupted.
 
+    .. versionadded:: 1.0
+
+    Example:
         t = set_interval(10, print, ('Hello, World!',))
         # t.cancel()    # Stop the timer
 
-    .. versionadded:: 1.0
-
-    :param daemon: if true, the timer will be daemon(Daemon threads are abruptly stopped at shutdown)
     :param interval: time interval in milliseconds
     :param function: callback function, which should do exception catching*
     :param args:
     :param kwargs:
     :param immediately: If True, the function will be executed immediately, otherwise it will be executed after the interval time
+    :param daemon: if true, the timer will be daemon(Daemon threads are abruptly stopped at shutdown)
     :return:
     """
     t = _IntervalTimer(interval, function, args=args, kwargs=kwargs, immediately=immediately, daemon=daemon)
     return t
 
 
 def set_timeout(interval, function, args=None, kwargs=None, daemon=True):
     """
     Set a timer which executes a function once the timer expires(milliseconds).
 
+     .. versionadded:: 1.0
+
+    Example:
         t = set_timeout(10, print, ('Hello, World!',))
         # t.cancel()    # Stop the timer
 
-     .. versionadded:: 1.0
-
-    :param daemon: if true, the timer will be daemon(Daemon threads are abruptly stopped at shutdown)
     :param interval: delay time in milliseconds before the specified function is executed
     :param function:
     :param args:
     :param kwargs:
+    :param daemon: if true, the timer will be daemon(Daemon threads are abruptly stopped at shutdown)
     :return:
     """
     t = Timer(interval / 1000, function, args=args, kwargs=kwargs)
     t.daemon = daemon
     t.start()
     return t
```

### Comparing `flaskz-1.3.1/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.5/src/flaskz.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.3.1
+Version: 1.5
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,41 +24,56 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.5** `2023/05/01`
+    - [A] 重构`flaskz.rest`路由生成模块*
+        - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
+        - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
+        - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
+        - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
+        - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
+        - 添加`register_model_query_route`函数，可用于生成指定数据模型的全量查询路由
+        - 添加`register_model_query_pss_route`函数，可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
+        - 添加`register_models_query_route`函数，可用于生成多个数据模型的全量查询路由
+    - [A] `ModelMixin.query_pss`方法支持多列排序*
+    - [A] `flaskz.models.init_model`和`flaskz.log.init_log`函数添加对`Class`类型参数的支持
+    - [A] `BaseModelMixin.delete_db`方法添加对`dict`类型参数的支持
+    - [A] `flaskz.utils`添加`cls_to_dict`函数, 用于生成类属性的dict对象
+    - [C] `BaseModelMixin.bulk_delete`方法会删除符合条件的所有数据(此前版本只删除第一个)
 - **1.3.1** `2023/03/02`
-    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决<2.2.3版本的Flask不会将结尾不带`/`的请求重定向到带`/`路由的问题???
+    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决<2.2.3版本的Flask不会将结尾不带`/`的请求重定向到带`/`路由的问题
 - **1.3** `2023/03/01`
     - [A] `init_model_rest_blueprint`函数生成的query路由, 添加对单个数据的查询功能(`[GET]url_prefix/did/`)
     - [A] `init_model_rest_blueprint`函数生成的update路由, 添加URL主键支持(`[PATCH]url_prefix/did/`)
     - [C] `init_model_rest_blueprint`函数生成的delete路由, 结尾添加`/`, 用于支持以`/`结尾的URL删除请求(`[DELETE]url_prefix/did/`)
     - [A] 添加`FLASKZ_DATABASE_ENGINE_KWARGS`参数, 用于自定义engine参数
 - **1.2** `2023/02/01`
     - [A] 添加`FLASKZ_DATABASE_POOL_PRE_PING`参数, 用于设置engine的`pool_pre_ping`参数
     - [A] `init_model`函数添加数据库连接异常处理和重新连接
-    - ~~[C] `init_model_rest_blueprint`函数生成的删除路由URL中的id参数添加`path`类型转换(已移除)~~
+    - ~~[C] `init_model_rest_blueprint`函数生成的删除路由URL中的id参数添加`path`类型转换(v1.3.1已移除)~~
 - **1.1** `2023/01/01`
-    - [F] 修复`BaseModelMixin`的`update_db`和`delete_db`方法在非flask应用或没有flask应用上下文时的操作失败问题
+    - [F] 修复`BaseModelMixin`的`update_db`和`delete_db`方法在非Flask应用或没有Flask应用上下文时的操作失败问题
 - **1.0** `2022/12/01`
-    - [A] 添加`flask.utils.set_timeout`和`flask.utils.set_interval`函数用于延迟和周期性函数执行
-    - [A] `flask.ext.ssh`添加`timeout`参数以设置超时时间(登录&命令执行)
+    - [A] 添加`flaskz.utils.set_timeout`和`flaskz.utils.set_interval`函数用于延迟和周期性函数执行
+    - [A] `flaskz.ext.ssh`添加`timeout`参数以设置超时时间(登录&命令执行)
     - [F] 修复`BaseModelMixin.bulk_delete`方法因某条数据删除失败导致的操作中断和部分删除问题
 - **0.9** `2022/10/01`
     - [A] 添加`flaskz.auth`包, 提供了JWS授权功能
     - [A] 添加`flaskz.ext.ssh`, 提供了ssh相关功能(`pip install paramiko`)
 - **0.8** `2022/08/01`
-    - [A] `BaseModelMixin`和`ModelMixin`模型扩展类添加没有flask上下文环境时的使用支持
+    - [A] `BaseModelMixin`和`ModelMixin`模型扩展类添加没有Flask上下文环境时的使用支持
     - [A] 添加`flaskz.ext`包用于存放扩展工具类, 请注意ext包中的代码依赖的第三方包, 不在flaskz的install_requires中, 需要单独安装
-    - [C] 将`flask.utils.RSACipher`和`flask.utils.AESCipher`类所在的`cypher.py`文件移到了`flaskz.ext`包中
+    - [C] 将`flaskz.utils.RSACipher`和`flaskz.utils.AESCipher`类所在的`cypher.py`文件移到了`flaskz.ext`包中
 - **0.7** `2022/06/01`
-    - [A] 添加`flask.utils.RSACipher`和`flask.utils.AESCipher`类用于加密&解密, 需要安装`pycryptodome`包
-    - [A] 添加`flask.utils.append_url_search_params`函数, 用于向url中添加search参数
+    - [A] 添加`flaskz.utils.RSACipher`和`flaskz.utils.AESCipher`类用于加密&解密, 需要安装`pycryptodome`包
+    - [A] 添加`flaskz.utils.append_url_search_params`函数, 用于向url中添加search参数
 - **0.6** `2022/05/06`
     - [F] 修复当数据模型relationship中设置`lazy=joined`时, 排序引起的`"Can't resolve label reference"`问题
     - [F] 修复`merge_dict`方法, 因使用iteritems导致的bug
     - [F] 修复`forward_request`方法, 因请求没有设置`Content-Type=application/json`, 获取json时引发的`BadRequest('Content-Type was not 'application/json')`异常
     - [F] 修复未调用`init_log`初始化, 调用flaskz_logger时, 引起的`NameError(name '_flaskz_logger' is not defined)`问题
 - **0.3** `2021/11/26`
     - [A] 添加`FLASKZ_LOGGER_DISABLED`参数, 用于控制flaskz_logger的启用和禁用
```

### Comparing `flaskz-1.3.1/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.5/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

