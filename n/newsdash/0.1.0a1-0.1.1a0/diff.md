# Comparing `tmp/newsdash-0.1.0a1.tar.gz` & `tmp/newsdash-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newsdash-0.1.0a1.tar", max compression
+gzip compressed data, was "newsdash-0.1.1a0.tar", max compression
```

## Comparing `newsdash-0.1.0a1.tar` & `newsdash-0.1.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3123 2023-04-21 11:57:52.134164 newsdash-0.1.0a1/README.md
--rw-r--r--   0        0        0       78 2023-04-21 11:57:52.134164 newsdash-0.1.0a1/newsdash/__init__.py
--rw-r--r--   0        0        0    22992 2023-04-21 11:57:52.134164 newsdash-0.1.0a1/newsdash/client.py
--rw-r--r--   0        0        0     1394 2023-04-21 11:57:52.134164 newsdash-0.1.0a1/newsdash/exceptions.py
--rw-r--r--   0        0        0     2715 2023-04-21 11:57:52.134164 newsdash-0.1.0a1/newsdash/http.py
--rw-r--r--   0        0        0      930 2023-04-21 11:57:52.134164 newsdash-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 newsdash-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     3123 2023-04-30 09:32:48.603865 newsdash-0.1.1a0/README.md
+-rw-r--r--   0        0        0       78 2023-04-30 09:32:48.603865 newsdash-0.1.1a0/newsdash/__init__.py
+-rw-r--r--   0        0        0     2695 2023-04-30 09:32:48.603865 newsdash-0.1.1a0/newsdash/_http.py
+-rw-r--r--   0        0        0    23819 2023-04-30 09:32:48.603865 newsdash-0.1.1a0/newsdash/client.py
+-rw-r--r--   0        0        0     1394 2023-04-30 09:32:48.603865 newsdash-0.1.1a0/newsdash/exceptions.py
+-rw-r--r--   0        0        0      925 2023-04-30 09:32:48.603865 newsdash-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 newsdash-0.1.1a0/PKG-INFO
```

### Comparing `newsdash-0.1.0a1/README.md` & `newsdash-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `newsdash-0.1.0a1/newsdash/client.py` & `newsdash-0.1.1a0/newsdash/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,55 @@
 import typing as tp
-from .http import HttpClient
+from ._http import HttpClient
 import loguru
 
 if tp.TYPE_CHECKING:
     import aiohttp
     import os
     from types import TracebackType
 
 
+class articleType(tp.TypedDict):
+    source: tp.TypedDict("source", {"id": str, "name": str})
+    author: str
+    title: str
+    description: str
+    url: str
+    urlToImage: str
+    publishedAt: str
+    content: str
+
+
+class newsapiGetEverythingResponse(tp.TypedDict):
+    status: tp.Literal["ok", "error"]
+    totalResults: int
+    articles: list[articleType]
+
+
+class newsapiGetTopHeadlinesResponse(tp.TypedDict):
+    status: tp.Literal["ok", "error"]
+    totalResults: int
+    articles: list[articleType]
+
+
+class sourceType(tp.TypedDict):
+    id: str
+    name: str
+    description: str
+    url: str
+    category: str
+    language: str
+    country: str
+
+
+class newsapiGetSourcesResponse(tp.TypedDict):
+    status: tp.Literal["ok", "error"]
+    sources: list[sourceType]
+
+
 class NewsDash:
     """
     A class to interact with NewsAPI.
 
     Attributes
     ----------
     logger : loguru.Logger
@@ -49,24 +87,24 @@
         Parameters
         ----------
         api_key : str
             The api key you get from NewsApi.
         session : typing.Optional[aiohttp.ClientSession], optional
             Custom ClientSession you want the client to use., by default None
         file_logging : typing.Union[bool,list[os.PathLike,typing.Union[bool, str],typing.Union[bool, str],typing.Union[bool, str],],], optional
-            Custom ClientSession you want the client to use., by default False
+            configuration for the file logging, by default False
 
         Returns
         -------
         NewsDash
             The NewsDash client.
         """
         self.logger = loguru.logger
         self.api_key = api_key
-        if file_logging != False:
+        if file_logging is not False:
             file = file_logging[0]
             if len(file_logging) > 1 and file_logging[1]:
                 rotation = file_logging[1]
             else:
                 rotation = None
             if len(file_logging) > 2 and file_logging[2]:
                 retention = file_logging[2]
@@ -83,16 +121,15 @@
 
     async def __aexit__(
         self,
         exc_type: tp.Optional[tp.Type[BaseException]],
         exc_val: tp.Optional[BaseException],
         exc_tb: tp.Optional["TracebackType"],
     ) -> None:
-        if self._http_client.session is not None:
-            await self._http_client.session.close()
+        await self.close()
 
     async def __aenter__(self) -> "NewsDash":
         return self
 
     async def close(self) -> None:
         """
         Closes the session, Note- no need to use it if you are using context manager.
@@ -169,15 +206,15 @@
         pageSize : int, optional
             The number of results to return per page, by default None
         page : int, optional
             Use this to page through the results, by default None
 
         Returns
         -------
-        typing.Any
+        newsapiGetEverythingResponse
             The response from NewsApi after getting news.
 
         Raises
         ------
         HTTPException
             raises HTTPException if the status code is not `ok`.
 
@@ -268,15 +305,15 @@
             if isinstance(page, int):
                 if page < 0:
                     raise ValueError("page should be greater than 0")
             else:
                 raise TypeError("page should be an integer")
             params["page"] = page
         headers = {"X-Api-Key": self.api_key}
-        data = await self._http_client.request(
+        data: newsapiGetEverythingResponse = await self._http_client.request(
             "https://newsapi.org/v2/everything", "GET", headers=headers, params=params
         )
         if data:
             return data
 
     async def get_top_headlines(
         self,
@@ -372,15 +409,15 @@
         Returns
         -------
          typing.Any
             The response from NewsApi after getting news.
 
         Raises
         ------
-        HTTPException
+        newsapiGetTopHeadlinesResponse
             raises HTTPException if the status code is not `ok`.
 
         Examples
         -------
         >>> from newsdash import NewsDash
         >>> import asyncio
         >>> async def main():
@@ -477,15 +514,15 @@
                 raise TypeError("pageSize should be an integer")
             params["pageSize"] = pageSize
         if page is not None:
             if not isinstance(page, int):
                 raise TypeError("page should be an integer")
             params["page"] = page
         headers = {"X-Api-Key": self.api_key}
-        data = await self._http_client.request(
+        data: newsapiGetTopHeadlinesResponse = await self._http_client.request(
             "https://newsapi.org/v2/top-headlines",
             "GET",
             headers=headers,
             params=params,
         )
         if data:
             return data
@@ -585,15 +622,15 @@
         language : typinp.Literal["ar", "de", "en", "es", "fr", "he", "it", "nl", "no", "pt", "ru", "sv", "ud", "zh"], optional
             The 2-letter ISO-639-1 code of the language you want to get headlines for. Possible options: ar de en es fr he it nl no pt ru sv ud zh, by default None
         category : typing.Literal["business","entertainment","general","health","science","sports","technology"] , optional
             The category you want to get headlines for. Possible options: business entertainment general health science sports technology, by default None
 
         Returns
         -------
-         typing.Any
+        newsapiGetSourcesResponse
             The response from NewsApi after getting sources.
 
         Raises
         ------
         HTTPException
             raises HTTPException if the status code is not `ok`.
 
@@ -699,15 +736,15 @@
                 "ud",
                 "zh",
             ]:
                 raise ValueError(
                     "language should be one out of languages provided by newsapi"
                 )
         headers = {"X-Api-Key": self.api_key}
-        data = await self._http_client.request(
+        data: newsapiGetSourcesResponse = await self._http_client.request(
             "https://newsapi.org/v2/top-headlines",
             "GET",
             headers=headers,
             params=params,
         )
         if data:
             return data
```

### Comparing `newsdash-0.1.0a1/newsdash/exceptions.py` & `newsdash-0.1.1a0/newsdash/exceptions.py`

 * *Files identical despite different names*

### Comparing `newsdash-0.1.0a1/newsdash/http.py` & `newsdash-0.1.1a0/newsdash/_http.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 import typing as tp
 from .exceptions import HTTPException
 
 if tp.TYPE_CHECKING:
     import loguru
 
 
+class errorResponse(tp.TypedDict):
+    status: tp.Literal["ok", "error"]
+    code: str
+    message: str
+
+
 class HttpClient:
     """
     The HTTP client that NewsDash is using
 
     Attributes
     ----------
     session : aiohttp.ClientSession, optional
@@ -64,32 +70,30 @@
         params : dict, optional
             The params for url for making request, by default {}
         headers : dict, optional
             The headers for url for making request, by default {}
 
         Returns
         -------
-        tp.Any
+        dict
             The response from api.
 
         Raises
         ------
         HTTPException.from_response
             If you get bad response codes.
-        HTTPException
-            If the session is not provided
         """
         if self.session is None:
             await self.connect()
-        if self.session is not None:
-            async with self.session.request(
-                method, url, params=params, headers=headers
-            ) as response:
-                if 300 > response.status >= 200:
-                    return await response.json()
-                else:
-                    resp = await response.json()
-                    message = f"received status code {response.status} with code > {resp['code']}"
-                    self.logger.error(message)
-                    raise HTTPException.from_response(await response.json())
-        else:
-            raise HTTPException("No session was provided")
+        async with self.session.request(
+            method, url, params=params, headers=headers
+        ) as response:
+            if 300 > response.status >= 200:
+                response = await response.json()
+                return response
+            else:
+                resp: errorResponse = await response.json()
+                message = (
+                    f"received status code {response.status} with code > {resp['code']}"
+                )
+                self.logger.error(message)
+                raise HTTPException.from_response(await response.json())
```

### Comparing `newsdash-0.1.0a1/pyproject.toml` & `newsdash-0.1.1a0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "newsdash"
-version = "0.1.0a1"
+version = "0.1.1a0"
 description = "NewsDash is a fast and reliable Python wrapper for the News API that simplifies accessing the latest news articles from around the world."
 license = "MIT"
 authors = ["NaviTheCoderboi <navindersingh568@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/NaviTheCoderboi/NewsDash"
 documentation = "https://NaviTheCoderboi.github.io/NewsDash"
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha"
+    "Development Status :: 3 - Alpha"
 ]
 packages = [
     { include = "newsdash" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.4"
 loguru = "^0.6.0"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+ruff = "^0.0.263"
 mkdocs = "^1.4.2"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 mkdocs-material = "^9.1.6"
 pygments = "^2.15.0"
 
-[tool.poetry.dev-dependencies]
-black = "^23.3.0"
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
+[tool.ruff]
+line-length = 380
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `newsdash-0.1.0a1/PKG-INFO` & `newsdash-0.1.1a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: newsdash
-Version: 0.1.0a1
+Version: 0.1.1a0
 Summary: NewsDash is a fast and reliable Python wrapper for the News API that simplifies accessing the latest news articles from around the world.
 Home-page: https://github.com/NaviTheCoderboi/NewsDash
 License: MIT
 Author: NaviTheCoderboi
 Author-email: navindersingh568@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
-Requires-Dist: mkdocs-material (>=9.1.6,<10.0.0)
-Requires-Dist: mkdocstrings[python] (>=0.21.2,<0.22.0)
-Requires-Dist: pygments (>=2.15.0,<3.0.0)
 Project-URL: Documentation, https://NaviTheCoderboi.github.io/NewsDash
 Project-URL: Repository, https://github.com/NaviTheCoderboi/NewsDash
 Description-Content-Type: text/markdown
 
 ![NewsDash](./readme-assets/poster.jpg)
 # NewsDash
 [![Python 3.9-3.11](https://img.shields.io/badge/Python-3.9--3.11-blue.svg)]()
```

