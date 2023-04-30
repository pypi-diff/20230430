# Comparing `tmp/rwpp-0.1.0.tar.gz` & `tmp/rwpp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwpp-0.1.0.tar", max compression
+gzip compressed data, was "rwpp-0.1.1.tar", max compression
```

## Comparing `rwpp-0.1.0.tar` & `rwpp-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1036 2023-04-12 08:44:40.294773 rwpp-0.1.0/LICENSE
--rw-r--r--   0        0        0     3325 2023-04-12 08:44:40.294773 rwpp-0.1.0/README.md
--rw-r--r--   0        0        0      389 2023-04-12 08:44:40.294773 rwpp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 08:44:40.294773 rwpp-0.1.0/rwpp/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-12 08:44:40.294773 rwpp-0.1.0/rwpp/main.py
--rw-r--r--   0        0        0     3876 1970-01-01 00:00:00.000000 rwpp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1036 2023-04-23 17:24:52.284417 rwpp-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4091 2023-04-30 18:16:20.252021 rwpp-0.1.1/README.md
+-rw-r--r--   0        0        0      458 2023-04-30 18:20:58.860055 rwpp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 17:24:52.284417 rwpp-0.1.1/rwpp/__init__.py
+-rw-r--r--   0        0        0     3230 2023-04-30 17:27:19.744237 rwpp-0.1.1/rwpp/main.py
+-rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 rwpp-0.1.1/PKG-INFO
```

### Comparing `rwpp-0.1.0/LICENSE` & `rwpp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rwpp-0.1.0/PKG-INFO` & `rwpp-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,98 @@
-Metadata-Version: 2.1
-Name: rwpp
-Version: 0.1.0
-Summary: 
-Author: Ducky
-Author-email: duckbox007@pm.me
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: redditwarp (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
-Description-Content-Type: text/markdown
-
 # Reddit Wallpaper Puller (rwpp)
 
 This project is a simple python command line application to download images from Reddit built using [Typer](https://typer.tiangolo.com) and [Redditwarp](https://redditwarp.readthedocs.io).
 
 ## Setup
 
 For general usage as a user you can simply install the program using `pip install rwpp`.
 
 ### Development Environment
 
-For development I have been simply creating a _virtualenv_ and installing the required dependencies.
+For development you can simply create a _virtualenv_ and install the required dependencies.
 
 ```bash
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -r requirements.txt
 ```
 
-The project now uses [Poetry](https://python-poetry.org/docs/) to build and upload the project to [PyPi](https://pypi.org/), those more familiar with it may use it instead to install dependencies in a development environment.
+The project now uses [Poetry](https://python-poetry.org/docs/) to build and upload the project to [PyPi](https://pypi.org/).
+You can setup and manage your virtual environments with [Poetry](https://python-poetry.org/docs/).
+
+```bash
+cd rwpp
+poetry shell
+poetry install
+
+```
 
 ## Usage
 
 After installing the program using `pip` you can call it from the command line using `rwpp`.
 The CLI will prompt you for a limit and a download path, press enter to use the defaults.
 
 ```bash
 rwpp earthporn
 
 # Output
 How many images would you like to download?  [10]:
 Where would you like to save the images?  [./downloads]:
 ```
 
+
 ### Development
 
 After setting up `rwpp` for development, you can call the `rwpp/main.py` file with the name of a _subreddit_.
 The CLI will prompt you for a limit and a download path, press enter to use the defaults.
 
 ```bash
 python rwpp/main.py earthporn
 
 # Output
 How many images would you like to download?  [10]:
 Where would you like to save the images?  [./downloads]:
 ```
 
+To run the program with [Poetry](https://python-poetry.org/docs/) simply use `poetry run`.
+
+```bash
+poetry run rwpp earthporn
+```
+
+
+### Publishing
+
+Publishing the project to Pypi or Test Pypi is now done using Poetry. After you have made all the necessary commits, tested everything to ensure it runs as expected and setup your Pypi tokens in Poetry ([read more here](https://stackoverflow.com/questions/68882603/using-python-poetry-to-publish-to-test-pypi-org)), the process is as follows below.
+
+```bash
+# Bump version
+poetry version patch
+
+# Publish
+poetry publish
+# poetry publish -r test-pypi
+```
+
 ## Notes
 
 This project is currently in beta and dev mode, no code is assumed to be safe.
 Run at your own risk, there is currently no check to make sure the url pulled from top posts contains an image, just a valid extension
 
 The script will check the given download paths for images that 'have already been downloaded'. This is a simple check against the names of the files (titles of their respective posts) to see what's been downloaded. This can become an issue when a user wants to download to multiple paths.
 A sqlite db/csv file could be implemented to save details about downloads so that when checking a given path for already downloaded images, the image in question does not have to be inside of the given directory.
 
 Had to save the images using the unique post.id rather then the post.title as sometimes it will throw an error if the title is too long.
 We can get the unique url which contains part of the title for a more detailed file name.
 
 ## Todo
 
-- [ ] Check to see if the subreddit exists before pulling images
-- [ ] Add time filters, so rather then top:all we can do top:day,week,month etc.
-- [ ] After adding extra time filters, add the option to pull 'hot' posts with the same filters
-- [ ] Add option to pull new posts
+- [ ] Check to see if the subreddit exists before pulling images/Handle errors for invalid subreddit
+- [x] Add time filters, so rather then top:all we can do top:day,week,month etc.
+- [x] ~After adding extra time filters, add the option to pull 'hot' posts with the same filters~
+- [x] ~Add time filter of new posts~
+
+Only top and controversial posts supports choosing a time range for the download.
 
 The goal is to get this script up to the state where it can be a simple command line utility you can run using `rwpp` and then pass in args such as subreddit(s), how many posts, whether to be top or hot posts, the downloads path to use if not the default one
 
 Currently doing a simple check against the list of the names ofs the images which have already been downloaded should be suffice, though I don't see it being an issue immediately, I do wonder how well it would scale and at what point does it really start to hinder performance. Maybe look at ways to do a more performant check.
-
```

