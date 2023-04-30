# Comparing `tmp/nudecrawler-0.3.8.tar.gz` & `tmp/nudecrawler-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudecrawler-0.3.8.tar", last modified: Mon Apr 10 19:14:11 2023, max compression
+gzip compressed data, was "nudecrawler-0.3.9.tar", last modified: Mon Apr 10 23:02:56 2023, max compression
```

## Comparing `nudecrawler-0.3.8.tar` & `nudecrawler-0.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    14950 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)    14438 2023-04-10 19:13:30.000000 nudecrawler-0.3.8/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/bin/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1458 2023-03-25 09:35:46.000000 nudecrawler-0.3.8/bin/detect-image-aid.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2497 2023-03-25 11:06:28.000000 nudecrawler-0.3.8/bin/detect-image-nsfw-api.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1527 2023-04-10 13:36:55.000000 nudecrawler-0.3.8/bin/detect-image-nudenet.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3527 2023-04-10 14:42:15.000000 nudecrawler-0.3.8/bin/detect-server-nudenet.py
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)    16131 2023-04-10 19:10:01.000000 nudecrawler-0.3.8/bin/nudecrawler
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      217 2023-04-01 23:30:57.000000 nudecrawler-0.3.8/bin/refresh-nsfw-api.sh
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/nudecrawler/
--rw-r--r--   0 xenon     (1000) xenon     (1000)       95 2023-03-20 17:34:21.000000 nudecrawler-0.3.8/nudecrawler/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1990 2023-04-03 19:10:18.000000 nudecrawler-0.3.8/nudecrawler/cache.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      293 2023-03-21 11:11:32.000000 nudecrawler-0.3.8/nudecrawler/exceptions.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      588 2023-03-25 09:36:26.000000 nudecrawler-0.3.8/nudecrawler/localimage.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12822 2023-04-10 18:00:20.000000 nudecrawler-0.3.8/nudecrawler/page.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     3082 2023-04-10 16:46:51.000000 nudecrawler-0.3.8/nudecrawler/remoteimage.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      952 2023-04-03 17:15:52.000000 nudecrawler-0.3.8/nudecrawler/tgru.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)      352 2023-02-28 18:19:59.000000 nudecrawler-0.3.8/nudecrawler/unbuffered.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1114 2023-04-08 13:56:10.000000 nudecrawler-0.3.8/nudecrawler/verbose.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)       15 2023-04-10 19:13:41.000000 nudecrawler-0.3.8/nudecrawler/version.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/nudecrawler.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    14950 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      619 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)      104 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/requires.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-10 19:14:11.000000 nudecrawler-0.3.8/nudecrawler.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)      880 2023-04-06 18:16:07.000000 nudecrawler-0.3.8/pyproject.toml
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/setup.cfg
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1688 2023-04-08 18:41:42.000000 nudecrawler-0.3.8/setup.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 19:14:11.327399 nudecrawler-0.3.8/tests/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      637 2023-04-03 22:33:06.000000 nudecrawler-0.3.8/tests/test_nudecrawler.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 23:02:56.941951 nudecrawler-0.3.9/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    14017 2023-04-10 23:02:56.941951 nudecrawler-0.3.9/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    13505 2023-04-10 22:48:22.000000 nudecrawler-0.3.9/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 23:02:56.937951 nudecrawler-0.3.9/bin/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1458 2023-03-25 09:35:46.000000 nudecrawler-0.3.9/bin/detect-image-aid.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2497 2023-03-25 11:06:28.000000 nudecrawler-0.3.9/bin/detect-image-nsfw-api.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1527 2023-04-10 13:36:55.000000 nudecrawler-0.3.9/bin/detect-image-nudenet.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     3527 2023-04-10 14:42:15.000000 nudecrawler-0.3.9/bin/detect-server-nudenet.py
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)    16130 2023-04-10 23:02:34.000000 nudecrawler-0.3.9/bin/nudecrawler
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      217 2023-04-01 23:30:57.000000 nudecrawler-0.3.9/bin/refresh-nsfw-api.sh
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 23:02:56.941951 nudecrawler-0.3.9/nudecrawler/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       95 2023-03-20 17:34:21.000000 nudecrawler-0.3.9/nudecrawler/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1990 2023-04-03 19:10:18.000000 nudecrawler-0.3.9/nudecrawler/cache.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      293 2023-03-21 11:11:32.000000 nudecrawler-0.3.9/nudecrawler/exceptions.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      588 2023-03-25 09:36:26.000000 nudecrawler-0.3.9/nudecrawler/localimage.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12822 2023-04-10 18:00:20.000000 nudecrawler-0.3.9/nudecrawler/page.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     3082 2023-04-10 16:46:51.000000 nudecrawler-0.3.9/nudecrawler/remoteimage.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      952 2023-04-03 17:15:52.000000 nudecrawler-0.3.9/nudecrawler/tgru.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      352 2023-02-28 18:19:59.000000 nudecrawler-0.3.9/nudecrawler/unbuffered.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     1114 2023-04-08 13:56:10.000000 nudecrawler-0.3.9/nudecrawler/verbose.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       15 2023-04-10 23:02:41.000000 nudecrawler-0.3.9/nudecrawler/version.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 23:02:56.941951 nudecrawler-0.3.9/nudecrawler.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    14017 2023-04-10 23:02:56.000000 nudecrawler-0.3.9/nudecrawler.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      619 2023-04-10 23:02:56.000000 nudecrawler-0.3.9/nudecrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-10 23:02:56.000000 nudecrawler-0.3.9/nudecrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      104 2023-04-10 23:02:56.000000 nudecrawler-0.3.9/nudecrawler.egg-info/requires.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-10 23:02:56.000000 nudecrawler-0.3.9/nudecrawler.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      880 2023-04-06 18:16:07.000000 nudecrawler-0.3.9/pyproject.toml
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-10 23:02:56.941951 nudecrawler-0.3.9/setup.cfg
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1688 2023-04-08 18:41:42.000000 nudecrawler-0.3.9/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-10 23:02:56.941951 nudecrawler-0.3.9/tests/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      637 2023-04-03 22:33:06.000000 nudecrawler-0.3.9/tests/test_nudecrawler.py
```

### Comparing `nudecrawler-0.3.8/PKG-INFO` & `nudecrawler-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudecrawler
-Version: 0.3.8
+Version: 0.3.9
 Summary: Crawl telegra.ph for nude pictures and videos
 Home-page: https://github.com/yaroslaff/nudecrawler
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
 Recommended (and most secure) way is using docker:
 ```
 mkdir /tmp/run
-sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
+sudo docker run --rm -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
 ```
 
 See below how to refine your searching and filtering.
 
 ### Alternative install
 ```
 pip3 install nudecrawler
@@ -93,33 +93,14 @@
 | filtering technology           | A time | A nudes | B time | B nudes                            |
 |---                             |---     | --      |---     |---                                 | 
 |:nude (bilt-in)                 | 127s   | 63      | 34s    | 14 (false positives/negatives)     |
 |detect-image-nsfw_api (docker)  | 90s    | 49      | 23s    | 12                                 |
 |detect-image-aid (docker)       | 124s   | 10      | 28s    | 6 (false negatives)                |
 |detect-image-nudenet  (scripts) | 90s    | 57      | 24s    | 12                                 |
 
-### Example usage:
-Check one page (using built-in :nude filter):
-~~~
-nudecrawler -v --url1 https://telegra.ph/your-page-address 
-~~~
-
-~~~
-nudecrawler -w urls.txt --nude 5 -d 30 -f 5 --stats .local/mystats.json  --log .local/nudecrawler.log 
-~~~
-process urls from urls.txt, report page if 5+ nude images (or 1 any video, default), nudity must be over 0.5 threshold, check from todays date to 30 days ago, append all found pages to .local/nudecrawler.log, save periodical statistics to .local/mystats.json
-
-If crawler will see page `Sasha-Grey-01-23-100`, but `Sasha-Grey-01-23-101` is 404 Not Found, it will try `-102` and so on. It will stop only if 5 (-f) pages in a row will fail. 
-
-~~~
-nudecrawler -v --detect-image bin/detect-image-nsfw-api.py -f 5 --total 10 --nude 3 -w urls.txt --stats .local/stats.json --log .local/urls.log --stop 1000 --refresh bin/refresh-nsfw-api.sh
-~~~
-
-Work verbosely (-v), use NSFW_API for resolving (and call refresh-nsfw-api.sh script to restart docker container every 1000 images).
-
 ## Options
 ~~~
 usage: nudecrawler [-h] [-d DAYS] [--url1 URL] [-f FAILS] [--day MONTH DAY] [--expr EXPR] [--total N] [--max-errors N] [--min-content-length N] [-a] [--detect-image SCRIPT]
                    [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--max-pictures N] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG]
                    [--bugreport] [--workdir WORKDIR] [-w WORDLIST] [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
                    [words ...]
 
@@ -275,17 +256,22 @@
 - Image URL or PATH passed as argv[1]
 - Return 0 if image is safe and boring, return 1 if image is interesting
 - Return 0 if there are any technical problems (timeout or 404)
 - Additional configuration could be specified via environment, NudeCrawler will pass environment to your script
 - NudeCrawler also sets env variables `NUDECRAWLER_PAGE_URL` and `NUDECRAWLER_IMAGE_URL`
 
 ### Building docker container
-Repository includes Dockerfile. Use `sudo docker build -t nudecrawler -f docker/Dockerfile .` to build it.
+Repository includes Dockerfile. Use `sudo docker build -t yaroslaff/nudecrawler:latest -f docker/Dockerfile .` to build it.
+
+Running docker container (example):
+~~~
+mkdir /tmp/run
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
+~~~
 
-Running docker container (example): `sudo docker run -v /tmp/run/:/work nudecrawler nudecrawler -w urls.txt -v`
 If you specify files for docker (like `-w`, `--stats`, `--resume`, `--log`, `--cache`) path will be modified starting from /work. e.g. `-w urls.txt` will be `-w /work/urls.txt` which is /tmp/run/urls.txt on host.
 
 
 ### Little bit about internals
 
 #### Prefiltering
 To speed-up processing, nudecrawler uses pre-filtering, HTTP HEAD request is performed for any image, and further processing is performed only if images passes basic check:
```

### Comparing `nudecrawler-0.3.8/README.md` & `nudecrawler-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
 Recommended (and most secure) way is using docker:
 ```
 mkdir /tmp/run
-sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
+sudo docker run --rm -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
 ```
 
 See below how to refine your searching and filtering.
 
 ### Alternative install
 ```
 pip3 install nudecrawler
@@ -77,33 +77,14 @@
 | filtering technology           | A time | A nudes | B time | B nudes                            |
 |---                             |---     | --      |---     |---                                 | 
 |:nude (bilt-in)                 | 127s   | 63      | 34s    | 14 (false positives/negatives)     |
 |detect-image-nsfw_api (docker)  | 90s    | 49      | 23s    | 12                                 |
 |detect-image-aid (docker)       | 124s   | 10      | 28s    | 6 (false negatives)                |
 |detect-image-nudenet  (scripts) | 90s    | 57      | 24s    | 12                                 |
 
-### Example usage:
-Check one page (using built-in :nude filter):
-~~~
-nudecrawler -v --url1 https://telegra.ph/your-page-address 
-~~~
-
-~~~
-nudecrawler -w urls.txt --nude 5 -d 30 -f 5 --stats .local/mystats.json  --log .local/nudecrawler.log 
-~~~
-process urls from urls.txt, report page if 5+ nude images (or 1 any video, default), nudity must be over 0.5 threshold, check from todays date to 30 days ago, append all found pages to .local/nudecrawler.log, save periodical statistics to .local/mystats.json
-
-If crawler will see page `Sasha-Grey-01-23-100`, but `Sasha-Grey-01-23-101` is 404 Not Found, it will try `-102` and so on. It will stop only if 5 (-f) pages in a row will fail. 
-
-~~~
-nudecrawler -v --detect-image bin/detect-image-nsfw-api.py -f 5 --total 10 --nude 3 -w urls.txt --stats .local/stats.json --log .local/urls.log --stop 1000 --refresh bin/refresh-nsfw-api.sh
-~~~
-
-Work verbosely (-v), use NSFW_API for resolving (and call refresh-nsfw-api.sh script to restart docker container every 1000 images).
-
 ## Options
 ~~~
 usage: nudecrawler [-h] [-d DAYS] [--url1 URL] [-f FAILS] [--day MONTH DAY] [--expr EXPR] [--total N] [--max-errors N] [--min-content-length N] [-a] [--detect-image SCRIPT]
                    [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--max-pictures N] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG]
                    [--bugreport] [--workdir WORKDIR] [-w WORDLIST] [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
                    [words ...]
 
@@ -259,17 +240,22 @@
 - Image URL or PATH passed as argv[1]
 - Return 0 if image is safe and boring, return 1 if image is interesting
 - Return 0 if there are any technical problems (timeout or 404)
 - Additional configuration could be specified via environment, NudeCrawler will pass environment to your script
 - NudeCrawler also sets env variables `NUDECRAWLER_PAGE_URL` and `NUDECRAWLER_IMAGE_URL`
 
 ### Building docker container
-Repository includes Dockerfile. Use `sudo docker build -t nudecrawler -f docker/Dockerfile .` to build it.
+Repository includes Dockerfile. Use `sudo docker build -t yaroslaff/nudecrawler:latest -f docker/Dockerfile .` to build it.
+
+Running docker container (example):
+~~~
+mkdir /tmp/run
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
+~~~
 
-Running docker container (example): `sudo docker run -v /tmp/run/:/work nudecrawler nudecrawler -w urls.txt -v`
 If you specify files for docker (like `-w`, `--stats`, `--resume`, `--log`, `--cache`) path will be modified starting from /work. e.g. `-w urls.txt` will be `-w /work/urls.txt` which is /tmp/run/urls.txt on host.
 
 
 ### Little bit about internals
 
 #### Prefiltering
 To speed-up processing, nudecrawler uses pre-filtering, HTTP HEAD request is performed for any image, and further processing is performed only if images passes basic check:
```

### Comparing `nudecrawler-0.3.8/bin/detect-image-aid.py` & `nudecrawler-0.3.9/bin/detect-image-aid.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/bin/detect-image-nsfw-api.py` & `nudecrawler-0.3.9/bin/detect-image-nsfw-api.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/bin/detect-image-nudenet.py` & `nudecrawler-0.3.9/bin/detect-image-nudenet.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/bin/detect-server-nudenet.py` & `nudecrawler-0.3.9/bin/detect-server-nudenet.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/bin/nudecrawler` & `nudecrawler-0.3.9/bin/nudecrawler`

 * *Files 1% similar despite different names*

```diff
@@ -333,42 +333,41 @@
         refresh
 
     words = None
     args = get_args()
     sanity_check(args)
 
     # when fastforward, we go to specific word/day/count quickly
-    fastforward = False
+    fastforward = False    
+
+    if args.unbuffered:
+        sys.stdout = Unbuffered(sys.stdout)
+
+
+    if args.workdir:
+        for attr in ['cache', 'wordlist', 'log', 'resume', 'stats']:
+            old = getattr(args, attr)
+            if old is not None:
+                new = os.path.join(args.workdir, old)
+                setattr(args, attr, new)
 
     if args.resume:
         print("Resume from", args.resume)
         try:
             load_stats(args.resume)
         except FileNotFoundError as e: 
             abort(f"Missing status file {args.resume}")
 
         cmd = stats['cmd']
         args = get_args(shlex.split(cmd)[1:])
         fastforward = True
     else:
         stats['cmd'] = ' '.join(sys.argv)
-    
 
 
-    if args.unbuffered:
-        sys.stdout = Unbuffered(sys.stdout)
-
-
-    if args.workdir:
-        for attr in ['cache', 'wordlist', 'log', 'resume', 'stats']:
-            old = getattr(args, attr)
-            if old is not None:
-                new = os.path.join(args.workdir, old)
-                setattr(args, attr, new)
-
 
     # nude = args.nude
     # video = args.video
     verbose = args.verbose
     all_found = args.all    
     matched_resume = False
     skipped_words = 0
```

### Comparing `nudecrawler-0.3.8/nudecrawler/cache.py` & `nudecrawler-0.3.9/nudecrawler/cache.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/nudecrawler/localimage.py` & `nudecrawler-0.3.9/nudecrawler/localimage.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/nudecrawler/page.py` & `nudecrawler-0.3.9/nudecrawler/page.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/nudecrawler/remoteimage.py` & `nudecrawler-0.3.9/nudecrawler/remoteimage.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/nudecrawler/tgru.py` & `nudecrawler-0.3.9/nudecrawler/tgru.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/nudecrawler/verbose.py` & `nudecrawler-0.3.9/nudecrawler/verbose.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/nudecrawler.egg-info/PKG-INFO` & `nudecrawler-0.3.9/nudecrawler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudecrawler
-Version: 0.3.8
+Version: 0.3.9
 Summary: Crawl telegra.ph for nude pictures and videos
 Home-page: https://github.com/yaroslaff/nudecrawler
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 Please use it only for legal and ethical purposes. And it's 18+ surely. 
 
 ## Install
 
 Recommended (and most secure) way is using docker:
 ```
 mkdir /tmp/run
-sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
+sudo docker run --rm -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
 ```
 
 See below how to refine your searching and filtering.
 
 ### Alternative install
 ```
 pip3 install nudecrawler
@@ -93,33 +93,14 @@
 | filtering technology           | A time | A nudes | B time | B nudes                            |
 |---                             |---     | --      |---     |---                                 | 
 |:nude (bilt-in)                 | 127s   | 63      | 34s    | 14 (false positives/negatives)     |
 |detect-image-nsfw_api (docker)  | 90s    | 49      | 23s    | 12                                 |
 |detect-image-aid (docker)       | 124s   | 10      | 28s    | 6 (false negatives)                |
 |detect-image-nudenet  (scripts) | 90s    | 57      | 24s    | 12                                 |
 
-### Example usage:
-Check one page (using built-in :nude filter):
-~~~
-nudecrawler -v --url1 https://telegra.ph/your-page-address 
-~~~
-
-~~~
-nudecrawler -w urls.txt --nude 5 -d 30 -f 5 --stats .local/mystats.json  --log .local/nudecrawler.log 
-~~~
-process urls from urls.txt, report page if 5+ nude images (or 1 any video, default), nudity must be over 0.5 threshold, check from todays date to 30 days ago, append all found pages to .local/nudecrawler.log, save periodical statistics to .local/mystats.json
-
-If crawler will see page `Sasha-Grey-01-23-100`, but `Sasha-Grey-01-23-101` is 404 Not Found, it will try `-102` and so on. It will stop only if 5 (-f) pages in a row will fail. 
-
-~~~
-nudecrawler -v --detect-image bin/detect-image-nsfw-api.py -f 5 --total 10 --nude 3 -w urls.txt --stats .local/stats.json --log .local/urls.log --stop 1000 --refresh bin/refresh-nsfw-api.sh
-~~~
-
-Work verbosely (-v), use NSFW_API for resolving (and call refresh-nsfw-api.sh script to restart docker container every 1000 images).
-
 ## Options
 ~~~
 usage: nudecrawler [-h] [-d DAYS] [--url1 URL] [-f FAILS] [--day MONTH DAY] [--expr EXPR] [--total N] [--max-errors N] [--min-content-length N] [-a] [--detect-image SCRIPT]
                    [--detect-url SCRIPT] [--detect METHOD] [--extensions [EXTENSIONS ...]] [--minsize MINSIZE] [--max-pictures N] [--cache PATH] [-v] [--unbuffered] [--urls] [--log LOG]
                    [--bugreport] [--workdir WORKDIR] [-w WORDLIST] [--stats STATS_FILE] [--resume STATS_FILE] [--stop NUM_IMAGES] [--refresh SCRIPT [ARG ...]]
                    [words ...]
 
@@ -275,17 +256,22 @@
 - Image URL or PATH passed as argv[1]
 - Return 0 if image is safe and boring, return 1 if image is interesting
 - Return 0 if there are any technical problems (timeout or 404)
 - Additional configuration could be specified via environment, NudeCrawler will pass environment to your script
 - NudeCrawler also sets env variables `NUDECRAWLER_PAGE_URL` and `NUDECRAWLER_IMAGE_URL`
 
 ### Building docker container
-Repository includes Dockerfile. Use `sudo docker build -t nudecrawler -f docker/Dockerfile .` to build it.
+Repository includes Dockerfile. Use `sudo docker build -t yaroslaff/nudecrawler:latest -f docker/Dockerfile .` to build it.
+
+Running docker container (example):
+~~~
+mkdir /tmp/run
+sudo docker run -v /tmp/run:/work yaroslaff/nudecrawler nudecrawler -a Eva "Sasha Grey" "Belle Delphine" Amouranth
+~~~
 
-Running docker container (example): `sudo docker run -v /tmp/run/:/work nudecrawler nudecrawler -w urls.txt -v`
 If you specify files for docker (like `-w`, `--stats`, `--resume`, `--log`, `--cache`) path will be modified starting from /work. e.g. `-w urls.txt` will be `-w /work/urls.txt` which is /tmp/run/urls.txt on host.
 
 
 ### Little bit about internals
 
 #### Prefiltering
 To speed-up processing, nudecrawler uses pre-filtering, HTTP HEAD request is performed for any image, and further processing is performed only if images passes basic check:
```

### Comparing `nudecrawler-0.3.8/nudecrawler.egg-info/SOURCES.txt` & `nudecrawler-0.3.9/nudecrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/pyproject.toml` & `nudecrawler-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/setup.py` & `nudecrawler-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `nudecrawler-0.3.8/tests/test_nudecrawler.py` & `nudecrawler-0.3.9/tests/test_nudecrawler.py`

 * *Files identical despite different names*

