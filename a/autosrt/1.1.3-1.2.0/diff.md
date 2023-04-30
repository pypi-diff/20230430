# Comparing `tmp/autosrt-1.1.3.tar.gz` & `tmp/autosrt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.1.3.tar", last modified: Thu Apr 27 11:43:27 2023, max compression
+gzip compressed data, was "autosrt-1.2.0.tar", last modified: Sun Apr 30 01:46:00 2023, max compression
```

## Comparing `autosrt-1.1.3.tar` & `autosrt-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 11:43:27.306422 autosrt-1.1.3/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2454 2023-04-27 11:43:27.307174 autosrt-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3799 2023-02-13 02:23:24.000000 autosrt-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 11:43:27.277954 autosrt-1.1.3/autosrt/
--rw-rw-rw-   0        0        0    29249 2023-04-27 11:33:00.000000 autosrt-1.1.3/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:43:27.304924 autosrt-1.1.3/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2454 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-27 11:43:27.000000 autosrt-1.1.3/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-27 11:43:26.000000 autosrt-1.1.3/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-27 11:43:27.309420 autosrt-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1858 2023-04-27 11:28:48.000000 autosrt-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:46:00.904402 autosrt-1.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-04-30 01:46:00.905153 autosrt-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3799 2023-02-13 02:23:24.000000 autosrt-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 01:46:00.874434 autosrt-1.2.0/autosrt/
+-rw-rw-rw-   0        0        0     9271 2023-04-30 01:36:39.000000 autosrt-1.2.0/autosrt/__init__.py
+-rw-rw-rw-   0        0        0    32560 2023-04-30 01:39:46.000000 autosrt-1.2.0/autosrt/autosrt.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:46:00.896160 autosrt-1.2.0/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-04-30 01:46:00.000000 autosrt-1.2.0/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-30 01:46:00.000000 autosrt-1.2.0/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 01:46:00.000000 autosrt-1.2.0/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-30 01:46:00.000000 autosrt-1.2.0/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      137 2023-04-30 01:46:00.000000 autosrt-1.2.0/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 01:46:00.000000 autosrt-1.2.0/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-30 01:46:00.907400 autosrt-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1487 2023-04-30 01:22:01.000000 autosrt-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 01:46:00.902156 autosrt-1.2.0/test/
+-rw-rw-rw-   0        0        0     6776 2023-04-29 21:28:12.000000 autosrt-1.2.0/test/test1.py
+-rw-rw-rw-   0        0        0     4079 2023-04-29 21:45:13.000000 autosrt-1.2.0/test/test2.py
```

### Comparing `autosrt-1.1.3/LICENSE` & `autosrt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.1.3/PKG-INFO` & `autosrt-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.1.3
-Summary: autosrt is a utility for automatic speech recognition and subtitle generation. It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles to disk. It supports a variety of input and output languages  and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Version: 1.2.0
+Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
         
@@ -24,8 +24,8 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 
-autosrt is a utility for automatic speech recognition and subtitle generation. It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles to disk. It supports a variety of input and output languages  and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.1.3/README.md` & `autosrt-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.1.3/autosrt.egg-info/PKG-INFO` & `autosrt-1.2.0/autosrt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.1.3
-Summary: autosrt is a utility for automatic speech recognition and subtitle generation. It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles to disk. It supports a variety of input and output languages  and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Version: 1.2.0
+Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
         
@@ -24,8 +24,8 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 
-autosrt is a utility for automatic speech recognition and subtitle generation. It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles to disk. It supports a variety of input and output languages  and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.1.3/setup.py` & `autosrt-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,39 +3,41 @@
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 long_description = (
-    'autosrt is a utility for automatic speech recognition and subtitle generation. '
+    'autosrt is a utility for automatic speech recognition and subtitle generation.'
     'It takes a video or an audio file as input, performs voice activity detection '
     'to find speech regions,  makes parallel requests to Google Web Speech API  to '
     'generate transcriptions for those regions,  (optionally) translates them to a '
-    'different language, and finally saves the resulting subtitles to disk. '
-    'It supports a variety of input and output languages  and can currently produce '
+    'different language, and finally saves the resulting subtitles file to disk.   '
+    'It supports a variety of input and output languages and can currently produce '
     'subtitles in SRT, VTT, JSON, and RAW format.'
 )
 
 setup(
     name="autosrt",
-    version="1.1.3",
-    description="autosrt is a utility for automatic speech recognition and subtitle generation. It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles to disk. It supports a variety of input and output languages  and can currently produce subtitles in SRT, VTT, JSON, and RAW format.",
+    version="1.2.0",
+    description="a utility for automatic speech recognition and subtitle generation",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/autosrt",
-    packages=[str("autosrt")],
+    packages=["autosrt"],
     entry_points={
         "console_scripts": [
             "autosrt = autosrt:main",
         ],
     },
     install_requires=[
         "requests>=2.3.0",
         "pysrt>=1.0.1",
         "progressbar2>=3.34.3",
         "six>=1.11.0",
         "ffmpeg_progress_yield>=0.7.2",
+        "python_magic>=0.4.27",
+        "python_magic_bin>=0.4.14",
     ],
     license=open("LICENSE").read()
 )
```

