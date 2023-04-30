# Comparing `tmp/uwuipy-0.1.4.tar.gz` & `tmp/uwuipy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwuipy-0.1.4.tar", last modified: Fri Aug 19 16:30:22 2022, max compression
+gzip compressed data, was "uwuipy-0.1.5.tar", last modified: Sun Apr 30 21:29:59 2023, max compression
```

## Comparing `uwuipy-0.1.4.tar` & `uwuipy-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-19 16:30:22.158109 uwuipy-0.1.4/
--rwxrwxrwx   0 root         (0) root         (0)     2160 2022-08-19 16:30:22.156110 uwuipy-0.1.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1510 2022-08-01 23:17:21.000000 uwuipy-0.1.4/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2022-08-19 16:30:22.158109 uwuipy-0.1.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      630 2022-08-19 16:20:31.000000 uwuipy-0.1.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-19 16:30:21.959080 uwuipy-0.1.4/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-19 16:30:21.991376 uwuipy-0.1.4/src/uwuipy/
--rwxrwxrwx   0 root         (0) root         (0)       26 2022-07-30 17:42:55.000000 uwuipy-0.1.4/src/uwuipy/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7455 2022-08-19 16:19:22.000000 uwuipy-0.1.4/src/uwuipy/uwuipy.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-19 16:30:22.141754 uwuipy-0.1.4/src/uwuipy.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2160 2022-08-19 16:30:21.000000 uwuipy-0.1.4/src/uwuipy.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      198 2022-08-19 16:30:21.000000 uwuipy-0.1.4/src/uwuipy.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2022-08-19 16:30:21.000000 uwuipy-0.1.4/src/uwuipy.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2022-08-19 16:30:21.000000 uwuipy-0.1.4/src/uwuipy.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 21:29:59.175965 uwuipy-0.1.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1084 2022-07-30 16:51:45.000000 uwuipy-0.1.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     2293 2023-04-30 21:29:59.171766 uwuipy-0.1.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2018 2023-04-30 21:25:36.000000 uwuipy-0.1.5/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-30 21:29:59.175965 uwuipy-0.1.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-30 21:26:22.000000 uwuipy-0.1.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 21:29:58.897080 uwuipy-0.1.5/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 21:29:59.025250 uwuipy-0.1.5/src/uwuipy/
+-rwxrwxrwx   0 root         (0) root         (0)       26 2022-07-30 17:42:55.000000 uwuipy-0.1.5/src/uwuipy/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1834 2023-04-30 21:25:36.000000 uwuipy-0.1.5/src/uwuipy/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7620 2023-04-30 21:15:42.000000 uwuipy-0.1.5/src/uwuipy/uwuipy.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-30 21:29:59.139976 uwuipy-0.1.5/src/uwuipy.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     2293 2023-04-30 21:29:58.000000 uwuipy-0.1.5/src/uwuipy.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      229 2023-04-30 21:29:58.000000 uwuipy-0.1.5/src/uwuipy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-30 21:29:58.000000 uwuipy-0.1.5/src/uwuipy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-04-30 21:29:58.000000 uwuipy-0.1.5/src/uwuipy.egg-info/top_level.txt
```

### Comparing `uwuipy-0.1.4/PKG-INFO` & `uwuipy-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 Metadata-Version: 2.1
 Name: uwuipy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Allows the easy implementation of uwuifying words for applications like Discord bots and websites
 Home-page: https://github.com/Cuprum77/uwuipy
-Author: Cuprum77, diminDDL, ThatRedKite
+Author: Cuprum77, diminDDL, R2Boyo25, ThatRedKite and pin-lee
 License: MIT
-Description: # uwuipy
-        An advanced uwuifier for python.
-        ## Install
-        To install just use PyPI `pip install uwuipy`
-        ## Usage
-        Basic usage for uwuifying user input.
-        ```python
-        from uwuipy import uwuipy
-        
-        uwu = uwuipy()
-        print(uwu.uwuify(input()))
-        ```
-        The constructor accepts several optional parameters:
-        * seed
-        * stutterchance
-        * facechance
-        * actionchance
-        * exclamationchance
-        
-        the seed sets the rng seed for the random events, and the values for the parameters (range is between 0 and 1.0) control the probability of them occuring.
-        ```python
-        from uwuipy import uwuipy
-        
-        uwu = uwuipy(None, 0.3, 0.3, 0.3, 1)
-        print(uwu.uwuify(input()))
-        ```
-        Usage of the above example:
-        ```
-        The quick brown fox jumps over the lazy dog
-        The quick b-b-b-bwown (・\`ω\´・) ***screeches*** fox jumps uvw t-t-t-the OwO wazy dog
-        ```
-        You can use an integer seed (for example the timestamp when a message was posted to give it a unique uwuify)
-        ```python
-        from datetime import datetime
-        from uwuipy import uwuipy
-        
-        message = "Hello this is a message posted in 2017."
-        seed = datetime(2017, 11, 28, 23, 55, 59, 342380).timestamp()
-        uwu = uwuipy(seed)
-        print(uwu.uwuify(message))
-        ```
-        as you can see we only use one method `uwuify()` it accepts a string and returns an uwuified string as per the values set in the contructor.
-        ## Contributing and Licence
-        Feel free contribute to the [github repo](https://github.com/Cuprum77/uwuipy) of the project.
-        
-        Licenced under [MIT](https://github.com/Cuprum77/uwuipy/blob/main/LICENSE)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# uwuipy
+An advanced uwuifier for python.
+## Install
+To install just use PyPI `pip install uwuipy`
+## Usage
+Usage from CLI:
+```bash
+python3 -m uwuipy The quick brown fox jumps over the lazy dog
+The quick b-b-b-bwown (・\`ω\´・) ***screeches*** fox jumps uvw t-t-t-the OwO wazy dog
+```
+
+It can also be used as a REPL:
+```bash
+python3 -m uwuipy 
+>>> The quick brown fox jumps over the lazy dog
+The quick b-b-b-bwown (・\`ω\´・) ***screeches*** fox jumps uvw t-t-t-the OwO wazy dog
+>>> ^D
+```
+
+For explanations of the CLI flags please run
+```bash
+python3 -m uwuipy --help
+```
+
+Basic usage as a library for uwuifying user input:
+```python
+from uwuipy import uwuipy
+
+uwu = uwuipy()
+print(uwu.uwuify(input()))
+```
+The constructor accepts several optional parameters:
+* seed
+* stutterchance
+* facechance
+* actionchance
+* exclamationchance
+
+the seed sets the rng seed for the random events, and the values for the parameters (range is between 0 and 1.0) control the probability of them occuring.
+```python
+from uwuipy import uwuipy
+
+uwu = uwuipy(None, 0.3, 0.3, 0.3, 1)
+print(uwu.uwuify(input()))
+```
+Usage of the above example:
+```
+The quick brown fox jumps over the lazy dog
+The quick b-b-b-bwown (・\`ω\´・) ***screeches*** fox jumps uvw t-t-t-the OwO wazy dog
+```
+You can use an integer seed (for example the timestamp when a message was posted to give it a unique uwuify)
+```python
+from datetime import datetime
+from uwuipy import uwuipy
+
+message = "Hello this is a message posted in 2017."
+seed = datetime(2017, 11, 28, 23, 55, 59, 342380).timestamp()
+uwu = uwuipy(seed)
+print(uwu.uwuify(message))
+```
+as you can see we only use one method `uwuify()` it accepts a string and returns an uwuified string as per the values set in the contructor.
+## Contributing and Licence
+Feel free contribute to the [github repo](https://github.com/Cuprum77/uwuipy) of the project.
+
+Licenced under [MIT](https://github.com/Cuprum77/uwuipy/blob/main/LICENSE)
```

### Comparing `uwuipy-0.1.4/README.md` & `uwuipy-0.1.5/src/uwuipy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,76 @@
-# uwuipy
-An advanced uwuifier for python.
-## Install
-To install just use PyPI `pip install uwuipy`
-## Usage
-Basic usage for uwuifying user input.
-```python
-from uwuipy import uwuipy
-
-uwu = uwuipy()
-print(uwu.uwuify(input()))
-```
-The constructor accepts several optional parameters:
-* seed
-* stutterchance
-* facechance
-* actionchance
-* exclamationchance
-
-the seed sets the rng seed for the random events, and the values for the parameters (range is between 0 and 1.0) control the probability of them occuring.
-```python
-from uwuipy import uwuipy
-
-uwu = uwuipy(None, 0.3, 0.3, 0.3, 1)
-print(uwu.uwuify(input()))
-```
-Usage of the above example:
-```
-The quick brown fox jumps over the lazy dog
-The quick b-b-b-bwown (・\`ω\´・) ***screeches*** fox jumps uvw t-t-t-the OwO wazy dog
-```
-You can use an integer seed (for example the timestamp when a message was posted to give it a unique uwuify)
-```python
-from datetime import datetime
-from uwuipy import uwuipy
-
-message = "Hello this is a message posted in 2017."
-seed = datetime(2017, 11, 28, 23, 55, 59, 342380).timestamp()
-uwu = uwuipy(seed)
-print(uwu.uwuify(message))
-```
-as you can see we only use one method `uwuify()` it accepts a string and returns an uwuified string as per the values set in the contructor.
-## Contributing and Licence
-Feel free contribute to the [github repo](https://github.com/Cuprum77/uwuipy) of the project.
-
-Licenced under [MIT](https://github.com/Cuprum77/uwuipy/blob/main/LICENSE)
+Metadata-Version: 2.1
+Name: uwuipy
+Version: 0.1.5
+Summary: Allows the easy implementation of uwuifying words for applications like Discord bots and websites
+Home-page: https://github.com/Cuprum77/uwuipy
+Author: Cuprum77, diminDDL, R2Boyo25, ThatRedKite and pin-lee
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# uwuipy
+An advanced uwuifier for python.
+## Install
+To install just use PyPI `pip install uwuipy`
+## Usage
+Usage from CLI:
+```bash
+python3 -m uwuipy The quick brown fox jumps over the lazy dog
+The quick b-b-b-bwown (・\`ω\´・) ***screeches*** fox jumps uvw t-t-t-the OwO wazy dog
+```
+
+It can also be used as a REPL:
+```bash
+python3 -m uwuipy 
+>>> The quick brown fox jumps over the lazy dog
+The quick b-b-b-bwown (・\`ω\´・) ***screeches*** fox jumps uvw t-t-t-the OwO wazy dog
+>>> ^D
+```
+
+For explanations of the CLI flags please run
+```bash
+python3 -m uwuipy --help
+```
+
+Basic usage as a library for uwuifying user input:
+```python
+from uwuipy import uwuipy
+
+uwu = uwuipy()
+print(uwu.uwuify(input()))
+```
+The constructor accepts several optional parameters:
+* seed
+* stutterchance
+* facechance
+* actionchance
+* exclamationchance
+
+the seed sets the rng seed for the random events, and the values for the parameters (range is between 0 and 1.0) control the probability of them occuring.
+```python
+from uwuipy import uwuipy
+
+uwu = uwuipy(None, 0.3, 0.3, 0.3, 1)
+print(uwu.uwuify(input()))
+```
+Usage of the above example:
+```
+The quick brown fox jumps over the lazy dog
+The quick b-b-b-bwown (・\`ω\´・) ***screeches*** fox jumps uvw t-t-t-the OwO wazy dog
+```
+You can use an integer seed (for example the timestamp when a message was posted to give it a unique uwuify)
+```python
+from datetime import datetime
+from uwuipy import uwuipy
+
+message = "Hello this is a message posted in 2017."
+seed = datetime(2017, 11, 28, 23, 55, 59, 342380).timestamp()
+uwu = uwuipy(seed)
+print(uwu.uwuify(message))
+```
+as you can see we only use one method `uwuify()` it accepts a string and returns an uwuified string as per the values set in the contructor.
+## Contributing and Licence
+Feel free contribute to the [github repo](https://github.com/Cuprum77/uwuipy) of the project.
+
+Licenced under [MIT](https://github.com/Cuprum77/uwuipy/blob/main/LICENSE)
```

### Comparing `uwuipy-0.1.4/setup.py` & `uwuipy-0.1.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="uwuipy",
-    version="0.1.4",
-    author="Cuprum77, diminDDL, ThatRedKite",
+    version="0.1.5",
+    author="Cuprum77, diminDDL, R2Boyo25, ThatRedKite and pin-lee",
     description="Allows the easy implementation of uwuifying words for applications like Discord bots and websites",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/Cuprum77/uwuipy",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     license="MIT"
```

### Comparing `uwuipy-0.1.4/src/uwuipy/uwuipy.py` & `uwuipy-0.1.5/src/uwuipy/uwuipy.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     __uwu_pattern = [
         (r'[rl]', 'w'),
         (r'[RL]', 'W'),
         (r'n([aeiou])', 'ny\g<1>'),
         (r'N([aeiou])', 'Ny\g<1>'),
         (r'N([AEIOU])', 'NY\g<1>'),
         (r'ove', 'uv'),
+        (r'pog', 'poggies'),
     ]
 
     __actions = [
         '***blushes***',
         '***whispers to self***',
         '***cries***',
         '***screams***',
@@ -33,15 +34,17 @@
         '***pounces on you***',
         '***nuzzles your necky wecky***',
         '***unzips your pants***',
         '***licks lips***',
         '***glomps and huggles***',
         '***glomps***',
         '***looks around suspiciously***',
-        '***smirks smuggly***'
+        '***smirks smuggly***',
+        '***pounces on your buldge***',
+        '***breaks into your house and aliases neofetch to rm -rf --no-preserve-root /***',
     ]
 
     __exclamations = [
         '!?',
         '?!!',
         '?!?1',
         '!!11',
```

