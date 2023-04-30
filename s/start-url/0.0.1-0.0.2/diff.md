# Comparing `tmp/start_url-0.0.1.tar.gz` & `tmp/start_url-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_url-0.0.1.tar", max compression
+gzip compressed data, was "start_url-0.0.2.tar", max compression
```

## Comparing `start_url-0.0.1.tar` & `start_url-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      241 2023-04-30 10:15:23.540749 start_url-0.0.1/README.md
--rw-r--r--   0        0        0     1535 2023-04-30 10:22:11.298738 start_url-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      119 2023-04-30 10:16:20.443899 start_url-0.0.1/start_url/__init__.py
--rw-r--r--   0        0        0      825 2023-04-30 10:18:52.801435 start_url-0.0.1/start_url/headers.py
--rw-r--r--   0        0        0     1574 2023-04-30 10:19:34.982114 start_url-0.0.1/start_url/main.py
--rw-r--r--   0        0        0     3642 2023-04-30 10:15:40.746706 start_url-0.0.1/start_url/meta.py
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 start_url-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-04-30 10:15:23.540749 start_url-0.0.2/README.md
+-rw-r--r--   0        0        0     1559 2023-04-30 12:16:46.231810 start_url-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-04-30 12:16:42.493825 start_url-0.0.2/start_url/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-30 11:48:56.827103 start_url-0.0.2/start_url/headers.py
+-rw-r--r--   0        0        0     2087 2023-04-30 12:15:28.250110 start_url-0.0.2/start_url/main.py
+-rw-r--r--   0        0        0     3630 2023-04-30 11:47:57.924317 start_url-0.0.2/start_url/meta.py
+-rw-r--r--   0        0        0     2030 2023-04-30 12:12:27.894551 start_url-0.0.2/start_url/repo.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 start_url-0.0.2/PKG-INFO
```

### Comparing `start_url-0.0.1/pyproject.toml` & `start_url-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "start-url"
 description = "httpx.get URL metadata with BeautifulSoup"
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-url"
 documentation = "https://mv3.dev/start-url"
 classifiers = [
@@ -13,18 +13,19 @@
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-dotenv = "^0.21"
+python-dotenv = "^1.0"
 python-dateutil = "^2.8.2"
 beautifulsoup4 = "^4.11.2"
 httpx = "^0.23.3"
+start-sdk = "^0.0.22"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3"
 black = "^23.1.0"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
@@ -33,15 +34,15 @@
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.0.13"
 ipython = "^8.13.1"
 ipykernel = "^6.22.0"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
-addopts = "-ra -q --doctest-modules start_"
+addopts = "-ra -q --doctest-modules start_url"
 testpaths = ["tests"]
 
 [tool.ruff]
 ignore = ["F401"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
```

### Comparing `start_url-0.0.1/start_url/headers.py` & `start_url-0.0.2/start_url/headers.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Self
 
 import httpx
 from dateutil.parser import parse
 
 
 @dataclass
-class HTMLHeaders:
+class SimpleResponseHeaders:
     content_type: str
     etag: str | None
     last_modified: datetime.datetime | None
     last_checked: datetime.datetime | None
 
     @classmethod
     def from_raw_headers(cls, data: httpx.Headers) -> Self | None:
```

### Comparing `start_url-0.0.1/start_url/main.py` & `start_url-0.0.2/start_url/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,64 @@
 from dataclasses import asdict, dataclass
 from http import HTTPStatus
 from urllib.parse import urlparse
 
 import httpx
 from bs4 import BeautifulSoup
 
-from .headers import HTMLHeaders
-from .meta import SimplifiedMeta
+from .headers import SimpleResponseHeaders
+from .meta import SimpleMeta
+from .repo import GithubRepo
 
 
 @dataclass
 class InspectedURL:
     url: str
-    head: httpx.Headers
-    content: bytes
+    head: httpx.Headers | None = None
+    content: bytes | None = None
 
     def __post_init__(self):
         r = httpx.get(self.url, follow_redirects=True)
         if not r.status_code == HTTPStatus.OK:
             raise Exception(f"Bad {self.url}: {r.status_code}")
         self.head = r.headers
         self.content = r.content
 
-    def prep(self, obj) -> dict:
-        return asdict(obj) if obj is not None else {}
+    def prep(self, dc) -> dict:
+        """Must be a dataclass."""
+        return {dc.__class__.__name__: asdict(dc)} if dc is not None else {}
 
     @property
-    def url_data(self) -> dict:
+    def parsed_url(self) -> dict:
         """Generates the parts of urlparse.ParsedResult as a dictionary."""
         parsed = urlparse(self.url)
-        return {k: getattr(parsed, k) for k in parsed._fields}
+        return {
+            "ParsedResult": {k: getattr(parsed, k) for k in parsed._fields}
+        }
 
     @property
-    def site_headers(self) -> HTMLHeaders | None:
+    def site_headers(self) -> SimpleResponseHeaders | None:
         """Selected HTML headers, requires content-type to include `text/html`."""
-        return HTMLHeaders.from_raw_headers(data=self.head)
+        if self.head:
+            return SimpleResponseHeaders.from_raw_headers(data=self.head)
 
     @property
-    def site_meta(self) -> SimplifiedMeta | None:
+    def site_meta(self) -> SimpleMeta | None:
         """Simplified summary of meta tags."""
-        html_soup = BeautifulSoup(self.content, "html.parser")
-        return SimplifiedMeta.from_soup(html_soup)
+        if self.content:
+            html_soup = BeautifulSoup(self.content, "html.parser")
+            return SimpleMeta.from_soup(html_soup)
+
+    @property
+    def repo_meta(self) -> GithubRepo | None:
+        """Usable fields from Github repository, requires Github token."""
+        if raw_data := GithubRepo.matches(self.url):
+            return GithubRepo(**raw_data)
 
     @property
     def export(self):
-        """Combines url, header, meta info into a single dictionary."""
-        url = self.url_data
+        """Combine url, header, meta, repo key-value pairs."""
+        data = self.parsed_url
         head = self.prep(self.site_headers) or {}
         meta = self.prep(self.site_meta) or {}
-        return url | head | meta
+        repo = self.prep(self.repo_meta) or {}
+        return data | head | meta | repo
```

### Comparing `start_url-0.0.1/start_url/meta.py` & `start_url-0.0.2/start_url/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'meta[name="author"]',
     'meta[name="twitter:creator"]',
 )
 TYPE = ('meta[property="og:type"]',)
 
 
 @dataclass
-class SimplifiedMeta:
+class SimpleMeta:
     """Extract generic website metadata based on a url fetched on a certain date.
 
     All of the fields, except the date, default to `None`.
 
     Field | Type | Description
     :--:|:--:|:--
     title | str | First matching title parsed from `<meta>` CSS selectors (and the `<title>` tag)
@@ -88,17 +88,17 @@
 
         Note the special rule on `title` as a selector.
 
         Examples:
             >>> from pathlib import Path
             >>> html = Path(__file__).parent.parent / "tests" / "data" / "test.html"
             >>> soup = BeautifulSoup(html.read_text(), "html.parser")
-            >>> SimplifiedMeta.select(soup, TITLE)
+            >>> SimpleMeta.select(soup, TITLE)
             'Hello World From Twitter Title!'
-            >>> SimplifiedMeta.select(soup, DESC)
+            >>> SimpleMeta.select(soup, DESC)
             'this is a description from twitter:desc'
 
         Args:
             soup (BeautifulSoup): Converted html content into a soup object
             selectors (Iterable[str]): CSS selectors as a tuple
 
         Returns:
```

### Comparing `start_url-0.0.1/PKG-INFO` & `start_url-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: start-url
-Version: 0.0.1
+Version: 0.0.2
 Summary: httpx.get URL metadata with BeautifulSoup
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: python-dotenv (>=0.21,<0.22)
+Requires-Dist: python-dotenv (>=1.0,<2.0)
+Requires-Dist: start-sdk (>=0.0.22,<0.0.23)
 Project-URL: Documentation, https://mv3.dev/start-url
 Project-URL: Repository, https://github.com/justmars/start-url
 Description-Content-Type: text/markdown
 
 # start-url
 
 ![Github CI](https://github.com/justmars/start-url/actions/workflows/main.yml/badge.svg)
```

