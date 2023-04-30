# Comparing `tmp/voxx-cli-1.0.1.tar.gz` & `tmp/voxx-cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxx-cli-1.0.1.tar", last modified: Sat Apr 29 09:55:27 2023, max compression
+gzip compressed data, was "voxx-cli-1.0.2.tar", last modified: Sun Apr 30 01:37:51 2023, max compression
```

## Comparing `voxx-cli-1.0.1.tar` & `voxx-cli-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cyr1en     (501) staff       (20)        0 2023-04-29 09:55:27.971742 voxx-cli-1.0.1/
--rw-r--r--   0 cyr1en     (501) staff       (20)     1004 2023-04-29 09:55:27.971467 voxx-cli-1.0.1/PKG-INFO
--rw-r--r--   0 cyr1en     (501) staff       (20)      558 2023-04-29 09:47:17.000000 voxx-cli-1.0.1/README.md
--rw-r--r--   0 cyr1en     (501) staff       (20)       38 2023-04-29 09:55:27.971856 voxx-cli-1.0.1/setup.cfg
--rw-r--r--   0 cyr1en     (501) staff       (20)     1387 2023-04-29 09:53:42.000000 voxx-cli-1.0.1/setup.py
-drwxr-xr-x   0 cyr1en     (501) staff       (20)        0 2023-04-29 09:55:27.966013 voxx-cli-1.0.1/voxx/
--rw-r--r--   0 cyr1en     (501) staff       (20)        0 2023-04-29 09:47:17.000000 voxx-cli-1.0.1/voxx/__init__.py
--rw-r--r--   0 cyr1en     (501) staff       (20)     1454 2023-04-29 09:47:17.000000 voxx-cli-1.0.1/voxx/__main__.py
--rw-r--r--   0 cyr1en     (501) staff       (20)     3589 2023-04-29 09:47:17.000000 voxx-cli-1.0.1/voxx/connection.py
-drwxr-xr-x   0 cyr1en     (501) staff       (20)        0 2023-04-29 09:55:27.967314 voxx-cli-1.0.1/voxx/css/
--rw-r--r--   0 cyr1en     (501) staff       (20)      846 2023-04-29 09:47:17.000000 voxx-cli-1.0.1/voxx/css/tui.css
--rw-r--r--   0 cyr1en     (501) staff       (20)     2221 2023-04-29 09:47:17.000000 voxx-cli-1.0.1/voxx/model.py
--rw-r--r--   0 cyr1en     (501) staff       (20)     5018 2023-04-29 09:49:19.000000 voxx-cli-1.0.1/voxx/tui.py
-drwxr-xr-x   0 cyr1en     (501) staff       (20)        0 2023-04-29 09:55:27.971001 voxx-cli-1.0.1/voxx_cli.egg-info/
--rw-r--r--   0 cyr1en     (501) staff       (20)     1004 2023-04-29 09:55:27.000000 voxx-cli-1.0.1/voxx_cli.egg-info/PKG-INFO
--rw-r--r--   0 cyr1en     (501) staff       (20)      308 2023-04-29 09:55:27.000000 voxx-cli-1.0.1/voxx_cli.egg-info/SOURCES.txt
--rw-r--r--   0 cyr1en     (501) staff       (20)       29 2023-04-29 09:55:27.000000 voxx-cli-1.0.1/voxx_cli.egg-info/dependency_links.txt
--rw-r--r--   0 cyr1en     (501) staff       (20)       48 2023-04-29 09:55:27.000000 voxx-cli-1.0.1/voxx_cli.egg-info/entry_points.txt
--rw-r--r--   0 cyr1en     (501) staff       (20)       29 2023-04-29 09:55:27.000000 voxx-cli-1.0.1/voxx_cli.egg-info/requires.txt
--rw-r--r--   0 cyr1en     (501) staff       (20)        5 2023-04-29 09:55:27.000000 voxx-cli-1.0.1/voxx_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 01:37:51.240804 voxx-cli-1.0.2/
+-rw-rw-rw-   0        0        0     1049 2023-04-30 01:37:51.240301 voxx-cli-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-04-29 08:26:49.000000 voxx-cli-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 01:37:51.240804 voxx-cli-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-04-30 01:32:11.000000 voxx-cli-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:37:51.215182 voxx-cli-1.0.2/voxx/
+-rw-rw-rw-   0        0        0        0 2023-04-29 05:40:38.000000 voxx-cli-1.0.2/voxx/__init__.py
+-rw-rw-rw-   0        0        0     1495 2023-04-29 23:38:15.000000 voxx-cli-1.0.2/voxx/__main__.py
+-rw-rw-rw-   0        0        0     3718 2023-04-29 05:54:49.000000 voxx-cli-1.0.2/voxx/connection.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:37:51.219188 voxx-cli-1.0.2/voxx/css/
+-rw-rw-rw-   0        0        0      900 2023-04-28 23:07:53.000000 voxx-cli-1.0.2/voxx/css/tui.css
+-rw-rw-rw-   0        0        0     2333 2023-04-30 00:51:11.000000 voxx-cli-1.0.2/voxx/model.py
+-rw-rw-rw-   0        0        0     5188 2023-04-30 00:51:11.000000 voxx-cli-1.0.2/voxx/tui.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:37:51.239299 voxx-cli-1.0.2/voxx_cli.egg-info/
+-rw-rw-rw-   0        0        0     1049 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       29 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/top_level.txt
```

### Comparing `voxx-cli-1.0.1/PKG-INFO` & `voxx-cli-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: voxx-cli
-Version: 1.0.1
-Summary: A command line interface client for Voxx
-Home-page: https://github.com/CyR1en/voxx-client-cli
-Download-URL: https://github.com/CyR1en/voxx-client-cli
-Author: CyR1en
-Author-email: ethan.bacurio@ucdenver.edu
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# Project Voxx CLI
-
-This is a command line interface client for Voxx.
-
-## Installation
-
-```
-pip install voxx-cli
-```
-
-## Usage
-
-```
-voxx-cli --help
-
-usage: voxx-cli [-h] [-addr ADDR] -user USER
-
-Voxx command line interface client
-
-optional arguments:
-  -h, --help  show this help message and exit
-  -addr ADDR  Voxx server address
-  -user USER  Username to register as
-```
-
-Currently, there is a Voxx server instance running at `repo.cyr1en.com:8008`.
-To connect to this Voxx server, you can run:
-
-```
-voxx-cli -addr repo.cyr1en.com:8008 -user <username>
-```
+Metadata-Version: 2.1
+Name: voxx-cli
+Version: 1.0.2
+Summary: A command line interface client for Voxx
+Home-page: https://github.com/CyR1en/voxx-client-cli
+Download-URL: https://github.com/CyR1en/voxx-client-cli
+Author: CyR1en
+Author-email: ethan.bacurio@ucdenver.edu
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# Project Voxx CLI
+
+This is a command line interface client for Voxx.
+
+## Installation
+
+```
+pip install voxx-cli
+```
+
+## Usage
+
+```
+voxx-cli --help
+
+usage: voxx-cli [-h] [-addr ADDR] -user USER
+
+Voxx command line interface client
+
+optional arguments:
+  -h, --help  show this help message and exit
+  -addr ADDR  Voxx server address
+  -user USER  Username to register as
+```
+
+Currently, there is a Voxx server instance running at `repo.cyr1en.com:8008`.
+To connect to this Voxx server, you can run:
+
+```
+voxx-cli -addr repo.cyr1en.com:8008 -user <username>
+```
```

### Comparing `voxx-cli-1.0.1/setup.py` & `voxx-cli-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from setuptools import setup, find_packages
-from io import open
-from os import path
-
-import pathlib
-
-HERE = pathlib.Path(__file__).parent
-
-README = (HERE / "README.md").read_text()
-
-with open(path.join(HERE, 'requirements.txt'), encoding='utf-8') as f:
-    all_reqs = f.read().split('\n')
-
-install_requires = [x.strip() for x in all_reqs if
-                    ('git+' not in x) and (not x.startswith('#')) and (not x.startswith('-'))]
-dependency_links = [x.strip().replace('git+', '') for x in all_reqs if 'git+' not in x]
-
-setup(
-    name='voxx-cli',
-    description='A command line interface client for Voxx',
-    version='1.0.1',
-    packages=find_packages(),  # list of all packages
-    install_requires=install_requires,
-    python_requires='>=3.7',  # any python greater than 2.7
-    package_data={'voxx': ['css/*.css']},
-    entry_points='''
-        [console_scripts]
-        voxx-cli=voxx.__main__:main
-    ''',
-    author="CyR1en",
-    keyword="voxx",
-    long_description=README,
-    long_description_content_type="text/markdown",
-    license='MIT',
-    url='https://github.com/CyR1en/voxx-client-cli',
-    download_url='https://github.com/CyR1en/voxx-client-cli',
-    dependency_links=dependency_links,
-    author_email='ethan.bacurio@ucdenver.edu',
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
-    ]
-)
+from setuptools import setup, find_packages
+from io import open
+from os import path
+
+import pathlib
+
+HERE = pathlib.Path(__file__).parent
+
+README = (HERE / "README.md").read_text()
+
+with open(path.join(HERE, 'requirements.txt'), encoding='utf-8') as f:
+    all_reqs = f.read().split('\n')
+
+install_requires = [x.strip() for x in all_reqs if
+                    ('git+' not in x) and (not x.startswith('#')) and (not x.startswith('-'))]
+dependency_links = [x.strip().replace('git+', '') for x in all_reqs if 'git+' not in x]
+
+setup(
+    name='voxx-cli',
+    description='A command line interface client for Voxx',
+    version='1.0.2',
+    packages=find_packages(),  # list of all packages
+    install_requires=install_requires,
+    python_requires='>=3.7',  # any python greater than 2.7
+    package_data={'voxx': ['css/*.css']},
+    entry_points='''
+        [console_scripts]
+        voxx-cli=voxx.__main__:main
+    ''',
+    author="CyR1en",
+    keyword="voxx",
+    long_description=README,
+    long_description_content_type="text/markdown",
+    license='MIT',
+    url='https://github.com/CyR1en/voxx-client-cli',
+    download_url='https://github.com/CyR1en/voxx-client-cli',
+    dependency_links=dependency_links,
+    author_email='ethan.bacurio@ucdenver.edu',
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.7",
+    ]
+)
```

### Comparing `voxx-cli-1.0.1/voxx/__main__.py` & `voxx-cli-1.0.2/voxx/__main__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import argparse
-import re
-import sys
-
-from voxx.connection import console, close
-from voxx.connection import establish_voxx_connection
-from voxx.tui import start_tui
-
-UNAME_RE = r'^[A-Za-z][A-Za-z0-9_]{3,6}$'
-ADDR_RE = r'(.*):(\d+)'
-
-
-class VoxxParser(argparse.ArgumentParser):
-    def _print_message(self, message, file=None):
-        console.print(message)
-
-
-parser = VoxxParser(prog='voxx-cli', description='Voxx command line interface client')
-parser.add_argument('-addr', type=str, help='Voxx server address', default='localhost:8008')
-parser.add_argument('-user', type=str, help='Username to register as', required=True)
-
-
-def main():
-    args = parser.parse_args()
-    if not re.match(ADDR_RE, args.addr):
-        console.print(f'[warning]Invalid address: [bold red]{args.addr}[/bold red][/warning]')
-        console.print(f'[italic]Address must be in the form of [bold green]host:port[/bold green][/italic]')
-        sys.exit(1)
-    if not re.match(UNAME_RE, args.user):
-        console.print(f'[warning]Invalid username: [bold red]{args.user}[/bold red][/warning]')
-        console.print(f'[italic]Username must be 4-7 characters long and start with a letter[/italic]')
-        sys.exit(1)
-    with console.status("[bold green]Connecting to server...") as status:
-        addr = tuple(args.addr.split(':'))
-        establish_voxx_connection(args.user, (addr[0], int(addr[1])))
-    start_tui()
-    close()
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import re
+import sys
+
+from voxx.connection import console, close
+from voxx.connection import establish_voxx_connection
+from voxx.tui import start_tui
+
+UNAME_RE = r'^[A-Za-z][A-Za-z0-9_]{3,6}$'
+ADDR_RE = r'(.*):(\d+)'
+
+
+class VoxxParser(argparse.ArgumentParser):
+    def _print_message(self, message, file=None):
+        console.print(message)
+
+
+parser = VoxxParser(prog='voxx-cli', description='Voxx command line interface client')
+parser.add_argument('-addr', type=str, help='Voxx server address', default='localhost:8008')
+parser.add_argument('-user', type=str, help='Username to register as', required=True)
+
+
+def main():
+    args = parser.parse_args()
+    if not re.match(ADDR_RE, args.addr):
+        console.print(f'[warning]Invalid address: [bold red]{args.addr}[/bold red][/warning]')
+        console.print(f'[italic]Address must be in the form of [bold green]host:port[/bold green][/italic]')
+        sys.exit(1)
+    if not re.match(UNAME_RE, args.user):
+        console.print(f'[warning]Invalid username: [bold red]{args.user}[/bold red][/warning]')
+        console.print(f'[italic]Username must be 4-7 characters long and start with a letter[/italic]')
+        sys.exit(1)
+    with console.status("[bold green]Connecting to server...") as status:
+        addr = tuple(args.addr.split(':'))
+        establish_voxx_connection(args.user, (addr[0], int(addr[1])))
+    start_tui()
+    close()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `voxx-cli-1.0.1/voxx/connection.py` & `voxx-cli-1.0.2/voxx/connection.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import asyncio
-import json
-import socket
-import sys
-from threading import Thread
-from types import SimpleNamespace
-
-from rich.console import Console
-from rich.theme import Theme
-
-from voxx.model import User, UID
-
-UM_HANDLERS = dict()
-console = Console(theme=Theme({
-    "info": "dim cyan",
-    "warning": "magenta",
-    "danger": "bold red"
-}))
-
-loop = asyncio.get_event_loop()
-
-
-class ResReqClient(socket.socket):
-    def __int__(self):
-        super().__init__(socket.AF_INET, socket.SOCK_STREAM)
-
-    def request(self, req: json) -> SimpleNamespace:
-        req = f'{json.dumps(req)}\n'
-        self.send(req.encode("utf-8"))
-        data = self.recv(1024).decode("utf-8")
-        return json.loads(data, object_hook=lambda d: SimpleNamespace(**d))
-
-
-class UMClient(ResReqClient, Thread):
-    def __init__(self, main_user: str, addr: tuple) -> None:
-        ResReqClient.__init__(self)
-        Thread.__init__(self)
-        self.connect(addr)
-        req = {"request-id": "su", "params": {"main-user": f'{main_user}'}}
-        self.request(req)
-        self._owning_instance = None
-
-    def set_runner_instance(self, instance):
-        self._owning_instance = instance
-
-    def run(self):
-        try:
-            while (data := self.recv(1024).decode("utf-8")) is not None:
-                msg = json.loads(data, object_hook=lambda d: SimpleNamespace(**d))
-                console.log(msg)
-                key = getattr(msg, 'update-message')
-                if key in UM_HANDLERS:
-                    func = UM_HANDLERS[key]
-                    func(self._owning_instance, msg)
-        except:
-            self.close()
-
-
-res_req_conn: ResReqClient
-um_conn: UMClient
-
-assoc_user: User
-
-
-def um_handler(func):
-    UM_HANDLERS[func.__name__] = func
-    return func
-
-
-def assert_rr(func):
-    def wrapper(*args, **kwargs):
-        if res_req_conn is None:
-            console.print("Response-Request connection not established!", style="bold red")
-            return
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-@assert_rr
-def ping() -> SimpleNamespace:
-    return res_req_conn.request({"request-id": "ping"})
-
-
-@assert_rr
-def register_user(username: str) -> SimpleNamespace:
-    return res_req_conn.request({"request-id": "ru", "params": {"uname": username}})
-
-
-@assert_rr
-def send_message(message='') -> SimpleNamespace:
-    """Send message to server"""
-    if message == '':
-        return SimpleNamespace()
-    return res_req_conn.request({'request-id': 'sm', 'params': {'message': f'{message}'}})
-
-
-@assert_rr
-def get_user_list() -> SimpleNamespace:
-    return res_req_conn.request({'request-id': 'ul'})
-
-
-@assert_rr
-def close() -> None:
-    res_req_conn.close()
-    um_conn.close()
-
-
-def establish_voxx_connection(user: str, addr: tuple):
-    global res_req_conn
-    global um_conn
-    global assoc_user
-    try:
-        res_req_conn = ResReqClient()
-        res_req_conn.connect(addr)
-
-        res = register_user(user)
-        if getattr(res, 'response-id') == 0:
-            console.print(f'Username [bold magenta]{user}[/bold magenta] is already taken!', style='bold red')
-            sys.exit(1)
-        uid_int = int(res.body.user.uid)
-        assoc_user = User(UID.of(uid_int), res.body.user.uname)
-        console.print(f'Connected to Voxx server as [bold magenta]{assoc_user.username}[/bold magenta]!', style='green')
-        um_conn = UMClient(user, addr)
-        um_conn.start()
-
-    except (TimeoutError, InterruptedError, ConnectionRefusedError):
-        console.print(f'Could not connect to Voxx server at {addr}!', style='bold red')
-        sys.exit(1)
+import asyncio
+import json
+import socket
+import sys
+from threading import Thread
+from types import SimpleNamespace
+
+from rich.console import Console
+from rich.theme import Theme
+
+from voxx.model import User, UID
+
+UM_HANDLERS = dict()
+console = Console(theme=Theme({
+    "info": "dim cyan",
+    "warning": "magenta",
+    "danger": "bold red"
+}))
+
+loop = asyncio.get_event_loop()
+
+
+class ResReqClient(socket.socket):
+    def __int__(self):
+        super().__init__(socket.AF_INET, socket.SOCK_STREAM)
+
+    def request(self, req: json) -> SimpleNamespace:
+        req = f'{json.dumps(req)}\n'
+        self.send(req.encode("utf-8"))
+        data = self.recv(1024).decode("utf-8")
+        return json.loads(data, object_hook=lambda d: SimpleNamespace(**d))
+
+
+class UMClient(ResReqClient, Thread):
+    def __init__(self, main_user: str, addr: tuple) -> None:
+        ResReqClient.__init__(self)
+        Thread.__init__(self)
+        self.connect(addr)
+        req = {"request-id": "su", "params": {"main-user": f'{main_user}'}}
+        self.request(req)
+        self._owning_instance = None
+
+    def set_runner_instance(self, instance):
+        self._owning_instance = instance
+
+    def run(self):
+        try:
+            while (data := self.recv(1024).decode("utf-8")) is not None:
+                msg = json.loads(data, object_hook=lambda d: SimpleNamespace(**d))
+                console.log(msg)
+                key = getattr(msg, 'update-message')
+                if key in UM_HANDLERS:
+                    func = UM_HANDLERS[key]
+                    func(self._owning_instance, msg)
+        except:
+            self.close()
+
+
+res_req_conn: ResReqClient
+um_conn: UMClient
+
+assoc_user: User
+
+
+def um_handler(func):
+    UM_HANDLERS[func.__name__] = func
+    return func
+
+
+def assert_rr(func):
+    def wrapper(*args, **kwargs):
+        if res_req_conn is None:
+            console.print("Response-Request connection not established!", style="bold red")
+            return
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+@assert_rr
+def ping() -> SimpleNamespace:
+    return res_req_conn.request({"request-id": "ping"})
+
+
+@assert_rr
+def register_user(username: str) -> SimpleNamespace:
+    return res_req_conn.request({"request-id": "ru", "params": {"uname": username}})
+
+
+@assert_rr
+def send_message(message='') -> SimpleNamespace:
+    """Send message to server"""
+    if message == '':
+        return SimpleNamespace()
+    return res_req_conn.request({'request-id': 'sm', 'params': {'message': f'{message}'}})
+
+
+@assert_rr
+def get_user_list() -> SimpleNamespace:
+    return res_req_conn.request({'request-id': 'ul'})
+
+
+@assert_rr
+def close() -> None:
+    res_req_conn.close()
+    um_conn.close()
+
+
+def establish_voxx_connection(user: str, addr: tuple):
+    global res_req_conn
+    global um_conn
+    global assoc_user
+    try:
+        res_req_conn = ResReqClient()
+        res_req_conn.connect(addr)
+
+        res = register_user(user)
+        if getattr(res, 'response-id') == 0:
+            console.print(f'Username [bold magenta]{user}[/bold magenta] is already taken!', style='bold red')
+            sys.exit(1)
+        uid_int = int(res.body.user.uid)
+        assoc_user = User(UID.of(uid_int), res.body.user.uname)
+        console.print(f'Connected to Voxx server as [bold magenta]{assoc_user.username}[/bold magenta]!', style='green')
+        um_conn = UMClient(user, addr)
+        um_conn.start()
+
+    except (TimeoutError, InterruptedError, ConnectionRefusedError):
+        console.print(f'Could not connect to Voxx server at {addr}!', style='bold red')
+        sys.exit(1)
```

### Comparing `voxx-cli-1.0.1/voxx/tui.py` & `voxx-cli-1.0.2/voxx/tui.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,132 +1,133 @@
-import asyncio
-from datetime import datetime
-from types import SimpleNamespace
-
-import pkg_resources
-from textual.app import App, ComposeResult
-from textual.containers import VerticalScroll, Container
-from textual.widgets import Input, Static
-
-from voxx import connection
-from voxx.connection import um_handler, assert_rr, send_message, get_user_list
-from voxx.model import UID, User
-
-
-class MessageBar(Container):
-    def __init__(self, sender: str, message: str, time: str = None):
-        super().__init__()
-        self.mount(Static(message, classes='message'))
-        self.border_title = sender
-        if time is not None:
-            self.border_subtitle = time
-
-
-class NotificationBar(Container):
-    def __init__(self, message: str, title: str = None, subtitle: str = None):
-        super().__init__()
-        self.mount(Static(message, classes='message'))
-        if title is not None:
-            self.border_title = title
-        if subtitle is not None:
-            self.border_subtitle = subtitle
-
-
-class Voxx(App):
-    CSS_PATH = pkg_resources.resource_filename(__name__, "css/tui.css")
-
-    def __int__(self):
-        super().__init__()
-
-    def compose(self) -> ComposeResult:
-        vert = VerticalScroll(id="results-container")
-        vert.border_title = "Voxx-cli"
-        yield vert
-        yield Input(id="msg-input", placeholder="Enter Message")
-
-    def _on_compose(self) -> None:
-        """A coroutine to handle a text changed message."""
-        asyncio.create_task(self.after_mount())
-        connection.um_conn.set_runner_instance(self)
-
-    async def after_mount(self):
-        msg = "Welcome to Voxx-CLI! This chat is not moderated, please be nice and civil."
-        time = datetime.now().strftime("%m/%d/%y %I:%M %p")
-        await self.add_message(msg, time, 'System')
-
-    @um_handler
-    def nu(self, msg: SimpleNamespace) -> None:
-        """Handles new user update message: called from thread-2"""
-        self.call_from_thread(self._add_notif, f'{msg.body.user.uname} has connected', 'User Connect', None)
-
-    @um_handler
-    def nm(self, msg: SimpleNamespace) -> None:
-        """Handles new message update message: called from thread-2"""
-        sender = User(UID.of(int(msg.body.sender.uid)), msg.body.sender.uname)
-        time = UID.of(int(msg.body.message.uid)).get_timestamp_string()
-        try:
-            self.call_from_thread(self._add_msg, msg.body.message.content, sender.username, time)
-        except Exception as e:
-            send_message(f'Exception: {e}')
-
-    @um_handler
-    def ud(self, msg: SimpleNamespace) -> None:
-        """Handles user disconnect update message: called from thread-2"""
-        self.call_from_thread(self._add_notif, f'{msg.body.user.uname} has disconnected', 'User Disconnect', None)
-
-    async def on_input_submitted(self, message: Input.Submitted) -> None:
-        """A coroutine to handle a text changed message."""
-        if not message.value:
-            return
-
-        if message.value == '/exit':
-            connection.close()
-            self.exit()
-            return
-
-        if message.value == '/ul':
-            asyncio.create_task(self.get_users())
-            self.clear_input()
-            return
-
-        if message.value:
-            response = send_message(message.value)
-            msg = response.body.message.content
-            user = connection.assoc_user.username
-            time = UID.of(int(response.body.message.uid))
-            self.run_worker(self.add_message(msg, sender=user, time=time.get_timestamp_string()))
-        self.clear_input()
-
-    def clear_input(self):
-        self.query_one("#msg-input").action_delete_left_all()
-
-    async def get_users(self):
-        response = get_user_list()
-        names = [user.uname for user in response.body.users]
-        ul = ', '.join(names)
-        asyncio.create_task(self.add_notif(ul, title='Connected users'))
-
-    async def add_notif(self, message: str, title=None, subtitle=None) -> None:
-        bar = NotificationBar(message, title, subtitle)
-        await self.query_one("#results-container").mount(bar)
-        self.call_after_refresh(self.query_one("#results-container").scroll_end, animate=False)
-
-    def _add_notif(self, *args) -> None:
-        """Non-coroutine version of add_notif"""
-        asyncio.create_task(self.add_notif(args[0], title=args[1], subtitle=args[2]))
-
-    async def add_message(self, message: str, time: str = datetime.now().strftime("%m/%d/%y %I:%M %p"),
-                          sender: str = 'System') -> None:
-        """Add message to the result container."""
-        bar = MessageBar(sender, message, time)
-        await self.query_one("#results-container").mount(bar)
-        self.call_after_refresh(self.query_one("#results-container").scroll_end, animate=False)
-
-    def _add_msg(self, *args) -> None:
-        """Non-coroutine version of add_message"""
-        asyncio.create_task(self.add_message(args[0], sender=args[1], time=args[2]))
-
-
-@assert_rr
-def start_tui():
-    app = Voxx()
-    app.run()
+import asyncio
+from datetime import datetime
+from types import SimpleNamespace
+
+import pkg_resources
+from textual.app import App, ComposeResult
+from textual.containers import VerticalScroll, Container
+from textual.widgets import Input, Static
+
+import voxx.model
+from voxx import connection
+from voxx.connection import um_handler, assert_rr, send_message, get_user_list
+from voxx.model import UID, User
+
+
+class MessageBar(Container):
+    def __init__(self, sender: str, message: str, time: str = None):
+        super().__init__()
+        self.mount(Static(message, classes='message'))
+        self.border_title = sender
+        if time is not None:
+            self.border_subtitle = time
+
+
+class NotificationBar(Container):
+    def __init__(self, message: str, title: str = None, subtitle: str = None):
+        super().__init__()
+        self.mount(Static(message, classes='message'))
+        if title is not None:
+            self.border_title = title
+        if subtitle is not None:
+            self.border_subtitle = subtitle
+
+
+class Voxx(App):
+    CSS_PATH = pkg_resources.resource_filename(__name__, "css/tui.css")
+
+    def __int__(self):
+        super().__init__()
+
+    def compose(self) -> ComposeResult:
+        vert = VerticalScroll(id="results-container")
+        vert.border_title = "Voxx-cli"
+        yield vert
+        yield Input(id="msg-input", placeholder="Enter Message")
+
+    def _on_compose(self) -> None:
+        """A coroutine to handle a text changed message."""
+        asyncio.create_task(self.after_mount())
+        connection.um_conn.set_runner_instance(self)
+
+    async def after_mount(self):
+        msg = "Welcome to Voxx-CLI! This chat is not moderated, please be nice and civil."
+        time = datetime.now().astimezone().strftime(voxx.model.TIME_FORMAT)
+        await self.add_message(msg, time, 'System')
+
+    @um_handler
+    def nu(self, msg: SimpleNamespace) -> None:
+        """Handles new user update message: called from thread-2"""
+        self.call_from_thread(self._add_notif, f'{msg.body.user.uname} has connected', 'User Connect', None)
+
+    @um_handler
+    def nm(self, msg: SimpleNamespace) -> None:
+        """Handles new message update message: called from thread-2"""
+        sender = User(UID.of(int(msg.body.sender.uid)), msg.body.sender.uname)
+        time = UID.of(int(msg.body.message.uid)).get_timestamp_string()
+        try:
+            self.call_from_thread(self._add_msg, msg.body.message.content, sender.username, time)
+        except Exception as e:
+            send_message(f'Exception: {e}')
+
+    @um_handler
+    def ud(self, msg: SimpleNamespace) -> None:
+        """Handles user disconnect update message: called from thread-2"""
+        self.call_from_thread(self._add_notif, f'{msg.body.user.uname} has disconnected', 'User Disconnect', None)
+
+    async def on_input_submitted(self, message: Input.Submitted) -> None:
+        """A coroutine to handle a text changed message."""
+        if not message.value:
+            return
+
+        if message.value == '/exit':
+            connection.close()
+            self.exit()
+            return
+
+        if message.value == '/ul':
+            asyncio.create_task(self.get_users())
+            self.clear_input()
+            return
+
+        if message.value:
+            response = send_message(message.value)
+            msg = response.body.message.content
+            user = connection.assoc_user.username
+            time = UID.of(int(response.body.message.uid))
+            self.run_worker(self.add_message(msg, sender=user, time=time.get_timestamp_string()))
+        self.clear_input()
+
+    def clear_input(self):
+        self.query_one("#msg-input").action_delete_left_all()
+
+    async def get_users(self):
+        response = get_user_list()
+        names = [user.uname for user in response.body.users]
+        ul = ', '.join(names)
+        asyncio.create_task(self.add_notif(ul, title='Connected users'))
+
+    async def add_notif(self, message: str, title=None, subtitle=None) -> None:
+        bar = NotificationBar(message, title, subtitle)
+        await self.query_one("#results-container").mount(bar)
+        self.call_after_refresh(self.query_one("#results-container").scroll_end, animate=False)
+
+    def _add_notif(self, *args) -> None:
+        """Non-coroutine version of add_notif"""
+        asyncio.create_task(self.add_notif(args[0], title=args[1], subtitle=args[2]))
+
+    async def add_message(self, message: str, time: str = datetime.now().strftime(voxx.model.TIME_FORMAT),
+                          sender: str = 'System') -> None:
+        """Add message to the result container."""
+        bar = MessageBar(sender, message, time)
+        await self.query_one("#results-container").mount(bar)
+        self.call_after_refresh(self.query_one("#results-container").scroll_end, animate=False)
+
+    def _add_msg(self, *args) -> None:
+        """Non-coroutine version of add_message"""
+        asyncio.create_task(self.add_message(args[0], sender=args[1], time=args[2]))
+
+
+@assert_rr
+def start_tui():
+    app = Voxx()
+    app.run()
```

### Comparing `voxx-cli-1.0.1/voxx_cli.egg-info/PKG-INFO` & `voxx-cli-1.0.2/voxx_cli.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: voxx-cli
-Version: 1.0.1
-Summary: A command line interface client for Voxx
-Home-page: https://github.com/CyR1en/voxx-client-cli
-Download-URL: https://github.com/CyR1en/voxx-client-cli
-Author: CyR1en
-Author-email: ethan.bacurio@ucdenver.edu
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# Project Voxx CLI
-
-This is a command line interface client for Voxx.
-
-## Installation
-
-```
-pip install voxx-cli
-```
-
-## Usage
-
-```
-voxx-cli --help
-
-usage: voxx-cli [-h] [-addr ADDR] -user USER
-
-Voxx command line interface client
-
-optional arguments:
-  -h, --help  show this help message and exit
-  -addr ADDR  Voxx server address
-  -user USER  Username to register as
-```
-
-Currently, there is a Voxx server instance running at `repo.cyr1en.com:8008`.
-To connect to this Voxx server, you can run:
-
-```
-voxx-cli -addr repo.cyr1en.com:8008 -user <username>
-```
+Metadata-Version: 2.1
+Name: voxx-cli
+Version: 1.0.2
+Summary: A command line interface client for Voxx
+Home-page: https://github.com/CyR1en/voxx-client-cli
+Download-URL: https://github.com/CyR1en/voxx-client-cli
+Author: CyR1en
+Author-email: ethan.bacurio@ucdenver.edu
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# Project Voxx CLI
+
+This is a command line interface client for Voxx.
+
+## Installation
+
+```
+pip install voxx-cli
+```
+
+## Usage
+
+```
+voxx-cli --help
+
+usage: voxx-cli [-h] [-addr ADDR] -user USER
+
+Voxx command line interface client
+
+optional arguments:
+  -h, --help  show this help message and exit
+  -addr ADDR  Voxx server address
+  -user USER  Username to register as
+```
+
+Currently, there is a Voxx server instance running at `repo.cyr1en.com:8008`.
+To connect to this Voxx server, you can run:
+
+```
+voxx-cli -addr repo.cyr1en.com:8008 -user <username>
+```
```

