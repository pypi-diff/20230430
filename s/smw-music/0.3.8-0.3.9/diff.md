# Comparing `tmp/smw_music-0.3.8.tar.gz` & `tmp/smw_music-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smw_music-0.3.8.tar", max compression
+gzip compressed data, was "smw_music-0.3.9.tar", max compression
```

## Comparing `smw_music-0.3.8.tar` & `smw_music-0.3.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0        0        0        0 2023-04-28 00:41:15.166135 smw_music-0.3.8/LICENSES/
--rw-r--r--   0        0        0     5252 2023-04-28 00:41:15.166135 smw_music-0.3.8/README.rst
--rw-r--r--   0        0        0     2496 2023-04-28 00:41:15.166135 smw_music-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      710 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/__init__.py
--rw-r--r--   0        0        0     9772 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/brr.py
--rw-r--r--   0        0        0    77544 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/ankha.gif
--rw-r--r--   0        0        0   131530 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/ashtley.gif
--rw-r--r--   0        0        0       84 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/codenames.csv
--rw-r--r--   0        0        0      252 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/convert.bat
--rw-r--r--   0        0        0      270 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/convert.sh
--rw-r--r--   0        0        0   126564 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/dashboard.ui
--rw-r--r--   0        0        0     9009 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/maestro.svg
--rw-r--r--   0        0        0     5330 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/mml.txt
--rw-r--r--   0        0        0     4321 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/preferences.ui
--rw-r--r--   0        0        0     2684 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/log.py
--rw-r--r--   0        0        0      500 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/__init__.py
--rw-r--r--   0        0        0     6716 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/channel.py
--rw-r--r--   0        0        0     5685 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/echo.py
--rw-r--r--   0        0        0    14750 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/instrument.py
--rw-r--r--   0        0        0    12411 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/mml.py
--rw-r--r--   0        0        0    16816 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/reduction.py
--rw-r--r--   0        0        0     1041 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/shared.py
--rw-r--r--   0        0        0    25691 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/song.py
--rw-r--r--   0        0        0    18411 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/tokens.py
--rw-r--r--   0        0        0     1759 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/nspc.py
--rw-r--r--   0        0        0        0 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/py.typed
--rw-r--r--   0        0        0      204 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/scripts/__init__.py
--rw-r--r--   0        0        0     2559 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/scripts/convert.py
--rw-r--r--   0        0        0     1645 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/scripts/dashboard.py
--rw-r--r--   0        0        0     7933 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/scripts/filttool.py
--rw-r--r--   0        0        0      205 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/__init__.py
--rw-r--r--   0        0        0    57971 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/dashboard.py
--rw-r--r--   0        0        0     9824 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/dashboard_view.py
--rw-r--r--   0        0        0     8356 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/envelope_preview.py
--rw-r--r--   0        0        0     8522 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/keyboard.py
--rw-r--r--   0        0        0    62892 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/model.py
--rw-r--r--   0        0        0      205 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/old_save/__init__.py
--rw-r--r--   0        0        0     6739 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/old_save/v0.py
--rw-r--r--   0        0        0     4568 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/preferences.py
--rw-r--r--   0        0        0      852 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/preferences_view.py
--rw-r--r--   0        0        0    22284 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/quotes.py
--rw-r--r--   0        0        0     6062 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/sample.py
--rw-r--r--   0        0        0    12081 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/save.py
--rw-r--r--   0        0        0     4084 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/state.py
--rw-r--r--   0        0        0     8040 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/utilization.py
--rw-r--r--   0        0        0     1261 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/utils.py
--rw-r--r--   0        0        0     1811 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/utils.py
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 smw_music-0.3.8/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-30 00:24:12.939586 smw_music-0.3.9/LICENSES/
+-rw-r--r--   0        0        0     5252 2023-04-30 00:24:12.939586 smw_music-0.3.9/README.rst
+-rw-r--r--   0        0        0     2496 2023-04-30 00:24:12.943586 smw_music-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-04-30 00:24:12.943586 smw_music-0.3.9/smw_music/__init__.py
+-rw-r--r--   0        0        0     9930 2023-04-30 00:24:12.943586 smw_music-0.3.9/smw_music/brr.py
+-rw-r--r--   0        0        0    77544 2023-04-30 00:24:12.943586 smw_music-0.3.9/smw_music/data/ankha.gif
+-rw-r--r--   0        0        0   131530 2023-04-30 00:24:12.943586 smw_music-0.3.9/smw_music/data/ashtley.gif
+-rw-r--r--   0        0        0      106 2023-04-30 00:24:12.943586 smw_music-0.3.9/smw_music/data/codenames.csv
+-rw-r--r--   0        0        0      258 2023-04-30 00:24:12.943586 smw_music-0.3.9/smw_music/data/convert.bat
+-rw-r--r--   0        0        0      270 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/data/convert.sh
+-rw-r--r--   0        0        0   126564 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/data/dashboard.ui
+-rw-r--r--   0        0        0     9009 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/data/maestro.svg
+-rw-r--r--   0        0        0     5330 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/data/mml.txt
+-rw-r--r--   0        0        0     4321 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/data/preferences.ui
+-rw-r--r--   0        0        0     2684 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/log.py
+-rw-r--r--   0        0        0      500 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/__init__.py
+-rw-r--r--   0        0        0     6716 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/channel.py
+-rw-r--r--   0        0        0     5685 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/echo.py
+-rw-r--r--   0        0        0    14743 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/instrument.py
+-rw-r--r--   0        0        0    12411 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/mml.py
+-rw-r--r--   0        0        0    16816 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/reduction.py
+-rw-r--r--   0        0        0     1041 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/shared.py
+-rw-r--r--   0        0        0    25691 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/song.py
+-rw-r--r--   0        0        0    18411 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/music_xml/tokens.py
+-rw-r--r--   0        0        0     1759 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/nspc.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/py.typed
+-rw-r--r--   0        0        0      204 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/scripts/__init__.py
+-rw-r--r--   0        0        0     2559 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/scripts/convert.py
+-rw-r--r--   0        0        0     1645 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/scripts/dashboard.py
+-rw-r--r--   0        0        0     7933 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/scripts/filttool.py
+-rw-r--r--   0        0        0      205 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/__init__.py
+-rw-r--r--   0        0        0    58180 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/dashboard.py
+-rw-r--r--   0        0        0     9824 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/dashboard_view.py
+-rw-r--r--   0        0        0     8356 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/envelope_preview.py
+-rw-r--r--   0        0        0     8522 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/keyboard.py
+-rw-r--r--   0        0        0    63709 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/model.py
+-rw-r--r--   0        0        0      205 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/old_save/__init__.py
+-rw-r--r--   0        0        0     6739 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/old_save/v0.py
+-rw-r--r--   0        0        0     4568 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/preferences.py
+-rw-r--r--   0        0        0      852 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/preferences_view.py
+-rw-r--r--   0        0        0    22284 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/quotes.py
+-rw-r--r--   0        0        0     6536 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/sample.py
+-rw-r--r--   0        0        0    12172 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/save.py
+-rw-r--r--   0        0        0     4084 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/state.py
+-rw-r--r--   0        0        0     8040 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/utilization.py
+-rw-r--r--   0        0        0     1261 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/ui/utils.py
+-rw-r--r--   0        0        0     1811 2023-04-30 00:24:12.947586 smw_music-0.3.9/smw_music/utils.py
+-rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 smw_music-0.3.9/PKG-INFO
```

### Comparing `smw_music-0.3.8/README.rst` & `smw_music-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/pyproject.toml` & `smw_music-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 filter_files = true
 known_first_party = ["smw_music"]
 known_third_party = ["music21"]
 skip_glob = ["smw_music/doc/"]
 
 [tool.poetry]
 name = "smw_music"
-version = "0.3.8"
+version = "0.3.9"
 description = "Tools for working with SMW Music"
 authors = ["Thomas A. Werne <werneta@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.rst"
 repository = "http://github.com/com-posers-pit/smw_music"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `smw_music-0.3.8/smw_music/__init__.py` & `smw_music-0.3.9/smw_music/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """Top level SMW Music Module."""
 
 ###############################################################################
 # API variable definitions
 ###############################################################################
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 ###############################################################################
 # API class definitions
 ###############################################################################
 
 
 class SmwMusicException(Exception):
```

### Comparing `smw_music-0.3.8/smw_music/brr.py` & `smw_music-0.3.9/smw_music/brr.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,19 +215,24 @@
 
     ###########################################################################
 
     @cached_property
     def fundamental(self) -> float:
         samples_per_loop = SAMPLES_PER_BLOCK * (self.nblocks - self.loop_block)
         target_samples = 64000
-        loops = math.ceil(target_samples / samples_per_loop)
+        try:
+            loops = math.ceil(target_samples / samples_per_loop)
+            start = self.loop_block * SAMPLES_PER_BLOCK
+        except ZeroDivisionError:
+            # Non-looping brr samples will use this branch
+            loops = 1
+            start = 0
 
         nyquist = SAMPLE_FREQ / 2
         waveform = self.generate_waveform(loops)
-        start = self.loop_block * SAMPLES_PER_BLOCK
         spec = np.abs(np.fft.rfft(waveform[start:]))
         spec /= spec.max()
         peak, *_ = find_peaks(spec, height=0.25)[0]
         return nyquist * peak / len(spec)
 
     ###########################################################################
```

### Comparing `smw_music-0.3.8/smw_music/data/ankha.gif` & `smw_music-0.3.9/smw_music/data/ankha.gif`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/data/ashtley.gif` & `smw_music-0.3.9/smw_music/data/ashtley.gif`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/data/dashboard.ui` & `smw_music-0.3.9/smw_music/data/dashboard.ui`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/data/maestro.svg` & `smw_music-0.3.9/smw_music/data/maestro.svg`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/data/mml.txt` & `smw_music-0.3.9/smw_music/data/mml.txt`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/data/preferences.ui` & `smw_music-0.3.9/smw_music/data/preferences.ui`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/log.py` & `smw_music-0.3.9/smw_music/log.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/music_xml/channel.py` & `smw_music-0.3.9/smw_music/music_xml/channel.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/music_xml/echo.py` & `smw_music-0.3.9/smw_music/music_xml/echo.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/music_xml/instrument.py` & `smw_music-0.3.9/smw_music/music_xml/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,23 +255,23 @@
         vxadsr1 = int(self.adsr_mode) << 7
         vxadsr1 |= self.decay_setting << 4
         vxadsr1 |= self.attack_setting
         vxadsr2 = (self.sus_level_setting << 5) | self.sus_rate_setting
 
         match self.gain_mode:
             case GainMode.DIRECT:
-                vxgain = 0x80 | self.gain_setting
+                vxgain = self.gain_setting
             case GainMode.INCLIN:
-                vxgain = 0x40 | self.gain_setting
+                vxgain = 0xC0 | self.gain_setting
             case GainMode.INCBENT:
-                vxgain = 0x60 | self.gain_setting
+                vxgain = 0xE0 | self.gain_setting
             case GainMode.DECLIN:
-                vxgain = 0x00 | self.gain_setting
+                vxgain = 0x80 | self.gain_setting
             case GainMode.DECEXP:
-                vxgain = 0x20 | self.gain_setting
+                vxgain = 0xA0 | self.gain_setting
 
         return (
             vxadsr1,
             vxadsr2,
             vxgain,
             self.tune_setting,
             self.subtune_setting,
```

### Comparing `smw_music-0.3.8/smw_music/music_xml/mml.py` & `smw_music-0.3.9/smw_music/music_xml/mml.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/music_xml/reduction.py` & `smw_music-0.3.9/smw_music/music_xml/reduction.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/music_xml/shared.py` & `smw_music-0.3.9/smw_music/music_xml/shared.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/music_xml/song.py` & `smw_music-0.3.9/smw_music/music_xml/song.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/music_xml/tokens.py` & `smw_music-0.3.9/smw_music/music_xml/tokens.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/nspc.py` & `smw_music-0.3.9/smw_music/nspc.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/scripts/convert.py` & `smw_music-0.3.9/smw_music/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/scripts/dashboard.py` & `smw_music-0.3.9/smw_music/scripts/dashboard.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/scripts/filttool.py` & `smw_music-0.3.9/smw_music/scripts/filttool.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/dashboard.py` & `smw_music-0.3.9/smw_music/ui/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """Dashboard application."""
 
 ###############################################################################
 # Imports
 ###############################################################################
 
 # Standard library imports
+import csv
 import enum
 from collections import deque
 from contextlib import ExitStack, suppress
 from functools import cached_property, partial
 from importlib import resources
 from os import stat
 from pathlib import Path
@@ -673,16 +674,21 @@
         self._view.statusBar().showMessage(msg)
 
     ###########################################################################
     # Private method definitions
     ###########################################################################
 
     def _about(self) -> None:
+        data_lib = resources.files("smw_music.data")
+        with open(data_lib / "codenames.csv") as fobj:
+            for row in csv.reader(fobj):
+                codename = row[-1]
+
         title = "About MusicXML -> MML"
-        text = f"Version: {__version__}"
+        text = f"Version: {__version__} ({codename})"
         text += "\nCopyright Ⓒ 2023 The SMW Music Python Project Authors"
         text += "\nHomepage: https://github.com/com-posers-pit/smw_music"
 
         QMessageBox.about(self._view, title, text)
 
     ###########################################################################
```

### Comparing `smw_music-0.3.8/smw_music/ui/dashboard_view.py` & `smw_music-0.3.9/smw_music/ui/dashboard_view.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/envelope_preview.py` & `smw_music-0.3.9/smw_music/ui/envelope_preview.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/keyboard.py` & `smw_music-0.3.9/smw_music/ui/keyboard.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/model.py` & `smw_music-0.3.9/smw_music/ui/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -801,15 +801,15 @@
         self.update_status("Recent projects cleared")
 
     ###########################################################################
 
     def on_redo_clicked(self) -> None:
         if self._undo_level > 0:
             self._undo_level -= 1
-            self._signal_state_change(update_aram_util=False)
+            self._signal_state_change()
             self.update_status("Redo")
 
     ###########################################################################
 
     def on_reload_musicxml_clicked(self) -> None:
         assert self.state.musicxml_fname is not None
         self._load_musicxml(self.state.musicxml_fname, True)
@@ -1040,30 +1040,42 @@
                 self.update_status("Using manual note tuning")
 
     ###########################################################################
 
     def on_undo_clicked(self) -> None:
         if self._undo_level < len(self._history) - 1:
             self._undo_level += 1
-            self._signal_state_change(update_aram_util=False)
+            self._signal_state_change()
             self.update_status("Undo")
 
     ###########################################################################
     # Private method definitions
     ###########################################################################
 
     def _append_recent_project(self, fname: Path) -> None:
+        fname = fname.resolve()
         history = self.recent_projects
         if fname in history:
             history.remove(fname)
         history.append(fname)
         self.recent_projects = history
 
     ###########################################################################
 
+    def _check_bad_tune(self) -> list[tuple[str, str]]:
+        bad_samples = []
+        for inst_name, inst in self.state.instruments.items():
+            for sample_name, sample in inst.samples.items():
+                if (sample.tune_setting, sample.subtune_setting) == (0, 0):
+                    bad_samples.append((inst_name, sample_name))
+
+        return bad_samples
+
+    ###########################################################################
+
     def _interpolate(self, level: Dynamics, setting: int) -> None:
         inst = self.state.instrument
         sample = self.state.sample
         dyns = sorted(inst.dynamics_present)
         dynamics = deepcopy(sample.dynamics)
 
         min_dyn = min(dyns)
@@ -1286,16 +1298,23 @@
                     self.state.start_measure,
                 )
                 self.mml_generated.emit(mml)
                 self.update_status("MML generated")
             except MusicXmlException as e:
                 msg = str(e)
             else:
-                error = False
-                msg = "Done"
+                bad_samples = self._check_bad_tune()
+                if bad_samples:
+                    msg = "\n".join(
+                        f"{inst}{f':{samp}' if samp else ''} has 0.0 tuning"
+                        for inst, samp in bad_samples
+                    )
+                else:
+                    error = False
+                    msg = "Done"
 
         if report or error:
             self.response_generated.emit(error, title, msg)
 
         return not error
 
     ###########################################################################
@@ -1400,34 +1419,32 @@
 
     ###########################################################################
 
     def _signal_state_change(
         self,
         update_instruments: bool = False,
         state_change: bool = True,
-        update_aram_util: bool = True,
     ) -> None:
         state = self.state
 
         state.unsaved = state_change
         self.state.unmapped = set()
 
         self._update_aram_util()
 
         brr: Brr | None = None
         with suppress(NoSample):
             sample = self.state.sample
-            if sample.sample_source == SampleSource.SAMPLEPACK:
-                pack, path = sample.pack_sample
-                brr = self._sample_packs[pack][path].brr
-
-            else:
-
-                with suppress(FileNotFoundError):
-                    brr = Brr.from_file(sample.brr_fname)
+            match sample.sample_source:
+                case SampleSource.SAMPLEPACK:
+                    pack, path = sample.pack_sample
+                    brr = self._sample_packs[pack][path].brr
+                case SampleSource.BRR:
+                    with suppress(FileNotFoundError):
+                        brr = Brr.from_file(sample.brr_fname)
 
         if brr is not None:
             tuning = self.state.sample.tuning
             scale = SAMPLE_FREQ / tuning.sample_freq
             source = tuning.source
 
             # When not in advanced mode, always use auto tuning
@@ -1639,25 +1656,27 @@
         with suppress(FileNotFoundError):
             with open(fname, "r", encoding="utf8") as fobj:
                 projects = yaml.safe_load(fobj)
 
         if projects is None:
             projects = []
 
-        return [Path(project) for project in projects]
+        return [Path(project).resolve() for project in projects]
 
     ###########################################################################
 
     @recent_projects.setter
     def recent_projects(self, projects: list[Path]) -> None:
         project_limit = 5
         projects = projects[-project_limit:]
 
         with open(self.recent_projects_fname, "w", encoding="utf8") as fobj:
-            yaml.safe_dump([str(project) for project in projects], fobj)
+            yaml.safe_dump(
+                [str(project.resolve()) for project in projects], fobj
+            )
 
         self.recent_projects_updated.emit(projects)
 
     ###########################################################################
 
     @property
     def recent_projects_fname(self) -> Path:
```

### Comparing `smw_music-0.3.8/smw_music/ui/old_save/v0.py` & `smw_music-0.3.9/smw_music/ui/old_save/v0.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/preferences.py` & `smw_music-0.3.9/smw_music/ui/preferences.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/preferences_view.py` & `smw_music-0.3.9/smw_music/ui/preferences_view.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/quotes.py` & `smw_music-0.3.9/smw_music/ui/quotes.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/sample.py` & `smw_music-0.3.9/smw_music/ui/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ###############################################################################
 # Imports
 ###############################################################################
 
 # Standard library imports
 from dataclasses import dataclass
 from functools import cached_property
-from glob import glob
+from glob import iglob
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import TextIO
 from zipfile import ZipFile
 
 # Package imports
 from smw_music.brr import Brr
@@ -78,29 +78,39 @@
                 sample_params = []
                 with open(Path(tdir) / pat_file, "r", encoding="utf8") as fobj:
                     sample_params = SampleParams.from_pattern_file(fobj)
 
                 # Stupid case insensitive file systems.  Build a map between
                 # the lower-case version of file name in the directory and its
                 brr_data = {}
-                for fname in glob("*.brr", root_dir=parent_dir):
+                for fname in iglob("*.brr", root_dir=parent_dir):
                     with open(parent_dir / fname, "rb") as fobj:
                         brr_data[fname.lower()] = fobj.read()
 
                 for brr_fname, params in sample_params:
                     try:
                         data = brr_data[brr_fname.lower()]
                         sample_file = parent / brr_fname
                         samples[sample_file] = Sample(
                             sample_file, params, data
                         )
                     except KeyError:
                         # If a file in the pattern file is missing, skip it
                         continue
 
+            # Add brr files that aren't in the !patterns.txt file
+            default_params = SampleParams.from_regs([0, 0, 0x7F, 0x10, 0])
+            for fname in iglob("**/*.brr", root_dir=tdir, recursive=True):
+                path = Path(fname)
+                if path not in samples:
+                    with open(Path(tdir) / fname, "rb") as fobj:
+                        data = fobj.read()
+
+                    samples[path] = Sample(path, default_params, data)
+
         self._samples = samples
 
 
 ###############################################################################
 
 
 @dataclass
```

### Comparing `smw_music-0.3.8/smw_music/ui/save.py` & `smw_music-0.3.9/smw_music/ui/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,20 +287,23 @@
 def _update_convert_scripts(dirname: Path) -> None:
     for fname in ["convert.bat", "convert.sh"]:
         fpath = dirname / fname
 
         with open(fpath, "r", encoding="utf8") as fobj:
             lines = fobj.readlines()
 
-        if "-visualize" not in lines[-1]:
-            split = lines[-1].split('"')
-            split[0] += "-visualize "
-            lines[-1] = '"'.join(split)
-            with open(fpath, "w", encoding="utf8") as fobj:
-                fobj.write("".join(lines))
+        for n, line in enumerate(lines):
+            if "AddmusicK" in line and "-visualize" not in line:
+                split = line.split('"')
+                split[0] += "-visualize "
+                line = '"'.join(split)
+                lines[n] = line
+
+        with open(fpath, "w", encoding="utf8") as fobj:
+            fobj.write("".join(lines))
 
 
 ###############################################################################
 # API function definitions
 ###############################################################################
```

### Comparing `smw_music-0.3.8/smw_music/ui/state.py` & `smw_music-0.3.9/smw_music/ui/state.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/utilization.py` & `smw_music-0.3.9/smw_music/ui/utilization.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/ui/utils.py` & `smw_music-0.3.9/smw_music/ui/utils.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/smw_music/utils.py` & `smw_music-0.3.9/smw_music/utils.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.8/PKG-INFO` & `smw_music-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smw-music
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tools for working with SMW Music
 Home-page: http://github.com/com-posers-pit/smw_music
 License: AGPL-3.0-only
 Author: Thomas A. Werne
 Author-email: werneta@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
```

