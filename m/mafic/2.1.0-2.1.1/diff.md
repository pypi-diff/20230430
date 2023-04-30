# Comparing `tmp/mafic-2.1.0.tar.gz` & `tmp/mafic-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.1.0.tar", max compression
+gzip compressed data, was "mafic-2.1.1.tar", max compression
```

## Comparing `mafic-2.1.0.tar` & `mafic-2.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2023-04-19 19:42:12.955674 mafic-2.1.0/LICENSE
--rw-r--r--   0        0        0     3315 2023-04-19 19:42:12.955674 mafic-2.1.0/README.md
--rw-r--r--   0        0        0      886 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/__main__.py
--rw-r--r--   0        0        0     4447 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/errors.py
--rw-r--r--   0        0        0     5609 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/ip.py
--rw-r--r--   0        0        0    35580 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/node.py
--rw-r--r--   0        0        0    23615 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/player.py
--rw-r--r--   0        0        0      929 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/plugin.py
--rw-r--r--   0        0        0     8150 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/py.typed
--rw-r--r--   0        0        0     3648 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/search_type.py
--rw-r--r--   0        0        0     3378 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/strategy.py
--rw-r--r--   0        0        0     4149 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/track.py
--rw-r--r--   0        0        0      747 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2817 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/common.py
--rw-r--r--   0        0        0     4018 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/http.py
--rw-r--r--   0        0        0     1968 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/incoming.py
--rw-r--r--   0        0        0      524 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/misc.py
--rw-r--r--   0        0        0     1152 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      139 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1129 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/utils/classproperty.py
--rw-r--r--   0        0        0     4987 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/utils/decode.py
--rw-r--r--   0        0        0      710 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-04-19 19:42:12.959674 mafic-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-30 15:29:52.014670 mafic-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3315 2023-04-30 15:29:52.014670 mafic-2.1.1/README.md
+-rw-r--r--   0        0        0      886 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/__main__.py
+-rw-r--r--   0        0        0     4447 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/errors.py
+-rw-r--r--   0        0        0     5609 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/ip.py
+-rw-r--r--   0        0        0    35618 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/node.py
+-rw-r--r--   0        0        0    23615 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/player.py
+-rw-r--r--   0        0        0      929 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/plugin.py
+-rw-r--r--   0        0        0     8150 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/search_type.py
+-rw-r--r--   0        0        0     3378 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/strategy.py
+-rw-r--r--   0        0        0     4149 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2817 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/typings/common.py
+-rw-r--r--   0        0        0     4018 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/typings/http.py
+-rw-r--r--   0        0        0     1968 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      524 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1152 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      139 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1129 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0     4987 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/utils/decode.py
+-rw-r--r--   0        0        0      710 2023-04-30 15:29:52.014670 mafic-2.1.1/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-04-30 15:29:52.014670 mafic-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.1.1/PKG-INFO
```

### Comparing `mafic-2.1.0/LICENSE` & `mafic-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/README.md` & `mafic-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/__init__.py` & `mafic-2.1.1/mafic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.1.0/mafic/__libraries.py` & `mafic-2.1.1/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/__main__.py` & `mafic-2.1.1/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/errors.py` & `mafic-2.1.1/mafic/errors.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/events.py` & `mafic-2.1.1/mafic/events.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/filter.py` & `mafic-2.1.1/mafic/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,15 @@
             and self.distortion == other.distortion
             and self.channel_mix == other.channel_mix
             and self.low_pass == other.low_pass
             and self.volume == other.volume
         )
 
     def __repr__(self) -> str:
-        """Gemerate the string representation of this filter."""
+        """Generate the string representation of this filter."""
         slots = self.__slots__
 
         attrs = [
             f"{attr}={getattr(self, attr)!r}"
             for attr in slots
             if getattr(self, attr) is not None
         ]
```

### Comparing `mafic-2.1.0/mafic/ip.py` & `mafic-2.1.1/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/node.py` & `mafic-2.1.1/mafic/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import re
 import warnings
 from asyncio import Event, TimeoutError, create_task, gather, sleep, wait_for
 from logging import getLogger
 from traceback import print_exc
 from typing import TYPE_CHECKING, Generic, cast
+from urllib.parse import quote
 
 import aiohttp
 import yarl
 
 from .__libraries import MISSING, ExponentialBackoff, dumps, loads
 from .errors import *
 from .ip import (
@@ -960,15 +961,15 @@
         None
             If the load type is ``NO_MATCHES``.
         """
         if not URL_REGEX.match(query):
             query = f"{search_type}:{query}"
 
         data: TrackLoadingResult = await self.__request(
-            "GET", "loadtracks", params={"identifier": query}
+            "GET", "loadtracks", params={"identifier": quote(query)}
         )
 
         if data["loadType"] == "NO_MATCHES":
             return []
         elif data["loadType"] == "TRACK_LOADED":
             return [Track.from_data_with_info(data["tracks"][0])]
         elif data["loadType"] == "PLAYLIST_LOADED":
```

### Comparing `mafic-2.1.0/mafic/player.py` & `mafic-2.1.1/mafic/player.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/playlist.py` & `mafic-2.1.1/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/plugin.py` & `mafic-2.1.1/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/pool.py` & `mafic-2.1.1/mafic/pool.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/region.py` & `mafic-2.1.1/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/search_type.py` & `mafic-2.1.1/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/stats.py` & `mafic-2.1.1/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/strategy.py` & `mafic-2.1.1/mafic/strategy.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/track.py` & `mafic-2.1.1/mafic/track.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/type_variables.py` & `mafic-2.1.1/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/typings/common.py` & `mafic-2.1.1/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/typings/http.py` & `mafic-2.1.1/mafic/typings/http.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/typings/incoming.py` & `mafic-2.1.1/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/typings/misc.py` & `mafic-2.1.1/mafic/typings/misc.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/typings/outgoing.py` & `mafic-2.1.1/mafic/typings/outgoing.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/utils/classproperty.py` & `mafic-2.1.1/mafic/utils/classproperty.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/utils/decode.py` & `mafic-2.1.1/mafic/utils/decode.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/mafic/warnings.py` & `mafic-2.1.1/mafic/warnings.py`

 * *Files identical despite different names*

### Comparing `mafic-2.1.0/pyproject.toml` & `mafic-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.1.0"
+version = "2.1.1"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
```

### Comparing `mafic-2.1.0/PKG-INFO` & `mafic-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.1.0
+Version: 2.1.1
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

