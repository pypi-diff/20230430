# Comparing `tmp/pygnmi-0.8.8.tar.gz` & `tmp/pygnmi-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygnmi-0.8.8.tar", last modified: Fri Aug 12 22:31:47 2022, max compression
+gzip compressed data, was "pygnmi-0.8.9.tar", last modified: Sun Aug 21 21:34:42 2022, max compression
```

## Comparing `pygnmi-0.8.8.tar` & `pygnmi-0.8.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-12 22:31:47.967197 pygnmi-0.8.8/
--rw-rw-r--   0 anton     (1000) anton     (1000)    18127 2022-08-12 22:31:47.967197 pygnmi-0.8.8/PKG-INFO
--rw-rw-r--   0 anton     (1000) anton     (1000)    13791 2022-08-12 22:29:09.527919 pygnmi-0.8.8/README.rst
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-12 22:31:47.967197 pygnmi-0.8.8/pygnmi/
--rw-rw-r--   0 anton     (1000) anton     (1000)      104 2022-08-12 22:29:09.527919 pygnmi-0.8.8/pygnmi/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     5323 2022-08-12 22:29:09.527919 pygnmi-0.8.8/pygnmi/arg_parser.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-12 22:31:47.967197 pygnmi-0.8.8/pygnmi/artefacts/
--rw-rw-r--   0 anton     (1000) anton     (1000)     1637 2022-06-24 17:57:08.171652 pygnmi-0.8.8/pygnmi/artefacts/messages.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    52111 2022-08-12 22:29:09.527919 pygnmi-0.8.8/pygnmi/client.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     1985 2022-07-24 12:53:02.054177 pygnmi-0.8.8/pygnmi/create_gnmi_extension.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     3350 2022-08-09 11:58:35.063076 pygnmi-0.8.8/pygnmi/create_gnmi_path.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-12 22:31:47.967197 pygnmi-0.8.8/pygnmi/spec/
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-12 22:31:47.967197 pygnmi-0.8.8/pygnmi/spec/v080/
--rw-rw-r--   0 anton     (1000) anton     (1000)     4913 2022-07-23 10:19:42.631581 pygnmi-0.8.8/pygnmi/spec/v080/gnmi_ext_pb2.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    20495 2022-07-23 10:17:08.764539 pygnmi-0.8.8/pygnmi/spec/v080/gnmi_pb2.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     8598 2022-07-22 14:54:15.697673 pygnmi-0.8.8/pygnmi/spec/v080/gnmi_pb2_grpc.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     6900 2022-06-25 18:10:54.299842 pygnmi-0.8.8/pygnmi/tools.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-12 22:31:47.967197 pygnmi-0.8.8/scripts/
--rw-rw-r--   0 anton     (1000) anton     (1000)     5347 2022-08-12 22:29:09.527919 pygnmi-0.8.8/scripts/pygnmicli
--rw-rw-r--   0 anton     (1000) anton     (1000)     1337 2022-08-12 22:29:09.527919 pygnmi-0.8.8/setup.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-21 21:34:42.776318 pygnmi-0.8.9/
+-rw-rw-r--   0 anton     (1000) anton     (1000)    18570 2022-08-21 21:34:42.776318 pygnmi-0.8.9/PKG-INFO
+-rw-rw-r--   0 anton     (1000) anton     (1000)    14186 2022-08-21 21:33:28.396574 pygnmi-0.8.9/README.rst
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-21 21:34:42.776318 pygnmi-0.8.9/pygnmi/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      104 2022-08-21 21:33:28.396574 pygnmi-0.8.9/pygnmi/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5475 2022-08-21 21:33:28.396574 pygnmi-0.8.9/pygnmi/arg_parser.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-21 21:34:42.776318 pygnmi-0.8.9/pygnmi/artefacts/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1637 2022-06-24 17:57:08.171652 pygnmi-0.8.9/pygnmi/artefacts/messages.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    52587 2022-08-21 21:33:28.396574 pygnmi-0.8.9/pygnmi/client.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1985 2022-07-24 12:53:02.054177 pygnmi-0.8.9/pygnmi/create_gnmi_extension.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     3350 2022-08-09 11:58:35.063076 pygnmi-0.8.9/pygnmi/create_gnmi_path.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-21 21:34:42.776318 pygnmi-0.8.9/pygnmi/spec/
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-21 21:34:42.776318 pygnmi-0.8.9/pygnmi/spec/v080/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4913 2022-07-23 10:19:42.631581 pygnmi-0.8.9/pygnmi/spec/v080/gnmi_ext_pb2.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    20495 2022-07-23 10:17:08.764539 pygnmi-0.8.9/pygnmi/spec/v080/gnmi_pb2.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     8598 2022-07-22 14:54:15.697673 pygnmi-0.8.9/pygnmi/spec/v080/gnmi_pb2_grpc.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     6900 2022-06-25 18:10:54.299842 pygnmi-0.8.9/pygnmi/tools.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-21 21:34:42.776318 pygnmi-0.8.9/scripts/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5379 2022-08-21 21:33:28.396574 pygnmi-0.8.9/scripts/pygnmicli
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1337 2022-08-21 21:33:28.396574 pygnmi-0.8.9/setup.py
```

### Comparing `pygnmi-0.8.8/PKG-INFO` & `pygnmi-0.8.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pygnmi
-Version: 0.8.8
+Version: 0.8.9
 Summary: Pure Python gNMI client to manage network functions and collect telemetry.
 Home-page: https://github.com/akarneliuk/pygnmi
 Author: Anton Karneliuk
 Author-email: anton@karneliuk.com
 License: bsd-3-clause
-Download-URL: https://github.com/akarneliuk/pygnmi/archive/v0.8.8.tar.gz
+Download-URL: https://github.com/akarneliuk/pygnmi/archive/v0.8.9.tar.gz
 Description: ==========================
         pyGNMI: Python gNMI client
         ==========================
         
         .. image:: https://github.com/akarneliuk/pygnmi/blob/master/logo.png
            :width: 300
            :height: 300
@@ -91,14 +91,20 @@
         - `Malanovo <https://github.com/malanovo>`_
         - `Sebastian Lohff <https://github.com/sebageek>`_
         
         =======
         Dev Log
         =======
         
+        Release **0.8.9**:
+        
+        - Default value for ``encoding`` everywhere is set to ``None``.
+        - Method ``capabilities()`` now is called as part of ``connect()`` to collect supported encoding as part of session establishing.
+        - If ``encoding`` is not specified by user, then it is auto-set based on the list collected via ``capabilites()`` with ``json`` having the first priority follwed by ``json_ietf``.
+        
         Release **0.8.8**:
         
         - Added new argument ``-e / --encoding`` to ``pygnmicli`` to specify the encoding, which overrides the default one. Fix for `Issue 58 <https://github.com/akarneliuk/pygnmi/issues/58>`_.
         - Fixed minor bug with encoding handling inside ``get()`` and ``subscribe2()`` methods.
         - Simplified the code.
         
         Release **0.8.7**:
@@ -416,15 +422,15 @@
         
         Release **0.1.0**:
         
         - The first release.
         
         (c)2020-2022, karneliuk.com
         
-        .. |version| image:: https://img.shields.io/static/v1?label=latest&message=v0.8.7&color=success
+        .. |version| image:: https://img.shields.io/static/v1?label=latest&message=v0.8.9&color=success
         .. _version: https://pypi.org/project/pygnmi/
         .. |tag| image:: https://img.shields.io/static/v1?label=status&message=stable&color=success
         .. _tag: https://pypi.org/project/pygnmi/
         .. |license| image:: https://img.shields.io/static/v1?label=license&message=BSD-3-clause&color=success
         .. _license: https://github.com/akarneliuk/pygnmi/blob/master/LICENSE.txt
         .. |project| image:: https://img.shields.io/badge/akarneliuk%2Fpygnmi-blueviolet.svg?logo=github&color=success
         .. _project: https://github.com/akarneliuk/pygnmi/
```

### Comparing `pygnmi-0.8.8/README.rst` & `pygnmi-0.8.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,20 @@
 - `Malanovo <https://github.com/malanovo>`_
 - `Sebastian Lohff <https://github.com/sebageek>`_
 
 =======
 Dev Log
 =======
 
+Release **0.8.9**:
+
+- Default value for ``encoding`` everywhere is set to ``None``.
+- Method ``capabilities()`` now is called as part of ``connect()`` to collect supported encoding as part of session establishing.
+- If ``encoding`` is not specified by user, then it is auto-set based on the list collected via ``capabilites()`` with ``json`` having the first priority follwed by ``json_ietf``.
+
 Release **0.8.8**:
 
 - Added new argument ``-e / --encoding`` to ``pygnmicli`` to specify the encoding, which overrides the default one. Fix for `Issue 58 <https://github.com/akarneliuk/pygnmi/issues/58>`_.
 - Fixed minor bug with encoding handling inside ``get()`` and ``subscribe2()`` methods.
 - Simplified the code.
 
 Release **0.8.7**:
@@ -407,15 +413,15 @@
 
 Release **0.1.0**:
 
 - The first release.
 
 (c)2020-2022, karneliuk.com
 
-.. |version| image:: https://img.shields.io/static/v1?label=latest&message=v0.8.7&color=success
+.. |version| image:: https://img.shields.io/static/v1?label=latest&message=v0.8.9&color=success
 .. _version: https://pypi.org/project/pygnmi/
 .. |tag| image:: https://img.shields.io/static/v1?label=status&message=stable&color=success
 .. _tag: https://pypi.org/project/pygnmi/
 .. |license| image:: https://img.shields.io/static/v1?label=license&message=BSD-3-clause&color=success
 .. _license: https://github.com/akarneliuk/pygnmi/blob/master/LICENSE.txt
 .. |project| image:: https://img.shields.io/badge/akarneliuk%2Fpygnmi-blueviolet.svg?logo=github&color=success
 .. _project: https://github.com/akarneliuk/pygnmi/
```

### Comparing `pygnmi-0.8.8/pygnmi/arg_parser.py` & `pygnmi-0.8.9/pygnmi/arg_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,20 @@
     )
     parser.add_argument(
         "--ext-history-snapshot-time",
         type=str,
         required=False,
         help="Specify the snapshit time for the GNMI history",
     )
+    parser.add_argument(
+        "--gnmi-timeout",
+        type=int,
+        required=False,
+        help="Specify the timeout for GNMI session",
+    )
 
     args = parser.parse_args()
 
     targets = args.target
     try:
         if re.match(r'\[.*\]', targets):
             parsed_args = re.sub(r'^\[([0-9a-fA-F:]+?)\]:(\d+?)$', r'\g<1> \g<2>', targets)
```

### Comparing `pygnmi-0.8.8/pygnmi/artefacts/messages.py` & `pygnmi-0.8.9/pygnmi/artefacts/messages.py`

 * *Files identical despite different names*

### Comparing `pygnmi-0.8.8/pygnmi/client.py` & `pygnmi-0.8.9/pygnmi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
                 # Set auto overrides
                 for san in self.__cert_sans:
                     self.__options.append(("grpc.ssl_target_name_override", san))
 
                 # Set empty override if neither CN ans SARs exist
                 if not ssl_cert_common_name and not self.__cert_sans:
-                    self.__options.append(("grpc.ssl_target_name_override", "".encode(encoding="utf-8")))
+                    self.__options.append(("grpc.ssl_target_name_override", ""))
 
                 logger.warning('ssl_target_name_override is applied, should be used for testing only!')
 
             # Set up SSL channel credentials
             if self.__path_key and self.__path_root:
                 cert = grpc.ssl_channel_credentials(root_certificates=root_cert,
                                                     private_key=key, certificate_chain=ssl_cert)
@@ -221,14 +221,16 @@
 
         if timeout is None:
             timeout = self.__gnmi_timeout
         if timeout is None or timeout > 0:
             self.wait_for_connect(timeout)
         self.__stub = gNMIStub(self.__channel)
 
+        self.__capabilities = self.capabilities()
+
         return self
 
     def wait_for_connect(self, timeout: int):
         """
         Wait for the gNMI connection to the server to come up, with given timeout
         """
         try:
@@ -289,29 +291,28 @@
                         response['supported_encodings'].append(dree)
 
                 if gnmi_message_response.gNMI_version:
                     response.update({'gnmi_version': gnmi_message_response.gNMI_version})
 
             logger.info(f'Collection of Capabilities is successfull')
 
-            self.__capabilities = response
             return response
 
         except grpc._channel._InactiveRpcError as err:
             logger.critical(f"GRPC ERROR Host: {self.__target_path}, Error: {err.details()}")
             raise gNMIException(f"GRPC ERROR Host: {self.__target_path}, Error: {err.details()}", err)
 
         except:
             logger.error('Collection of Capabilities is failed.')
 
             return None
 
     def get(self, prefix: str = "", path: list = None,
             target: str = None, datatype: str = 'all',
-            encoding: str = 'json'):
+            encoding: str = None):
         """
         Collecting the information about the resources from defined paths.
 
         Path is provided as a list in the following format:
           path = ['yang-module:container/container[key=value]', 'yang-module:container/container[key=value]', ..]
 
         Available path formats:
@@ -464,15 +465,15 @@
             raise gNMIException(f"GRPC ERROR Host: {self.__target_path}, Error: {err.details()}", err)
 
         except Exception as e:
             logger.error('Collection of Get information failed: %s.', e)
             raise gNMIException(f'Collection of Get information failed: {e}', e)
 
     def set(self, delete: list = None, replace: list = None,
-            update: list = None, encoding: str = 'json',
+            update: list = None, encoding: str = None,
             prefix: str = "", target: str = None):
         """
         Changing the configuration on the destination network elements.
         Could provide a single attribute or multiple attributes.
 
         delete:
           - list of paths with the resources to delete. The format is the same as for get() request
@@ -493,17 +494,29 @@
           - json_ietf
         """
         del_protobuf_paths = []
         replace_msg = []
         update_msg = []
         diff_list = []
 
-        if encoding.upper() not in Encoding.keys():
-            logger.error(f'The encoding {encoding} is not supported. The allowed are: {", ".join(Encoding.keys())}.')
-            raise gNMIException(f'The encoding {encoding} is not supported. The allowed are: {", ".join(Encoding.keys())}.')
+        # Set the encoding
+        if encoding:
+            if encoding.upper() not in Encoding.keys():
+                logger.error(f'The encoding {encoding} is not supported. The allowed are: {", ".join(Encoding.keys())}.')
+                raise gNMIException(f'The encoding {encoding} is not supported. The allowed are: {", ".join(Encoding.keys())}.')
+
+        else:
+            if "supported_encodings" in self.__capabilities and "json" in self.__capabilities['supported_encodings']:
+                encoding = "json"
+
+            elif "supported_encodings" in self.__capabilities and "json_ietf" in self.__capabilities['supported_encodings']:
+                encoding = "json_ietf"
+
+            else:
+                raise gNMIException('It is impossible to automtically detect encoding')
 
         # Gnmi PREFIX
         try:
             protobuf_prefix = gnmi_path_generator(prefix, target)
 
         except Exception as e:
             logger.error('Conversion of gNMI prefix to the Protobuf format failed')
@@ -607,15 +620,15 @@
             logger.critical(f"GRPC ERROR Host: {self.__target_path}, Error: {err.details()}")
             raise gNMIException(f"GRPC ERROR Host: {self.__target_path}, Error: {err.details()}", err)
         except Exception as e:
             logger.error("Set failed: %s", e)
             raise gNMIException(f"Set failed: {e}", e)
 
 
-    def set_with_retry(self, delete: list = None, replace: list = None, update: list = None, encoding: str = 'json', retry_delay: int = 3):
+    def set_with_retry(self, delete: list = None, replace: list = None, update: list = None, encoding: str = None, retry_delay: int = 3):
         """
         Performs a set and retries (once) after a temporary failure with StatusCode.FAILED_PRECONDITION
         """
         try:
             return self.set(delete=delete, replace=replace, update=update, encoding=encoding)
         except gNMIException as e:
             grpc_error = e.orig_exc
```

### Comparing `pygnmi-0.8.8/pygnmi/create_gnmi_extension.py` & `pygnmi-0.8.9/pygnmi/create_gnmi_extension.py`

 * *Files identical despite different names*

### Comparing `pygnmi-0.8.8/pygnmi/create_gnmi_path.py` & `pygnmi-0.8.9/pygnmi/create_gnmi_path.py`

 * *Files identical despite different names*

### Comparing `pygnmi-0.8.8/pygnmi/spec/v080/gnmi_ext_pb2.py` & `pygnmi-0.8.9/pygnmi/spec/v080/gnmi_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `pygnmi-0.8.8/pygnmi/spec/v080/gnmi_pb2.py` & `pygnmi-0.8.9/pygnmi/spec/v080/gnmi_pb2.py`

 * *Files identical despite different names*

### Comparing `pygnmi-0.8.8/pygnmi/spec/v080/gnmi_pb2_grpc.py` & `pygnmi-0.8.9/pygnmi/spec/v080/gnmi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pygnmi-0.8.8/pygnmi/tools.py` & `pygnmi-0.8.9/pygnmi/tools.py`

 * *Files identical despite different names*

### Comparing `pygnmi-0.8.8/scripts/pygnmicli` & `pygnmi-0.8.9/scripts/pygnmicli`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     args = parse_args(msg)
 
     # gNMI operation
     with gNMIclient(
         target=args.target, username=args.username, password=args.password, token=args.token,
         path_cert=args.path_cert, path_key=args.path_key, path_root=args.path_root,
         override=args.override, insecure=args.insecure, debug=args.debug,
-        show_diff=args.compare, skip_verify=args.skip_verify
+        show_diff=args.compare, skip_verify=args.skip_verify, gnmi_timeout=args.gnmi_timeout
     ) as GC:
 
         result = None
 
         # Collecting supported capabilities (needed to figure out encoding for telemetry)
         GC.capabilities()
```

### Comparing `pygnmi-0.8.8/setup.py` & `pygnmi-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open('README.rst', encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
   name='pygnmi',
   packages=['pygnmi', 'pygnmi.spec.v080', 'pygnmi.artefacts'],
-  version='0.8.8',
+  version='0.8.9',
   license='bsd-3-clause',
   description='Pure Python gNMI client to manage network functions and collect telemetry.',
   long_description=long_description,
   long_description_content_type='text/x-rst',
   author='Anton Karneliuk',
   author_email='anton@karneliuk.com',
   url='https://github.com/akarneliuk/pygnmi',
-  download_url='https://github.com/akarneliuk/pygnmi/archive/v0.8.8.tar.gz',
+  download_url='https://github.com/akarneliuk/pygnmi/archive/v0.8.9.tar.gz',
   keywords=['gnmi', 'automation', 'grpc', 'network'],
   install_requires=[
           'grpcio',
           'protobuf',
           'cryptography',
           'dictdiffer'
   ],
```

