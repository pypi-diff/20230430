# Comparing `tmp/elevenlabslib-0.5.3.tar.gz` & `tmp/elevenlabslib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.5.3.tar", last modified: Fri Apr 28 09:19:30 2023, max compression
+gzip compressed data, was "elevenlabslib-0.6.0.tar", last modified: Sun Apr 30 12:48:16 2023, max compression
```

## Comparing `elevenlabslib-0.5.3.tar` & `elevenlabslib-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 09:19:30.768159 elevenlabslib-0.5.3/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.5.3/LICENSE
--rw-rw-rw-   0        0        0     2706 2023-04-28 09:19:30.767163 elevenlabslib-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 09:19:30.752162 elevenlabslib-0.5.3/elevenlabslib/
--rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.5.3/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.5.3/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    13846 2023-04-28 09:10:06.000000 elevenlabslib-0.5.3/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    31783 2023-04-28 09:17:07.000000 elevenlabslib-0.5.3/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.5.3/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5524 2023-04-26 11:42:12.000000 elevenlabslib-0.5.3/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:19:30.766159 elevenlabslib-0.5.3/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2706 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 09:19:30.000000 elevenlabslib-0.5.3/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      856 2023-04-28 09:17:16.000000 elevenlabslib-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 09:19:30.768159 elevenlabslib-0.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 12:48:16.057144 elevenlabslib-0.6.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2705 2023-04-30 12:48:16.055143 elevenlabslib-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 12:48:16.041143 elevenlabslib-0.6.0/elevenlabslib/
+-rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.6.0/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.6.0/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    14498 2023-04-30 12:31:41.000000 elevenlabslib-0.6.0/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    32952 2023-04-30 12:27:19.000000 elevenlabslib-0.6.0/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.6.0/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     5592 2023-04-30 12:39:02.000000 elevenlabslib-0.6.0/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:48:16.054142 elevenlabslib-0.6.0/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2705 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-04-30 12:47:22.000000 elevenlabslib-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 12:48:16.057144 elevenlabslib-0.6.0/setup.cfg
```

### Comparing `elevenlabslib-0.5.3/LICENSE` & `elevenlabslib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.3/PKG-INFO` & `elevenlabslib-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.5.3
+Version: 0.6.0
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # elevenlabslib
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)
```

### Comparing `elevenlabslib-0.5.3/README.md` & `elevenlabslib-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.3/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.6.0/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.3/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.6.0/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.5.3/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.6.0/elevenlabslib/ElevenLabsUser.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,35 +134,41 @@
             Some of these may be unusable due to subscription tier changes.
             Use get_available_voices if you only need the currently useable ones.
 
         Returns:
             list[ElevenLabsVoice]: A list containing all the voices.
         """
         response = _api_get("/voices", headers=self._headers)
-        availableVoices: list[ElevenLabsVoice] = list()
+        allVoices: list[ElevenLabsVoice] = list()
         voicesData = response.json()
         from elevenlabslib.ElevenLabsVoice import ElevenLabsVoice
         for voiceData in voicesData["voices"]:
-            availableVoices.append(ElevenLabsVoice.voiceFactory(voiceData, self))
-        return availableVoices
+            allVoices.append(ElevenLabsVoice.voiceFactory(voiceData, self))
+        return allVoices
 
     def get_available_voices(self) -> list[ElevenLabsVoice | ElevenLabsDesignedVoice | ElevenLabsClonedVoice]:
         """
-        Gets a list of voices this account can currently use.
+        Gets a list of voices this account can currently use for TTS.
 
         Returns:
             list[ElevenLabsVoice]: A list of currently usable voices.
         """
-        allVoices = self.get_all_voices()
+        response = _api_get("/voices", headers=self._headers)
+        voicesData = response.json()
         availableVoices = list()
         canUseClonedVoices = self.get_voice_clone_available()
-        for voice in allVoices:
-            if voice.category == "cloned" and not canUseClonedVoices:
+        from elevenlabslib.ElevenLabsVoice import ElevenLabsVoice
+        for voiceData in voicesData["voices"]:
+            if voiceData["category"] == "cloned" and not canUseClonedVoices:
+                continue
+            if voiceData["category"] == "professional" and voiceData["fine_tuning"]["finetuning_state"] != "complete":
+                #TODO: Change this value to the proper one once I actually know what it is. "complete" is merely a placeholder.
                 continue
-            availableVoices.append(voice)
+            availableVoices.append(ElevenLabsVoice.voiceFactory(voiceData, linkedUser=self))
+
         return availableVoices
 
     def get_voice_by_ID(self, voiceID: str) -> ElevenLabsVoice | ElevenLabsDesignedVoice | ElevenLabsClonedVoice:
         """
         Gets a specific voice by ID.
 
         Args:
@@ -184,19 +190,22 @@
 
         Args:
             voiceName (str): The name of the voices to get.
 
         Returns:
             list[ElevenLabsVoice|ElevenLabsDesignedVoice|ElevenLabsClonedVoice]: A list of matching voices.
         """
-        allVoices = self.get_available_voices()
+        response = _api_get("/voices", headers=self._headers)
+        voicesData = response.json()
         matchingVoices = list()
-        for voice in allVoices:
-            if voice.initialName == voiceName:
-                matchingVoices.append(voice)
+        from elevenlabslib.ElevenLabsVoice import ElevenLabsVoice
+        for voiceData in voicesData["voices"]:
+            if voiceData["name"] == voiceName:
+                matchingVoices.append(ElevenLabsVoice.voiceFactory(voiceData, linkedUser=self))
+
         return matchingVoices
 
     def get_history_items(self) -> list[ElevenLabsHistoryItem]:
         """
         Returns:
             list[ElevenLabsHistoryItem]: A list containing all of the user's history items.
         """
```

### Comparing `elevenlabslib-0.5.3/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.6.0/elevenlabslib/ElevenLabsVoice.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,22 +57,25 @@
         Args:
             voiceData: A dictionary containing the voice data.
             linkedUser: An instance of the ElevenLabsUser class representing the linked user.
 
         Returns:
             ElevenLabsVoice | ElevenLabsDesignedVoice | ElevenLabsClonedVoice: The voice object
         """
-        if voiceData["category"] == "premade":
+        category = voiceData["category"]
+        if category == "premade":
             return ElevenLabsVoice(voiceData, linkedUser)
-        elif voiceData["category"] == "cloned":
+        elif category == "cloned":
             return ElevenLabsClonedVoice(voiceData, linkedUser)
-        elif voiceData["category"] == "generated":
+        elif category == "generated":
             return ElevenLabsDesignedVoice(voiceData, linkedUser)
+        elif category == "professional":
+            return ElevenLabsProfessionalVoice(voiceData, linkedUser)
         else:
-            raise ValueError(voiceData["category"] + " is not a valid voice category!")
+            raise ValueError(f"{category} is not a valid voice category!")
 
     def __init__(self, voiceData, linkedUser:ElevenLabsUser):
         """
         Initializes a new instance of the ElevenLabsVoice class.
         Don't use this constructor directly. Use the factory instead.
 
         Args:
@@ -367,20 +370,47 @@
         This function deletes the voice, and also sets the voiceID to be empty.
         """
         if self._category == "premade":
             raise RuntimeError("Cannot delete premade voices!")
         response = _api_del("/voices/" + self._voiceID, self._linkedUser.headers)
         self._voiceID = ""
 
+class ElevenLabsProfessionalVoice(ElevenLabsDesignedVoice):
+    """
+    Note:
+        This is merely a stub for the time being, as professional voices are not yet fully available.
+    """
+    def __init__(self, voiceData, linkedUser: ElevenLabsUser):
+        super().__init__(voiceData, linkedUser)
+
+    def get_samples(self) -> list[ElevenLabsSample]:
+        """
+        Caution:
+            There is an API bug here. The /voices/voiceID endpoint does not correctly return sample data for professional cloning voices.
+
+        Returns:
+            list[ElevenLabsSample]: The samples that make up this professional voice clone.
+        """
+        outputList = list()
+        samplesData = self.get_info()["samples"]
+        from elevenlabslib.ElevenLabsSample import ElevenLabsSample
+        for sampleData in samplesData:
+            outputList.append(ElevenLabsSample(sampleData, self))
+        return outputList
 
 class ElevenLabsClonedVoice(ElevenLabsDesignedVoice):
     def __init__(self, voiceData, linkedUser: ElevenLabsUser):
         super().__init__(voiceData, linkedUser)
 
     def get_samples(self) -> list[ElevenLabsSample]:
+        """
+        Returns:
+            list[ElevenLabsSample]: The samples that make up this voice clone.
+        """
+
         outputList = list()
         samplesData = self.get_info()["samples"]
         from elevenlabslib.ElevenLabsSample import ElevenLabsSample
         for sampleData in samplesData:
             outputList.append(ElevenLabsSample(sampleData, self))
         return outputList
```

### Comparing `elevenlabslib-0.5.3/elevenlabslib/helpers.py` & `elevenlabslib-0.6.0/elevenlabslib/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import threading
 from typing import Optional, BinaryIO, Callable, Union
 
 import sounddevice as sd
 import soundfile
 import soundfile as sf
 import requests
+import os
 
 api_endpoint = "https://api.elevenlabs.io/v1"
 default_headers = {'accept': '*/*'}
 
 def _api_call(requestType, path, headers, jsonData=None, filesData=None) -> requests.Response:
     if path[0] != "/":
         path = "/"+path
@@ -101,15 +102,16 @@
     tempSoundFile = soundfile.SoundFile(io.BytesIO(audioData))
 
     if isinstance(saveLocation, str):
         with open(saveLocation, "wb") as fp:
             sf.write(fp, tempSoundFile.read(), tempSoundFile.samplerate, format=outputFormat)
     else:
         sf.write(saveLocation, tempSoundFile.read(), tempSoundFile.samplerate, format=outputFormat)
-        saveLocation.flush()
+        if callable(getattr(saveLocation,"flush")):
+            saveLocation.flush()
 
 #This class just helps with the callback stuff.
 class _SDPlaybackWrapper:
     def __init__(self, audioData, deviceID, onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None):
         soundFile = sf.SoundFile(io.BytesIO(audioData))
         soundFile.seek(0)
         self.onPlaybackStart = onPlaybackStart
```

### Comparing `elevenlabslib-0.5.3/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.6.0/elevenlabslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.5.3
+Version: 0.6.0
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # elevenlabslib
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)
```

### Comparing `elevenlabslib-0.5.3/pyproject.toml` & `elevenlabslib-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.5.3"
+version = "0.6.0"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
@@ -19,14 +19,14 @@
     "numpy",
     "soundfile >= 0.12.1"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha"
+    "Development Status :: 4 - Beta"
 ]
 
 [project.urls]
 "Documentation" = "https://elevenlabslib.readthedocs.io/en/latest/"
 "Homepage" = "https://github.com/lugia19/elevenlabslib"
 "Bug Tracker" = "https://github.com/lugia19/elevenlabslib"
```

