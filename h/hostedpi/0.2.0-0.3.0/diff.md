# Comparing `tmp/hostedpi-0.2.0.tar.gz` & `tmp/hostedpi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostedpi-0.2.0.tar", last modified: Sat Jul 17 22:01:39 2021, max compression
+gzip compressed data, was "hostedpi-0.3.0.tar", last modified: Sun Apr 30 11:23:43 2023, max compression
```

## Comparing `hostedpi-0.2.0.tar` & `hostedpi-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2021-07-17 22:01:39.808998 hostedpi-0.2.0/
--rw-rw-r--   0 ben       (1000) ben       (1000)     1571 2021-03-17 02:56:32.000000 hostedpi-0.2.0/LICENSE.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       39 2021-03-17 02:56:32.000000 hostedpi-0.2.0/MANIFEST.in
--rw-rw-r--   0 ben       (1000) ben       (1000)     4544 2021-07-17 22:01:39.808998 hostedpi-0.2.0/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)     2668 2021-07-17 22:00:29.000000 hostedpi-0.2.0/README.rst
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2021-07-17 22:01:39.808998 hostedpi-0.2.0/hostedpi/
--rw-rw-r--   0 ben       (1000) ben       (1000)      114 2021-03-17 02:56:32.000000 hostedpi-0.2.0/hostedpi/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)       22 2021-07-17 21:53:28.000000 hostedpi-0.2.0/hostedpi/__version__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1628 2021-03-17 02:56:32.000000 hostedpi-0.2.0/hostedpi/auth.py
--rw-rw-r--   0 ben       (1000) ben       (1000)    20945 2021-07-06 11:41:33.000000 hostedpi-0.2.0/hostedpi/cli.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      197 2021-03-17 02:56:32.000000 hostedpi-0.2.0/hostedpi/exc.py
--rw-rw-r--   0 ben       (1000) ben       (1000)    13791 2021-07-08 23:28:43.000000 hostedpi-0.2.0/hostedpi/pi.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     9244 2021-07-08 17:26:56.000000 hostedpi-0.2.0/hostedpi/picloud.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1901 2021-03-17 02:56:32.000000 hostedpi-0.2.0/hostedpi/utils.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2021-07-17 22:01:39.808998 hostedpi-0.2.0/hostedpi.egg-info/
--rw-rw-r--   0 ben       (1000) ben       (1000)     4544 2021-07-17 22:01:39.000000 hostedpi-0.2.0/hostedpi.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      394 2021-07-17 22:01:39.000000 hostedpi-0.2.0/hostedpi.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        1 2021-07-17 22:01:39.000000 hostedpi-0.2.0/hostedpi.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       48 2021-07-17 22:01:39.000000 hostedpi-0.2.0/hostedpi.egg-info/entry_points.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       87 2021-07-17 22:01:39.000000 hostedpi-0.2.0/hostedpi.egg-info/requires.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        9 2021-07-17 22:01:39.000000 hostedpi-0.2.0/hostedpi.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)     1335 2021-07-17 22:01:39.812998 hostedpi-0.2.0/setup.cfg
--rw-rw-r--   0 ben       (1000) ben       (1000)       38 2021-03-17 02:56:32.000000 hostedpi-0.2.0/setup.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-04-30 11:23:43.764764 hostedpi-0.3.0/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1571 2021-03-17 02:56:32.000000 hostedpi-0.3.0/LICENSE.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       39 2021-03-17 02:56:32.000000 hostedpi-0.3.0/MANIFEST.in
+-rw-rw-r--   0 ben       (1000) ben       (1000)     3832 2023-04-30 11:23:43.764764 hostedpi-0.3.0/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)     2668 2021-07-17 22:00:29.000000 hostedpi-0.3.0/README.rst
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-04-30 11:23:43.764764 hostedpi-0.3.0/hostedpi/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      114 2021-03-17 02:56:32.000000 hostedpi-0.3.0/hostedpi/__init__.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)       22 2023-04-30 11:16:55.000000 hostedpi-0.3.0/hostedpi/__version__.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1797 2023-04-30 11:16:55.000000 hostedpi-0.3.0/hostedpi/auth.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)    21824 2023-04-30 11:16:55.000000 hostedpi-0.3.0/hostedpi/cli.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      198 2023-04-30 11:16:55.000000 hostedpi-0.3.0/hostedpi/exc.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-04-30 11:23:43.764764 hostedpi-0.3.0/hostedpi/models/
+-rw-rw-r--   0 ben       (1000) ben       (1000)        0 2022-09-03 14:02:51.000000 hostedpi-0.3.0/hostedpi/models/__init__.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      500 2023-04-22 13:26:31.000000 hostedpi-0.3.0/hostedpi/models/auth.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      172 2023-04-22 13:26:31.000000 hostedpi-0.3.0/hostedpi/models/settings.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)    14932 2023-04-30 11:16:55.000000 hostedpi-0.3.0/hostedpi/pi.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)    10249 2023-04-30 11:16:55.000000 hostedpi-0.3.0/hostedpi/picloud.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     2187 2023-04-30 11:16:55.000000 hostedpi-0.3.0/hostedpi/utils.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-04-30 11:23:43.764764 hostedpi-0.3.0/hostedpi.egg-info/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     3832 2023-04-30 11:23:43.000000 hostedpi-0.3.0/hostedpi.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)      474 2023-04-30 11:23:43.000000 hostedpi-0.3.0/hostedpi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)        1 2023-04-30 11:23:43.000000 hostedpi-0.3.0/hostedpi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       47 2023-04-30 11:23:43.000000 hostedpi-0.3.0/hostedpi.egg-info/entry_points.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       51 2023-04-30 11:23:43.000000 hostedpi-0.3.0/hostedpi.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)        9 2023-04-30 11:23:43.000000 hostedpi-0.3.0/hostedpi.egg-info/top_level.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1297 2023-04-30 11:23:43.764764 hostedpi-0.3.0/setup.cfg
+-rw-rw-r--   0 ben       (1000) ben       (1000)       38 2021-03-17 02:56:32.000000 hostedpi-0.3.0/setup.py
```

### Comparing `hostedpi-0.2.0/LICENSE.txt` & `hostedpi-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hostedpi-0.2.0/PKG-INFO` & `hostedpi-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,115 @@
 Metadata-Version: 2.1
 Name: hostedpi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python interface to the Mythic Beasts Hosted Pi API
 Home-page: https://hostedpi.readthedocs.io/
 Author: The piwheels team
 Author-email: ben@bennuttall.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://hostedpi.readthedocs.io/
 Project-URL: Source Code, https://github.com/piwheels/hostedpi
 Project-URL: Issue Tracker, https://github.com/piwheels/hostedpi/issues
-Description: ========
-        hostedpi
-        ========
-        
-        .. image:: https://badge.fury.io/py/hostedpi.svg
-            :target: https://badge.fury.io/py/hostedpi
-            :alt: Latest Version
-        
-        Python interface to the `Mythic Beasts Hosted Pi`_ API, developed by the
-        `piwheels`_ team (`Ben Nuttall`_ and `Dave Jones`_).
-        
-        .. _Mythic Beasts Hosted Pi: https://www.mythic-beasts.com/order/rpi
-        .. _piwheels: https://www.piwheels.org/
-        .. _Ben Nuttall: https://twitter.com/ben_nuttall
-        .. _Dave Jones: https://twitter.com/waveform80
-        
-        This module provides a Pythonic interface to the API, as well as a command line
-        interface.
-        
-        The authors of this library are not affiliated with Mythic Beasts, but we use
-        their Pi cloud to power the piwheels project.
-        
-        Documentation of the API itself can be found at
-        https://www.mythic-beasts.com/support/api/raspberry-pi
-        
-        Usage
-        =====
-        
-        View the information about a Pi from the command line:
-        
-        .. code-block:: console
-        
-            $ hostedpi show mypi
-            Name: mypi
-            Provision status: live
-            Model: Raspberry Pi 3B
-            Disk size: 10GB
-            Power: on
-            IPv6 address: 2a00:1098:8:5b::1
-            IPv6 network: 2a00:1098:8:5b00::/56
-            Initialised keys: yes
-            SSH keys: 4
-            IPv4 SSH port: 5091
-            Location: MER
-            URLs:
-              http://www.mypi.hostedpi.com
-              https://www.mypi.hostedpi.com
-            SSH commands:
-              ssh -p 5091 root@ssh.mypi.hostedpi.com  #IPv4
-              ssh root@[2a00:1098:8:5b::1]  #IPv6
-        
-        Provision a new Pi and view its SSH command (using Python):
-        
-        .. code-block:: pycon
-        
-            >>> from hostedpi import PiCloud
-            >>> api_id = '8t29hvcux5g9vud8'
-            >>> secret = 'QNwsvxZY8SxT3OiLt:Vmz-D1mWQuoZ'
-            >>> cloud = PiCloud(api_id, secret, ssh_key_path='/home/ben/.ssh/id_rsa.pub')
-            >>> pi = cloud.create_pi('mypi')
-            >>> print(pi.ssh_command)
-            ssh -p 5123 root@ssh.mypi.hostedpi.com
-        
-        See the `getting started`_ page for information on how to authenticate, and
-        see the `command line interface`_ page for information on using the command line
-        interface.
-        
-        .. _getting started: https://hostedpi.readthedocs.io/en/latest/getting_started.html
-        .. _command line interface: https://hostedpi.readthedocs.io/en/latest/cli.html
-        
-        Documentation
-        =============
-        
-        Documentation for this module can be found at https://hostedpi.readthedocs.io/
-        
-        Documentation of the API itself can be found at
-        https://www.mythic-beasts.com/support/api/raspberry-pi
-        
-        Contributing
-        ============
-        
-        * Source code can be found on GitHub at https://github.com/piwheels/hostedpi
-        * Code and documentation contributions welcome
-        * The issue tracker can be found at https://github.com/piwheels/hostedpi/issues
-        * For issues with the API itself, please contact Mythic Beasts support
-          https://www.mythic-beasts.com/support
-        
 Keywords: raspberrypi,mythicbeasts,picloud,piwheels
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.5
-Provides-Extra: test
+Requires-Python: >=3.7
 Provides-Extra: doc
+License-File: LICENSE.txt
+
+========
+hostedpi
+========
+
+.. image:: https://badge.fury.io/py/hostedpi.svg
+    :target: https://badge.fury.io/py/hostedpi
+    :alt: Latest Version
+
+Python interface to the `Mythic Beasts Hosted Pi`_ API, developed by the
+`piwheels`_ team (`Ben Nuttall`_ and `Dave Jones`_).
+
+.. _Mythic Beasts Hosted Pi: https://www.mythic-beasts.com/order/rpi
+.. _piwheels: https://www.piwheels.org/
+.. _Ben Nuttall: https://twitter.com/ben_nuttall
+.. _Dave Jones: https://twitter.com/waveform80
+
+This module provides a Pythonic interface to the API, as well as a command line
+interface.
+
+The authors of this library are not affiliated with Mythic Beasts, but we use
+their Pi cloud to power the piwheels project.
+
+Documentation of the API itself can be found at
+https://www.mythic-beasts.com/support/api/raspberry-pi
+
+Usage
+=====
+
+View the information about a Pi from the command line:
+
+.. code-block:: console
+
+    $ hostedpi show mypi
+    Name: mypi
+    Provision status: live
+    Model: Raspberry Pi 3B
+    Disk size: 10GB
+    Power: on
+    IPv6 address: 2a00:1098:8:5b::1
+    IPv6 network: 2a00:1098:8:5b00::/56
+    Initialised keys: yes
+    SSH keys: 4
+    IPv4 SSH port: 5091
+    Location: MER
+    URLs:
+      http://www.mypi.hostedpi.com
+      https://www.mypi.hostedpi.com
+    SSH commands:
+      ssh -p 5091 root@ssh.mypi.hostedpi.com  #IPv4
+      ssh root@[2a00:1098:8:5b::1]  #IPv6
+
+Provision a new Pi and view its SSH command (using Python):
+
+.. code-block:: pycon
+
+    >>> from hostedpi import PiCloud
+    >>> api_id = '8t29hvcux5g9vud8'
+    >>> secret = 'QNwsvxZY8SxT3OiLt:Vmz-D1mWQuoZ'
+    >>> cloud = PiCloud(api_id, secret, ssh_key_path='/home/ben/.ssh/id_rsa.pub')
+    >>> pi = cloud.create_pi('mypi')
+    >>> print(pi.ssh_command)
+    ssh -p 5123 root@ssh.mypi.hostedpi.com
+
+See the `getting started`_ page for information on how to authenticate, and
+see the `command line interface`_ page for information on using the command line
+interface.
+
+.. _getting started: https://hostedpi.readthedocs.io/en/latest/getting_started.html
+.. _command line interface: https://hostedpi.readthedocs.io/en/latest/cli.html
+
+Documentation
+=============
+
+Documentation for this module can be found at https://hostedpi.readthedocs.io/
+
+Documentation of the API itself can be found at
+https://www.mythic-beasts.com/support/api/raspberry-pi
+
+Contributing
+============
+
+* Source code can be found on GitHub at https://github.com/piwheels/hostedpi
+* Code and documentation contributions welcome
+* The issue tracker can be found at https://github.com/piwheels/hostedpi/issues
+* For issues with the API itself, please contact Mythic Beasts support
+  https://www.mythic-beasts.com/support
```

### Comparing `hostedpi-0.2.0/README.rst` & `hostedpi-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `hostedpi-0.2.0/hostedpi/auth.py` & `hostedpi-0.3.0/hostedpi/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 from datetime import datetime, timedelta
 
-import requests
-from requests.exceptions import HTTPError
+from requests import Session, HTTPError
 
 from .exc import MythicAuthenticationError
 from .__version__ import __version__
 
 
 class MythicAuth:
     _LOGIN_URL = "https://auth.mythic-beasts.com/login"
 
-    def __init__(self, api_id, api_secret):
+    def __init__(self, api_id: str, api_secret: str):
         self._creds = (api_id, api_secret)
         self._token = None
         self._token_expiry = datetime.now()
-        self._headers = {
-            'User-Agent': 'python-hostedpi/' + __version__,
+        self._session = Session()
+        self._session.headers = {
+            "User-Agent": f"python-hostedpi/{__version__}",
         }
-        self._authenticate()
+        # force the session to authenticate now
+        self.session
 
     def __repr__(self):
         return "<MythicAuth>"
 
     @property
-    def headers(self):
-        headers = self._headers
-        headers['Authorization'] = 'Bearer ' + self.token
-        return headers
+    def session(self) -> Session:
+        self._session.headers["Authorization"] = f"Bearer {self.token}"
+        return self._session
 
     @property
-    def token(self):
+    def token(self) -> str:
         if datetime.now() > self._token_expiry:
-            self._token = self._authenticate()
+            data = {"grant_type": "client_credentials"}
+            self._session.headers.pop("Authorization", None)
+            self._session.headers.pop("Content-Type", None)
+            r = self._session.post(self._LOGIN_URL, auth=self._creds, data=data)
+
+            try:
+                r.raise_for_status()
+            except HTTPError as e:
+                print(r.text)
+                raise MythicAuthenticationError("Failed to authenticate") from e
+
+            body = r.json()
+            if "access_token" in body:
+                self._token = body["access_token"]
+                expires = body.get("expires_in", 0)
+                self._token_expiry = datetime.now() + timedelta(seconds=expires)
+                self._token = body["access_token"]
+            else:
+                raise MythicAuthenticationError("No access token in response")
         return self._token
-
-    def _authenticate(self):
-        data = {
-            'grant_type': 'client_credentials'
-        }
-        r = requests.post(self._LOGIN_URL, headers=self._headers,
-                          auth=self._creds, data=data)
-
-        try:
-            r.raise_for_status()
-        except HTTPError as e:
-            raise MythicAuthenticationError("Failed to authenticate") from e
-
-        body = r.json()
-        if 'access_token' in body:
-            self._token = body['access_token']
-            expires = body.get('expires_in', 0)
-            self._token_expiry = datetime.now() + timedelta(seconds=expires)
-            return body['access_token']
-        raise MythicAuthenticationError("no access token in response")
```

### Comparing `hostedpi-0.2.0/hostedpi/cli.py` & `hostedpi-0.3.0/hostedpi/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,27 +20,29 @@
         self._pis = None
 
     def __call__(self, args=None):
         self._args = self.parser.parse_args(args)
         try:
             return self._args.func()
         except HostedPiException as e:
-            sys.stderr.write("hostedpi error: {e}\n".format(e=e))
+            sys.stderr.write(f"hostedpi error: {e}\n")
             return 2
         except KeyboardInterrupt:
             print("Operation cancelled during process")
 
     @property
     def cloud(self):
         if self._cloud is None:
-            API_ID = os.environ.get('HOSTEDPI_ID')
-            API_SECRET = os.environ.get('HOSTEDPI_SECRET')
+            API_ID = os.environ.get("HOSTEDPI_ID")
+            API_SECRET = os.environ.get("HOSTEDPI_SECRET")
             if API_ID is None or API_SECRET is None:
-                print("HOSTEDPI_ID and HOSTEDPI_SECRET environment variables "
-                      "must be set")
+                print(
+                    "HOSTEDPI_ID and HOSTEDPI_SECRET environment variables "
+                    "must be set"
+                )
             self._cloud = PiCloud(API_ID, API_SECRET)
         return self._cloud
 
     @property
     def pis(self):
         if self._pis is None:
             self._pis = self.cloud.pis
@@ -63,263 +65,336 @@
             self._parser, self._commands = self._get_parser()
         return self._commands
 
     def _get_parser(self):
         parser = argparse.ArgumentParser(
             description=(
                 "hostedpi is a tool for provisioning and managing Raspberry Pis "
-                "in the Mythic Beasts Pi Cloud"))
-        parser.add_argument(
-            '--version', action='version', version=__version__)
+                "in the Mythic Beasts Pi Cloud"
+            )
+        )
+        parser.add_argument("--version", action="version", version=__version__)
         parser.set_defaults(func=self.do_help, cmd=None)
         commands = parser.add_subparsers(title=("commands"))
 
         help_cmd = commands.add_parser(
-            "help", aliases=["h"],
+            "help",
+            aliases=["h"],
             description=(
                 "With no arguments, displays the list of hostedpi "
                 "commands. If a command name is given, displays the "
                 "description and options for the named command. If a "
                 "setting name is given, displays the description and "
-                "default value for that setting."),
-            help=("Displays help about the specified command or setting"))
+                "default value for that setting."
+            ),
+            help=("Displays help about the specified command or setting"),
+        )
         help_cmd.add_argument(
-            "cmd", metavar="cmd", nargs='?',
-            help=("The name of the command to output help for")
+            "cmd",
+            metavar="cmd",
+            nargs="?",
+            help=("The name of the command to output help for"),
         )
         help_cmd.set_defaults(func=self.do_help)
 
         test_cmd = commands.add_parser(
-            "test", aliases=["connect"],
+            "test",
+            aliases=["connect"],
             description=(
                 "Test a connection to the Mythic Beasts API using API ID and "
-                "secret in environment variables."),
-            help=("Test a connection to the Mythic Beasts API"))
+                "secret in environment variables"
+            ),
+            help=("Test a connection to the Mythic Beasts API"),
+        )
         test_cmd.set_defaults(func=self.do_test)
 
         get_images_cmd = commands.add_parser(
             "images",
-            description=("Retrieve the list of operating system images available for the given Pi model."),
-            help=("Retrieve the list of operating system images available for the given Pi model"))
+            description=(
+                "Retrieve the list of operating system images available for the given Pi model"
+            ),
+            help=(
+                "Retrieve the list of operating system images available for the given Pi model"
+            ),
+        )
         get_images_cmd.add_argument(
-            "model", metavar="model", nargs='?', type=int,
-            help=("The Pi model number (3 or 4) to get operating systems for")
+            "model",
+            metavar="model",
+            nargs="?",
+            type=int,
+            help=("The Pi model number (3 or 4) to get operating systems for"),
         )
         get_images_cmd.set_defaults(func=self.do_get_images)
 
         list_cmd = commands.add_parser(
-            "list", aliases=["ls"],
+            "list",
+            aliases=["ls"],
             description=("List all Pis in the account"),
-            help=("List all Pis in the account"))
+            help=("List all Pis in the account"),
+        )
         list_cmd.set_defaults(func=self.do_list)
 
         show_cmd = commands.add_parser(
-            "show", aliases=["cat"],
+            "show",
+            aliases=["cat"],
             description=("Show the information about one or more Pis in the account"),
-            help=("Show the information about one or more Pis in the account"))
+            help=("Show the information about one or more Pis in the account"),
+        )
         show_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The names of the Pis to show information for")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to show information for"),
         )
         show_cmd.set_defaults(func=self.do_show_pis)
 
         create_cmd = commands.add_parser(
             "create",
             description=("Provision a new Pi in the account"),
-            help=("Provision a new Pi in the account"))
+            help=("Provision a new Pi in the account"),
+        )
         create_cmd.add_argument(
-            "name", metavar="name",
-            help=("The name of the new Pi to provision")
+            "name", metavar="name", help=("The name of the new Pi to provision")
         )
         create_cmd.add_argument(
-            "--model", metavar="model", type=int, nargs='?',
-            help=("The model of the new Pi to provision (3 or 4)")
+            "--model",
+            metavar="model",
+            type=int,
+            nargs="?",
+            help=("The model of the new Pi to provision (3 or 4)"),
         )
         create_cmd.add_argument(
-            "--disk", metavar="disk", type=int, nargs='?',
-            help=("The disk size in GB")
+            "--disk", metavar="disk", type=int, nargs="?", help=("The disk size in GB")
         )
         create_cmd.add_argument(
-            "--image", metavar="image", type=str, nargs='?',
-            help=("The operating system image to use")
+            "--image",
+            metavar="image",
+            type=str,
+            nargs="?",
+            help=("The operating system image to use"),
         )
         create_cmd.add_argument(
-            "--ssh-key-path", metavar="ssh_key_path", nargs='?',
-            help=("The path to an SSH public key file to add to the Pi")
+            "--ssh-key-path",
+            metavar="ssh_key_path",
+            nargs="?",
+            help=("The path to an SSH public key file to add to the Pi"),
         )
         create_cmd.set_defaults(func=self.do_create)
 
         provision_status_cmd = commands.add_parser(
             "status",
             description=("Get the provision status of one or more Pis"),
-            help=("Get the provision status of one or more Pis"))
+            help=("Get the provision status of one or more Pis"),
+        )
         provision_status_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The names of the Pis to get the provision status for")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to get the provision status for"),
         )
         provision_status_cmd.set_defaults(func=self.do_provision_status)
 
         power_status_cmd = commands.add_parser(
             "power",
             description=("Get the power status for one or more Pis"),
-            help=("Get the power status (on/off) for one or more Pis"))
+            help=("Get the power status (on/off) for one or more Pis"),
+        )
         power_status_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The names of the Pis to get the power status for")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to get the power status for"),
         )
         power_status_cmd.set_defaults(func=self.do_power_status)
 
         reboot_cmd = commands.add_parser(
             "reboot",
             description=("Reboot one or more Pis in the account"),
-            help=("Reboot one or more Pis in the account"))
+            help=("Reboot one or more Pis in the account"),
+        )
         reboot_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The name of the Pi to reboot")
+            "names", metavar="names", nargs="*", help=("The names of the Pis to reboot")
         )
         reboot_cmd.set_defaults(func=self.do_reboot)
 
         power_on_cmd = commands.add_parser(
-            "on", aliases=["poweron"],
+            "on",
             description=("Power on one or more Pis in the account"),
-            help=("Power on one or more Pis in the account"))
+            help=("Power on one or more Pis in the account"),
+        )
         power_on_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The name of the Pi to power on")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to power on"),
         )
         power_on_cmd.set_defaults(func=self.do_power_on)
 
         power_off_cmd = commands.add_parser(
-            "off", aliases=["poweroff"],
+            "off",
             description=("Power off one or more Pis in the account"),
-            help=("Power off one or more Pis in the account"))
+            help=("Power off one or more Pis in the account"),
+        )
         power_off_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The name of the Pi to power off")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to power off"),
         )
         power_off_cmd.set_defaults(func=self.do_power_off)
 
         cancel_cmd = commands.add_parser(
             "cancel",
+            aliases=["rm"],
             description=("Cancel one or more Pis in the account"),
-            help=("Cancel one or more Pis in the account"))
+            help=("Cancel one or more Pis in the account"),
+        )
         cancel_cmd.add_argument(
-            "names", metavar="names", nargs='+',
-            help=("The names of the Pis to cancel")
+            "names", metavar="names", nargs="+", help=("The names of the Pis to cancel")
         )
         cancel_cmd.add_argument(
-            "-y", "--yes",
-            action="store_true",
-            help=("Proceed without confirmation")
+            "-y", "--yes", action="store_true", help=("Proceed without confirmation")
         )
         cancel_cmd.set_defaults(func=self.do_cancel)
 
         count_keys_cmd = commands.add_parser(
-            "count-keys", aliases=["num-keys"],
+            "count-keys",
             description=("Show the number of SSH keys currently on one or more Pis"),
-            help=("Show the number of SSH keys currently on one or more Pis"))
+            help=("Show the number of SSH keys currently on one or more Pis"),
+        )
         count_keys_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The names of the Pis to get keys for")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to count keys for"),
         )
         count_keys_cmd.set_defaults(func=self.do_count_keys)
 
         show_keys_cmd = commands.add_parser(
             "keys",
             description=("Show the SSH keys currently on a Pi"),
-            help=("Show the SSH keys currently on a Pi"))
+            help=("Show the SSH keys currently on a Pi"),
+        )
         show_keys_cmd.add_argument(
-            "name", metavar="name",
-            help=("The name of the Pi to get keys for")
+            "name", metavar="name", help=("The name of the Pi to show keys for")
         )
         show_keys_cmd.set_defaults(func=self.do_show_keys)
 
         add_key_cmd = commands.add_parser(
             "add-key",
             description=("Add an SSH key from a public key file to one or more Pis"),
-            help=("Add an SSH key from a public key file to one or more Pis"))
+            help=("Add an SSH key from a public key file to one or more Pis"),
+        )
         add_key_cmd.add_argument(
-            "ssh_key_path", metavar="ssh_key_path", nargs='?',
-            help=("The path to an SSH public key file to add to the Pi")
+            "ssh_key_path",
+            metavar="ssh_key_path",
+            help=("The path to an SSH public key file to add to the Pi"),
         )
         add_key_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The name of the Pis to add keys to")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to add keys to"),
         )
         add_key_cmd.set_defaults(func=self.do_add_key)
 
         copy_keys_cmd = commands.add_parser(
-            "copy-keys", aliases=["cp"],
+            "copy-keys",
+            aliases=["cp"],
             description=("Copy all SSH keys from one Pi to one or more others"),
-            help=("Copy all SSH keys from one Pi to one or more others"))
+            help=("Copy all SSH keys from one Pi to one or more others"),
+        )
         copy_keys_cmd.add_argument(
-            "name_src", metavar="name_src",
-            help=("The name of the Pi to copy keys from")
+            "name_src",
+            metavar="name_src",
+            help=("The name of the Pi to copy keys from"),
         )
         copy_keys_cmd.add_argument(
-            "names_dest", metavar="names_dest", nargs='*',
-            help=("The name of the Pis to copy keys to")
+            "names_dest",
+            metavar="names_dest",
+            nargs="*",
+            help=("The names of the Pis to copy keys to"),
         )
         copy_keys_cmd.set_defaults(func=self.do_copy_keys)
 
         remove_keys_cmd = commands.add_parser(
             "remove-keys",
             description=("Remove all SSH keys from one or more Pis"),
-            help=("Remove all SSH keys from one or more Pis"))
+            help=("Remove all SSH keys from one or more Pis"),
+        )
         remove_keys_cmd.add_argument(
-            "names", metavar="names", nargs='+',
-            help=("The names of the Pis to remove keys from")
+            "names",
+            metavar="names",
+            nargs="+",
+            help=("The names of the Pis to remove keys from"),
         )
         remove_keys_cmd.set_defaults(func=self.do_remove_keys)
 
         ssh_import_id_cmd = commands.add_parser(
             "ssh-import-id",
-            description=("Import SSH keys from GitHub or Launchpad and add them to one or more Pis"),
-            help=("Import SSH keys from GitHub or Launchpad and add them to one or more Pis"))
+            description=(
+                "Import SSH keys from GitHub or Launchpad and add them to one or more Pis"
+            ),
+            help=(
+                "Import SSH keys from GitHub or Launchpad and add them to one or more Pis"
+            ),
+        )
         ssh_import_id_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The names of the Pis to import keys onto")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to import keys onto"),
         )
         ssh_import_id_cmd.add_argument(
-            "--gh", metavar="github username", nargs='?',
-            help=("The GitHub username to import keys from")
+            "--gh",
+            metavar="github username",
+            nargs="?",
+            help=("The GitHub username to import keys from"),
         )
         ssh_import_id_cmd.add_argument(
-            "--lp", metavar="launchpad username", nargs='?',
-            help=("The Launchpad username to import keys from")
+            "--lp",
+            metavar="launchpad username",
+            nargs="?",
+            help=("The Launchpad username to import keys from"),
         )
         ssh_import_id_cmd.set_defaults(func=self.do_ssh_import_id)
 
         ssh_command_cmd = commands.add_parser(
             "ssh-command",
             description=("Output the SSH command for one or more Pis in the account"),
-            help=("Output the (IPv4 or IPv6) SSH command for one or more Pis in the account"))
+            help=(
+                "Output the SSH command for one or more Pis in the account"
+            ),
+        )
         ssh_command_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The names of the Pis to get SSH commands for")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to get SSH commands for"),
         )
         ssh_command_cmd.add_argument(
-            "--ipv6",
-            action="store_true",
-            help=("Show IPv6 command")
+            "--ipv6", action="store_true", help=("Show IPv6 command")
         )
         ssh_command_cmd.set_defaults(func=self.do_ssh_command)
 
         ssh_config_cmd = commands.add_parser(
             "ssh-config",
             description=("Output the SSH config for one or more Pis in the account"),
-            help=("Output the (IPv4 or IPv6) SSH config for one or more Pis in the account"))
+            help=(
+                "Output the SSH config for one or more Pis in the account"
+            ),
+        )
         ssh_config_cmd.add_argument(
-            "names", metavar="names", nargs='*',
-            help=("The names of the Pis to get SSH config for")
+            "names",
+            metavar="names",
+            nargs="*",
+            help=("The names of the Pis to get SSH config for"),
         )
         ssh_config_cmd.add_argument(
-            "--ipv6",
-            action="store_true",
-            help=("Show IPv6 command")
+            "--ipv6", action="store_true", help=("Use IPv6 connection details")
         )
         ssh_config_cmd.set_defaults(func=self.do_ssh_config)
 
         return parser, commands.choices
 
     def get_pi(self, name):
         pi = self.pis.get(name)
@@ -330,195 +405,204 @@
 
     def get_pis(self, names):
         if not names:
             return self.pis.items()
         return {name: self.pis.get(name) for name in names}.items()
 
     def print_not_found(self, name):
-        sys.stderr.write("{name} not found\n".format(name=name))
+        sys.stderr.write(f"{name} not found\n")
 
     def do_help(self):
         if self._args.cmd:
-            self.parser.parse_args([self._args.cmd, '-h'])
+            self.parser.parse_args([self._args.cmd, "-h"])
         else:
-            self.parser.parse_args(['-h'])
+            self.parser.parse_args(["-h"])
 
     def do_test(self):
         if self.cloud:
             print("Connected to the Mythic Beasts API")
             return
         return 2
 
     def do_get_images(self):
         if self._args.model is None:
             models = [3, 4]
         else:
-            models = [self._args.model]
+            models = [int(m) for m in self._args.model]
 
         for model in models:
-            print("Images for Pi {model}:".format(model=model))
+            print(f"Images for Pi {model}:")
             images = self.cloud.get_operating_systems(model=model)
             col_width = max(len(name) for name in images.values()) + 1
             for id, name in images.items():
-                print("{name:{col_width}}: {id}".format(name=name, id=id, col_width=col_width))
+                print(f"{name:{col_width}}: {id}")
             print()
 
     def do_list(self):
         for name in self.pis:
             print(name)
 
     def do_show_pis(self):
         for name, pi in self.get_pis(self._args.names):
             if pi:
-                print(pi, end='\n\n')
+                print(pi, end="\n\n")
             else:
                 self.print_not_found(name)
 
     def do_create(self):
         name = self._args.name
         model = self._args.model
         disk_size = self._args.disk
         ssh_key_path = self._args.ssh_key_path
         os_image = self._args.image
         args = {
-            'model': model,
-            'disk_size': disk_size,
-            'ssh_key_path': ssh_key_path,
-            'os_image': os_image,
+            "model": model,
+            "disk_size": disk_size,
+            "ssh_key_path": ssh_key_path,
+            "os_image": os_image,
         }
 
         kwargs = {k: v for k, v in args.items() if v is not None}
-        pi = self.cloud.create_pi(name, **kwargs)
+        self.cloud.create_pi(name, **kwargs)
 
-        print("Pi {} provisioned successfully".format(name))
-        print()
-        print(pi)
+        print(f"Pi {name} provisioned successfully")
 
     def do_reboot(self):
         for name, pi in self.get_pis(self._args.names):
             if pi:
                 pi.reboot()
-                print("{name} rebooted".format(name=name))
+                print(f"{name} rebooted")
             else:
                 self.print_not_found(name)
 
     def do_power_on(self):
         for name, pi in self.get_pis(self._args.names):
             if pi:
                 pi.on()
-                print("{name} powered on".format(name=name))
+                print(f"{name} powered on")
             else:
                 self.print_not_found(name)
 
     def do_power_off(self):
         for name, pi in self.get_pis(self._args.names):
             if pi:
                 pi.off()
-                print("{name} powered off".format(name=name))
+                print(f"{name} powered off")
             else:
                 self.print_not_found(name)
 
     def do_cancel(self):
         if not self._args.yes:
-            num_pis = len(self._args.names)
+            pis_to_cancel = sorted(set(self._args.names) & set(self.pis))
+            if len(pis_to_cancel) == 0:
+                print("No Pis to cancel. Check the server names are correct.")
+                return
+            elif len(pis_to_cancel) == 1:
+                pi = pis_to_cancel[0]
+                cancel_prompt = (
+                    f"Cancelling {pi}. Proceed? [Y/n] "
+                )
+            else:
+                cancel_prompt = (
+                    f"Cancelling {len(pis_to_cancel)} Pis: [{', '.join(pis_to_cancel)}]. Proceed? [Y/n] "
+                )
             try:
-                s = '' if num_pis == 1 else 's'
-                y = input("Cancelling {n} Pi{s}. Proceed? [Y/n]".format(n=num_pis, s=s))
+                y = input(cancel_prompt)
             except KeyboardInterrupt:
                 print()
                 print("Not cancelled")
                 return
             if y.lower() not in 'y':
                 print("Not cancelled")
                 return
         for name, pi in self.get_pis(self._args.names):
             if pi:
                 pi.cancel()
-                print("{name} cancelled".format(name=name))
+                print(f"{name} cancelled")
             else:
                 self.print_not_found(name)
 
     def do_show_keys(self):
         pi = self.get_pi(self._args.name)
         if not pi:
             return 2
-        print(*pi.ssh_keys, sep='\n')
+        print(*pi.ssh_keys, sep="\n")
 
     def do_count_keys(self):
         for name, pi in self.get_pis(self._args.names):
             num_keys = len(pi.ssh_keys)
-            s = '' if num_keys == 1 else 's'
-            print("{name}: {n} key{s}".format(name=name, n=num_keys, s=s))
+            s = "" if num_keys == 1 else "s"
+            print(f"{name}: {num_keys} key{s}")
 
     def do_add_key(self):
         ssh_key = read_ssh_key(self._args.ssh_key_path)
 
         for name, pi in self.get_pis(self._args.names):
             keys_before = len(pi.ssh_keys)
             pi.ssh_keys |= {ssh_key}
             keys_after = len(pi.ssh_keys)
             num_keys = keys_after - keys_before
-            s = '' if num_keys == 1 else ''
-            print("{n} key{s} added to {name}".format(n=num_keys, name=name, s=s))
+            s = "" if num_keys == 1 else ""
+            print(f"{num_keys} key{s} added to {name}")
 
     def do_copy_keys(self):
         src_pi = self.get_pi(self._args.name_src)
         if not src_pi:
             return 2
         ssh_keys = src_pi.ssh_keys
 
         for name, pi in self.get_pis(self._args.names_dest):
             if pi:
                 keys_before = len(pi.ssh_keys)
                 pi.ssh_keys |= ssh_keys
                 keys_after = len(pi.ssh_keys)
                 num_keys = keys_after - keys_before
-                s = '' if num_keys == 1 else 's'
-                print("{n} key{s} added to {name}".format(n=num_keys, name=name, s=s))
+                s = "" if num_keys == 1 else "s"
+                print(f"{num_keys} key{s} added to {name}")
 
     def do_remove_keys(self):
         for name, pi in self.get_pis(self._args.names):
             if pi:
                 num_keys = len(pi.ssh_keys)
                 pi.ssh_keys = set()
-                s = '' if num_keys == 1 else 's'
-                print("{n} key{s} removed from {name}".format(n=num_keys, name=name, s=s))
+                s = "" if num_keys == 1 else "s"
+                print(f"{num_keys} key{s} removed from {name}")
             else:
                 self.print_not_found(name)
 
     def do_ssh_import_id(self):
         github = self._args.gh
         launchpad = self._args.lp
         github_keys = set()
         launchpad_keys = set()
 
         if github:
             github_keys |= ssh_import_id(github=github)
-            s = '' if len(github_keys) == 1 else 's'
-            print("{n} key{s} retrieved from GitHub".format(n=len(github_keys), s=s))
+            s = "" if len(github_keys) == 1 else "s"
+            print(f"{len(github_keys)} key{s} retrieved from GitHub")
         if launchpad:
             launchpad_keys |= ssh_import_id(launchpad=launchpad)
-            s = '' if len(launchpad_keys) == 1 else 's'
-            print("{n} key{s} retrieved from Launchpad".format(n=len(launchpad_keys), s=s))
+            s = "" if len(launchpad_keys) == 1 else "s"
+            print(f"{len(launchpad_keys)} key{s} retrieved from Launchpad")
 
         print()
         new_keys = github_keys | launchpad_keys
         if len(new_keys) < (len(github_keys) + len(launchpad_keys)):
-            s = '' if len(new_keys) == 1 else 's'
-            print("{n} key{s} to add".format(n=len(new_keys), s=s))
+            s = "" if len(new_keys) == 1 else "s"
+            print(f"{len(new_keys)} key{s} to add")
 
         if new_keys:
             for name, pi in self.get_pis(self._args.names):
                 if pi:
                     keys_before = len(pi.ssh_keys)
                     pi.ssh_keys |= new_keys
                     keys_after = len(pi.ssh_keys)
                     num_keys = keys_after - keys_before
-                    s = '' if num_keys == 1 else 's'
-                    print("{n} key{s} added to {name}".format(n=num_keys, name=name, s=s))
+                    s = "" if num_keys == 1 else "s"
+                    print(f"{num_keys} key{s} added to {name}")
                 else:
                     self.print_not_found(name)
         else:
             print("No keys to add")
 
     def do_ssh_command(self):
         for name, pi in self.get_pis(self._args.names):
@@ -539,20 +623,21 @@
                     print(pi.ipv4_ssh_config)
             else:
                 self.print_not_found(name)
 
     def do_provision_status(self):
         for name, pi in self.get_pis(self._args.names):
             if pi:
-                print("{pi.name}: {pi.provision_status}".format(pi=pi))
+                print(f"{pi.name}: {pi.provision_status}")
             else:
                 self.print_not_found(name)
 
     def do_power_status(self):
         for name, pi in self.get_pis(self._args.names):
             if pi:
                 on_off = "on" if pi.power else "off"
-                print("{name}: powered {on_off}".format(name=name, on_off=on_off))
+                print(f"{name}: powered {on_off}")
             else:
                 self.print_not_found(name)
 
+
 main = CLI()
```

### Comparing `hostedpi-0.2.0/hostedpi/picloud.py` & `hostedpi-0.3.0/hostedpi/picloud.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import string
+from typing import Optional, Union, Dict, List, Set
 
-import requests
-from requests.exceptions import HTTPError
+from requests import Session, HTTPError
 
 from .auth import MythicAuth
 from .pi import Pi
 from .utils import parse_ssh_keys
 from .exc import HostedPiException
 
 
@@ -48,86 +48,111 @@
     .. note::
         If any SSH keys are provided on class initialisation, they will be used
         when creating Pis but are overriden by any passed to the
         :meth:`~hostedpi.picloud.PiCloud.create_pi` method.
 
         All SSH arguments provided will be used in combination.
     """
-    _API_URL = 'https://api.mythic-beasts.com/beta/pi'
 
-    def __init__(self, api_id=None, api_secret=None, *, ssh_keys=None,
-                 ssh_key_path=None, ssh_import_github=None,
-                 ssh_import_launchpad=None):
+    _API_URL = "https://api.mythic-beasts.com/beta/pi"
+
+    def __init__(
+        self,
+        api_id: Optional[str] = None,
+        api_secret: Optional[str] = None,
+        *,
+        ssh_keys: Optional[Union[List[str], Set[str]]] = None,
+        ssh_key_path: Optional[str] = None,
+        ssh_import_github: Optional[Union[List[str], Set[str]]] = None,
+        ssh_import_launchpad: Optional[Union[List[str], Set[str]]] = None,
+    ):
         if api_id is None:
-            api_id = os.environ.get('HOSTEDPI_ID')
+            api_id = os.environ.get("HOSTEDPI_ID")
 
         if api_secret is None:
-            api_secret = os.environ.get('HOSTEDPI_SECRET')
+            api_secret = os.environ.get("HOSTEDPI_SECRET")
 
         if api_id is None or api_secret is None:
             raise HostedPiException(
                 "Environment variables HOSTEDPI_ID and HOSTEDPI_SECRET must be "
                 "set or api_id and api_secret passed as arguments"
             )
 
-        self.ssh_keys = parse_ssh_keys(ssh_keys, ssh_key_path,
-                                       ssh_import_github, ssh_import_launchpad)
+        self.ssh_keys = parse_ssh_keys(
+            ssh_keys, ssh_key_path, ssh_import_github, ssh_import_launchpad
+        )
 
         self._auth = MythicAuth(api_id, api_secret)
 
     def __repr__(self):
         return "<PiCloud>"
 
     def __str__(self):
-        "String of information about all the Pis in the account"
-        print(*self.pis, sep='\n\n')
+        """
+        String of information about all the Pis in the account
+        """
+        print(*self.pis, sep="\n\n")
 
     @property
-    def headers(self):
-        return self._auth.headers
+    def session(self) -> Session:
+        return self._auth.session
 
     @property
-    def pis(self):
-        "A dictionary of :class:`~hostedpi.pi.Pi` objects keyed by their names."
-        url = '{self._API_URL}/servers'.format(self=self)
-        r = requests.get(url, headers=self.headers)
+    def pis(self) -> Dict[str, Pi]:
+        """
+        A dictionary of :class:`~hostedpi.pi.Pi` objects keyed by their names
+        """
+        # https://www.mythic-beasts.com/support/api/raspberry-pi#ep-get-piservers
+        url = f"{self._API_URL}/servers"
+        r = self.session.get(url)
 
         try:
             r.raise_for_status()
         except HTTPError as e:
+            if r.status_code == 403:
+                raise HostedPiException("Not authorised") from e
             raise HostedPiException(e) from e
 
-        pis = r.json()['servers']
+        pis = r.json()["servers"]
 
         return {
-            name: Pi(cloud=self, name=name, model=data['model'])
+            name: Pi(cloud=self, name=name, model=data["model"])
             for name, data in sorted(pis.items())
         }
 
     @property
-    def ipv4_ssh_config(self):
+    def ipv4_ssh_config(self) -> str:
         """
         A string containing the IPv4 SSH config for all Pis within the account.
         The contents could be added to an SSH config file for easy access to the
         Pis in the account.
         """
-        return '\n'.join(pi.ipv4_ssh_config for pi in self.pis.values())
+        return "\n".join(pi.ipv4_ssh_config for pi in self.pis.values())
 
     @property
-    def ipv6_ssh_config(self):
+    def ipv6_ssh_config(self) -> str:
         """
         A string containing the IPv6 SSH config for all Pis within the account.
         The contents could be added to an SSH config file for easy access to the
         Pis in the account.
         """
-        return '\n'.join(pi.ipv6_ssh_config for pi in self.pis.values())
+        return "\n".join(pi.ipv6_ssh_config for pi in self.pis.values())
 
-    def create_pi(self, name, *, model=3, disk_size=10,
-                  os_image=None, ssh_keys=None, ssh_key_path=None,
-                  ssh_import_github=None, ssh_import_launchpad=None):
+    def create_pi(
+        self,
+        name: str,
+        *,
+        model: int = 3,
+        disk_size: int = 10,
+        os_image: Optional[str] = None,
+        ssh_keys: Optional[Union[List[str], Set[str]]] = None,
+        ssh_key_path: Optional[str] = None,
+        ssh_import_github: Optional[Union[List[str], Set[str]]] = None,
+        ssh_import_launchpad: Optional[Union[List[str], Set[str]]] = None,
+    ) -> Pi:
         """
         Provision a new cloud Pi with the specified name, model, disk size and
         SSH keys. Return a new :class:`~hostedpi.pi.Pi` instance.
 
         :type name: str
         :param name:
             A unique identifier for the server. This will form part of the
@@ -176,83 +201,89 @@
             used here but are overriden by any passed to this method.
 
         .. note::
             When requesting a Pi 3, you will either get a model 3B or 3B+. It is
             not possible to request a particular model beyond 3 or 4. The Pi 4
             is the 4GB RAM model.
         """
-        ssh_keys_set = parse_ssh_keys(ssh_keys, ssh_key_path, ssh_import_github,
-                                      ssh_import_launchpad)
+        # https://www.mythic-beasts.com/support/api/raspberry-pi#ep-post-piserversidentifier
+        ssh_keys_set = parse_ssh_keys(
+            ssh_keys, ssh_key_path, ssh_import_github, ssh_import_launchpad
+        )
         ssh_keys_str = "\r\n".join(ssh_keys_set)
 
         server_name = name.lower()
-        model = str(model)
         self._validate_server_name(server_name)
         self._validate_model(model)
         self._validate_disk_size(disk_size)
 
-        url = "{self._API_URL}/servers/{name}".format(self=self, name=name)
+        url = f"{self._API_URL}/servers/{name}"
         data = {
-            'disk': disk_size,
-            'model': model,
-            'os_image': os_image,
+            "disk": disk_size,
+            "model": model,
+            "os_image": os_image,
         }
 
         if ssh_keys:
-            data['ssh_key'] = ssh_keys_str
+            data["ssh_key"] = ssh_keys_str
 
-        r = requests.post(url, headers=self.headers, json=data)
+        r = self.session.post(url, json=data)
 
         try:
             r.raise_for_status()
         except HTTPError as e:
+            if r.status_code == 400:
+                error = r.json().get("error", "")
+                raise HostedPiException(f"Invalid parameters: {error}") from e
             if r.status_code == 403:
                 raise HostedPiException("Not authorised to provision server") from e
             if r.status_code == 409:
                 raise HostedPiException("Server name already exists") from e
             if r.status_code == 503:
-                raise HostedPiException(
-                    "Out of stock of Pi Model {model}".format(model=model)) from e
+                raise HostedPiException(f"Out of stock of Pi Model {model}") from e
             raise HostedPiException(e) from e
 
         return Pi(cloud=self, name=name, model=model)
 
     def _validate_server_name(self, server_name):
-        valid_chars = string.ascii_lowercase + string.digits + '-_'
+        valid_chars = string.ascii_lowercase + string.digits + "-_"
         if not all(c in valid_chars for c in server_name):
             raise HostedPiException(
-                "Server name must consist of alphanumeric characters and "
-                "hyphens")
+                "Server name must consist of alphanumeric characters and " "hyphens"
+            )
 
-    def _validate_model(self, model):
-        if model not in ('3', '4'):
+    def _validate_model(self, model: int):
+        if model not in {3, 4}:
             raise HostedPiException("Model must be 3 or 4")
 
-    def _validate_disk_size(self, disk_size):
+    def _validate_disk_size(self, disk_size: int):
         if disk_size < 10 or disk_size % 10 > 0:
             raise HostedPiException("Disk size must be a multiple of 10")
 
-    def get_operating_systems(self, *, model):
+    def get_operating_systems(self, *, model: int) -> Dict[str, str]:
         """
         Return a dict of operating systems supported by the given Pi *model* (3
-        or 4). Dict keys are identifiers (e.g. "raspbian-buster") which can be
+        or 4). Dict keys are identifiers (e.g. "rpi-buster-armhf") which can be
         used when provisioning a new Pi with
         :meth:`~hostedpi.picloud.PiCloud.create_pi`; dict values are text labels
-        of the OS/distro names (e.g. "Raspbian Buster").
+        of the OS/distro names (e.g. "Raspberry Pi OS Bullseye (32 bit)").
 
         :type model: int
         :param model:
             The Raspberry Pi model (3 or 4) to get operating systems for
             (keyword-only argument)
         """
-        model = str(model)
-        if model not in ('3', '4'):
+        # https://www.mythic-beasts.com/support/api/raspberry-pi#ep-get-piimagesmodel
+        if model not in {3, 4}:
             raise HostedPiException("model must be 3 or 4")
-        url = "{self._API_URL}/images/{model}".format(self=self, model=model)
-        r = requests.get(url, headers=self.headers)
+        url = f"{self._API_URL}/images/{model}"
+        r = self.session.get(url)
 
         try:
             r.raise_for_status()
         except HTTPError as e:
+            if r.status_code == 400:
+                error = r.json()["error"]
+                raise HostedPiException(error) from e
             raise HostedPiException(e) from e
 
         return r.json()
```

### Comparing `hostedpi-0.2.0/hostedpi/utils.py` & `hostedpi-0.3.0/hostedpi/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,76 @@
+from typing import Optional, Union, Set
+from pathlib import Path
+
 import requests
 from requests.exceptions import HTTPError
 
 from .exc import HostedPiException
 
 
-def ssh_import_id(*, github=None, launchpad=None):
-    "Returns a set of SSH keys imported from GitHub or Launchpad"
+def ssh_import_id(
+    *, github: Optional[str] = None, launchpad: Optional[str] = None
+) -> Set[str]:
+    """
+    Returns a set of SSH keys imported from GitHub or Launchpad
+    """
     if github is None and launchpad is None:
         raise HostedPiException("GitHub or Launchpad username must be provided")
 
     keys = set()
     if github is not None:
-        url = 'https://github.com/{}.keys'.format(github)
-        sep = '\n'
+        url = f"https://github.com/{github}.keys"
+        sep = "\n"
         keys |= fetch_keys(url, sep)
     if launchpad is not None:
-        url = 'https://launchpad.net/~{}/+sshkeys'.format(launchpad)
-        sep = '\r\n\n'
+        url = f"https://launchpad.net/~{launchpad}/+sshkeys"
+        sep = "\r\n\n"
         keys |= fetch_keys(url, sep)
 
     return keys
 
 
-def fetch_keys(url, sep):
-    "Retrieve keys from *url* and return a set of keys"
+def fetch_keys(url: str, sep: str) -> Set[str]:
+    """
+    Retrieve keys from *url* and return a set of keys
+    """
     r = requests.get(url)
 
     try:
         r.raise_for_status()
     except HTTPError as e:
         raise HostedPiException(e) from e
 
     return set(r.text.strip().split(sep))
 
 
-def read_ssh_key(ssh_key_path):
-    "Read the SSH key from the given path and return the file contents"
-    with open(ssh_key_path) as f:
-        return f.read()
-
-
-def parse_ssh_keys(ssh_keys=None, ssh_key_path=None, ssh_import_github=None,
-                   ssh_import_launchpad=None):
-    "Parse SSH keys from any of various sources"
-    if type(ssh_import_github) == str:
+def read_ssh_key(ssh_key_path: Path) -> str:
+    """
+    Read the SSH key from the given path and return the file contents
+    """
+    return ssh_key_path.read_text()
+
+
+def parse_ssh_keys(
+    ssh_keys: Optional[Set[str]] = None,
+    ssh_key_path: Optional[Path] = None,
+    ssh_import_github: Optional[Union[Set[str], str]] = None,
+    ssh_import_launchpad: Optional[Union[Set[str], str]] = None,
+) -> Set[str]:
+    """
+    Parse SSH keys from any of various sources
+    """
+    if type(ssh_import_github) is str:
         ssh_import_github = {ssh_import_github}
-    if type(ssh_import_launchpad) == str:
+    if type(ssh_import_launchpad) is str:
         ssh_import_launchpad = {ssh_import_launchpad}
 
     ssh_keys_set = set()
     if ssh_keys:
-        ssh_keys_set |= set(ssh_keys)
+        ssh_keys_set |= ssh_keys
     if ssh_key_path:
         ssh_keys_set |= {read_ssh_key(ssh_key_path)}
     if ssh_import_github:
         for username in ssh_import_github:
             ssh_keys_set |= ssh_import_id(github=username)
     if ssh_import_launchpad:
         for username in ssh_import_launchpad:
```

### Comparing `hostedpi-0.2.0/hostedpi.egg-info/PKG-INFO` & `hostedpi-0.3.0/hostedpi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,115 @@
 Metadata-Version: 2.1
 Name: hostedpi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python interface to the Mythic Beasts Hosted Pi API
 Home-page: https://hostedpi.readthedocs.io/
 Author: The piwheels team
 Author-email: ben@bennuttall.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://hostedpi.readthedocs.io/
 Project-URL: Source Code, https://github.com/piwheels/hostedpi
 Project-URL: Issue Tracker, https://github.com/piwheels/hostedpi/issues
-Description: ========
-        hostedpi
-        ========
-        
-        .. image:: https://badge.fury.io/py/hostedpi.svg
-            :target: https://badge.fury.io/py/hostedpi
-            :alt: Latest Version
-        
-        Python interface to the `Mythic Beasts Hosted Pi`_ API, developed by the
-        `piwheels`_ team (`Ben Nuttall`_ and `Dave Jones`_).
-        
-        .. _Mythic Beasts Hosted Pi: https://www.mythic-beasts.com/order/rpi
-        .. _piwheels: https://www.piwheels.org/
-        .. _Ben Nuttall: https://twitter.com/ben_nuttall
-        .. _Dave Jones: https://twitter.com/waveform80
-        
-        This module provides a Pythonic interface to the API, as well as a command line
-        interface.
-        
-        The authors of this library are not affiliated with Mythic Beasts, but we use
-        their Pi cloud to power the piwheels project.
-        
-        Documentation of the API itself can be found at
-        https://www.mythic-beasts.com/support/api/raspberry-pi
-        
-        Usage
-        =====
-        
-        View the information about a Pi from the command line:
-        
-        .. code-block:: console
-        
-            $ hostedpi show mypi
-            Name: mypi
-            Provision status: live
-            Model: Raspberry Pi 3B
-            Disk size: 10GB
-            Power: on
-            IPv6 address: 2a00:1098:8:5b::1
-            IPv6 network: 2a00:1098:8:5b00::/56
-            Initialised keys: yes
-            SSH keys: 4
-            IPv4 SSH port: 5091
-            Location: MER
-            URLs:
-              http://www.mypi.hostedpi.com
-              https://www.mypi.hostedpi.com
-            SSH commands:
-              ssh -p 5091 root@ssh.mypi.hostedpi.com  #IPv4
-              ssh root@[2a00:1098:8:5b::1]  #IPv6
-        
-        Provision a new Pi and view its SSH command (using Python):
-        
-        .. code-block:: pycon
-        
-            >>> from hostedpi import PiCloud
-            >>> api_id = '8t29hvcux5g9vud8'
-            >>> secret = 'QNwsvxZY8SxT3OiLt:Vmz-D1mWQuoZ'
-            >>> cloud = PiCloud(api_id, secret, ssh_key_path='/home/ben/.ssh/id_rsa.pub')
-            >>> pi = cloud.create_pi('mypi')
-            >>> print(pi.ssh_command)
-            ssh -p 5123 root@ssh.mypi.hostedpi.com
-        
-        See the `getting started`_ page for information on how to authenticate, and
-        see the `command line interface`_ page for information on using the command line
-        interface.
-        
-        .. _getting started: https://hostedpi.readthedocs.io/en/latest/getting_started.html
-        .. _command line interface: https://hostedpi.readthedocs.io/en/latest/cli.html
-        
-        Documentation
-        =============
-        
-        Documentation for this module can be found at https://hostedpi.readthedocs.io/
-        
-        Documentation of the API itself can be found at
-        https://www.mythic-beasts.com/support/api/raspberry-pi
-        
-        Contributing
-        ============
-        
-        * Source code can be found on GitHub at https://github.com/piwheels/hostedpi
-        * Code and documentation contributions welcome
-        * The issue tracker can be found at https://github.com/piwheels/hostedpi/issues
-        * For issues with the API itself, please contact Mythic Beasts support
-          https://www.mythic-beasts.com/support
-        
 Keywords: raspberrypi,mythicbeasts,picloud,piwheels
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.5
-Provides-Extra: test
+Requires-Python: >=3.7
 Provides-Extra: doc
+License-File: LICENSE.txt
+
+========
+hostedpi
+========
+
+.. image:: https://badge.fury.io/py/hostedpi.svg
+    :target: https://badge.fury.io/py/hostedpi
+    :alt: Latest Version
+
+Python interface to the `Mythic Beasts Hosted Pi`_ API, developed by the
+`piwheels`_ team (`Ben Nuttall`_ and `Dave Jones`_).
+
+.. _Mythic Beasts Hosted Pi: https://www.mythic-beasts.com/order/rpi
+.. _piwheels: https://www.piwheels.org/
+.. _Ben Nuttall: https://twitter.com/ben_nuttall
+.. _Dave Jones: https://twitter.com/waveform80
+
+This module provides a Pythonic interface to the API, as well as a command line
+interface.
+
+The authors of this library are not affiliated with Mythic Beasts, but we use
+their Pi cloud to power the piwheels project.
+
+Documentation of the API itself can be found at
+https://www.mythic-beasts.com/support/api/raspberry-pi
+
+Usage
+=====
+
+View the information about a Pi from the command line:
+
+.. code-block:: console
+
+    $ hostedpi show mypi
+    Name: mypi
+    Provision status: live
+    Model: Raspberry Pi 3B
+    Disk size: 10GB
+    Power: on
+    IPv6 address: 2a00:1098:8:5b::1
+    IPv6 network: 2a00:1098:8:5b00::/56
+    Initialised keys: yes
+    SSH keys: 4
+    IPv4 SSH port: 5091
+    Location: MER
+    URLs:
+      http://www.mypi.hostedpi.com
+      https://www.mypi.hostedpi.com
+    SSH commands:
+      ssh -p 5091 root@ssh.mypi.hostedpi.com  #IPv4
+      ssh root@[2a00:1098:8:5b::1]  #IPv6
+
+Provision a new Pi and view its SSH command (using Python):
+
+.. code-block:: pycon
+
+    >>> from hostedpi import PiCloud
+    >>> api_id = '8t29hvcux5g9vud8'
+    >>> secret = 'QNwsvxZY8SxT3OiLt:Vmz-D1mWQuoZ'
+    >>> cloud = PiCloud(api_id, secret, ssh_key_path='/home/ben/.ssh/id_rsa.pub')
+    >>> pi = cloud.create_pi('mypi')
+    >>> print(pi.ssh_command)
+    ssh -p 5123 root@ssh.mypi.hostedpi.com
+
+See the `getting started`_ page for information on how to authenticate, and
+see the `command line interface`_ page for information on using the command line
+interface.
+
+.. _getting started: https://hostedpi.readthedocs.io/en/latest/getting_started.html
+.. _command line interface: https://hostedpi.readthedocs.io/en/latest/cli.html
+
+Documentation
+=============
+
+Documentation for this module can be found at https://hostedpi.readthedocs.io/
+
+Documentation of the API itself can be found at
+https://www.mythic-beasts.com/support/api/raspberry-pi
+
+Contributing
+============
+
+* Source code can be found on GitHub at https://github.com/piwheels/hostedpi
+* Code and documentation contributions welcome
+* The issue tracker can be found at https://github.com/piwheels/hostedpi/issues
+* For issues with the API itself, please contact Mythic Beasts support
+  https://www.mythic-beasts.com/support
```

### Comparing `hostedpi-0.2.0/setup.cfg` & `hostedpi-0.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -14,37 +14,32 @@
 license = BSD 3-Clause License
 classifiers = 
 	Development Status :: 4 - Beta
 	Operating System :: POSIX
 	Operating System :: Unix
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.5
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Intended Audience :: Developers
 	Topic :: Utilities
 	License :: OSI Approved :: BSD License
 license_files = LICENSE.txt
 
 [options]
 packages = find:
-python_requires = >=3.5
+python_requires = >=3.7
 install_requires = 
 	setuptools
 	requests
 
 [options.extras_require]
-test = 
-	pytest
-	coverage
-	mock
-	pylint
 doc = 
 	sphinx
 	sphinx-rtd-theme
 
 [options.entry_points]
 console_scripts = 
 	hostedpi = hostedpi.cli:main
```

