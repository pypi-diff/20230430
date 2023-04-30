# Comparing `tmp/pagemeta-0.0.1.tar.gz` & `tmp/pagemeta-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagemeta-0.0.1.tar", max compression
+gzip compressed data, was "pagemeta-0.0.2.tar", max compression
```

## Comparing `pagemeta-0.0.1.tar` & `pagemeta-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      237 2023-03-17 04:25:29.899823 pagemeta-0.0.1/README.md
--rw-r--r--   0        0        0       49 2023-03-17 04:25:29.900345 pagemeta-0.0.1/pagemeta/__init__.py
--rw-r--r--   0        0        0     4405 2023-03-17 04:30:00.808924 pagemeta-0.0.1/pagemeta/main.py
--rw-r--r--   0        0        0     1526 2023-03-17 04:29:05.400223 pagemeta-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 pagemeta-0.0.1/setup.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 pagemeta-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      237 2023-03-17 04:25:29.899823 pagemeta-0.0.2/README.md
+-rw-r--r--   0        0        0       76 2023-04-30 08:33:35.210012 pagemeta-0.0.2/pagemeta/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-30 08:19:59.914858 pagemeta-0.0.2/pagemeta/headers.py
+-rw-r--r--   0        0        0      881 2023-04-30 08:20:20.198218 pagemeta-0.0.2/pagemeta/main.py
+-rw-r--r--   0        0        0     3624 2023-04-30 08:34:53.941419 pagemeta-0.0.2/pagemeta/meta.py
+-rw-r--r--   0        0        0     1553 2023-04-30 08:33:31.539006 pagemeta-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 pagemeta-0.0.2/PKG-INFO
```

### Comparing `pagemeta-0.0.1/pagemeta/main.py` & `pagemeta-0.0.2/pagemeta/meta.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,104 @@
-import datetime
 from dataclasses import dataclass
 from typing import Iterable
-from urllib.parse import urlparse
 
-import httpx
 from bs4 import BeautifulSoup
 
-META_TITLE_SELECTORS = (
+TITLE = (
     'meta[name="twitter:title"]',
     'meta[property="og:title"]',
     "title",
 )
-META_DESC_SELECTORS = (
+DESC = (
     'meta[name="twitter:description"]',
     'meta[property="og:description"]',
     'meta[name="description"]',
 )
-META_IMAGE_SELECTORS = (
+IMG = (
     'meta[name="twitter:image"]',
     'meta[property="og:image"]',
 )
-META_TYPE_SELECTORS = ('meta[property="og:type"]',)
+AUTHOR = (
+    'meta[name="author"]',
+    'meta[name="twitter:creator"]',
+)
+TYPE = ('meta[property="og:type"]',)
 
 
 @dataclass
 class PageMeta:
     """Extract generic website metadata based on a url fetched on a certain date.
 
     All of the fields, except the date, default to `None`.
 
     Field | Type | Description
     :--:|:--:|:--
-    id | str | Generated id based on the url's path
-    etag | str | ETag header on `date` fetched
-    netloc | str | URL domain
-    path | str | URL path
     title | str | First matching title parsed from `<meta>` CSS selectors (and the `<title>` tag)
     description | str | First matching description Parsed from `<meta>` CSS selectors
-    og_img_url | str | An [open graph](https://ogp.me/) (OG) image url detected
-    og_type | str | A type detected from OG values
-    soup | BeautifulSoup | See bs4 [docs](https://www.crummy.com/software/BeautifulSoup)
-    date | str | The date metadata was fetched in ISO Format
+    author | str | Either the author or the creator, if the author is absent
+    image | str | An [open graph](https://ogp.me/) (OG) image url detected
+    category | str | A type detected from OG ("og:type") values
     """  # noqa: E501
 
-    url: str
-    id: str | None = None
-    etag: str | None = None
-    netloc: str | None = None
-    path: str | None = None
     title: str | None = None
     description: str | None = None
-    og_img_url: str | None = None
-    og_type: str | None = None
-    date: str = datetime.datetime.now().isoformat()
-    soup: BeautifulSoup | None = None
-
-    def __post_init__(self):
-        parsed = urlparse(self.url)
-        r = httpx.get(self.url)
-        self.soup = BeautifulSoup(r.content, "html.parser")
-        self.id = parsed.path.removeprefix("/").removesuffix("/")
-        self.netloc = parsed.netloc
-        self.path = parsed.path
-        self.etag = r.headers.get("etag")
-        self.title = self.select(self.soup, META_TITLE_SELECTORS)
-        self.description = self.select(self.soup, META_DESC_SELECTORS)
-        self.og_img_url = self.select(self.soup, META_IMAGE_SELECTORS)
-        self.og_type = self.select(self.soup, META_TYPE_SELECTORS)
+    author: str | None = None
+    image: str | None = None
+    category: str | None = None
 
-    def __repr__(self) -> str:
-        return f"PageMeta: {self.netloc}/{self.path}"
+    @classmethod
+    def from_soup(cls, soup: BeautifulSoup):
+        return cls(
+            title=cls.select(soup, TITLE),
+            description=cls.select(soup, DESC),
+            author=cls.select(soup, AUTHOR),
+            image=cls.select(soup, IMG),
+            category=cls.select(soup, TYPE),
+        )
 
     @classmethod
     def select(
         cls, soup: BeautifulSoup, selectors: Iterable[str]
     ) -> str | None:
         """The order of CSS selectors. The first one
         matched, retrieves the content, if found.
 
         See present list of selectors used to extract content:
 
         ```py
-        META_TITLE_SELECTORS = (
+        TITLE = (
             'meta[name="twitter:title"]',
             'meta[property="og:title"]',
             "title",
         )
-        META_DESC_SELECTORS = (
+        DESC = (
             'meta[name="twitter:description"]',
             'meta[property="og:description"]',
             'meta[name="description"]',
         )
-        META_IMAGE_SELECTORS = (
+        IMG = (
             'meta[name="twitter:image"]',
             'meta[property="og:image"]',
         )
-        META_TYPE_SELECTORS = ('meta[property="og:type"]',)
+        AUTHOR = (
+            'meta[name="author"]',
+            'meta[name="twitter:creator"]',
+        )
+        TYPE = ('meta[property="og:type"]',)
         ```
 
         Note the special rule on `title` as a selector.
 
         Examples:
             >>> from pathlib import Path
             >>> html = Path(__file__).parent.parent / "tests" / "data" / "test.html"
             >>> soup = BeautifulSoup(html.read_text(), "html.parser")
-            >>> PageMeta.select(soup, META_TITLE_SELECTORS)
+            >>> PageMeta.select(soup, TITLE)
             'Hello World From Twitter Title!'
-            >>> PageMeta.select(soup, META_DESC_SELECTORS)
+            >>> PageMeta.select(soup, DESC)
             'this is a description from twitter:desc'
 
         Args:
             soup (BeautifulSoup): Converted html content into a soup object
             selectors (Iterable[str]): CSS selectors as a tuple
 
         Returns:
@@ -119,9 +107,10 @@
         for selector in selectors:
             if selector.startswith("meta"):
                 if desc := soup.select(selector):
                     if content := desc[0].get("content"):
                         if content and isinstance(content, str):
                             return content
             elif selector == "title":
-                return soup("title")[0].get_text()
+                if titles := soup("title"):
+                    return titles[0].get_text()
         return None
```

### Comparing `pagemeta-0.0.1/pyproject.toml` & `pagemeta-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pagemeta"
 description = "Extract Open Graph metadata from a URL via BeautifulSoup."
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/pagemeta"
 documentation = "https://mv3.dev/pagemeta"
 classifiers = [
@@ -16,14 +16,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.21"
 beautifulsoup4 = "^4.11.2"
 httpx = "^0.23.3"
+python-dateutil = "^2.8.2"
 
 [tool.poetry.group.dev.dependencies] # latest as of Jan. 2023
 rich = "^13.3"
 black = "^23.1.0"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
```

### Comparing `pagemeta-0.0.1/PKG-INFO` & `pagemeta-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagemeta
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extract Open Graph metadata from a URL via BeautifulSoup.
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21,<0.22)
 Project-URL: Documentation, https://mv3.dev/pagemeta
 Project-URL: Repository, https://github.com/justmars/pagemeta
 Description-Content-Type: text/markdown
 
 # pagemeta
```

