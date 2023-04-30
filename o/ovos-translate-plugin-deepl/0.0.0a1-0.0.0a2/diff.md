# Comparing `tmp/ovos_translate_plugin_deepl-0.0.0a1-py3-none-any.whl.zip` & `tmp/ovos_translate_plugin_deepl-0.0.0a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7835 bytes, number of entries: 8
--rw-r--r--  2.0 unx     5141 b- defN 23-Apr-30 00:35 ovos_translate_plugin_deepl/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-30 00:36 ovos_translate_plugin_deepl/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-30 00:36 ovos_translate_plugin_deepl-0.0.0a1.dist-info/LICENSE
--rw-r--r--  2.0 unx      867 b- defN 23-Apr-30 00:36 ovos_translate_plugin_deepl-0.0.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 00:36 ovos_translate_plugin_deepl-0.0.0a1.dist-info/WHEEL
--rw-r--r--  2.0 unx      189 b- defN 23-Apr-30 00:36 ovos_translate_plugin_deepl-0.0.0a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-30 00:36 ovos_translate_plugin_deepl-0.0.0a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      804 b- defN 23-Apr-30 00:36 ovos_translate_plugin_deepl-0.0.0a1.dist-info/RECORD
-8 files, 18655 bytes uncompressed, 6389 bytes compressed:  65.8%
+Zip file size: 7945 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     5534 b- defN 23-Apr-30 18:46 ovos_translate_plugin_deepl/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-30 18:46 ovos_translate_plugin_deepl/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-30 18:46 ovos_translate_plugin_deepl-0.0.0a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      867 b- defN 23-Apr-30 18:46 ovos_translate_plugin_deepl-0.0.0a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-30 18:46 ovos_translate_plugin_deepl-0.0.0a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      189 b- defN 23-Apr-30 18:46 ovos_translate_plugin_deepl-0.0.0a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-30 18:46 ovos_translate_plugin_deepl-0.0.0a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      804 b- defN 23-Apr-30 18:46 ovos_translate_plugin_deepl-0.0.0a2.dist-info/RECORD
+8 files, 19048 bytes uncompressed, 6499 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_translate_plugin_deepl/__init__.py
 Comment: 
 
 Filename: ovos_translate_plugin_deepl/version.py
 Comment: 
 
-Filename: ovos_translate_plugin_deepl-0.0.0a1.dist-info/LICENSE
+Filename: ovos_translate_plugin_deepl-0.0.0a2.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_translate_plugin_deepl-0.0.0a1.dist-info/METADATA
+Filename: ovos_translate_plugin_deepl-0.0.0a2.dist-info/METADATA
 Comment: 
 
-Filename: ovos_translate_plugin_deepl-0.0.0a1.dist-info/WHEEL
+Filename: ovos_translate_plugin_deepl-0.0.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_translate_plugin_deepl-0.0.0a1.dist-info/entry_points.txt
+Filename: ovos_translate_plugin_deepl-0.0.0a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_translate_plugin_deepl-0.0.0a1.dist-info/top_level.txt
+Filename: ovos_translate_plugin_deepl-0.0.0a2.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_translate_plugin_deepl-0.0.0a1.dist-info/RECORD
+Filename: ovos_translate_plugin_deepl-0.0.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_translate_plugin_deepl/__init__.py

```diff
@@ -1,12 +1,16 @@
-from ovos_plugin_manager.templates.language import LanguageDetector,\
-    LanguageTranslator
-from deepl import Translator
 from typing import Union, List
 
+from deepl import Translator
+from ovos_utils.log import LOG
+from ovos_plugin_manager.templates.language import (
+    LanguageDetector,
+    LanguageTranslator
+)
+
 
 class DeepLTranslator(LanguageTranslator):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.api_key = self.config.get("api_key")
         self.translator = Translator(self.api_key)
         self.boost = False
@@ -75,18 +79,23 @@
         if not text or not target:
             return ""
         
         tx = self.translator.translate_text(text,
                                             source_lang=source,
                                             target_lang=target)
 
+        source = source or ""
         if isinstance(tx, list):
-            return [t.text for t in tx]
+            translations = [t.text.strip() for t in tx]
+            LOG.debug(f"Batch translation ({source}->{target}): {translations}")
+            return translations
         
-        return tx.text.strip()
+        translation = tx.text.strip()
+        LOG.debug(f"Translation ({source}->{target}): {translation}")
+        return translation
     
     @property
     def available_languages(self) -> set:
         """
         The available target languages with the service
 
         Returns:
@@ -147,15 +156,18 @@
             text (str): the text to detect from
 
         Returns:
             str: langcode detected (lowered)
         """
         tx = self.translator.translate_text(text,
                                             target_lang="en-us")
-        return tx.detected_source_lang.lower() or self.default_language
+        lang = tx.detected_source_lang.lower()
+        if lang:
+            LOG.debug(f"Language ({lang}) detected") 
+        return lang or self.default_language
     
     @property
     def available_languages(self) -> set:
         """
         The available source languages that can be detected
 
         Returns:
```

## ovos_translate_plugin_deepl/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 1
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `ovos_translate_plugin_deepl-0.0.0a1.dist-info/LICENSE` & `ovos_translate_plugin_deepl-0.0.0a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_translate_plugin_deepl-0.0.0a1.dist-info/METADATA` & `ovos_translate_plugin_deepl-0.0.0a2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-translate-plugin-deepl
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: OVOS translation/detection module wrapping deepl-python
 Home-page: https://github.com/emphasize/ovos-translate-plugin-deepl
 Author: emphasize
 Author-email: UNKNOWN
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

