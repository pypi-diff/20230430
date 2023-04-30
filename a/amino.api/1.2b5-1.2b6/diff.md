# Comparing `tmp/amino.api-1.2b5.tar.gz` & `tmp/amino.api-1.2b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.2b5.tar", last modified: Sat Apr 29 17:32:17 2023, max compression
+gzip compressed data, was "amino.api-1.2b6.tar", last modified: Sun Apr 30 12:02:57 2023, max compression
```

## Comparing `amino.api-1.2b5.tar` & `amino.api-1.2b6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 17:32:17.968560 amino.api-1.2b5/
--rw-rw-rw-   0        0        0      773 2023-04-29 17:32:17.968560 amino.api-1.2b5/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.2b5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 17:32:17.945092 amino.api-1.2b5/amino/
--rw-rw-rw-   0        0        0      922 2023-04-29 17:31:29.000000 amino.api-1.2b5/amino/__init__.py
--rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/async_client.py
--rw-rw-rw-   0        0        0       56 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/async_full_client.py
--rw-rw-rw-   0        0        0       59 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/async_local_client.py
--rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/async_socket.py
--rw-rw-rw-   0        0        0    36475 2023-04-28 13:47:41.000000 amino.api-1.2b5/amino/client.py
--rw-rw-rw-   0        0        0    18444 2023-04-29 14:43:07.000000 amino.api-1.2b5/amino/full_client.py
--rw-rw-rw-   0        0        0    10956 2023-04-28 22:02:14.000000 amino.api-1.2b5/amino/local_client.py
--rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b5/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:32:17.967560 amino.api-1.2b5/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/utils/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-04-28 13:22:02.000000 amino.api-1.2b5/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     7429 2023-04-22 10:56:39.000000 amino.api-1.2b5/amino/utils/helpers.py
--rw-rw-rw-   0        0        0    14652 2023-04-29 15:04:24.000000 amino.api-1.2b5/amino/utils/objects.py
--rw-rw-rw-   0        0        0     2270 2023-04-22 10:51:46.000000 amino.api-1.2b5/amino/utils/requester.py
--rw-rw-rw-   0        0        0     3660 2023-04-26 13:04:41.000000 amino.api-1.2b5/amino/utils/snippetTools.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:32:17.958558 amino.api-1.2b5/amino.api.egg-info/
--rw-rw-rw-   0        0        0      773 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 17:32:17.970560 amino.api-1.2b5/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-04-29 17:31:45.000000 amino.api-1.2b5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:02:56.978902 amino.api-1.2b6/
+-rw-rw-rw-   0        0        0      773 2023-04-30 12:02:56.978902 amino.api-1.2b6/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.2b6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 12:02:56.924304 amino.api-1.2b6/amino/
+-rw-rw-rw-   0        0        0      922 2023-04-30 12:02:36.000000 amino.api-1.2b6/amino/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/async_client.py
+-rw-rw-rw-   0        0        0       56 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/async_full_client.py
+-rw-rw-rw-   0        0        0       59 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/async_local_client.py
+-rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/async_socket.py
+-rw-rw-rw-   0        0        0    36475 2023-04-28 13:47:41.000000 amino.api-1.2b6/amino/client.py
+-rw-rw-rw-   0        0        0    18667 2023-04-30 11:43:28.000000 amino.api-1.2b6/amino/full_client.py
+-rw-rw-rw-   0        0        0    10956 2023-04-28 22:02:14.000000 amino.api-1.2b6/amino/local_client.py
+-rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b6/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:02:56.977911 amino.api-1.2b6/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b6/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-04-28 13:22:02.000000 amino.api-1.2b6/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7429 2023-04-22 10:56:39.000000 amino.api-1.2b6/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0    14849 2023-04-30 11:43:14.000000 amino.api-1.2b6/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2270 2023-04-22 10:51:46.000000 amino.api-1.2b6/amino/utils/requester.py
+-rw-rw-rw-   0        0        0     3660 2023-04-26 13:04:41.000000 amino.api-1.2b6/amino/utils/snippetTools.py
+drwxrwxrwx   0        0        0        0 2023-04-30 12:02:56.950239 amino.api-1.2b6/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      773 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 12:02:55.000000 amino.api-1.2b6/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 12:02:56.980779 amino.api-1.2b6/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-04-30 12:02:24.000000 amino.api-1.2b6/setup.py
```

### Comparing `amino.api-1.2b5/PKG-INFO` & `amino.api-1.2b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.2b5
+Version: 1.2b6
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.2b5/amino/__init__.py` & `amino.api-1.2b6/amino/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from json import loads
 from requests import get
 
 __title__ = 'amino.api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.2b5'
+__version__ = '1.2b6'
 __newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `amino.api-1.2b5/amino/client.py` & `amino.api-1.2b6/amino/client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b5/amino/full_client.py` & `amino.api-1.2b6/amino/full_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,14 +440,18 @@
 
 
 		elif wikiId:
 			response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/item/{wikiId}")
 			return objects.WikiInfo(response.json()["item"])
 
 
+	def get_chat_thread(self, chatId: str, comId: Union[str, int] = None):
+
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/chat/thread/{chatId}")
+		return objects.Thread(response.json()["thread"])
 
 
 
 	def get_wiki_items(self, comId: Union[str, int], categoryId: str = None, start: int = 0, size: int = 100):
 		fId = f"/{categoryId}?pagingType=t&size={size}&start={start}" if categoryId else ""
 
 		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/item-category{fId}")
```

### Comparing `amino.api-1.2b5/amino/local_client.py` & `amino.api-1.2b6/amino/local_client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b5/amino/socket.py` & `amino.api-1.2b6/amino/socket.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b5/amino/utils/exceptions.py` & `amino.api-1.2b6/amino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b5/amino/utils/helpers.py` & `amino.api-1.2b6/amino/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b5/amino/utils/objects.py` & `amino.api-1.2b6/amino/utils/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 		self.blogsCount = self.json.get("blogsCount")
 
 
 class linkInfo:
 	def __init__(self, data: dict = {}):
 		self.json = data
 		linkInfo = self.json.get("extensions", {}).get("linkInfo", {})
-		self.community = CommunityInfo(self.json.get("extensions", {}).get("community"))
+		self.community = CommunityInfo(self.json.get("extensions", {}).get("community", {}))
 
 		self.path = self.json.get("path")
 		self.objectId = linkInfo.get("objectId")
 		self.targetCode = linkInfo.get("targetCode")
 		self.comId = linkInfo.get("ndcId") if linkInfo.get("ndcId") else self.community.comId
 		self.fullPath = linkInfo.get("fullPath")
 		self.shortCode = linkInfo.get("shortCode")
@@ -262,14 +262,19 @@
 		self.condition = self.json.get("condition")
 		self.icon = self.json.get("icon")
 		self.latestActivityTime = self.json.get("latestActivityTime")
 		self.author = UserProfile(self.json.get("author", {}))
 		self.extensions = self.json.get("extensions", {})
 		self.comId = self.json.get("ndcId")
 		self.createdTime = self.json.get("createdTime")
+		self.userId = self.json.get("uid")
+		self.publishToGlobal = self.json.get("publishToGlobal")
+		self.tipInfo = self.json.get("tipInfo")
+		self.chatBubbles = self.json.get("chatBubbles")
+
 
 		for member in self.json.get("membersSummary", []):
 			self.membersSummary.append(UserProfile(member))
 
 
 
 class MessageList:
```

### Comparing `amino.api-1.2b5/amino/utils/requester.py` & `amino.api-1.2b6/amino/utils/requester.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b5/amino/utils/snippetTools.py` & `amino.api-1.2b6/amino/utils/snippetTools.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b5/amino.api.egg-info/PKG-INFO` & `amino.api-1.2b6/amino.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.2b5
+Version: 1.2b6
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.2b5/amino.api.egg-info/SOURCES.txt` & `amino.api-1.2b6/amino.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b5/setup.py` & `amino.api-1.2b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 info = {
 	"name": "amino.api",
-	"version": "1.2b5",
+	"version": "1.2b6",
 	"github_page": "https://github.com/xXxCLOTIxXx/amino.api",
 	"download_link": "https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip",
 	"license": "MIT",
 	"author": "Xsarz",
 	"author_email": "xsarzy@gmail.com",
 	"description": "Library for creating amino bots and scripts.",
 	"long_description": None,
```

