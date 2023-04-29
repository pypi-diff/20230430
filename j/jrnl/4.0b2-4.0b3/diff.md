# Comparing `tmp/jrnl-4.0b2.tar.gz` & `tmp/jrnl-4.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jrnl-4.0b2.tar", max compression
+gzip compressed data, was "jrnl-4.0b3.tar", max compression
```

## Comparing `jrnl-4.0b2.tar` & `jrnl-4.0b3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    34916 2023-04-22 20:46:21.805482 jrnl-4.0b2/LICENSE.md
--rw-r--r--   0        0        0     3117 2023-04-22 20:46:21.805482 jrnl-4.0b2/README.md
--rw-r--r--   0        0        0      213 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/__init__.py
--rw-r--r--   0        0        0      183 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/__main__.py
--rw-r--r--   0        0        0       27 2023-04-22 20:46:35.453758 jrnl-4.0b2/jrnl/__version__.py
--rw-r--r--   0        0        0    13777 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/args.py
--rw-r--r--   0        0        0     3227 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/color.py
--rw-r--r--   0        0        0     4942 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/commands.py
--rw-r--r--   0        0        0     8445 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/config.py
--rw-r--r--   0        0        0    16420 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/controller.py
--rw-r--r--   0        0        0     2031 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/editor.py
--rw-r--r--   0        0        0     1480 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/encryption/BaseEncryption.py
--rw-r--r--   0        0        0      192 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/encryption/BaseKeyEncryption.py
--rw-r--r--   0        0        0     2447 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/encryption/BasePasswordEncryption.py
--rw-r--r--   0        0        0     1657 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/encryption/Jrnlv1Encryption.py
--rw-r--r--   0        0        0     1850 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/encryption/Jrnlv2Encryption.py
--rw-r--r--   0        0        0      571 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/encryption/NoEncryption.py
--rw-r--r--   0        0        0      954 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/encryption/__init__.py
--rw-r--r--   0        0        0      635 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/exception.py
--rw-r--r--   0        0        0     5856 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/install.py
--rw-r--r--   0        0        0     8969 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/journals/DayOneJournal.py
--rw-r--r--   0        0        0     8050 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/journals/Entry.py
--rw-r--r--   0        0        0     4405 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/journals/FolderJournal.py
--rw-r--r--   0        0        0    18385 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/journals/Journal.py
--rw-r--r--   0        0        0      156 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/journals/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/keyring.py
--rw-r--r--   0        0        0     2263 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/main.py
--rw-r--r--   0        0        0      409 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/messages/Message.py
--rw-r--r--   0        0        0     2259 2023-04-22 20:46:21.809482 jrnl-4.0b2/jrnl/messages/MsgStyle.py
--rw-r--r--   0        0        0     9438 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/messages/MsgText.py
--rw-r--r--   0        0        0      282 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/messages/__init__.py
--rw-r--r--   0        0        0      415 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/os_compat.py
--rw-r--r--   0        0        0     3429 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/output.py
--rw-r--r--   0        0        0     2463 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/override.py
--rw-r--r--   0        0        0      350 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/path.py
--rw-r--r--   0        0        0     1545 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/__init__.py
--rw-r--r--   0        0        0     1033 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/dates_exporter.py
--rw-r--r--   0        0        0     3997 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/fancy_exporter.py
--rw-r--r--   0        0        0     1549 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/jrnl_importer.py
--rw-r--r--   0        0        0     2566 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/json_exporter.py
--rw-r--r--   0        0        0     3309 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/markdown_exporter.py
--rw-r--r--   0        0        0     1272 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/tag_exporter.py
--rw-r--r--   0        0        0     3844 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/text_exporter.py
--rw-r--r--   0        0        0     1107 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/util.py
--rw-r--r--   0        0        0     2605 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/xml_exporter.py
--rw-r--r--   0        0        0     5230 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/plugins/yaml_exporter.py
--rw-r--r--   0        0        0     2086 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/prompt.py
--rw-r--r--   0        0        0      220 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/templates/sample.template
--rw-r--r--   0        0        0     3118 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/time.py
--rw-r--r--   0        0        0     6164 2023-04-22 20:46:21.813482 jrnl-4.0b2/jrnl/upgrade.py
--rw-r--r--   0        0        0     4096 2023-04-22 20:46:35.401756 jrnl-4.0b2/pyproject.toml
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 jrnl-4.0b2/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-04-29 22:50:50.970518 jrnl-4.0b3/LICENSE.md
+-rw-r--r--   0        0        0     3122 2023-04-29 22:50:50.970518 jrnl-4.0b3/README.md
+-rw-r--r--   0        0        0      213 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/__init__.py
+-rw-r--r--   0        0        0      183 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/__main__.py
+-rw-r--r--   0        0        0       27 2023-04-29 22:51:01.426529 jrnl-4.0b3/jrnl/__version__.py
+-rw-r--r--   0        0        0    13777 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/args.py
+-rw-r--r--   0        0        0     3227 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/color.py
+-rw-r--r--   0        0        0     4942 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/commands.py
+-rw-r--r--   0        0        0     8445 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/config.py
+-rw-r--r--   0        0        0    16420 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/controller.py
+-rw-r--r--   0        0        0     2031 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/editor.py
+-rw-r--r--   0        0        0     1480 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/encryption/BaseEncryption.py
+-rw-r--r--   0        0        0      192 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/encryption/BaseKeyEncryption.py
+-rw-r--r--   0        0        0     2447 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/encryption/BasePasswordEncryption.py
+-rw-r--r--   0        0        0     1657 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/encryption/Jrnlv1Encryption.py
+-rw-r--r--   0        0        0     1850 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/encryption/Jrnlv2Encryption.py
+-rw-r--r--   0        0        0      571 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/encryption/NoEncryption.py
+-rw-r--r--   0        0        0      954 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/encryption/__init__.py
+-rw-r--r--   0        0        0      635 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/exception.py
+-rw-r--r--   0        0        0     5856 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/install.py
+-rw-r--r--   0        0        0     8969 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/journals/DayOneJournal.py
+-rw-r--r--   0        0        0     8050 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/journals/Entry.py
+-rw-r--r--   0        0        0     5711 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/journals/FolderJournal.py
+-rw-r--r--   0        0        0    18385 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/journals/Journal.py
+-rw-r--r--   0        0        0      156 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/journals/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/keyring.py
+-rw-r--r--   0        0        0     2263 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/main.py
+-rw-r--r--   0        0        0      409 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/messages/Message.py
+-rw-r--r--   0        0        0     2259 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/messages/MsgStyle.py
+-rw-r--r--   0        0        0     9438 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/messages/MsgText.py
+-rw-r--r--   0        0        0      282 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/messages/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/os_compat.py
+-rw-r--r--   0        0        0     3429 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/output.py
+-rw-r--r--   0        0        0     2463 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/override.py
+-rw-r--r--   0        0        0      350 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/path.py
+-rw-r--r--   0        0        0     1545 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/__init__.py
+-rw-r--r--   0        0        0     1033 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/dates_exporter.py
+-rw-r--r--   0        0        0     3997 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/fancy_exporter.py
+-rw-r--r--   0        0        0     1549 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/jrnl_importer.py
+-rw-r--r--   0        0        0     2566 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/json_exporter.py
+-rw-r--r--   0        0        0     3309 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/markdown_exporter.py
+-rw-r--r--   0        0        0     1272 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/tag_exporter.py
+-rw-r--r--   0        0        0     3844 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/text_exporter.py
+-rw-r--r--   0        0        0     1107 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/util.py
+-rw-r--r--   0        0        0     2605 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/xml_exporter.py
+-rw-r--r--   0        0        0     5230 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/plugins/yaml_exporter.py
+-rw-r--r--   0        0        0     2086 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/prompt.py
+-rw-r--r--   0        0        0      220 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/templates/sample.template
+-rw-r--r--   0        0        0     3297 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/time.py
+-rw-r--r--   0        0        0     6164 2023-04-29 22:50:50.974518 jrnl-4.0b3/jrnl/upgrade.py
+-rw-r--r--   0        0        0     4096 2023-04-29 22:51:01.386528 jrnl-4.0b3/pyproject.toml
+-rw-r--r--   0        0        0     4465 1970-01-01 00:00:00.000000 jrnl-4.0b3/PKG-INFO
```

### Comparing `jrnl-4.0b2/LICENSE.md` & `jrnl-4.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/README.md` & `jrnl-4.0b3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 `jrnl` couldn't exist without each and every one of you!
 
 <a href="https://github.com/jrnl-org/jrnl/graphs/contributors"><img
 src="https://opencollective.com/jrnl/contributors.svg?width=890&button=false"
 /></a>
 
 If you'd also like to help make `jrnl` better, please see our [contributing
-documentation](CONTRIBUTING.md).
+documentation](docs/contributing.md).
 
 ### Financial Backers
 
 Another way show support is through direct financial contributions. These funds
 go to covering our costs, and are a quick way to show your appreciation for
 `jrnl`.
```

#### html2text {}

```diff
@@ -26,12 +26,12 @@
 maintainers help keep the lights on for the project: * Jonathan Wren ([wren]
 (https://github.com/wren)) * Micah Ellison ([micahellison](https://github.com/
 micahellison)) Please thank them if you like `jrnl`! ### Code Contributors This
 project is made with love by the many fabulous people who have contributed.
 `jrnl` couldn't exist without each and every one of you! [https://
 opencollective.com/jrnl/contributors.svg?width=890&button=false] If you'd also
 like to help make `jrnl` better, please see our [contributing documentation]
-(CONTRIBUTING.md). ### Financial Backers Another way show support is through
-direct financial contributions. These funds go to covering our costs, and are a
-quick way to show your appreciation for `jrnl`. [Become a financial
+(docs/contributing.md). ### Financial Backers Another way show support is
+through direct financial contributions. These funds go to covering our costs,
+and are a quick way to show your appreciation for `jrnl`. [Become a financial
 contributor](https://opencollective.com/jrnl/contribute) and help us sustain
 our community. [https://opencollective.com/jrnl/individuals.svg?width=890]
```

### Comparing `jrnl-4.0b2/jrnl/args.py` & `jrnl-4.0b3/jrnl/args.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/color.py` & `jrnl-4.0b3/jrnl/color.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/commands.py` & `jrnl-4.0b3/jrnl/commands.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/config.py` & `jrnl-4.0b3/jrnl/config.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/controller.py` & `jrnl-4.0b3/jrnl/controller.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/editor.py` & `jrnl-4.0b3/jrnl/editor.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/encryption/BaseEncryption.py` & `jrnl-4.0b3/jrnl/encryption/BaseEncryption.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/encryption/BasePasswordEncryption.py` & `jrnl-4.0b3/jrnl/encryption/BasePasswordEncryption.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/encryption/Jrnlv1Encryption.py` & `jrnl-4.0b3/jrnl/encryption/Jrnlv1Encryption.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/encryption/Jrnlv2Encryption.py` & `jrnl-4.0b3/jrnl/encryption/Jrnlv2Encryption.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/encryption/NoEncryption.py` & `jrnl-4.0b3/jrnl/encryption/NoEncryption.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/encryption/__init__.py` & `jrnl-4.0b3/jrnl/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/exception.py` & `jrnl-4.0b3/jrnl/exception.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/install.py` & `jrnl-4.0b3/jrnl/install.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/journals/DayOneJournal.py` & `jrnl-4.0b3/jrnl/journals/DayOneJournal.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/journals/Entry.py` & `jrnl-4.0b3/jrnl/journals/Entry.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/journals/FolderJournal.py` & `jrnl-4.0b3/jrnl/journals/FolderJournal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # Copyright © 2012-2023 jrnl contributors
 # License: https://www.gnu.org/licenses/gpl-3.0.html
 
 import codecs
-import fnmatch
 import os
+import pathlib
 from typing import TYPE_CHECKING
 
 from jrnl import time
 
 from .Journal import Journal
 
 if TYPE_CHECKING:
     from jrnl.journals import Entry
 
-
-def get_files(journal_config: str) -> list[str]:
-    """Searches through sub directories starting with journal_config and find all text files"""
-    filenames = []
-    for root, dirnames, f in os.walk(journal_config):
-        for filename in fnmatch.filter(f, "*.txt"):
-            filenames.append(os.path.join(root, filename))
-    return filenames
+# glob search patterns for folder/file structure
+DIGIT_PATTERN = "[0123456789]"
+YEAR_PATTERN = DIGIT_PATTERN * 4
+MONTH_PATTERN = "[01]" + DIGIT_PATTERN
+DAY_PATTERN = "[0123]" + DIGIT_PATTERN + ".txt"
 
 
 class Folder(Journal):
     """A Journal handling multiple files in a folder"""
 
     def __init__(self, name: str = "default", **kwargs):
         self.entries = []
         self._diff_entry_dates = []
         self.can_be_encrypted = False
         super().__init__(name, **kwargs)
 
     def open(self) -> "Folder":
         filenames = []
         self.entries = []
-        filenames = get_files(self.config["journal"])
-        for filename in filenames:
-            with codecs.open(filename, "r", "utf-8") as f:
-                journal = f.read()
-                self.entries.extend(self._parse(journal))
-        self.sort()
+
+        if os.path.exists(self.config["journal"]):
+            filenames = Folder._get_files(self.config["journal"])
+            for filename in filenames:
+                with codecs.open(filename, "r", "utf-8") as f:
+                    journal = f.read()
+                    self.entries.extend(self._parse(journal))
+            self.sort()
+
         return self
 
     def write(self) -> None:
         """Writes only the entries that have been modified into proper files."""
         # Create a list of dates of modified entries. Start with diff_entry_dates
         modified_dates = self._diff_entry_dates
         seen_dates = set(self._diff_entry_dates)
@@ -77,15 +77,15 @@
                 ):
                     write_entries.append(e)
             journal = "\n".join([e.__str__() for e in write_entries])
             with codecs.open(filename, "w", "utf-8") as journal_file:
                 journal_file.write(journal)
         # look for and delete empty files
         filenames = []
-        filenames = get_files(self.config["journal"])
+        filenames = Folder._get_files(self.config["journal"])
         for filename in filenames:
             if os.stat(filename).st_size <= 0:
                 os.remove(filename)
 
     def delete_entries(self, entries_to_delete: list["Entry"]) -> None:
         """Deletes specific entries from a journal."""
         for entry in entries_to_delete:
@@ -115,7 +115,43 @@
         # these to modified, so we can get a count of how many entries got
         # modified and how many got deleted later.
         for entry in mod_entries:
             entry.modified = not any(entry == old_entry for old_entry in self.entries)
 
         self.increment_change_counts_by_edit(mod_entries)
         self.entries = mod_entries
+
+    @staticmethod
+    def _get_files(journal_path: str) -> list[str]:
+        """Searches through sub directories starting with journal_path and find all text files that look like entries"""
+        for year_folder in Folder._get_year_folders(pathlib.Path(journal_path)):
+            for month_folder in Folder._get_month_folders(year_folder):
+                yield from Folder._get_day_files(month_folder)
+
+    @staticmethod
+    def _get_year_folders(path: pathlib.Path) -> list[pathlib.Path]:
+        for child in path.glob(YEAR_PATTERN):
+            if child.is_dir():
+                yield child
+        return
+
+    @staticmethod
+    def _get_month_folders(path: pathlib.Path) -> list[pathlib.Path]:
+        for child in path.glob(MONTH_PATTERN):
+            if int(child.name) > 0 and int(child.name) <= 12 and path.is_dir():
+                yield child
+        return
+
+    @staticmethod
+    def _get_day_files(path: pathlib.Path) -> list[str]:
+        for child in path.glob(DAY_PATTERN):
+            if (
+                int(child.stem) > 0
+                and int(child.stem) <= 31
+                and time.is_valid_date(
+                    year=int(path.parent.name),
+                    month=int(path.name),
+                    day=int(child.stem),
+                )
+                and child.is_file()
+            ):
+                yield str(child)
```

### Comparing `jrnl-4.0b2/jrnl/journals/Journal.py` & `jrnl-4.0b3/jrnl/journals/Journal.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/keyring.py` & `jrnl-4.0b3/jrnl/keyring.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/main.py` & `jrnl-4.0b3/jrnl/main.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/messages/MsgStyle.py` & `jrnl-4.0b3/jrnl/messages/MsgStyle.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/messages/MsgText.py` & `jrnl-4.0b3/jrnl/messages/MsgText.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/output.py` & `jrnl-4.0b3/jrnl/output.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/override.py` & `jrnl-4.0b3/jrnl/override.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/__init__.py` & `jrnl-4.0b3/jrnl/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/dates_exporter.py` & `jrnl-4.0b3/jrnl/plugins/dates_exporter.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/fancy_exporter.py` & `jrnl-4.0b3/jrnl/plugins/fancy_exporter.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/jrnl_importer.py` & `jrnl-4.0b3/jrnl/plugins/jrnl_importer.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/json_exporter.py` & `jrnl-4.0b3/jrnl/plugins/json_exporter.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/markdown_exporter.py` & `jrnl-4.0b3/jrnl/plugins/markdown_exporter.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/tag_exporter.py` & `jrnl-4.0b3/jrnl/plugins/tag_exporter.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/text_exporter.py` & `jrnl-4.0b3/jrnl/plugins/text_exporter.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/util.py` & `jrnl-4.0b3/jrnl/plugins/util.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/xml_exporter.py` & `jrnl-4.0b3/jrnl/plugins/xml_exporter.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/plugins/yaml_exporter.py` & `jrnl-4.0b3/jrnl/plugins/yaml_exporter.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/prompt.py` & `jrnl-4.0b3/jrnl/prompt.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/jrnl/time.py` & `jrnl-4.0b3/jrnl/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,7 +85,15 @@
     # Ugly heuristic: if the date is more than 4 weeks in the future, we got the year wrong.
     # Rather than this, we would like to see parsedatetime patched so we can tell it to prefer
     # past dates
     dt = datetime.datetime.now() - date
     if dt.days < -28 and not year_present:
         date = date.replace(date.year - 1)
     return date
+
+
+def is_valid_date(year: int, month: int, day: int) -> bool:
+    try:
+        datetime.datetime(year, month, day)
+        return True
+    except ValueError:
+        return False
```

### Comparing `jrnl-4.0b2/jrnl/upgrade.py` & `jrnl-4.0b3/jrnl/upgrade.py`

 * *Files identical despite different names*

### Comparing `jrnl-4.0b2/pyproject.toml` & `jrnl-4.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jrnl"
-version = "v4.0-beta2"
+version = "v4.0-beta3"
 description = "Collect your thoughts and notes without leaving the command line."
 authors = [
     "jrnl contributors <maintainers@jrnl.sh>",
     "Manuel Ebert <manuel@1450.me>",
     "Jonathan Wren <jonathan@nowandwren.com>",
     "Micah Ellison <micahellison@gmail.com>"
 ]
```

### Comparing `jrnl-4.0b2/PKG-INFO` & `jrnl-4.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jrnl
-Version: 4.0b2
+Version: 4.0b3
 Summary: Collect your thoughts and notes without leaving the command line.
 Home-page: https://jrnl.sh
 License: GPL-3.0-only
 Author: jrnl contributors
 Author-email: maintainers@jrnl.sh
 Maintainer: Jonathan Wren and Micah Ellison
 Maintainer-email: maintainers@jrnl.sh
@@ -100,15 +100,15 @@
 `jrnl` couldn't exist without each and every one of you!
 
 <a href="https://github.com/jrnl-org/jrnl/graphs/contributors"><img
 src="https://opencollective.com/jrnl/contributors.svg?width=890&button=false"
 /></a>
 
 If you'd also like to help make `jrnl` better, please see our [contributing
-documentation](CONTRIBUTING.md).
+documentation](docs/contributing.md).
 
 ### Financial Backers
 
 Another way show support is through direct financial contributions. These funds
 go to covering our costs, and are a quick way to show your appreciation for
 `jrnl`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jrnl Version: 4.0b2 Summary: Collect your thoughts
+Metadata-Version: 2.1 Name: jrnl Version: 4.0b3 Summary: Collect your thoughts
 and notes without leaving the command line. Home-page: https://jrnl.sh License:
 GPL-3.0-only Author: jrnl contributors Author-email: maintainers@jrnl.sh
 Maintainer: Jonathan Wren and Micah Ellison Maintainer-email:
 maintainers@jrnl.sh Requires-Python: >=3.10.0,<3.13 Classifier: Environment ::
 Console Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
@@ -44,12 +44,12 @@
 maintainers help keep the lights on for the project: * Jonathan Wren ([wren]
 (https://github.com/wren)) * Micah Ellison ([micahellison](https://github.com/
 micahellison)) Please thank them if you like `jrnl`! ### Code Contributors This
 project is made with love by the many fabulous people who have contributed.
 `jrnl` couldn't exist without each and every one of you! [https://
 opencollective.com/jrnl/contributors.svg?width=890&button=false] If you'd also
 like to help make `jrnl` better, please see our [contributing documentation]
-(CONTRIBUTING.md). ### Financial Backers Another way show support is through
-direct financial contributions. These funds go to covering our costs, and are a
-quick way to show your appreciation for `jrnl`. [Become a financial
+(docs/contributing.md). ### Financial Backers Another way show support is
+through direct financial contributions. These funds go to covering our costs,
+and are a quick way to show your appreciation for `jrnl`. [Become a financial
 contributor](https://opencollective.com/jrnl/contribute) and help us sustain
 our community. [https://opencollective.com/jrnl/individuals.svg?width=890]
```

