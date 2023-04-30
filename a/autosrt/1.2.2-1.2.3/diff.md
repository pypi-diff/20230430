# Comparing `tmp/autosrt-1.2.2.tar.gz` & `tmp/autosrt-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.2.2.tar", last modified: Sun Apr 30 03:58:12 2023, max compression
+gzip compressed data, was "autosrt-1.2.3.tar", last modified: Sun Apr 30 13:30:55 2023, max compression
```

## Comparing `autosrt-1.2.2.tar` & `autosrt-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 03:58:12.743286 autosrt-1.2.2/
--rwxrwxrwx   0 root         (0) root         (0)     1087 2023-01-06 18:50:17.000000 autosrt-1.2.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-01-06 18:50:17.000000 autosrt-1.2.2/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     1987 2023-04-30 03:58:12.743577 autosrt-1.2.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5250 2023-04-30 03:29:13.000000 autosrt-1.2.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 03:58:12.734497 autosrt-1.2.2/autosrt/
--rwxrwxrwx   0 root         (0) root         (0)     9271 2023-04-30 03:54:52.000000 autosrt-1.2.2/autosrt/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    32560 2023-04-30 01:39:46.000000 autosrt-1.2.2/autosrt/autosrt.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 03:58:12.740015 autosrt-1.2.2/autosrt.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1987 2023-04-30 03:58:12.000000 autosrt-1.2.2/autosrt.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-30 03:58:12.000000 autosrt-1.2.2/autosrt.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-30 03:58:12.000000 autosrt-1.2.2/autosrt.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-30 03:58:12.000000 autosrt-1.2.2/autosrt.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      112 2023-04-30 03:58:12.000000 autosrt-1.2.2/autosrt.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-04-30 03:58:12.000000 autosrt-1.2.2/autosrt.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      136 2023-04-30 03:58:12.744683 autosrt-1.2.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1610 2023-04-30 03:54:44.000000 autosrt-1.2.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 03:58:12.742440 autosrt-1.2.2/test/
--rwxrwxrwx   0 root         (0) root         (0)     6874 2023-04-30 02:05:08.000000 autosrt-1.2.2/test/test1.py
--rwxrwxrwx   0 root         (0) root         (0)     4087 2023-04-30 02:05:48.000000 autosrt-1.2.2/test/test2.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:30:55.177793 autosrt-1.2.3/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-04-30 13:30:55.177793 autosrt-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 13:30:55.144827 autosrt-1.2.3/autosrt/
+-rw-rw-rw-   0        0        0     9271 2023-04-30 13:28:57.000000 autosrt-1.2.3/autosrt/__init__.py
+-rw-rw-rw-   0        0        0    32560 2023-04-30 13:27:29.000000 autosrt-1.2.3/autosrt/autosrt.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:30:55.166555 autosrt-1.2.3/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-04-30 13:30:54.000000 autosrt-1.2.3/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-30 13:30:55.000000 autosrt-1.2.3/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 13:30:54.000000 autosrt-1.2.3/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-30 13:30:54.000000 autosrt-1.2.3/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      141 2023-04-30 13:30:54.000000 autosrt-1.2.3/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-30 13:30:54.000000 autosrt-1.2.3/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-30 13:30:55.180789 autosrt-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-04-30 13:30:32.000000 autosrt-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:30:55.175547 autosrt-1.2.3/test/
+-rw-rw-rw-   0        0        0     6874 2023-04-30 02:05:08.000000 autosrt-1.2.3/test/test1.py
+-rw-rw-rw-   0        0        0     4087 2023-04-30 02:05:48.000000 autosrt-1.2.3/test/test2.py
```

### Comparing `autosrt-1.2.2/LICENSE` & `autosrt-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.2/PKG-INFO` & `autosrt-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: autosrt
-Version: 1.2.2
-Summary: a utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: autosrt
+Version: 1.2.3
+Summary: a utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.2.2/README.md` & `autosrt-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   
 ### Auto generate subtitle files for any video / audio files
 autosrt is a simple command line tool made with python to auto generate subtitle/closed caption for any video or audio files and translate it automatically for free using a simple unofficial online Google Translate API.
 
 This script is a modified version of original autosub made by Anastasis Germanidis at https://github.com/agermanidis/autosub
 
 ### UPDATE NOTES
-Since version 1.2.1 I tried to make some class modules, so in case you want to use them in your own project you can just import them. They are Language, WavConverter, SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, SubtitleFormatter, and SubtitleWriter. You can import them like this :
+Since version 1.2.2 I tried to make some class modules, so in case you want to use them in your own project you can just import them. They are Language, WavConverter, SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, SubtitleFormatter, and SubtitleWriter. You can import them like this :
 ```
 from autosrt import Language, WavConverter, SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
     SubtitleFormatter,  SubtitleWriter
 ```
 
 You can learn how to use them by playing around with those scripts inside test folder. Check every def function on each class to know how to use them. They are not to difficult to understand.
 
@@ -48,22 +48,23 @@
 The executable compiled file will be placed by pyinstaller into dist subfolder of your current working folder, so you can just rename and put that compiled file into a folder that has been added to your PATH ENVIRONTMENT so you can execute it from anywhere
 
 I was succesfuly compiled it in Windows 10 with pyinstaller-5.1 and Pyhton-3.10.4, and python-3.8.12 in Debian 9
 
 Another alternative way to install this script with python is by cloning this git (or downloading this git as zip then extract it into a folder), and then just type :
 
 ```
+pip install wheel
 python setup.py build
-python setup.py python setup.py bdist_wheel
+python setup.py bdist_wheel
 ```
 
-Then check the name of the whl file in dist folder. In case the filename is autosrt-1.2.0-py2.py3-none-any.whl then you can install that whl file with pip :
+Then check the name of the whl file created in dist folder. In case the filename is autosrt-1.2.2-py2.py3-none-any.whl then you can install that whl file with pip :
 ```
 cd dist
-pip install autosrt-1.2.0-py2.py3-none-any.whl
+pip install autosrt-1.2.2-py2.py3-none-any.whl
 ```
 
 You can also install this script (or any pip package) in ANDROID DEVICES via PYTHON package in TERMUX APP
 
 https://github.com/termux/termux-app/releases/tag/v0.118.0
 
 Choose the right apk for your device, install it, then open it
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # autosrt [https://img.shields.io/pypi/v/autosrt.svg] ### Auto generate
 subtitle files for any video / audio files autosrt is a simple command line
 tool made with python to auto generate subtitle/closed caption for any video or
 audio files and translate it automatically for free using a simple unofficial
 online Google Translate API. This script is a modified version of original
 autosub made by Anastasis Germanidis at https://github.com/agermanidis/autosub
-### UPDATE NOTES Since version 1.2.1 I tried to make some class modules, so in
+### UPDATE NOTES Since version 1.2.2 I tried to make some class modules, so in
 case you want to use them in your own project you can just import them. They
 are Language, WavConverter, SpeechRegionFinder, FLACConverter,
 SpeechRecognizer, SentenceTranslator, SubtitleFormatter, and SubtitleWriter.
 You can import them like this : ``` from autosrt import Language, WavConverter,
 SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
 SubtitleFormatter, SubtitleWriter ``` You can learn how to use them by playing
 around with those scripts inside test folder. Check every def function on each
@@ -29,23 +29,23 @@
 install pyinstaller pyinstaller --onefile autosrt.py ``` The executable
 compiled file will be placed by pyinstaller into dist subfolder of your current
 working folder, so you can just rename and put that compiled file into a folder
 that has been added to your PATH ENVIRONTMENT so you can execute it from
 anywhere I was succesfuly compiled it in Windows 10 with pyinstaller-5.1 and
 Pyhton-3.10.4, and python-3.8.12 in Debian 9 Another alternative way to install
 this script with python is by cloning this git (or downloading this git as zip
-then extract it into a folder), and then just type : ``` python setup.py build
-python setup.py python setup.py bdist_wheel ``` Then check the name of the whl
-file in dist folder. In case the filename is autosrt-1.2.0-py2.py3-none-any.whl
-then you can install that whl file with pip : ``` cd dist pip install autosrt-
-1.2.0-py2.py3-none-any.whl ``` You can also install this script (or any pip
-package) in ANDROID DEVICES via PYTHON package in TERMUX APP https://
-github.com/termux/termux-app/releases/tag/v0.118.0 Choose the right apk for
-your device, install it, then open it Type these commands to get python, pip,
-this autosrt, (and any other pip packages) : ``` termux-setup-storage pkg
+then extract it into a folder), and then just type : ``` pip install wheel
+python setup.py build python setup.py bdist_wheel ``` Then check the name of
+the whl file created in dist folder. In case the filename is autosrt-1.2.2-
+py2.py3-none-any.whl then you can install that whl file with pip : ``` cd dist
+pip install autosrt-1.2.2-py2.py3-none-any.whl ``` You can also install this
+script (or any pip package) in ANDROID DEVICES via PYTHON package in TERMUX APP
+https://github.com/termux/termux-app/releases/tag/v0.118.0 Choose the right apk
+for your device, install it, then open it Type these commands to get python,
+pip, this autosrt, (and any other pip packages) : ``` termux-setup-storage pkg
 update -y pkg install -y python pkg install -y ffmpeg pip install autosrt ```
 ### Simple usage example ``` autosrt --list-languages autosrt -S zh-CN -D en
 "Episode 1.mp4" ``` For multiple video/audio files (starts from version 1.1.0),
 you can use wildcard ``` autosrt -S zh-CN -D en "C:\Movies\*.mp4" ``` If you
 don't need translations just type : ``` autosrt -S zh-CN "Episode 1.mp4" ```
 ### Usage ``` usage: autosrt [-h] [-S SRC_LANGUAGE] [-D DST_LANGUAGE] [-ll] [-
 o OUTPUT] [-F FORMAT] [-lf] [-C CONCURRENCY] [-v] [source_path ...] positional
```

### Comparing `autosrt-1.2.2/autosrt/__init__.py` & `autosrt-1.2.3/autosrt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in video/audio source_path", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-ll', '--list-languages', help="List all supported languages", action='store_true')
     parser.add_argument('-o', '--output', help="Output file path for subtitles (by default, subtitles are saved in the same directory and named with the source_path base name)")
     parser.add_argument('-F', '--format', help="Desired subtitle format", default="srt")
     parser.add_argument('-lf', '--list-formats', help="List all supported subtitle formats", action='store_true')
     parser.add_argument('-C', '--concurrency', help="Number of concurrent API requests to make", type=int, default=10)
-    parser.add_argument('-v', '--version', action='version', version='1.2.2')
+    parser.add_argument('-v', '--version', action='version', version='1.2.3')
 
     args = parser.parse_args()
 
     language = Language()
 
     if args.list_languages:
         print("List of supported languages:")
```

### Comparing `autosrt-1.2.2/autosrt/autosrt.py` & `autosrt-1.2.3/autosrt/autosrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,15 +740,15 @@
             translated_sentence = []
             # handle the special case: empty string.
             if not sentence:
                 return None
             translated_sentence = self.GoogleTranslate(sentence, src=self.src, dst=self.dst)
             fail_to_translate = translated_sentence[-1] == '\n'
             while fail_to_translate and patience:
-                translated_sentence = translator.translate(translated_sentence, src=self.src, dst=self.dst).text
+                translated_sentence = self.GoogleTranslate(translated_sentence, src=self.src, dst=self.dst).text
                 if translated_sentence[-1] == '\n':
                     if patience == -1:
                         continue
                     patience -= 1
                 else:
                     fail_to_translate = False
```

### Comparing `autosrt-1.2.2/autosrt.egg-info/PKG-INFO` & `autosrt-1.2.3/autosrt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: autosrt
-Version: 1.2.2
-Summary: a utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: autosrt
+Version: 1.2.3
+Summary: a utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+autosrt is a utility for automatic speech recognition and subtitle generation.It takes a video or an audio file as input, performs voice activity detection to find speech regions,  makes parallel requests to Google Web Speech API  to generate transcriptions for those regions,  (optionally) translates them to a different language, and finally saves the resulting subtitles file to disk.   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `autosrt-1.2.2/setup.py` & `autosrt-1.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 
 install_requires=[
         "requests>=2.3.0",
         "pysrt>=1.0.1",
         "progressbar2>=3.34.3",
         "six>=1.11.0",
         "ffmpeg_progress_yield>=0.7.2",
+        "python_magic_bin>=0.4.14",
 ]
 
 if sys.platform == "win32":
     install_requires.append("python_magic_bin>=0.4.14")
-else:
-    install_requires.append("python_magic>=0.4.27")
+#else:
+#    install_requires.append("python_magic>=0.4.27")
 
 setup(
     name="autosrt",
-    version="1.2.2",
+    version="1.2.3",
     description="a utility for automatic speech recognition and subtitle generation",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/autosrt",
     packages=["autosrt"],
     entry_points={
```

### Comparing `autosrt-1.2.2/test/test1.py` & `autosrt-1.2.3/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.2.2/test/test2.py` & `autosrt-1.2.3/test/test2.py`

 * *Files identical despite different names*

