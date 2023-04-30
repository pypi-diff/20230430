# Comparing `tmp/anime-api-0.9.1.tar.gz` & `tmp/anime-api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anime-api-0.9.1.tar", max compression
+gzip compressed data, was "anime-api-1.0.0.tar", max compression
```

## Comparing `anime-api-0.9.1.tar` & `anime-api-1.0.0.tar`

### file list

```diff
@@ -1,55 +1,53 @@
--rw-r--r--   0        0        0     2581 2022-09-23 05:36:47.349353 anime-api-0.9.1/anime_api/__init__.py
--rw-r--r--   0        0        0      399 2022-09-23 06:38:08.313600 anime-api-0.9.1/anime_api/apis/__init__.py
--rw-r--r--   0        0        0      648 2022-09-23 06:38:12.745509 anime-api-0.9.1/anime_api/apis/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2196 2022-09-22 02:18:06.574704 anime-api-0.9.1/anime_api/apis/anime_facts_rest_api/__init__.py
--rw-r--r--   0        0        0     2634 2022-09-22 02:39:04.523957 anime-api-0.9.1/anime_api/apis/anime_facts_rest_api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1390 2022-09-21 18:39:09.649505 anime-api-0.9.1/anime_api/apis/anime_facts_rest_api/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0      817 2022-09-21 18:07:56.599661 anime-api-0.9.1/anime_api/apis/anime_facts_rest_api/objects.py
--rw-r--r--   0        0        0     2731 2022-09-22 17:28:11.425134 anime-api-0.9.1/anime_api/apis/animechan/__init__.py
--rw-r--r--   0        0        0     3064 2022-09-22 18:10:52.140697 anime-api-0.9.1/anime_api/apis/animechan/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      626 2022-09-22 02:39:04.539578 anime-api-0.9.1/anime_api/apis/animechan/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0      291 2022-09-22 02:18:06.578699 anime-api-0.9.1/anime_api/apis/animechan/objects.py
--rw-r--r--   0        0        0     4279 2022-09-23 04:10:06.116378 anime-api-0.9.1/anime_api/apis/animu/__init__.py
--rw-r--r--   0        0        0     3926 2022-09-23 05:46:53.880685 anime-api-0.9.1/anime_api/apis/animu/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2447 2022-09-23 03:38:16.671237 anime-api-0.9.1/anime_api/apis/animu/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0     1112 2022-09-22 20:11:35.410670 anime-api-0.9.1/anime_api/apis/animu/__pycache__/operators.cpython-310.pyc
--rw-r--r--   0        0        0     1630 2022-09-23 03:25:30.667047 anime-api-0.9.1/anime_api/apis/animu/__pycache__/types.cpython-310.pyc
--rw-r--r--   0        0        0     1173 2022-09-23 03:38:04.445841 anime-api-0.9.1/anime_api/apis/animu/objects.py
--rw-r--r--   0        0        0      305 2022-09-22 20:07:30.139095 anime-api-0.9.1/anime_api/apis/animu/operators.py
--rw-r--r--   0        0        0     1389 2022-09-23 03:16:38.377363 anime-api-0.9.1/anime_api/apis/animu/types.py
--rw-r--r--   0        0        0      954 2022-09-23 05:49:03.249801 anime-api-0.9.1/anime_api/apis/hmtai/__init__.py
--rw-r--r--   0        0        0     1267 2022-09-23 05:49:11.072389 anime-api-0.9.1/anime_api/apis/hmtai/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      490 2022-09-23 05:48:40.063358 anime-api-0.9.1/anime_api/apis/hmtai/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0     2908 2022-09-23 05:48:40.057369 anime-api-0.9.1/anime_api/apis/hmtai/__pycache__/types.cpython-310.pyc
--rw-r--r--   0        0        0      154 2022-09-23 05:30:57.313492 anime-api-0.9.1/anime_api/apis/hmtai/objects.py
--rw-r--r--   0        0        0     2695 2022-09-23 05:48:34.623887 anime-api-0.9.1/anime_api/apis/hmtai/types.py
--rw-r--r--   0        0        0     1878 2022-09-22 18:07:45.282716 anime-api-0.9.1/anime_api/apis/kyoko/__init__.py
--rw-r--r--   0        0        0     1882 2022-09-22 18:10:52.171939 anime-api-0.9.1/anime_api/apis/kyoko/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      857 2022-09-22 18:10:52.171939 anime-api-0.9.1/anime_api/apis/kyoko/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0      403 2022-09-22 18:05:57.144262 anime-api-0.9.1/anime_api/apis/kyoko/objects.py
--rw-r--r--   0        0        0     3516 2022-09-23 06:53:16.302109 anime-api-0.9.1/anime_api/apis/nekos_life/__init__.py
--rw-r--r--   0        0        0     3191 2022-09-23 06:39:10.391799 anime-api-0.9.1/anime_api/apis/nekos_life/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      894 2022-09-23 06:38:13.334445 anime-api-0.9.1/anime_api/apis/nekos_life/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0      859 2022-09-23 06:38:13.340429 anime-api-0.9.1/anime_api/apis/nekos_life/__pycache__/types.cpython-310.pyc
--rw-r--r--   0        0        0      376 2022-09-23 06:53:10.701078 anime-api-0.9.1/anime_api/apis/nekos_life/objects.py
--rw-r--r--   0        0        0      572 2022-09-23 06:24:35.549196 anime-api-0.9.1/anime_api/apis/nekos_life/types.py
--rw-r--r--   0        0        0     8992 2022-09-22 07:09:04.847318 anime-api-0.9.1/anime_api/apis/studio_ghibli_api/__init__.py
--rw-r--r--   0        0        0     6463 2022-09-22 07:10:37.450845 anime-api-0.9.1/anime_api/apis/studio_ghibli_api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    15083 2022-09-22 07:14:25.736188 anime-api-0.9.1/anime_api/apis/studio_ghibli_api/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0    19826 2022-09-22 07:14:16.663507 anime-api-0.9.1/anime_api/apis/studio_ghibli_api/objects.py
--rw-r--r--   0        0        0     4432 2022-09-22 02:18:06.581683 anime-api-0.9.1/anime_api/apis/trace_moe/__init__.py
--rw-r--r--   0        0        0     3608 2022-09-22 02:39:04.098243 anime-api-0.9.1/anime_api/apis/trace_moe/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1363 2022-09-21 18:40:06.456565 anime-api-0.9.1/anime_api/apis/trace_moe/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0      838 2022-09-21 18:40:02.678562 anime-api-0.9.1/anime_api/apis/trace_moe/objects.py
--rw-r--r--   0        0        0     2326 2022-09-22 17:42:34.392420 anime-api-0.9.1/anime_api/apis/waifu_pics/__init__.py
--rw-r--r--   0        0        0     2475 2022-09-22 18:10:52.156325 anime-api-0.9.1/anime_api/apis/waifu_pics/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      495 2022-09-22 04:35:57.271203 anime-api-0.9.1/anime_api/apis/waifu_pics/__pycache__/objects.cpython-310.pyc
--rw-r--r--   0        0        0     1538 2022-09-22 04:35:57.266251 anime-api-0.9.1/anime_api/apis/waifu_pics/__pycache__/types.cpython-310.pyc
--rw-r--r--   0        0        0      154 2022-09-22 04:28:16.528286 anime-api-0.9.1/anime_api/apis/waifu_pics/objects.py
--rw-r--r--   0        0        0     1166 2022-09-22 04:22:41.729368 anime-api-0.9.1/anime_api/apis/waifu_pics/types.py
--rw-r--r--   0        0        0      733 2022-09-21 18:40:51.876604 anime-api-0.9.1/anime_api/exceptions.py
--rw-r--r--   0        0        0    14851 2022-09-21 17:32:59.458040 anime-api-0.9.1/LICENSE.md
--rw-r--r--   0        0        0      481 2022-09-23 06:58:04.222972 anime-api-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5469 2022-09-23 06:57:48.761880 anime-api-0.9.1/README.md
--rw-r--r--   0        0        0     6438 1970-01-01 00:00:00.000000 anime-api-0.9.1/setup.py
--rw-r--r--   0        0        0     5961 1970-01-01 00:00:00.000000 anime-api-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2880 2023-04-30 19:27:15.471233 anime-api-1.0.0/anime_api/__init__.py
+-rw-r--r--   0        0        0      639 2023-04-30 19:28:07.202199 anime-api-1.0.0/anime_api/apis/__init__.py
+-rw-r--r--   0        0        0     2310 2022-09-23 18:02:56.614001 anime-api-1.0.0/anime_api/apis/anime_facts_rest_api/__init__.py
+-rw-r--r--   0        0        0      691 2022-09-23 17:57:02.261044 anime-api-1.0.0/anime_api/apis/anime_facts_rest_api/objects.py
+-rw-r--r--   0        0        0     2773 2023-04-30 18:36:29.547204 anime-api-1.0.0/anime_api/apis/animechan/__init__.py
+-rw-r--r--   0        0        0      291 2022-09-22 02:18:06.578699 anime-api-1.0.0/anime_api/apis/animechan/objects.py
+-rw-r--r--   0        0        0     4279 2022-09-23 04:10:06.116378 anime-api-1.0.0/anime_api/apis/animu/__init__.py
+-rw-r--r--   0        0        0     1173 2022-09-23 03:38:04.445841 anime-api-1.0.0/anime_api/apis/animu/objects.py
+-rw-r--r--   0        0        0      305 2022-09-22 20:07:30.139095 anime-api-1.0.0/anime_api/apis/animu/operators.py
+-rw-r--r--   0        0        0     1389 2022-09-23 18:09:21.227565 anime-api-1.0.0/anime_api/apis/animu/types.py
+-rw-r--r--   0        0        0     2417 2023-04-30 19:43:43.560542 anime-api-1.0.0/anime_api/apis/catboys/__init__.py
+-rw-r--r--   0        0        0      729 2023-04-30 19:41:10.887944 anime-api-1.0.0/anime_api/apis/catboys/objects.py
+-rw-r--r--   0        0        0      954 2022-09-23 05:49:03.249801 anime-api-1.0.0/anime_api/apis/hmtai/__init__.py
+-rw-r--r--   0        0        0      154 2022-09-23 05:30:57.313492 anime-api-1.0.0/anime_api/apis/hmtai/objects.py
+-rw-r--r--   0        0        0     2695 2022-09-23 05:48:34.623887 anime-api-1.0.0/anime_api/apis/hmtai/types.py
+-rw-r--r--   0        0        0     1878 2022-09-22 18:07:45.282716 anime-api-1.0.0/anime_api/apis/kyoko/__init__.py
+-rw-r--r--   0        0        0      403 2022-09-22 18:05:57.144262 anime-api-1.0.0/anime_api/apis/kyoko/objects.py
+-rw-r--r--   0        0        0     1093 2022-09-24 03:54:18.762863 anime-api-1.0.0/anime_api/apis/neko_love/__init__.py
+-rw-r--r--   0        0        0      154 2022-09-24 03:48:07.233630 anime-api-1.0.0/anime_api/apis/neko_love/obejcts.py
+-rw-r--r--   0        0        0      551 2022-09-24 03:50:18.715909 anime-api-1.0.0/anime_api/apis/neko_love/types.py
+-rw-r--r--   0        0        0     2480 2023-01-05 00:21:13.478349 anime-api-1.0.0/anime_api/apis/nekobot/__init__.py
+-rw-r--r--   0        0        0      218 2022-09-23 19:45:24.021158 anime-api-1.0.0/anime_api/apis/nekobot/objects.py
+-rw-r--r--   0        0        0     2619 2022-09-23 19:34:10.172188 anime-api-1.0.0/anime_api/apis/nekobot/types.py
+-rw-r--r--   0        0        0     8825 2023-04-30 18:42:02.897707 anime-api-1.0.0/anime_api/apis/nekos_api/__init__.py
+-rw-r--r--   0        0        0     2866 2023-01-22 19:39:45.893226 anime-api-1.0.0/anime_api/apis/nekos_api/objects.py
+-rw-r--r--   0        0        0      273 2023-01-07 01:51:02.302708 anime-api-1.0.0/anime_api/apis/nekos_api/types.py
+-rw-r--r--   0        0        0      906 2023-01-20 16:26:36.249866 anime-api-1.0.0/anime_api/apis/nekos_api/utils.py
+-rw-r--r--   0        0        0     3081 2022-09-25 06:27:20.877554 anime-api-1.0.0/anime_api/apis/nekos_best/__init__.py
+-rw-r--r--   0        0        0      567 2022-09-24 07:23:19.795916 anime-api-1.0.0/anime_api/apis/nekos_best/objects.py
+-rw-r--r--   0        0        0      968 2022-09-24 07:25:19.739409 anime-api-1.0.0/anime_api/apis/nekos_best/types.py
+-rw-r--r--   0        0        0     3516 2022-09-23 06:53:16.302109 anime-api-1.0.0/anime_api/apis/nekos_life/__init__.py
+-rw-r--r--   0        0        0      376 2022-09-23 06:53:10.701078 anime-api-1.0.0/anime_api/apis/nekos_life/objects.py
+-rw-r--r--   0        0        0      572 2022-09-23 06:24:35.549196 anime-api-1.0.0/anime_api/apis/nekos_life/types.py
+-rw-r--r--   0        0        0    13268 2022-09-24 06:38:01.720449 anime-api-1.0.0/anime_api/apis/nekos_moe/__init__.py
+-rw-r--r--   0        0        0     7566 2022-09-24 06:29:46.181259 anime-api-1.0.0/anime_api/apis/nekos_moe/objects.py
+-rw-r--r--   0        0        0      204 2022-09-24 05:11:01.078976 anime-api-1.0.0/anime_api/apis/nekos_moe/types.py
+-rw-r--r--   0        0        0     8992 2022-09-22 07:09:04.847318 anime-api-1.0.0/anime_api/apis/studio_ghibli_api/__init__.py
+-rw-r--r--   0        0        0    19826 2022-09-22 07:14:16.663507 anime-api-1.0.0/anime_api/apis/studio_ghibli_api/objects.py
+-rw-r--r--   0        0        0     4432 2022-09-22 02:18:06.581683 anime-api-1.0.0/anime_api/apis/trace_moe/__init__.py
+-rw-r--r--   0        0        0      838 2022-09-21 18:40:02.678562 anime-api-1.0.0/anime_api/apis/trace_moe/objects.py
+-rw-r--r--   0        0        0     5117 2023-04-30 18:36:29.550442 anime-api-1.0.0/anime_api/apis/waifu_im/__init__.py
+-rw-r--r--   0        0        0      851 2022-11-29 17:41:53.845590 anime-api-1.0.0/anime_api/apis/waifu_im/objects.py
+-rw-r--r--   0        0        0     1328 2022-11-29 18:09:33.344067 anime-api-1.0.0/anime_api/apis/waifu_im/types.py
+-rw-r--r--   0        0        0     2326 2022-09-22 17:42:34.392420 anime-api-1.0.0/anime_api/apis/waifu_pics/__init__.py
+-rw-r--r--   0        0        0      154 2022-09-22 04:28:16.528286 anime-api-1.0.0/anime_api/apis/waifu_pics/objects.py
+-rw-r--r--   0        0        0     1166 2022-09-22 04:22:41.729368 anime-api-1.0.0/anime_api/apis/waifu_pics/types.py
+-rw-r--r--   0        0        0     1119 2023-01-07 02:40:38.038715 anime-api-1.0.0/anime_api/exceptions.py
+-rw-r--r--   0        0        0      479 2022-12-31 21:12:21.271167 anime-api-1.0.0/anime_api/utils.py
+-rw-r--r--   0        0        0    14851 2022-09-21 17:32:59.458040 anime-api-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0      509 2023-04-30 19:30:20.930473 anime-api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11404 2023-04-30 19:29:40.267119 anime-api-1.0.0/README.md
+-rw-r--r--   0        0        0    12608 1970-01-01 00:00:00.000000 anime-api-1.0.0/setup.py
+-rw-r--r--   0        0        0    11764 1970-01-01 00:00:00.000000 anime-api-1.0.0/PKG-INFO
```

### Comparing `anime-api-0.9.1/anime_api/__init__.py` & `anime-api-1.0.0/anime_api/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ),
     (
         "Trace.moe API",
         apis.TraceMoeAPI,
         "https://soruly.github.io/trace.moe-api/",
         True,
     ),
-    ("Animechan", apis.AnimechanAPI, "https://animechan.vercel.app/guide", True),
+    ("Animechan", apis.AnimechanAPI, "https://animechan.vercel.app/docs", True),
     ("Jikan", None, "https://jikan.docs.apiary.io/#", False),
     ("Waifu Pics", apis.WaifuPicsAPI, "https://waifu.pics/docs", True),
     ("Studio Ghibli API", apis.StudioGhibliAPI, "https://ghibliapi.herokuapp.com/", True),
     ("Kitsu", None, "https://kitsu.docs.apiary.io/#", False),
     ("AniList", None, "https://anilist.gitbook.io/anilist-apiv2-docs/", False),
     ("AniDB", None, "https://wiki.anidb.net/w/API", False),
     ("Kyoko", apis.KyokoAPI, "https://github.com/Elliottophellia/kyoko", True),
@@ -33,30 +33,40 @@
         None,
         "https://www.animenewsnetwork.com/encyclopedia/api.php",
         False,
     ),
     ("Notify.moe", None, "https://notify.moe/api", False),
     ("Hmtai", apis.HmtaiAPI, "https://hmtai.herokuapp.com/endpoints", True),
     ("Nekos.life", None, "https://github.com/Nekos-life/nekos.py", False),
-    ("NekoBot", None, "https://docs.nekobot.xyz/", False),
-    ("Neko-love", None, "https://docs.neko-love.xyz/", False),
-    ("Nekos.moe", None, "https://docs.nekos.moe/", False),
-    ("Nekos.best", None, "https://docs.nekos.best/", False),
+    ("NekoBot", apis.NekoBotAPI, "https://docs.nekobot.xyz/", True),
+    ("Neko-love", apis.NekoLoveAPI, "https://docs.neko-love.xyz/", True),
+    ("Nekos.moe", apis.NekosMoeAPI, "https://docs.nekos.moe/", True),
+    ("Nekos.best", apis.NekosBest, "https://docs.nekos.best/", True),
     ("Shikimori", None, "https://shikimori.one/api/doc", False),
     ("Mangadex", None, "https://api.mangadex.org/docs.html", False),
     ("Danbooru", None, "https://danbooru.donmai.us/wiki_pages/help:api", False),
     (
         "Yandere",
         None,
         "https://yande.re/help/api",
         False,
     ),  # Yandere and Konachan are forks of the same github repo. That's why they have almost-identical apis.
     ("Konachan", None, "https://konachan.com/help/api", False),
-    ("Waifu.im", None, "https://waifu.im/", False),
-    ("Catboys", None, "https://catboys.com/api", False),
+    ("Waifu.im", apis.WaifuImAPI, "https://waifu.im/", True),
+    ("Catboys", apis.CatboysAPI, "https://catboys.com/api", True),
     (
         "Anime Character Database",
         None,
         "http://wiki.animecharactersdatabase.com/index.php?title=API_Access",
         False,
     ),
+    (
+        "Nekos API",
+        apis.NekosAPI,
+        "https://nekos.nekidev.com/docs/rest-api/endpoints",
+        True,
+    ),
 ]
+
+__version__ = '0.15.0'
+__authors__ = ['Nekidev <neki@nekidev.com>']
+__license__ = "MIT License"
```

### Comparing `anime-api-0.9.1/anime_api/apis/anime_facts_rest_api/__init__.py` & `anime-api-1.0.0/anime_api/apis/anime_facts_rest_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """
 Base module for the anime facts rest api. The API documentation can be found at 
 https://chandan-02.github.io/anime-facts-rest-api/
 
 Mantainer of the API: Chandan Kumar (https://github.com/chandan-02)
 """
-import typing, requests
+import typing, requests, random
 
 from anime_api import exceptions
 from anime_api.apis.anime_facts_rest_api.objects import Anime, Fact
 
 
 class AnimeFactsRestAPI:
     """
     Docs: https://chandan-02.github.io/anime-facts-rest-api/
     """
 
     endpoint = "https://anime-facts-rest-api.herokuapp.com/api/v1"
 
-    def __init__(self, endpoint: typing.Optional[str] = None):
-        self.endpoint = endpoint or self.endpoint
-
     def get_animes(self) -> typing.List[Anime]:
         """
         Returns a list of all animes.
         """
         response = requests.get(self.endpoint)
 
         if response.status_code != 200:
@@ -51,14 +48,20 @@
                 status_code=response.status_code
             )
 
         return [
             Fact(id=fact["fact_id"], fact=fact["fact"]) for fact in response.json()["data"]
         ]
 
+    def get_anime_random_fact(self, anime_name: str) -> Fact:
+        """
+        Return a random fact about the given anime (by it's name).
+        """
+        return random.choice(self.get_anime_facts(anime_name))
+
     def get_fact(self, anime_name: str, fact_id: int) -> Fact:
         """
         Returns a specific Fact by it's ID and it's anime's name.
         """
         response = requests.get(f"{self.endpoint}/{anime_name}/{fact_id}")
 
         if response.status_code != 200:
```

### Comparing `anime-api-0.9.1/anime_api/apis/animechan/__init__.py` & `anime-api-1.0.0/anime_api/apis/animechan/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 """
 Base module for the Animechan API. The documentation is available at
-https://animechan.vercel.app/guide
+https://animechan.vercel.app/docs
 """
+from urllib.parse import quote_plus
+
 import typing
 import requests
 
 from anime_api import exceptions
 from anime_api.apis.animechan.objects import Quote
 
 
 class AnimechanAPI:
     """
-    Docs: https://animechan.vercel.app/guide
+    Docs: https://animechan.vercel.app/docs
     """
 
     endpoint = "https://animechan.vercel.app/api"
 
     def __init__(self, endpoint: typing.Optional[str] = None):
         self.endpoint = endpoint or self.endpoint
 
-    def get_random_quote(self) -> Quote:
+    def get_random_quote(
+        self,
+        anime_title: typing.Optional[str] = None,
+        character_name: typing.Optional[str] = None,
+    ) -> Quote:
         """
         Get a random quote from the API.
         """
-        response = requests.get(f"{self.endpoint}/random")
+        response = requests.get(
+            f"{self.endpoint}/random"
+            + (
+                "/character?name=" + quote_plus(character_name)
+                if character_name
+                else "/anime?title=" + quote_plus(anime_title)
+                if anime_title
+                else ""
+            ),
+            timeout=5
+        )
 
-        if response.status_code != 200:
-            raise exceptions.ServerError(
-                status_code=response.status_code,
-            )
+        AnimechanAPI._check_response_code(response.status_code)
 
         return Quote(**response.json())
 
     def get_many_random_quotes(self) -> typing.List[Quote]:
         """
         Get 10 random quotes from the API.
         """
         response = requests.get(f"{self.endpoint}/quotes")
 
-        if response.status_code != 200:
-            raise exceptions.ServerError(
-                status_code=response.status_code,
-            )
+        AnimechanAPI._check_response_code(response.status_code)
 
         return [Quote(**quote) for quote in response.json()]
 
-    def search_by_anime_title(self, anime_title: str, page: int = 1) -> Quote:
+    def search_by_anime_title(
+        self, anime_title: str, page: int = 1
+    ) -> typing.List[Quote]:
         """
         Return a list of quotes from the given anime.
         """
         response = requests.get(
             f"{self.endpoint}/quotes/anime", params={"title": anime_title, "page": page}
         )
 
-        if response.status_code != 200:
-            raise exceptions.ServerError(
-                status_code=response.status_code,
-            )
+        AnimechanAPI._check_response_code(response.status_code)
 
         return [Quote(**quote) for quote in response.json()]
 
-    def search_by_character_name(self, character_name: str, page: int = 1) -> Quote:
+    def search_by_character_name(
+        self, character_name: str, page: int = 1
+    ) -> typing.List[Quote]:
         """
         Return a list of quotes from the given character.
         """
         response = requests.get(
             f"{self.endpoint}/quotes/character",
             params={"name": character_name, "page": page},
         )
 
-        if response.status_code != 200:
-            raise exceptions.ServerError(
-                status_code=response.status_code,
-            )
+        AnimechanAPI._check_response_code(response.status_code)
 
         return [Quote(**quote) for quote in response.json()]
 
-    def get_animes(self, page: int = 1) -> typing.List[str]:
-        """
-        Return a list of animes.
-        """
-        response = requests.get(f"{self.endpoint}/available/anime", params={"page": page})
-
-        if response.status_code != 200:
-            raise exceptions.ServerError(
-                status_code=response.status_code,
-            )
-
-        return response.json()
+    @staticmethod
+    def _check_response_code(status_code: int, msg: str = ""):
+        if status_code == 404:
+            raise exceptions.NotFound()
+        if status_code != 200:
+            raise exceptions.ServerError(status_code=status_code, msg=msg)
```

### Comparing `anime-api-0.9.1/anime_api/apis/animu/__init__.py` & `anime-api-1.0.0/anime_api/apis/animu/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/animu/objects.py` & `anime-api-1.0.0/anime_api/apis/animu/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/animu/types.py` & `anime-api-1.0.0/anime_api/apis/animu/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/hmtai/__init__.py` & `anime-api-1.0.0/anime_api/apis/hmtai/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/hmtai/types.py` & `anime-api-1.0.0/anime_api/apis/hmtai/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/kyoko/__init__.py` & `anime-api-1.0.0/anime_api/apis/kyoko/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/nekos_life/__init__.py` & `anime-api-1.0.0/anime_api/apis/nekos_life/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/nekos_life/types.py` & `anime-api-1.0.0/anime_api/apis/nekos_life/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/studio_ghibli_api/__init__.py` & `anime-api-1.0.0/anime_api/apis/studio_ghibli_api/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/studio_ghibli_api/objects.py` & `anime-api-1.0.0/anime_api/apis/studio_ghibli_api/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/trace_moe/__init__.py` & `anime-api-1.0.0/anime_api/apis/trace_moe/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/trace_moe/objects.py` & `anime-api-1.0.0/anime_api/apis/trace_moe/objects.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/waifu_pics/__init__.py` & `anime-api-1.0.0/anime_api/apis/waifu_pics/__init__.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/apis/waifu_pics/types.py` & `anime-api-1.0.0/anime_api/apis/waifu_pics/types.py`

 * *Files identical despite different names*

### Comparing `anime-api-0.9.1/anime_api/exceptions.py` & `anime-api-1.0.0/anime_api/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 
 class ServerError(Exception):
     """
     Errors from the server.
     """
 
-    def __init__(self, status_code: int, msg: typing.Optional[str] = None, *args, **kwargs):
+    def __init__(
+        self, status_code: int, msg: typing.Optional[str] = None, *args, **kwargs
+    ):
         super().__init__(
-            f"The server returned an error{': ' + msg if msg else ''}. (Status code: {status_code})",
+            f"The server returned an error{': ' + msg if msg else '.'} (Status code: {status_code})",
             *args,
             **kwargs,
         )
 
 
 class UploadLimitExceeded(Exception):
     """
@@ -24,7 +26,22 @@
     """
 
 
 class UnsupportedFileType(Exception):
     """
     Error raised when the file type is not supported by the API.
     """
+
+
+class Forbidden(Exception):
+    """
+    Error raised when the user is not authorized to perform the action.
+    """
+
+
+class NotFound(ServerError):
+    """
+    Error raised when the item is not found.
+    """
+
+    def __init__(self, msg: typing.Optional[str] = "Not found", *args, **kwargs):
+        ServerError.__init__(self, 404, msg, *args, **kwargs)
```

### Comparing `anime-api-0.9.1/LICENSE.md` & `anime-api-1.0.0/LICENSE.md`

 * *Files identical despite different names*

