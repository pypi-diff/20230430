# Comparing `tmp/term-image-0.6.0.tar.gz` & `tmp/term-image-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "term-image-0.6.0.tar", last modified: Thu Mar 30 17:30:45 2023, max compression
+gzip compressed data, was "term-image-0.6.1.tar", last modified: Sun Apr 30 18:57:28 2023, max compression
```

## Comparing `term-image-0.6.0.tar` & `term-image-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-03-30 17:30:45.433094 term-image-0.6.0/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1076 2023-03-06 12:44:15.000000 term-image-0.6.0/LICENSE
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9591 2023-03-30 17:30:45.429761 term-image-0.6.0/PKG-INFO
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     8020 2023-03-30 16:22:44.000000 term-image-0.6.0/README.md
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      268 2023-03-29 13:56:11.000000 term-image-0.6.0/pyproject.toml
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-03-30 17:30:45.433094 term-image-0.6.0/setup.cfg
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1979 2023-03-30 17:01:01.000000 term-image-0.6.0/setup.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-03-30 17:30:45.426427 term-image-0.6.0/src/
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-03-30 17:30:45.429761 term-image-0.6.0/src/term_image/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     6539 2023-03-30 16:48:23.000000 term-image-0.6.0/src/term_image/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2499 2023-03-20 16:23:42.000000 term-image-0.6.0/src/term_image/exceptions.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-03-30 17:30:45.429761 term-image-0.6.0/src/term_image/image/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2502 2023-03-30 03:34:36.000000 term-image-0.6.0/src/term_image/image/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     5965 2023-03-25 21:38:19.000000 term-image-0.6.0/src/term_image/image/block.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    85250 2023-03-30 17:19:03.000000 term-image-0.6.0/src/term_image/image/common.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    28024 2023-03-26 23:39:36.000000 term-image-0.6.0/src/term_image/image/iterm2.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    21887 2023-03-25 21:38:19.000000 term-image-0.6.0/src/term_image/image/kitty.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    26949 2023-03-29 13:56:06.000000 term-image-0.6.0/src/term_image/utils.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-03-30 17:30:45.429761 term-image-0.6.0/src/term_image/widget/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      305 2023-03-06 02:28:38.000000 term-image-0.6.0/src/term_image/widget/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    23966 2023-03-30 13:52:38.000000 term-image-0.6.0/src/term_image/widget/urwid.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-03-30 17:30:45.429761 term-image-0.6.0/src/term_image.egg-info/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9591 2023-03-30 17:30:45.000000 term-image-0.6.0/src/term_image.egg-info/PKG-INFO
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      577 2023-03-30 17:30:45.000000 term-image-0.6.0/src/term_image.egg-info/SOURCES.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)        1 2023-03-30 17:30:45.000000 term-image-0.6.0/src/term_image.egg-info/dependency_links.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-03-30 17:30:45.000000 term-image-0.6.0/src/term_image.egg-info/requires.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       11 2023-03-30 17:30:45.000000 term-image-0.6.0/src/term_image.egg-info/top_level.txt
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-03-30 17:30:45.429761 term-image-0.6.0/tests/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    13479 2023-03-30 13:54:35.000000 term-image-0.6.0/tests/test_iterator.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2036 2023-02-28 01:12:57.000000 term-image-0.6.0/tests/test_top_level.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.145185 term-image-0.6.1/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1076 2023-03-06 12:44:15.000000 term-image-0.6.1/LICENSE
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9747 2023-04-30 18:57:28.145185 term-image-0.6.1/PKG-INFO
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     8125 2023-04-30 17:57:47.000000 term-image-0.6.1/README.md
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      268 2023-03-29 13:56:11.000000 term-image-0.6.1/pyproject.toml
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-04-30 18:57:28.145185 term-image-0.6.1/setup.cfg
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2025 2023-04-30 18:56:54.000000 term-image-0.6.1/setup.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.138519 term-image-0.6.1/src/
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.141852 term-image-0.6.1/src/term_image/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     6539 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2499 2023-03-20 16:23:42.000000 term-image-0.6.1/src/term_image/exceptions.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.141852 term-image-0.6.1/src/term_image/image/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2502 2023-03-30 03:34:36.000000 term-image-0.6.1/src/term_image/image/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     5965 2023-03-25 21:38:19.000000 term-image-0.6.1/src/term_image/image/block.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    85250 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/image/common.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    28024 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/image/iterm2.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    21887 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/image/kitty.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    28444 2023-04-22 04:14:12.000000 term-image-0.6.1/src/term_image/utils.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.145185 term-image-0.6.1/src/term_image/widget/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      305 2023-03-06 02:28:38.000000 term-image-0.6.1/src/term_image/widget/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    24532 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/widget/urwid.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.141852 term-image-0.6.1/src/term_image.egg-info/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9747 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/PKG-INFO
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      577 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/SOURCES.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)        1 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/dependency_links.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/requires.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       11 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/top_level.txt
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.145185 term-image-0.6.1/tests/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    13479 2023-03-30 13:54:35.000000 term-image-0.6.1/tests/test_iterator.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2036 2023-02-28 01:12:57.000000 term-image-0.6.1/tests/test_top_level.py
```

### Comparing `term-image-0.6.0/LICENSE` & `term-image-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/PKG-INFO` & `term-image-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-image
-Version: 0.6.0
+Version: 0.6.1
 Summary: Display images in the terminal
 Home-page: https://github.com/AnonymouX47/term-image
 Author: Toluwaleke Ogundipe
 Author-email: anonymoux47@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://term-image.readthedocs.io/
@@ -14,47 +14,52 @@
 Keywords: image,terminal,viewer,PIL,Pillow,console,xterm,library,cli,tui,ANSI,ASCII-Art,kitty,iterm2,sixel,graphics
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Android
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Terminals :: Terminal Emulators/X Terminals
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
+   <img align="right" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
+</a><br><br>
+
 <div align="center">
 
 <h1><b>Term-Image</b></h1>
 
-<p align="center">
+<p>
 <img src="https://raw.githubusercontent.com/AnonymouX47/term-image/abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png" height="200">
 </p>
 
-<p align="center">
+<p>
 <b>Display images in the terminal with Python</b>
 </p>
 
-<p align="center">
+<p>
    &#128214; <a href='https://term-image.readthedocs.io'>Docs</a>
     &#9553; 
    &#127979; <a href='https://term-image.readthedocs.io/en/stable/start/tutorial.html'>Tutorial</a>
 </p>
 
-<p align="center">
+<p>
    <a href='https://pypi.org/project/term-image/'>
       <img src='https://img.shields.io/pypi/v/term-image.svg'>
    </a>
    <a href='https://pepy.tech/project/term-image'>
       <img src="https://pepy.tech/badge/term-image/month">
    </a>
    <a href='https://pypi.org/project/term-image/'>
@@ -66,15 +71,15 @@
    <a href='https://github.com/AnonymouX47/term-image/actions/workflows/test.yml'>
       <img src='https://github.com/AnonymouX47/term-image/actions/workflows/test.yml/badge.svg'>
    </a>
    <a href='https://term-image.readthedocs.io'>
       <img src='https://readthedocs.org/projects/term-image/badge/?version=latest' alt='Documentation Status' />
    </a>
    <img src="https://img.shields.io/github/last-commit/AnonymouX47/term-image">
-   <a href="https://twitter.com/intent/tweet?text=Display%20and%20browse%20images%20in%20the%20the%20terminal&url=https://github.com/AnonymouX47/term-image&hashtags=developers,images,terminal,python">
+   <a href="https://twitter.com/intent/tweet?text=Display%20images%20in%20the%20terminal%20with%20Python&url=https://github.com/AnonymouX47/term-image&hashtags=developers,images,terminal,python">
       <img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social">
    </a>
 </p>
 
 </div>
 
 
@@ -106,21 +111,21 @@
   - support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/graphics-protocol/).
   - support for the [iTerm2 inline image protocol](https://iterm2.com/documentation-images.html).
   - full Unicode support and ANSI 24-bit color support
 
   **Plans to support a wider variety of terminal emulators are in motion** (see [Planned Features](#planned-features)).
 
 ### Steps
-The latest **stable** version can be installed from [PyPI](https://pypi.python.org/pypi/term-image) using `pip` (**recommended**):
+The latest **stable** version can be installed from [PyPI](https://pypi.org/project/term-image) with:
 
 ```shell
 pip install term-image
 ```
 
-The **development** version can be installed thus:
+The **development** version can be installed with:
 
 ```shell
 pip install git+https://github.com/AnonymouX47/term-image.git
 ```
 
 ### Supported Terminal Emulators
 See [here](https://term-image.readthedocs.io/en/stable/start/installation.html#supported-terminal-emulators) for a list of tested terminal emulators.
@@ -244,21 +249,16 @@
 
 The following projects have been (and are still) crucial to the development of this project:
 
 - [Pillow](https://python-pillow.org)
 
 ## Donate
 
-Your donation will go a long way in aiding the progress and development of this project.
-
-```
-USDT Address: TKP6d3hLcs7i5R18WRFxLe3zsPQcCBS1Ro
-Network: TRC20
-```
-I'm sincerly sorry for any inconviences that may result from the means of donation.
-
-Please bare with me, as usual means of accepting donations are not available in the region of the world where I reside.
+<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
+   <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
+</a>
 
+Your donation will go a long way in aiding the progress and development of this project.
 Thank you! 💓
 
 
 [termvisage]: https://github.com/AnonymouX47/termvisage
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 2.1 Name: term-image Version: 0.6.0 Summary: Display images
+Metadata-Version: 2.1 Name: term-image Version: 0.6.1 Summary: Display images
 in the terminal Home-page: https://github.com/AnonymouX47/term-image Author:
 Toluwaleke Ogundipe Author-email: anonymoux47@gmail.com License: MIT Project-
 URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/
 CHANGELOG.md Project-URL: Documentation, https://term-image.readthedocs.io/
 Project-URL: Funding, https://github.com/AnonymouX47/term-image#donate Project-
 URL: Source, https://github.com/AnonymouX47/term-image Project-URL: Tracker,
 https://github.com/AnonymouX47/term-image/issues Keywords:
 image,terminal,viewer,PIL,Pillow,console,xterm,library,cli,tui,ANSI,ASCII-
 Art,kitty,iterm2,sixel,graphics Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: MIT License Classifier: Intended Audience ::
 Developers Classifier: Operating System :: POSIX :: Linux Classifier: Operating
 System :: MacOS Classifier: Operating System :: Android Classifier: Operating
-System :: Microsoft :: Windows :: Windows 10 Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Multimedia :: Graphics :: Viewers Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE
+System :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Topic :: Software Development :: Libraries Classifier: Topic
+:: Terminals :: Terminal Emulators/X Terminals Classifier: Topic :: Multimedia
+:: Graphics :: Viewers Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE [Buy_Me_A_Coffee]
+
                            ****** Term-Image ******
           [https://raw.githubusercontent.com/AnonymouX47/term-image/
    abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png]
                   Display images in the terminal with Python
                                Docs ║  Tutorial
  [https://img.shields.io/pypi/v/term-image.svg] [https://pepy.tech/badge/term-
 image/month] [https://img.shields.io/pypi/pyversions/term-image.svg] [https://
@@ -40,55 +42,54 @@
 (https://term-image.readthedocs.io/en/stable/faqs.html)) - [Python](https://
 www.python.org/) >= 3.7 - A terminal emulator with **any** of the following: -
 support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/
 graphics-protocol/). - support for the [iTerm2 inline image protocol](https://
 iterm2.com/documentation-images.html). - full Unicode support and ANSI 24-bit
 color support **Plans to support a wider variety of terminal emulators are in
 motion** (see [Planned Features](#planned-features)). ### Steps The latest
-**stable** version can be installed from [PyPI](https://pypi.python.org/pypi/
-term-image) using `pip` (**recommended**): ```shell pip install term-image ```
-The **development** version can be installed thus: ```shell pip install
-git+https://github.com/AnonymouX47/term-image.git ``` ### Supported Terminal
-Emulators See [here](https://term-image.readthedocs.io/en/stable/start/
-installation.html#supported-terminal-emulators) for a list of tested terminal
-emulators. If you've tested this library on any other terminal emulator that
-meets the requirements for any of the render styles, please mention the name
-(and version) in a new thread under [this discussion](https://github.com/
-AnonymouX47/term-image/discussions/4). Also, if you have any issue with
-terminal support, you may report or check information about it in the
-discussion linked above. ## Features - Multiple image formats (basically all
-formats supported by [`PIL.Image.open()`](https://pillow.readthedocs.io/en/
-stable/handbook/image-file-formats.html)) - Multiple image source types: PIL
-image instance, local file, URL - Multiple image render styles (with automatic
-support detection) - Support for multiple terminal graphics protocols: [Kitty]
-(https://sw.kovidgoyal.net/kitty/graphics-protocol/), [iTerm2](https://
-iterm2.com/documentation-images.html) - Exposes various features of the
-protocols - Transparency support (with multiple options) - Animated image
-support (including transparent ones) - Multiple formats: GIF, WEBP, APNG (and
-possibly more) - Fully controllable iteration over rendered frames of animated
-images - Image animation with multiple parameters - Integration into various
-TUI / terminal-based output libraries. - Terminal size awareness - Automatic
-and manual image sizing - Horizontal and vertical alignment - Automatic and
-manual font ratio adjustment (to preserve image aspect ratio) - and more...
-ð ## Demo Check out this [image viewer][termvisage] based on this library.
-## Quick Start ### Creating an instance 1. Initialize with a file path:
-```python from term_image.image import from_file image = from_file("path/to/
-image.png") ``` 2. Initialize with a URL: ```python from term_image.image
-import from_url image = from_url("https://www.example.com/image.png") ``` 3.
-Initialize with a PIL (Pillow) image instance: ```python from PIL import Image
-from term_image.image import AutoImage img = Image.open("path/to/image.png")
-image = AutoImage(img) ``` ### Drawing/Displaying an Image There are two basic
-ways to draw an image to the terminal screen: 1. Using the `draw()` method:
-```python image.draw() ``` **NOTE:** `draw()` has various parameters for render
-formatting. 2. Using `print()` with an image render output: ```python print
-(image) # without formatting # OR print(f"{image:>200.^100#ffffff}") # with
-formatting ``` For animated images, only the former animates the output, the
-latter only draws the current frame. See the [tutorial](https://term-
-image.readthedocs.io/en/stable/start/tutorial.html) for a more detailed
-introduction. ## Usage
+**stable** version can be installed from [PyPI](https://pypi.org/project/term-
+image) with: ```shell pip install term-image ``` The **development** version
+can be installed with: ```shell pip install git+https://github.com/AnonymouX47/
+term-image.git ``` ### Supported Terminal Emulators See [here](https://term-
+image.readthedocs.io/en/stable/start/installation.html#supported-terminal-
+emulators) for a list of tested terminal emulators. If you've tested this
+library on any other terminal emulator that meets the requirements for any of
+the render styles, please mention the name (and version) in a new thread under
+[this discussion](https://github.com/AnonymouX47/term-image/discussions/4).
+Also, if you have any issue with terminal support, you may report or check
+information about it in the discussion linked above. ## Features - Multiple
+image formats (basically all formats supported by [`PIL.Image.open()`](https://
+pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)) - Multiple
+image source types: PIL image instance, local file, URL - Multiple image render
+styles (with automatic support detection) - Support for multiple terminal
+graphics protocols: [Kitty](https://sw.kovidgoyal.net/kitty/graphics-protocol/
+), [iTerm2](https://iterm2.com/documentation-images.html) - Exposes various
+features of the protocols - Transparency support (with multiple options) -
+Animated image support (including transparent ones) - Multiple formats: GIF,
+WEBP, APNG (and possibly more) - Fully controllable iteration over rendered
+frames of animated images - Image animation with multiple parameters -
+Integration into various TUI / terminal-based output libraries. - Terminal size
+awareness - Automatic and manual image sizing - Horizontal and vertical
+alignment - Automatic and manual font ratio adjustment (to preserve image
+aspect ratio) - and more... ð ## Demo Check out this [image viewer]
+[termvisage] based on this library. ## Quick Start ### Creating an instance 1.
+Initialize with a file path: ```python from term_image.image import from_file
+image = from_file("path/to/image.png") ``` 2. Initialize with a URL: ```python
+from term_image.image import from_url image = from_url("https://
+www.example.com/image.png") ``` 3. Initialize with a PIL (Pillow) image
+instance: ```python from PIL import Image from term_image.image import
+AutoImage img = Image.open("path/to/image.png") image = AutoImage(img) ``` ###
+Drawing/Displaying an Image There are two basic ways to draw an image to the
+terminal screen: 1. Using the `draw()` method: ```python image.draw() ```
+**NOTE:** `draw()` has various parameters for render formatting. 2. Using
+`print()` with an image render output: ```python print(image) # without
+formatting # OR print(f"{image:>200.^100#ffffff}") # with formatting ``` For
+animated images, only the former animates the output, the latter only draws the
+current frame. See the [tutorial](https://term-image.readthedocs.io/en/stable/
+start/tutorial.html) for a more detailed introduction. ## Usage
    ð§ Under Construction - There will most likely be incompatible changes
                     between minor versions of version_zero!
 **If you want to use this library in a project while it's still on version
 zero, ensure you pin the dependency version to a specific minor version e.g
 `>=0.4,<0.5`.** See the [docs](https://term-image.readthedocs.io) for the User
 Guide and API Reference. ## Contribution Please read through the [guidelines]
 (https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md). For code
@@ -100,14 +101,10 @@
 the implementation can be discussed. Hint: You can filter issues by *label* or
 simply *search* using the features's description. Thanks! ð ## Planned
 Features See [here](https://term-image.readthedocs.io/en/stable/planned.html).
 ## Known Issues See [here](https://term-image.readthedocs.io/en/stable/
 issues.html). ## FAQs See the [FAQs](https://term-image.readthedocs.io/en/
 stable/faqs.html) section of the docs. ## Credits The following projects have
 been (and are still) crucial to the development of this project: - [Pillow]
-(https://python-pillow.org) ## Donate Your donation will go a long way in
-aiding the progress and development of this project. ``` USDT Address:
-TKP6d3hLcs7i5R18WRFxLe3zsPQcCBS1Ro Network: TRC20 ``` I'm sincerly sorry for
-any inconviences that may result from the means of donation. Please bare with
-me, as usual means of accepting donations are not available in the region of
-the world where I reside. Thank you! ð [termvisage]: https://github.com/
-AnonymouX47/termvisage
+(https://python-pillow.org) ## Donate [Buy_Me_A_Coffee] Your donation will go a
+long way in aiding the progress and development of this project. Thank you!
+ð [termvisage]: https://github.com/AnonymouX47/termvisage
```

### Comparing `term-image-0.6.0/README.md` & `term-image-0.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
+   <img align="right" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
+</a><br><br>
+
 <div align="center">
 
 <h1><b>Term-Image</b></h1>
 
-<p align="center">
+<p>
 <img src="https://raw.githubusercontent.com/AnonymouX47/term-image/abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png" height="200">
 </p>
 
-<p align="center">
+<p>
 <b>Display images in the terminal with Python</b>
 </p>
 
-<p align="center">
+<p>
    &#128214; <a href='https://term-image.readthedocs.io'>Docs</a>
     &#9553; 
    &#127979; <a href='https://term-image.readthedocs.io/en/stable/start/tutorial.html'>Tutorial</a>
 </p>
 
-<p align="center">
+<p>
    <a href='https://pypi.org/project/term-image/'>
       <img src='https://img.shields.io/pypi/v/term-image.svg'>
    </a>
    <a href='https://pepy.tech/project/term-image'>
       <img src="https://pepy.tech/badge/term-image/month">
    </a>
    <a href='https://pypi.org/project/term-image/'>
@@ -32,15 +36,15 @@
    <a href='https://github.com/AnonymouX47/term-image/actions/workflows/test.yml'>
       <img src='https://github.com/AnonymouX47/term-image/actions/workflows/test.yml/badge.svg'>
    </a>
    <a href='https://term-image.readthedocs.io'>
       <img src='https://readthedocs.org/projects/term-image/badge/?version=latest' alt='Documentation Status' />
    </a>
    <img src="https://img.shields.io/github/last-commit/AnonymouX47/term-image">
-   <a href="https://twitter.com/intent/tweet?text=Display%20and%20browse%20images%20in%20the%20the%20terminal&url=https://github.com/AnonymouX47/term-image&hashtags=developers,images,terminal,python">
+   <a href="https://twitter.com/intent/tweet?text=Display%20images%20in%20the%20terminal%20with%20Python&url=https://github.com/AnonymouX47/term-image&hashtags=developers,images,terminal,python">
       <img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social">
    </a>
 </p>
 
 </div>
 
 
@@ -72,21 +76,21 @@
   - support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/graphics-protocol/).
   - support for the [iTerm2 inline image protocol](https://iterm2.com/documentation-images.html).
   - full Unicode support and ANSI 24-bit color support
 
   **Plans to support a wider variety of terminal emulators are in motion** (see [Planned Features](#planned-features)).
 
 ### Steps
-The latest **stable** version can be installed from [PyPI](https://pypi.python.org/pypi/term-image) using `pip` (**recommended**):
+The latest **stable** version can be installed from [PyPI](https://pypi.org/project/term-image) with:
 
 ```shell
 pip install term-image
 ```
 
-The **development** version can be installed thus:
+The **development** version can be installed with:
 
 ```shell
 pip install git+https://github.com/AnonymouX47/term-image.git
 ```
 
 ### Supported Terminal Emulators
 See [here](https://term-image.readthedocs.io/en/stable/start/installation.html#supported-terminal-emulators) for a list of tested terminal emulators.
@@ -210,21 +214,16 @@
 
 The following projects have been (and are still) crucial to the development of this project:
 
 - [Pillow](https://python-pillow.org)
 
 ## Donate
 
-Your donation will go a long way in aiding the progress and development of this project.
-
-```
-USDT Address: TKP6d3hLcs7i5R18WRFxLe3zsPQcCBS1Ro
-Network: TRC20
-```
-I'm sincerly sorry for any inconviences that may result from the means of donation.
-
-Please bare with me, as usual means of accepting donations are not available in the region of the world where I reside.
+<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
+   <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
+</a>
 
+Your donation will go a long way in aiding the progress and development of this project.
 Thank you! 💓
 
 
 [termvisage]: https://github.com/AnonymouX47/termvisage
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
+[Buy_Me_A_Coffee]
+
                            ****** Term-Image ******
           [https://raw.githubusercontent.com/AnonymouX47/term-image/
    abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png]
                   Display images in the terminal with Python
                                Docs ║  Tutorial
  [https://img.shields.io/pypi/v/term-image.svg] [https://pepy.tech/badge/term-
 image/month] [https://img.shields.io/pypi/pyversions/term-image.svg] [https://
@@ -19,55 +21,54 @@
 (https://term-image.readthedocs.io/en/stable/faqs.html)) - [Python](https://
 www.python.org/) >= 3.7 - A terminal emulator with **any** of the following: -
 support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/
 graphics-protocol/). - support for the [iTerm2 inline image protocol](https://
 iterm2.com/documentation-images.html). - full Unicode support and ANSI 24-bit
 color support **Plans to support a wider variety of terminal emulators are in
 motion** (see [Planned Features](#planned-features)). ### Steps The latest
-**stable** version can be installed from [PyPI](https://pypi.python.org/pypi/
-term-image) using `pip` (**recommended**): ```shell pip install term-image ```
-The **development** version can be installed thus: ```shell pip install
-git+https://github.com/AnonymouX47/term-image.git ``` ### Supported Terminal
-Emulators See [here](https://term-image.readthedocs.io/en/stable/start/
-installation.html#supported-terminal-emulators) for a list of tested terminal
-emulators. If you've tested this library on any other terminal emulator that
-meets the requirements for any of the render styles, please mention the name
-(and version) in a new thread under [this discussion](https://github.com/
-AnonymouX47/term-image/discussions/4). Also, if you have any issue with
-terminal support, you may report or check information about it in the
-discussion linked above. ## Features - Multiple image formats (basically all
-formats supported by [`PIL.Image.open()`](https://pillow.readthedocs.io/en/
-stable/handbook/image-file-formats.html)) - Multiple image source types: PIL
-image instance, local file, URL - Multiple image render styles (with automatic
-support detection) - Support for multiple terminal graphics protocols: [Kitty]
-(https://sw.kovidgoyal.net/kitty/graphics-protocol/), [iTerm2](https://
-iterm2.com/documentation-images.html) - Exposes various features of the
-protocols - Transparency support (with multiple options) - Animated image
-support (including transparent ones) - Multiple formats: GIF, WEBP, APNG (and
-possibly more) - Fully controllable iteration over rendered frames of animated
-images - Image animation with multiple parameters - Integration into various
-TUI / terminal-based output libraries. - Terminal size awareness - Automatic
-and manual image sizing - Horizontal and vertical alignment - Automatic and
-manual font ratio adjustment (to preserve image aspect ratio) - and more...
-ð ## Demo Check out this [image viewer][termvisage] based on this library.
-## Quick Start ### Creating an instance 1. Initialize with a file path:
-```python from term_image.image import from_file image = from_file("path/to/
-image.png") ``` 2. Initialize with a URL: ```python from term_image.image
-import from_url image = from_url("https://www.example.com/image.png") ``` 3.
-Initialize with a PIL (Pillow) image instance: ```python from PIL import Image
-from term_image.image import AutoImage img = Image.open("path/to/image.png")
-image = AutoImage(img) ``` ### Drawing/Displaying an Image There are two basic
-ways to draw an image to the terminal screen: 1. Using the `draw()` method:
-```python image.draw() ``` **NOTE:** `draw()` has various parameters for render
-formatting. 2. Using `print()` with an image render output: ```python print
-(image) # without formatting # OR print(f"{image:>200.^100#ffffff}") # with
-formatting ``` For animated images, only the former animates the output, the
-latter only draws the current frame. See the [tutorial](https://term-
-image.readthedocs.io/en/stable/start/tutorial.html) for a more detailed
-introduction. ## Usage
+**stable** version can be installed from [PyPI](https://pypi.org/project/term-
+image) with: ```shell pip install term-image ``` The **development** version
+can be installed with: ```shell pip install git+https://github.com/AnonymouX47/
+term-image.git ``` ### Supported Terminal Emulators See [here](https://term-
+image.readthedocs.io/en/stable/start/installation.html#supported-terminal-
+emulators) for a list of tested terminal emulators. If you've tested this
+library on any other terminal emulator that meets the requirements for any of
+the render styles, please mention the name (and version) in a new thread under
+[this discussion](https://github.com/AnonymouX47/term-image/discussions/4).
+Also, if you have any issue with terminal support, you may report or check
+information about it in the discussion linked above. ## Features - Multiple
+image formats (basically all formats supported by [`PIL.Image.open()`](https://
+pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)) - Multiple
+image source types: PIL image instance, local file, URL - Multiple image render
+styles (with automatic support detection) - Support for multiple terminal
+graphics protocols: [Kitty](https://sw.kovidgoyal.net/kitty/graphics-protocol/
+), [iTerm2](https://iterm2.com/documentation-images.html) - Exposes various
+features of the protocols - Transparency support (with multiple options) -
+Animated image support (including transparent ones) - Multiple formats: GIF,
+WEBP, APNG (and possibly more) - Fully controllable iteration over rendered
+frames of animated images - Image animation with multiple parameters -
+Integration into various TUI / terminal-based output libraries. - Terminal size
+awareness - Automatic and manual image sizing - Horizontal and vertical
+alignment - Automatic and manual font ratio adjustment (to preserve image
+aspect ratio) - and more... ð ## Demo Check out this [image viewer]
+[termvisage] based on this library. ## Quick Start ### Creating an instance 1.
+Initialize with a file path: ```python from term_image.image import from_file
+image = from_file("path/to/image.png") ``` 2. Initialize with a URL: ```python
+from term_image.image import from_url image = from_url("https://
+www.example.com/image.png") ``` 3. Initialize with a PIL (Pillow) image
+instance: ```python from PIL import Image from term_image.image import
+AutoImage img = Image.open("path/to/image.png") image = AutoImage(img) ``` ###
+Drawing/Displaying an Image There are two basic ways to draw an image to the
+terminal screen: 1. Using the `draw()` method: ```python image.draw() ```
+**NOTE:** `draw()` has various parameters for render formatting. 2. Using
+`print()` with an image render output: ```python print(image) # without
+formatting # OR print(f"{image:>200.^100#ffffff}") # with formatting ``` For
+animated images, only the former animates the output, the latter only draws the
+current frame. See the [tutorial](https://term-image.readthedocs.io/en/stable/
+start/tutorial.html) for a more detailed introduction. ## Usage
    ð§ Under Construction - There will most likely be incompatible changes
                     between minor versions of version_zero!
 **If you want to use this library in a project while it's still on version
 zero, ensure you pin the dependency version to a specific minor version e.g
 `>=0.4,<0.5`.** See the [docs](https://term-image.readthedocs.io) for the User
 Guide and API Reference. ## Contribution Please read through the [guidelines]
 (https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md). For code
@@ -79,14 +80,10 @@
 the implementation can be discussed. Hint: You can filter issues by *label* or
 simply *search* using the features's description. Thanks! ð ## Planned
 Features See [here](https://term-image.readthedocs.io/en/stable/planned.html).
 ## Known Issues See [here](https://term-image.readthedocs.io/en/stable/
 issues.html). ## FAQs See the [FAQs](https://term-image.readthedocs.io/en/
 stable/faqs.html) section of the docs. ## Credits The following projects have
 been (and are still) crucial to the development of this project: - [Pillow]
-(https://python-pillow.org) ## Donate Your donation will go a long way in
-aiding the progress and development of this project. ``` USDT Address:
-TKP6d3hLcs7i5R18WRFxLe3zsPQcCBS1Ro Network: TRC20 ``` I'm sincerly sorry for
-any inconviences that may result from the means of donation. Please bare with
-me, as usual means of accepting donations are not available in the region of
-the world where I reside. Thank you! ð [termvisage]: https://github.com/
-AnonymouX47/termvisage
+(https://python-pillow.org) ## Donate [Buy_Me_A_Coffee] Your donation will go a
+long way in aiding the progress and development of this project. Thank you!
+ð [termvisage]: https://github.com/AnonymouX47/termvisage
```

### Comparing `term-image-0.6.0/setup.py` & `term-image-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Android",
-    "Operating System :: Microsoft :: Windows :: Windows 10",
+    "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries",
+    "Topic :: Terminals :: Terminal Emulators/X Terminals",
     "Topic :: Multimedia :: Graphics :: Viewers",
 ]
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="term-image",
-    version="0.6.0",
+    version="0.6.1",
     author="Toluwaleke Ogundipe",
     author_email="anonymoux47@gmail.com",
     url="https://github.com/AnonymouX47/term-image",
     description="Display images in the terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `term-image-0.6.0/src/term_image/__init__.py` & `term-image-0.6.1/src/term_image/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from operator import truediv
 from typing import Optional, Union
 
 from . import utils
 from .exceptions import TermImageError
 from .utils import get_cell_size
 
-version_info = (0, 6, 0)
+version_info = (0, 6, 1)
 
 # Follows https://semver.org/spec/v2.0.0.html
 __version__ = ".".join(map(str, version_info[:3]))
 if version_info[3:]:
     __version__ += "-" + ".".join(map(str, version_info[3:]))
 
 #: Default timeout for :ref:`terminal-queries`
```

### Comparing `term-image-0.6.0/src/term_image/exceptions.py` & `term-image-0.6.1/src/term_image/exceptions.py`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/src/term_image/image/__init__.py` & `term-image-0.6.1/src/term_image/image/__init__.py`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/src/term_image/image/block.py` & `term-image-0.6.1/src/term_image/image/block.py`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/src/term_image/image/common.py` & `term-image-0.6.1/src/term_image/image/common.py`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/src/term_image/image/iterm2.py` & `term-image-0.6.1/src/term_image/image/iterm2.py`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/src/term_image/image/kitty.py` & `term-image-0.6.1/src/term_image/image/kitty.py`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/src/term_image/utils.py` & `term-image-0.6.1/src/term_image/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -212,42 +212,52 @@
     """Synchronizes access to the :term:`active terminal`.
 
     Args:
         func: The function to be wrapped.
 
     When a decorated function is called, a re-entrant lock is acquired by the current
     process or thread and released after the call, such that any other decorated
-    function called within another thread or subprocess has to wait till the lock is
+    function called within another thread or subprocess waits until the lock is
     fully released (i.e has been released as many times as acquired) by the current
     process or thread.
 
     NOTE:
-        It automatically works across parent-/sub-processes, started directly or
-        indirectly via :py:class:`multiprocessing.Process` (or a subclass of it) and
-        their threads.
-
-    IMPORTANT:
-        It only works if :py:mod:`multiprocessing.synchronize` is supported on the host
-        platform.  If not supported, a warning is issued when starting a subprocess.
+        It works across parent-/sub-processes, started directly or indirectly via
+        :py:class:`multiprocessing.Process` (or a subclass of it), and their threads,
+        provided :py:mod:`multiprocessing.synchronize` is supported on the host
+        platform. Otherwise, a warning is issued when starting a subprocess.
+
+    WARNING:
+        If :py:mod:`multiprocessing.synchronize` is supported and a subprocess is
+        started within a call (possibly recursive) to a decorated function, the thread
+        in which that occurs will be out of sync until that call returns.
+        Hence, avoid starting a subprocess within a decorated function.
     """
 
     @wraps(func)
     def lock_tty_wrapper(*args, **kwargs):
-        with _tty_lock:
+        # If a thread reaches this point while the lock is being changed
+        # (the old lock has been acquired but hasn't been changed), after the lock has
+        # been changed and the former lock is released, the waiting thread will acquire
+        # the old lock making it to be out of sync.
+        # Hence the second expression, which allows such a thread to acquire the new
+        # lock and be in sync.
+        # NB: Multiple expressions are processed as multiple nested with statements.
+        with _tty_lock, _tty_lock:
             # logging.debug(f"{func.__name__} acquired TTY lock", stacklevel=3)
             return func(*args, **kwargs)
 
     if func.__doc__ is not None:
         lock_tty_wrapper.__doc__ = (
             func.__doc__.rstrip()
             + """
 
-        IMPORTANT:
-            Synchronized with :py:func:`~term_image.utils.lock_tty`.
-        """
+    IMPORTANT:
+        Synchronized with :py:func:`term_image.utils.lock_tty`.
+    """
         )
 
     return lock_tty_wrapper
 
 
 @no_redecorate
 def terminal_size_cached(func: FunctionType) -> FunctionType:
@@ -371,15 +381,16 @@
     Returns:
         For each color:
 
         * an RGB 3-tuple, if *hex* is ``False``
         * an RGB hex string if *hex* is ``True``
         * ``None`` if undetermined
     """
-    with _tty_lock:  # All of the terminal's reply isn't read in `query_terminal()`
+    # The terminal's response to the queries is not read all at once
+    with _tty_lock, _tty_lock:  # See the comment in `lock_tty_wrapper()`
         response = query_terminal(
             # Not all terminals (e.g VTE-based) support multiple queries in one escape
             # sequence, hence the repetition of OSC ... ST
             f"{OSC}10;?{ST}{OSC}11;?{ST}{CSI}c".encode(),
             # The response might contain a "c"; can't stop reading at "c"
             lambda s: not s.endswith(CSI_b),
         )
@@ -403,15 +414,16 @@
 def get_terminal_name_version() -> Tuple[Optional[str], Optional[str]]:
     """Returns the name and version of the :term:`active terminal`, if available.
 
     Returns:
         A 2-tuple, ``(name, version)``. If either is not available, returns ``None``
         in its place.
     """
-    with _tty_lock:  # the terminal's response to the query is not read all at once
+    # The terminal's response to the queries is not read all at once
+    with _tty_lock, _tty_lock:  # See the comment in `lock_tty_wrapper()`
         # Terminal name/version query + terminal attribute query
         # The latter is to speed up the entire query since most (if not all)
         # terminals should support it and most terminals treat queries as FIFO
         response = query_terminal(
             f"{CSI}>q{CSI}c".encode(),
             # The response might contain a "c"; can't stop reading at "c"
             lambda s: not s.endswith(CSI_b),
@@ -465,15 +477,22 @@
 
     The speed of this implementation is almost entirely dependent on the terminal; the
     method it supports and its response time if it has to be queried.
 
     Returns ``None`` if the size couldn't be gotten in time or the terminal lacks
     support.
     """
-    with _win_size_lock:
+    # If a thread reaches this point while the lock is being changed
+    # (the old lock has been acquired but hasn't been changed), after the lock has
+    # been changed and the former lock is released, the waiting thread will acquire
+    # the old lock making it to be out of sync.
+    # Hence the second expression, which allows such a thread to acquire the new
+    # lock and be in sync.
+    # NB: Multiple expressions are processed as multiple nested with statements.
+    with _win_size_lock, _win_size_lock:
         ts = get_terminal_size()
         if ts == tuple(_win_size_cache[:2]):
             size = tuple(_win_size_cache[2:])
             return None if 0 in size else size
 
         # First try ioctl
         size = None
@@ -644,16 +663,16 @@
 def read_tty_all() -> bytes:
     """Reads all available input directly from the :term:`active terminal` **without
     blocking**.
 
     Returns:
         The input read.
 
-    HINT:
-        Synchronized with :py:func:`lock_tty`.
+    IMPORTANT:
+        Synchronized with :py:func:`term_image.utils.lock_tty`.
     """
     return read_tty()
 
 
 @unix_tty_only
 @lock_tty
 def write_tty(data: bytes) -> None:
@@ -674,20 +693,22 @@
     # One hex char -> 4 bits
     return tuple(int(x, 16) * 255 // ((1 << (len(x) * 4)) - 1) for x in spec.split("/"))
 
 
 def _process_start_wrapper(self, *args, **kwargs):
     global _tty_lock, _win_size_cache, _win_size_lock
 
-    # Ensure it's not acquired by another process/thread before changing it.
-    # The only way this can be countered is if the owner thread is the
-    # one starting a process, which is very unlikely within a function meant
-    # for input/output :|
+    # Ensure a lock is not acquired by another process/thread before changing it.
+    # The only case in which this is useless is when the owner thread is the
+    # one starting a process. In such a situation, the owner thread will be partially
+    # (may acquire the new lock in a nested call while still holding the old lock)
+    # out of sync until it has fully released the old lock.
+
     with _tty_lock:
-        if isinstance(_tty_lock, type(RLock())):
+        if isinstance(_tty_lock, _rlock_type):
             try:
                 self._tty_lock = _tty_lock = mp_RLock()
             except ImportError:
                 self._tty_lock = None
                 warnings.warn(
                     "Multi-process synchronization is not supported on this platform!\n"
                     "Hence, if any subprocess will be writing/reading to/from the "
@@ -701,35 +722,34 @@
                     "any subprocess) if not using any of the affected features.",
                     TermImageWarning,
                 )
         else:
             self._tty_lock = _tty_lock
 
     with _win_size_lock:
-        if isinstance(_win_size_lock, type(RLock())):
+        if isinstance(_win_size_lock, _rlock_type):
             try:
                 self._win_size_cache = _win_size_cache = Array("i", _win_size_cache)
                 _win_size_lock = _win_size_cache.get_lock()
             except ImportError:
                 self._win_size_cache = None
         else:
             self._win_size_cache = _win_size_cache
 
     return _process_start_wrapper.__wrapped__(self, *args, **kwargs)
 
 
-def _process_run_wrapper(self, *args, set_tty_lock: bool = True, **kwargs):
+def _process_run_wrapper(self, *args, **kwargs):
     global _tty_lock, _win_size_cache, _win_size_lock
 
-    if set_tty_lock:
-        if self._tty_lock:
-            _tty_lock = self._tty_lock
-        if self._win_size_cache:
-            _win_size_cache = self._win_size_cache
-            _win_size_lock = _win_size_cache.get_lock()
+    if self._tty_lock:
+        _tty_lock = self._tty_lock
+    if self._win_size_cache:
+        _win_size_cache = self._win_size_cache
+        _win_size_lock = _win_size_cache.get_lock()
 
     return _process_run_wrapper.__wrapped__(self, *args, **kwargs)
 
 
 RGB_SPEC = re.compile(r"\033](\d+);rgb:([\da-fA-F/]+)\033\\", re.ASCII)
 WIN_SIZE = re.compile(r"\033\[4;(\d+);(\d+)t", re.ASCII)
 NAME_VERSION = re.compile(r"\033P>\|(\w+)[( ]([^)\033]+)\)?\033\\", re.ASCII)
@@ -765,14 +785,15 @@
 _query_timeout = 0.1
 _queries_enabled: bool = True
 _swap_win_size: bool = False
 _tty: Optional[int] = None
 _tty_lock = RLock()
 _win_size_cache = [0] * 4
 _win_size_lock = RLock()
+_rlock_type = type(_tty_lock)
 
 if OS_IS_UNIX:
     for stream in ("out", "in", "err"):  # In order of priority
         try:
             _tty = os.ttyname(getattr(sys, f"__std{stream}__").fileno())
             break
         except (OSError, AttributeError):
```

### Comparing `term-image-0.6.0/src/term_image/widget/urwid.py` & `term-image-0.6.1/src/term_image/widget/urwid.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,33 +29,38 @@
         image: The image to be rendered by the widget.
         format_spec: :ref:`Render format specifier <format-spec>`. Padding width and
           height are ignored.
         upscale: If ``True``, the image will be upscaled to fit maximally within the
           available size, if neccessary, while still preserving the aspect ratio.
           Otherwise, the image is never upscaled.
 
+    Raises:
+        TypeError: An argument is of an inappropriate type.
+        ValueError: An argument is of an appropriate type but has an
+          unexpected/invalid value.
+        term_image.exceptions.StyleError: Invalid style-specific format specifier.
+        term_image.exceptions.UrwidImageError: Too many image widgets rendering images
+          with the *kitty* render style.
+
     | Any ample space in the widget's render size is filled with spaces.
     | For animated images, the current frame (at render-time) is rendered.
 
     TIP:
         If *image* is of a :ref:`graphics-based <graphics-based>` render style and the
         widget is being used as or within a **flow** widget, with overlays or in any
         other case where the canvas will require vertical trimming, make sure to use a
         render method that splits images across lines such as the **LINES** render
         method for *kitty* and *iterm2* render styles.
 
     NOTE:
-        The `z_index` style-specific parameter for the
-        :py:class:`kitty <term_image.image.KittyImage>` render style is ignored as this
-        is used internally.
-
-    WARNING:
-        If *image* is of the *iterm2* render style, prevent the widget from reaching the
-        **last line** of the screen as **Wezterm** doesn't work properly in this case
-        (it scrolls the screen).
+        * The `z-index` style-specific format spec field for
+          :py:class:`~term_image.image.KittyImage` is ignored as this is used
+          internally.
+        * A **maximum** of ``2**32 - 2`` instances initialized with
+          :py:class:`~term_image.image.KittyImage` instances may exist at the same time.
 
     IMPORTANT:
         This is defined if and only if the ``urwid`` package is available.
     """
 
     _sizing = frozenset((urwid.BOX, urwid.FLOW))
     ignore_focus = True
@@ -105,19 +110,16 @@
             # better on Konsole as it reduces/eliminates flicker.
             if KittyImage._TERM != "konsole":
                 # To clear directly overlapped images when urwid redraws a line without
                 # a change in image position
                 style_args["blend"] = False
 
     def __del__(self) -> None:
-        try:
-            if isinstance(self._ti_image, KittyImage):
-                type(self)._ti_free_z_indexes.add(self._ti_z_index)
-        except AttributeError:  # Object initialization most likely failed
-            pass
+        if hasattr(self, "_ti_z_index"):
+            __class__._ti_free_z_indexes.add(self._ti_z_index)
 
     image = property(
         lambda self: self._ti_image,
         doc="""
         The image rendered by the widget.
 
         :type: BaseImage
@@ -204,31 +206,34 @@
     @classmethod
     def set_error_placeholder(cls, widget: Optional[urwid.Widget]) -> None:
         """Sets the widget to be rendered in place of an image when rendering fails.
 
         Args:
             widget: The placholder widget or ``None`` to remove the placeholder.
 
+        Raises:
+            TypeError: *widget* is not an urwid widget.
+
         If set, any exception raised during rendering is **suppressed** and the
         placeholder is rendered in place of the image.
         """
         if not isinstance(widget, urwid.Widget):
             raise TypeError("Invalid type for 'widget' (got: {type(widget).__name__})")
 
         cls._ti_error_placeholder = widget
 
-    @classmethod
-    def _ti_get_z_index(cls) -> int:
-        if cls._ti_free_z_indexes:
-            return cls._ti_free_z_indexes.pop()
+    @staticmethod
+    def _ti_get_z_index() -> int:
+        if __class__._ti_free_z_indexes:
+            return __class__._ti_free_z_indexes.pop()
 
-        z_index = cls._ti_next_z_index
+        z_index = __class__._ti_next_z_index
         if z_index == 2**31:
             raise UrwidImageError("Too many image widgets with the kitty render style")
-        cls._ti_next_z_index = -z_index if z_index > 0 else -z_index + 1
+        __class__._ti_next_z_index = -z_index if z_index > 0 else -z_index + 1
 
         return z_index
 
 
 class UrwidImageCanvas(urwid.Canvas):
     """Image canvas for the urwid TUI framework.
 
@@ -512,29 +517,35 @@
 class UrwidImageScreen(urwid.raw_display.Screen):
     """A screen that supports drawing images.
 
     It monitors images of some :ref:`graphics-based <graphics-based>` render styles
     and clears them off the screen when necessary (e.g at startup, when scrolling,
     upon terminal resize and at exit).
 
-    It also synchronizes output on terminal emulators that support the feature to
-    reduce/eliminate image flickering/tearing.
-
     See the baseclass for further description.
 
     IMPORTANT:
         This is defined if and only if the ``urwid`` package is available.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._ti_screen_canv = None
         self._ti_image_cviews = frozenset()
 
+    # `@lock_tty` prevents queries during a synced update.
+    # Otherwise, responses would be delayed until the synced update ends and that might
+    # be after the query has timed out.
+    @lock_tty
     def draw_screen(self, maxres, canvas):
+        """See the description of the baseclass' method.
+
+        Synchronizes output on terminal emulators that support the feature to
+        reduce/eliminate image flickering and screen tearing.
+        """
         self.write(BEGIN_SYNCED_UPDATE)
         try:
             if canvas is not self._ti_screen_canv:
                 self._ti_screen_canv = canvas
                 self._ti_clear_images()
             return super().draw_screen(maxres, canvas)
         finally:
```

### Comparing `term-image-0.6.0/src/term_image.egg-info/PKG-INFO` & `term-image-0.6.1/src/term_image.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-image
-Version: 0.6.0
+Version: 0.6.1
 Summary: Display images in the terminal
 Home-page: https://github.com/AnonymouX47/term-image
 Author: Toluwaleke Ogundipe
 Author-email: anonymoux47@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://term-image.readthedocs.io/
@@ -14,47 +14,52 @@
 Keywords: image,terminal,viewer,PIL,Pillow,console,xterm,library,cli,tui,ANSI,ASCII-Art,kitty,iterm2,sixel,graphics
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Android
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Terminals :: Terminal Emulators/X Terminals
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
+   <img align="right" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
+</a><br><br>
+
 <div align="center">
 
 <h1><b>Term-Image</b></h1>
 
-<p align="center">
+<p>
 <img src="https://raw.githubusercontent.com/AnonymouX47/term-image/abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png" height="200">
 </p>
 
-<p align="center">
+<p>
 <b>Display images in the terminal with Python</b>
 </p>
 
-<p align="center">
+<p>
    &#128214; <a href='https://term-image.readthedocs.io'>Docs</a>
     &#9553; 
    &#127979; <a href='https://term-image.readthedocs.io/en/stable/start/tutorial.html'>Tutorial</a>
 </p>
 
-<p align="center">
+<p>
    <a href='https://pypi.org/project/term-image/'>
       <img src='https://img.shields.io/pypi/v/term-image.svg'>
    </a>
    <a href='https://pepy.tech/project/term-image'>
       <img src="https://pepy.tech/badge/term-image/month">
    </a>
    <a href='https://pypi.org/project/term-image/'>
@@ -66,15 +71,15 @@
    <a href='https://github.com/AnonymouX47/term-image/actions/workflows/test.yml'>
       <img src='https://github.com/AnonymouX47/term-image/actions/workflows/test.yml/badge.svg'>
    </a>
    <a href='https://term-image.readthedocs.io'>
       <img src='https://readthedocs.org/projects/term-image/badge/?version=latest' alt='Documentation Status' />
    </a>
    <img src="https://img.shields.io/github/last-commit/AnonymouX47/term-image">
-   <a href="https://twitter.com/intent/tweet?text=Display%20and%20browse%20images%20in%20the%20the%20terminal&url=https://github.com/AnonymouX47/term-image&hashtags=developers,images,terminal,python">
+   <a href="https://twitter.com/intent/tweet?text=Display%20images%20in%20the%20terminal%20with%20Python&url=https://github.com/AnonymouX47/term-image&hashtags=developers,images,terminal,python">
       <img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social">
    </a>
 </p>
 
 </div>
 
 
@@ -106,21 +111,21 @@
   - support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/graphics-protocol/).
   - support for the [iTerm2 inline image protocol](https://iterm2.com/documentation-images.html).
   - full Unicode support and ANSI 24-bit color support
 
   **Plans to support a wider variety of terminal emulators are in motion** (see [Planned Features](#planned-features)).
 
 ### Steps
-The latest **stable** version can be installed from [PyPI](https://pypi.python.org/pypi/term-image) using `pip` (**recommended**):
+The latest **stable** version can be installed from [PyPI](https://pypi.org/project/term-image) with:
 
 ```shell
 pip install term-image
 ```
 
-The **development** version can be installed thus:
+The **development** version can be installed with:
 
 ```shell
 pip install git+https://github.com/AnonymouX47/term-image.git
 ```
 
 ### Supported Terminal Emulators
 See [here](https://term-image.readthedocs.io/en/stable/start/installation.html#supported-terminal-emulators) for a list of tested terminal emulators.
@@ -244,21 +249,16 @@
 
 The following projects have been (and are still) crucial to the development of this project:
 
 - [Pillow](https://python-pillow.org)
 
 ## Donate
 
-Your donation will go a long way in aiding the progress and development of this project.
-
-```
-USDT Address: TKP6d3hLcs7i5R18WRFxLe3zsPQcCBS1Ro
-Network: TRC20
-```
-I'm sincerly sorry for any inconviences that may result from the means of donation.
-
-Please bare with me, as usual means of accepting donations are not available in the region of the world where I reside.
+<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
+   <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
+</a>
 
+Your donation will go a long way in aiding the progress and development of this project.
 Thank you! 💓
 
 
 [termvisage]: https://github.com/AnonymouX47/termvisage
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 2.1 Name: term-image Version: 0.6.0 Summary: Display images
+Metadata-Version: 2.1 Name: term-image Version: 0.6.1 Summary: Display images
 in the terminal Home-page: https://github.com/AnonymouX47/term-image Author:
 Toluwaleke Ogundipe Author-email: anonymoux47@gmail.com License: MIT Project-
 URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/
 CHANGELOG.md Project-URL: Documentation, https://term-image.readthedocs.io/
 Project-URL: Funding, https://github.com/AnonymouX47/term-image#donate Project-
 URL: Source, https://github.com/AnonymouX47/term-image Project-URL: Tracker,
 https://github.com/AnonymouX47/term-image/issues Keywords:
 image,terminal,viewer,PIL,Pillow,console,xterm,library,cli,tui,ANSI,ASCII-
 Art,kitty,iterm2,sixel,graphics Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: MIT License Classifier: Intended Audience ::
 Developers Classifier: Operating System :: POSIX :: Linux Classifier: Operating
 System :: MacOS Classifier: Operating System :: Android Classifier: Operating
-System :: Microsoft :: Windows :: Windows 10 Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Multimedia :: Graphics :: Viewers Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE
+System :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Topic :: Software Development :: Libraries Classifier: Topic
+:: Terminals :: Terminal Emulators/X Terminals Classifier: Topic :: Multimedia
+:: Graphics :: Viewers Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE [Buy_Me_A_Coffee]
+
                            ****** Term-Image ******
           [https://raw.githubusercontent.com/AnonymouX47/term-image/
    abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png]
                   Display images in the terminal with Python
                                Docs ║  Tutorial
  [https://img.shields.io/pypi/v/term-image.svg] [https://pepy.tech/badge/term-
 image/month] [https://img.shields.io/pypi/pyversions/term-image.svg] [https://
@@ -40,55 +42,54 @@
 (https://term-image.readthedocs.io/en/stable/faqs.html)) - [Python](https://
 www.python.org/) >= 3.7 - A terminal emulator with **any** of the following: -
 support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/
 graphics-protocol/). - support for the [iTerm2 inline image protocol](https://
 iterm2.com/documentation-images.html). - full Unicode support and ANSI 24-bit
 color support **Plans to support a wider variety of terminal emulators are in
 motion** (see [Planned Features](#planned-features)). ### Steps The latest
-**stable** version can be installed from [PyPI](https://pypi.python.org/pypi/
-term-image) using `pip` (**recommended**): ```shell pip install term-image ```
-The **development** version can be installed thus: ```shell pip install
-git+https://github.com/AnonymouX47/term-image.git ``` ### Supported Terminal
-Emulators See [here](https://term-image.readthedocs.io/en/stable/start/
-installation.html#supported-terminal-emulators) for a list of tested terminal
-emulators. If you've tested this library on any other terminal emulator that
-meets the requirements for any of the render styles, please mention the name
-(and version) in a new thread under [this discussion](https://github.com/
-AnonymouX47/term-image/discussions/4). Also, if you have any issue with
-terminal support, you may report or check information about it in the
-discussion linked above. ## Features - Multiple image formats (basically all
-formats supported by [`PIL.Image.open()`](https://pillow.readthedocs.io/en/
-stable/handbook/image-file-formats.html)) - Multiple image source types: PIL
-image instance, local file, URL - Multiple image render styles (with automatic
-support detection) - Support for multiple terminal graphics protocols: [Kitty]
-(https://sw.kovidgoyal.net/kitty/graphics-protocol/), [iTerm2](https://
-iterm2.com/documentation-images.html) - Exposes various features of the
-protocols - Transparency support (with multiple options) - Animated image
-support (including transparent ones) - Multiple formats: GIF, WEBP, APNG (and
-possibly more) - Fully controllable iteration over rendered frames of animated
-images - Image animation with multiple parameters - Integration into various
-TUI / terminal-based output libraries. - Terminal size awareness - Automatic
-and manual image sizing - Horizontal and vertical alignment - Automatic and
-manual font ratio adjustment (to preserve image aspect ratio) - and more...
-ð ## Demo Check out this [image viewer][termvisage] based on this library.
-## Quick Start ### Creating an instance 1. Initialize with a file path:
-```python from term_image.image import from_file image = from_file("path/to/
-image.png") ``` 2. Initialize with a URL: ```python from term_image.image
-import from_url image = from_url("https://www.example.com/image.png") ``` 3.
-Initialize with a PIL (Pillow) image instance: ```python from PIL import Image
-from term_image.image import AutoImage img = Image.open("path/to/image.png")
-image = AutoImage(img) ``` ### Drawing/Displaying an Image There are two basic
-ways to draw an image to the terminal screen: 1. Using the `draw()` method:
-```python image.draw() ``` **NOTE:** `draw()` has various parameters for render
-formatting. 2. Using `print()` with an image render output: ```python print
-(image) # without formatting # OR print(f"{image:>200.^100#ffffff}") # with
-formatting ``` For animated images, only the former animates the output, the
-latter only draws the current frame. See the [tutorial](https://term-
-image.readthedocs.io/en/stable/start/tutorial.html) for a more detailed
-introduction. ## Usage
+**stable** version can be installed from [PyPI](https://pypi.org/project/term-
+image) with: ```shell pip install term-image ``` The **development** version
+can be installed with: ```shell pip install git+https://github.com/AnonymouX47/
+term-image.git ``` ### Supported Terminal Emulators See [here](https://term-
+image.readthedocs.io/en/stable/start/installation.html#supported-terminal-
+emulators) for a list of tested terminal emulators. If you've tested this
+library on any other terminal emulator that meets the requirements for any of
+the render styles, please mention the name (and version) in a new thread under
+[this discussion](https://github.com/AnonymouX47/term-image/discussions/4).
+Also, if you have any issue with terminal support, you may report or check
+information about it in the discussion linked above. ## Features - Multiple
+image formats (basically all formats supported by [`PIL.Image.open()`](https://
+pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)) - Multiple
+image source types: PIL image instance, local file, URL - Multiple image render
+styles (with automatic support detection) - Support for multiple terminal
+graphics protocols: [Kitty](https://sw.kovidgoyal.net/kitty/graphics-protocol/
+), [iTerm2](https://iterm2.com/documentation-images.html) - Exposes various
+features of the protocols - Transparency support (with multiple options) -
+Animated image support (including transparent ones) - Multiple formats: GIF,
+WEBP, APNG (and possibly more) - Fully controllable iteration over rendered
+frames of animated images - Image animation with multiple parameters -
+Integration into various TUI / terminal-based output libraries. - Terminal size
+awareness - Automatic and manual image sizing - Horizontal and vertical
+alignment - Automatic and manual font ratio adjustment (to preserve image
+aspect ratio) - and more... ð ## Demo Check out this [image viewer]
+[termvisage] based on this library. ## Quick Start ### Creating an instance 1.
+Initialize with a file path: ```python from term_image.image import from_file
+image = from_file("path/to/image.png") ``` 2. Initialize with a URL: ```python
+from term_image.image import from_url image = from_url("https://
+www.example.com/image.png") ``` 3. Initialize with a PIL (Pillow) image
+instance: ```python from PIL import Image from term_image.image import
+AutoImage img = Image.open("path/to/image.png") image = AutoImage(img) ``` ###
+Drawing/Displaying an Image There are two basic ways to draw an image to the
+terminal screen: 1. Using the `draw()` method: ```python image.draw() ```
+**NOTE:** `draw()` has various parameters for render formatting. 2. Using
+`print()` with an image render output: ```python print(image) # without
+formatting # OR print(f"{image:>200.^100#ffffff}") # with formatting ``` For
+animated images, only the former animates the output, the latter only draws the
+current frame. See the [tutorial](https://term-image.readthedocs.io/en/stable/
+start/tutorial.html) for a more detailed introduction. ## Usage
    ð§ Under Construction - There will most likely be incompatible changes
                     between minor versions of version_zero!
 **If you want to use this library in a project while it's still on version
 zero, ensure you pin the dependency version to a specific minor version e.g
 `>=0.4,<0.5`.** See the [docs](https://term-image.readthedocs.io) for the User
 Guide and API Reference. ## Contribution Please read through the [guidelines]
 (https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md). For code
@@ -100,14 +101,10 @@
 the implementation can be discussed. Hint: You can filter issues by *label* or
 simply *search* using the features's description. Thanks! ð ## Planned
 Features See [here](https://term-image.readthedocs.io/en/stable/planned.html).
 ## Known Issues See [here](https://term-image.readthedocs.io/en/stable/
 issues.html). ## FAQs See the [FAQs](https://term-image.readthedocs.io/en/
 stable/faqs.html) section of the docs. ## Credits The following projects have
 been (and are still) crucial to the development of this project: - [Pillow]
-(https://python-pillow.org) ## Donate Your donation will go a long way in
-aiding the progress and development of this project. ``` USDT Address:
-TKP6d3hLcs7i5R18WRFxLe3zsPQcCBS1Ro Network: TRC20 ``` I'm sincerly sorry for
-any inconviences that may result from the means of donation. Please bare with
-me, as usual means of accepting donations are not available in the region of
-the world where I reside. Thank you! ð [termvisage]: https://github.com/
-AnonymouX47/termvisage
+(https://python-pillow.org) ## Donate [Buy_Me_A_Coffee] Your donation will go a
+long way in aiding the progress and development of this project. Thank you!
+ð [termvisage]: https://github.com/AnonymouX47/termvisage
```

### Comparing `term-image-0.6.0/src/term_image.egg-info/SOURCES.txt` & `term-image-0.6.1/src/term_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/tests/test_iterator.py` & `term-image-0.6.1/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `term-image-0.6.0/tests/test_top_level.py` & `term-image-0.6.1/tests/test_top_level.py`

 * *Files identical despite different names*

