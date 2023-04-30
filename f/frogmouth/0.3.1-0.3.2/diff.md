# Comparing `tmp/frogmouth-0.3.1.tar.gz` & `tmp/frogmouth-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogmouth-0.3.1.tar", max compression
+gzip compressed data, was "frogmouth-0.3.2.tar", max compression
```

## Comparing `frogmouth-0.3.1.tar` & `frogmouth-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.3.1/LICENSE
--rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.3.1/README.md
--rw-r--r--   0        0        0      283 2023-04-27 14:46:52.802054 frogmouth-0.3.1/frogmouth/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.3.1/frogmouth/__main__.py
--rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.3.1/frogmouth/app/__init__.py
--rw-r--r--   0        0        0     2149 2023-04-30 07:26:36.701179 frogmouth-0.3.1/frogmouth/app/app.py
--rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.3.1/frogmouth/data/__init__.py
--rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.3.1/frogmouth/data/bookmarks.py
--rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.3.1/frogmouth/data/config.py
--rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.3.1/frogmouth/data/data_directory.py
--rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.3.1/frogmouth/data/history.py
--rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.3.1/frogmouth/dialogs/__init__.py
--rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.3.1/frogmouth/dialogs/error.py
--rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.3.1/frogmouth/dialogs/help_dialog.py
--rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.3.1/frogmouth/dialogs/information.py
--rw-r--r--   0        0        0     4278 2023-04-27 14:46:52.803185 frogmouth-0.3.1/frogmouth/dialogs/input_dialog.py
--rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.3.1/frogmouth/dialogs/text_dialog.py
--rw-r--r--   0        0        0     4898 2023-04-27 14:46:52.803359 frogmouth-0.3.1/frogmouth/dialogs/yes_no_dialog.py
--rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.3.1/frogmouth/screens/__init__.py
--rw-r--r--   0        0        0    19015 2023-04-29 20:35:07.285373 frogmouth-0.3.1/frogmouth/screens/main.py
--rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.3.1/frogmouth/utility/__init__.py
--rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.3.1/frogmouth/utility/advertising.py
--rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.3.1/frogmouth/utility/forge.py
--rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.3.1/frogmouth/utility/type_tests.py
--rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.3.1/frogmouth/widgets/__init__.py
--rw-r--r--   0        0        0     4398 2023-04-29 14:55:46.079307 frogmouth-0.3.1/frogmouth/widgets/navigation.py
--rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.3.1/frogmouth/widgets/navigation_panes/__init__.py
--rw-r--r--   0        0        0     5889 2023-04-29 14:55:46.079533 frogmouth-0.3.1/frogmouth/widgets/navigation_panes/bookmarks.py
--rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.3.1/frogmouth/widgets/navigation_panes/history.py
--rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.3.1/frogmouth/widgets/navigation_panes/local_files.py
--rw-r--r--   0        0        0      667 2023-04-29 14:55:46.080110 frogmouth-0.3.1/frogmouth/widgets/navigation_panes/navigation_pane.py
--rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.3.1/frogmouth/widgets/navigation_panes/table_of_contents.py
--rw-r--r--   0        0        0    11675 2023-04-28 17:16:37.437633 frogmouth-0.3.1/frogmouth/widgets/omnibox.py
--rw-r--r--   0        0        0     9806 2023-04-27 15:34:09.464460 frogmouth-0.3.1/frogmouth/widgets/viewer.py
--rw-r--r--   0        0        0     1468 2023-04-30 07:26:48.343032 frogmouth-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 frogmouth-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.3.2/README.md
+-rw-r--r--   0        0        0      283 2023-04-30 11:12:52.375078 frogmouth-0.3.2/frogmouth/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.3.2/frogmouth/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.3.2/frogmouth/app/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.3.2/frogmouth/app/app.py
+-rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.3.2/frogmouth/data/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.3.2/frogmouth/data/bookmarks.py
+-rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.3.2/frogmouth/data/config.py
+-rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.3.2/frogmouth/data/data_directory.py
+-rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.3.2/frogmouth/data/history.py
+-rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.3.2/frogmouth/dialogs/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.3.2/frogmouth/dialogs/error.py
+-rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.3.2/frogmouth/dialogs/help_dialog.py
+-rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.3.2/frogmouth/dialogs/information.py
+-rw-r--r--   0        0        0     4278 2023-04-27 14:46:52.803185 frogmouth-0.3.2/frogmouth/dialogs/input_dialog.py
+-rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.3.2/frogmouth/dialogs/text_dialog.py
+-rw-r--r--   0        0        0     4898 2023-04-27 14:46:52.803359 frogmouth-0.3.2/frogmouth/dialogs/yes_no_dialog.py
+-rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.3.2/frogmouth/screens/__init__.py
+-rw-r--r--   0        0        0    18984 2023-04-30 11:10:42.376816 frogmouth-0.3.2/frogmouth/screens/main.py
+-rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.3.2/frogmouth/utility/__init__.py
+-rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.3.2/frogmouth/utility/advertising.py
+-rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.3.2/frogmouth/utility/forge.py
+-rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.3.2/frogmouth/utility/type_tests.py
+-rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.3.2/frogmouth/widgets/__init__.py
+-rw-r--r--   0        0        0     4398 2023-04-29 14:55:46.079307 frogmouth-0.3.2/frogmouth/widgets/navigation.py
+-rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/__init__.py
+-rw-r--r--   0        0        0     5889 2023-04-29 14:55:46.079533 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/bookmarks.py
+-rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/history.py
+-rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/local_files.py
+-rw-r--r--   0        0        0      667 2023-04-29 14:55:46.080110 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/navigation_pane.py
+-rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.3.2/frogmouth/widgets/navigation_panes/table_of_contents.py
+-rw-r--r--   0        0        0    11675 2023-04-28 17:16:37.437633 frogmouth-0.3.2/frogmouth/widgets/omnibox.py
+-rw-r--r--   0        0        0     9806 2023-04-27 15:34:09.464460 frogmouth-0.3.2/frogmouth/widgets/viewer.py
+-rw-r--r--   0        0        0     1468 2023-04-30 11:13:02.337061 frogmouth-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 frogmouth-0.3.2/PKG-INFO
```

### Comparing `frogmouth-0.3.1/LICENSE` & `frogmouth-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/README.md` & `frogmouth-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/app/app.py` & `frogmouth-0.3.2/frogmouth/app/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 class MarkdownViewer(App[None]):
     """The main application class."""
 
     TITLE = APPLICATION_TITLE
     """The main title for the application."""
 
-    SUB_TITLE = f"{__version__}"
-    """The sub-title for the application."""
-
     def __init__(self, cli_args: Namespace) -> None:
         """Initialise the application.
 
         Args:
             cli_args: The command line arguments.
         """
         super().__init__()
```

### Comparing `frogmouth-0.3.1/frogmouth/data/bookmarks.py` & `frogmouth-0.3.2/frogmouth/data/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/data/config.py` & `frogmouth-0.3.2/frogmouth/data/config.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/data/data_directory.py` & `frogmouth-0.3.2/frogmouth/data/data_directory.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/data/history.py` & `frogmouth-0.3.2/frogmouth/data/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/dialogs/error.py` & `frogmouth-0.3.2/frogmouth/dialogs/error.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/dialogs/help_dialog.py` & `frogmouth-0.3.2/frogmouth/dialogs/help_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/dialogs/input_dialog.py` & `frogmouth-0.3.2/frogmouth/dialogs/input_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/dialogs/text_dialog.py` & `frogmouth-0.3.2/frogmouth/dialogs/text_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/dialogs/yes_no_dialog.py` & `frogmouth-0.3.2/frogmouth/dialogs/yes_no_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/screens/main.py` & `frogmouth-0.3.2/frogmouth/screens/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from httpx import URL
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Horizontal
 from textual.events import Paste
 from textual.screen import Screen
-from textual.widgets import Footer, Header, Markdown
+from textual.widgets import Footer, Markdown
 
 from .. import __version__
 from ..data import load_config, load_history, save_config, save_history
 from ..dialogs import ErrorDialog, HelpDialog, InformationDialog, InputDialog
 from ..utility import (
     build_raw_bitbucket_url,
     build_raw_github_url,
@@ -115,15 +115,14 @@
 
     def compose(self) -> ComposeResult:
         """Compose the main screen.
 
         Returns:
             The result of composing the screen.
         """
-        yield Header()
         yield Omnibox(classes="focusable")
         with Horizontal():
             yield Navigation()
             yield Viewer(classes="focusable")
         yield Footer()
 
     def visit(self, location: Path | URL, remember: bool = True) -> None:
```

### Comparing `frogmouth-0.3.1/frogmouth/utility/advertising.py` & `frogmouth-0.3.2/frogmouth/utility/advertising.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/utility/forge.py` & `frogmouth-0.3.2/frogmouth/utility/forge.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/utility/type_tests.py` & `frogmouth-0.3.2/frogmouth/utility/type_tests.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/widgets/navigation.py` & `frogmouth-0.3.2/frogmouth/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/widgets/navigation_panes/bookmarks.py` & `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/widgets/navigation_panes/history.py` & `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/widgets/navigation_panes/local_files.py` & `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/local_files.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/widgets/navigation_panes/navigation_pane.py` & `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/navigation_pane.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/widgets/navigation_panes/table_of_contents.py` & `frogmouth-0.3.2/frogmouth/widgets/navigation_panes/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/widgets/omnibox.py` & `frogmouth-0.3.2/frogmouth/widgets/omnibox.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/frogmouth/widgets/viewer.py` & `frogmouth-0.3.2/frogmouth/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.3.1/pyproject.toml` & `frogmouth-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "frogmouth"
 homepage = "https://github.com/Textualize/frogmouth"
-version = "0.3.1"
+version = "0.3.2"
 description = "A Markdown document viewer for the terminal"
 authors = ["Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "frogmouth"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `frogmouth-0.3.1/PKG-INFO` & `frogmouth-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogmouth
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Markdown document viewer for the terminal
 Home-page: https://github.com/Textualize/frogmouth
 License: MIT
 Author: Dave Pearson
 Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frogmouth Version: 0.3.1 Summary: A Markdown
+Metadata-Version: 2.1 Name: frogmouth Version: 0.3.2 Summary: A Markdown
 document viewer for the terminal Home-page: https://github.com/Textualize/
 frogmouth License: MIT Author: Dave Pearson Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: License :: OSI Approved :: MIT License Classifier:
```

