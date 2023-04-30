# Comparing `tmp/voxx-cli-1.0.2.tar.gz` & `tmp/voxx-cli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxx-cli-1.0.2.tar", last modified: Sun Apr 30 01:37:51 2023, max compression
+gzip compressed data, was "voxx-cli-1.0.3.tar", last modified: Sun Apr 30 08:11:18 2023, max compression
```

## Comparing `voxx-cli-1.0.2.tar` & `voxx-cli-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 01:37:51.240804 voxx-cli-1.0.2/
--rw-rw-rw-   0        0        0     1049 2023-04-30 01:37:51.240301 voxx-cli-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-04-29 08:26:49.000000 voxx-cli-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 01:37:51.240804 voxx-cli-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-04-30 01:32:11.000000 voxx-cli-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:37:51.215182 voxx-cli-1.0.2/voxx/
--rw-rw-rw-   0        0        0        0 2023-04-29 05:40:38.000000 voxx-cli-1.0.2/voxx/__init__.py
--rw-rw-rw-   0        0        0     1495 2023-04-29 23:38:15.000000 voxx-cli-1.0.2/voxx/__main__.py
--rw-rw-rw-   0        0        0     3718 2023-04-29 05:54:49.000000 voxx-cli-1.0.2/voxx/connection.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:37:51.219188 voxx-cli-1.0.2/voxx/css/
--rw-rw-rw-   0        0        0      900 2023-04-28 23:07:53.000000 voxx-cli-1.0.2/voxx/css/tui.css
--rw-rw-rw-   0        0        0     2333 2023-04-30 00:51:11.000000 voxx-cli-1.0.2/voxx/model.py
--rw-rw-rw-   0        0        0     5188 2023-04-30 00:51:11.000000 voxx-cli-1.0.2/voxx/tui.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:37:51.239299 voxx-cli-1.0.2/voxx_cli.egg-info/
--rw-rw-rw-   0        0        0     1049 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       29 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-30 01:37:51.000000 voxx-cli-1.0.2/voxx_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 08:11:18.107745 voxx-cli-1.0.3/
+-rw-rw-rw-   0        0        0     2693 2023-04-30 08:11:18.107245 voxx-cli-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2023-04-30 08:10:08.000000 voxx-cli-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 08:11:18.108003 voxx-cli-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-04-30 04:35:11.000000 voxx-cli-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:11:18.096919 voxx-cli-1.0.3/voxx/
+-rw-rw-rw-   0        0        0      140 2023-04-30 07:53:09.000000 voxx-cli-1.0.3/voxx/__init__.py
+-rw-rw-rw-   0        0        0     3330 2023-04-30 08:05:30.000000 voxx-cli-1.0.3/voxx/__main__.py
+-rw-rw-rw-   0        0        0     3718 2023-04-29 05:54:49.000000 voxx-cli-1.0.3/voxx/connection.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:11:18.098226 voxx-cli-1.0.3/voxx/css/
+-rw-rw-rw-   0        0        0      900 2023-04-28 23:07:53.000000 voxx-cli-1.0.3/voxx/css/tui.css
+-rw-rw-rw-   0        0        0     2333 2023-04-30 00:51:11.000000 voxx-cli-1.0.3/voxx/model.py
+-rw-rw-rw-   0        0        0     5188 2023-04-30 00:51:11.000000 voxx-cli-1.0.3/voxx/tui.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:11:18.105738 voxx-cli-1.0.3/voxx_cli.egg-info/
+-rw-rw-rw-   0        0        0     2693 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       29 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-30 08:11:18.000000 voxx-cli-1.0.3/voxx_cli.egg-info/top_level.txt
```

### Comparing `voxx-cli-1.0.2/setup.py` & `voxx-cli-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from setuptools import setup, find_packages
 from io import open
 from os import path
-
+from voxx import __app_name__, __description__, __author__, __voxx_version__
 import pathlib
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 with open(path.join(HERE, 'requirements.txt'), encoding='utf-8') as f:
     all_reqs = f.read().split('\n')
 
 install_requires = [x.strip() for x in all_reqs if
                     ('git+' not in x) and (not x.startswith('#')) and (not x.startswith('-'))]
 dependency_links = [x.strip().replace('git+', '') for x in all_reqs if 'git+' not in x]
 
 setup(
-    name='voxx-cli',
-    description='A command line interface client for Voxx',
-    version='1.0.2',
+    name=__app_name__,
+    description=__description__,
+    version=__voxx_version__,
     packages=find_packages(),  # list of all packages
     install_requires=install_requires,
     python_requires='>=3.7',  # any python greater than 2.7
     package_data={'voxx': ['css/*.css']},
-    entry_points='''
+    entry_points=f'''
         [console_scripts]
-        voxx-cli=voxx.__main__:main
+        {__app_name__}=voxx.__main__:main
     ''',
-    author="CyR1en",
+    author=__author__,
     keyword="voxx",
     long_description=README,
     long_description_content_type="text/markdown",
     license='MIT',
     url='https://github.com/CyR1en/voxx-client-cli',
     download_url='https://github.com/CyR1en/voxx-client-cli',
     dependency_links=dependency_links,
```

### Comparing `voxx-cli-1.0.2/voxx/__main__.py` & `voxx-cli-1.0.3/voxx/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,92 @@
 import argparse
 import re
 import sys
 
+from rich import box
+from rich.box import Box
+from rich.console import Group
+from rich.panel import Panel
+from rich.table import Table
+from rich.text import Text
+
 from voxx.connection import console, close
 from voxx.connection import establish_voxx_connection
 from voxx.tui import start_tui
+from voxx import __voxx_version__, __app_name__, __description__
 
 UNAME_RE = r'^[A-Za-z][A-Za-z0-9_]{3,6}$'
 ADDR_RE = r'(.*):(\d+)'
 
+EMPTY: Box = Box(
+    """\
+    
+    
+    
+    
+    
+    
+    
+    
+"""
+)
+
 
 class VoxxParser(argparse.ArgumentParser):
     def _print_message(self, message, file=None):
         console.print(message)
 
-
-parser = VoxxParser(prog='voxx-cli', description='Voxx command line interface client')
-parser.add_argument('-addr', type=str, help='Voxx server address', default='localhost:8008')
-parser.add_argument('-user', type=str, help='Username to register as', required=True)
+    def format_help(self):
+        out: str
+        table = Table(box=EMPTY,
+                      show_header=False,
+                      show_lines=False,
+                      pad_edge=False)
+
+        table.add_column(min_width=1)
+        table.add_column(min_width=25)
+        table.add_column(min_width=10)
+
+        for action in self._actions:
+            metavar = action.metavar if action.metavar else ''
+            table.add_row(f'[aquamarine1]{action.option_strings[0]}[/aquamarine1]',
+                          f'[cyan3]{action.option_strings[1]}[/cyan3] [gold3]{metavar}[/gold3]',
+                          f'[bright_black]{action.help}[/bright_black]')
+
+        group = Group(
+            Text.assemble('Voxx CLI ', (f'v{__voxx_version__}', 'bold magenta'), justify='center', end='\n\n'),
+            Text.assemble((f'{__description__}', 'bright_black'), justify='center', end='\n\n'),
+            Text.assemble(f' Usage: {__app_name__} [options] ', (f'<arg>', 'bold gold3'), justify='left', end='\n\n'),
+            Panel.fit(table, title='options', title_align='left', border_style='bright_black')
+        )
+        return Panel.fit(group, box=EMPTY)
+
+
+parser = VoxxParser(prog='voxx-cli', description=__description__)
+parser.add_argument('-a', '--address', metavar='ADDRESS', type=str, help='voxx server address',
+                    default='localhost:8008')
+parser.add_argument('-u', '--user', metavar='USERNAME', type=str, help='username to register as', required=True)
+parser.add_argument('-v', '--version', action='version',
+                    version=f'[bold magenta]{__app_name__}[/bold magenta] version {__voxx_version__}')
 
 
 def main():
     args = parser.parse_args()
-    if not re.match(ADDR_RE, args.addr):
+    addr = args.a if hasattr(args, 'a') else args.address
+    user = args.u if hasattr(args, 'u') else args.user
+    if not re.match(ADDR_RE, addr):
         console.print(f'[warning]Invalid address: [bold red]{args.addr}[/bold red][/warning]')
         console.print(f'[italic]Address must be in the form of [bold green]host:port[/bold green][/italic]')
         sys.exit(1)
-    if not re.match(UNAME_RE, args.user):
+    if not re.match(UNAME_RE, user):
         console.print(f'[warning]Invalid username: [bold red]{args.user}[/bold red][/warning]')
         console.print(f'[italic]Username must be 4-7 characters long and start with a letter[/italic]')
         sys.exit(1)
     with console.status("[bold green]Connecting to server...") as status:
-        addr = tuple(args.addr.split(':'))
+        addr = tuple(addr.split(':'))
         establish_voxx_connection(args.user, (addr[0], int(addr[1])))
     start_tui()
     close()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `voxx-cli-1.0.2/voxx/connection.py` & `voxx-cli-1.0.3/voxx/connection.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.2/voxx/css/tui.css` & `voxx-cli-1.0.3/voxx/css/tui.css`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.2/voxx/model.py` & `voxx-cli-1.0.3/voxx/model.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.2/voxx/tui.py` & `voxx-cli-1.0.3/voxx/tui.py`

 * *Files identical despite different names*

