# Comparing `tmp/bib_lookup-0.0.8.tar.gz` & `tmp/bib_lookup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bib_lookup-0.0.8.tar", last modified: Sun Apr 10 14:24:59 2022, max compression
+gzip compressed data, was "dist/bib_lookup-0.0.9.tar", last modified: Tue Apr 12 06:28:48 2022, max compression
```

## Comparing `bib_lookup-0.0.8.tar` & `bib_lookup-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6239 2022-04-10 13:49:47.000000 bib_lookup-0.0.8/README.md
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1576 2022-04-06 03:38:18.000000 bib_lookup-0.0.8/setup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       38 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/setup.cfg
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8452 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/PKG-INFO
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/bib_lookup.egg-info/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       11 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/bib_lookup.egg-info/top_level.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      478 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/bib_lookup.egg-info/SOURCES.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        1 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/bib_lookup.egg-info/dependency_links.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8452 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/bib_lookup.egg-info/PKG-INFO
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       52 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/bib_lookup.egg-info/entry_points.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      124 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/bib_lookup.egg-info/requires.txt
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/test/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      409 2022-04-07 15:03:53.000000 bib_lookup-0.0.8/test/test_checking.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1211 2022-04-06 02:15:52.000000 bib_lookup-0.0.8/test/test_io.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2634 2022-04-06 02:15:52.000000 bib_lookup-0.0.8/test/test_doi_bib_lookup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1564 2022-04-06 02:15:52.000000 bib_lookup-0.0.8/test/test_arxiv_bib_lookup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2866 2022-04-06 02:15:52.000000 bib_lookup-0.0.8/test/test_pubmed_bib_lookup.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-04-10 14:24:59.000000 bib_lookup-0.0.8/bib_lookup/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     7000 2022-04-10 03:19:08.000000 bib_lookup-0.0.8/bib_lookup/utils.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      119 2022-03-31 03:40:32.000000 bib_lookup-0.0.8/bib_lookup/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    29832 2022-04-10 03:19:08.000000 bib_lookup-0.0.8/bib_lookup/bib_lookup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    19547 2022-04-07 15:03:53.000000 bib_lookup-0.0.8/bib_lookup/_bib.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       22 2022-04-10 14:24:38.000000 bib_lookup-0.0.8/bib_lookup/version.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4981 2022-04-07 15:03:53.000000 bib_lookup-0.0.8/bib_lookup/cli.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    11234 2022-04-12 04:08:23.000000 bib_lookup-0.0.9/README.md
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1576 2022-04-06 03:38:18.000000 bib_lookup-0.0.9/setup.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       38 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/setup.cfg
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    14823 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/PKG-INFO
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/bib_lookup.egg-info/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       11 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/bib_lookup.egg-info/top_level.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      478 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/bib_lookup.egg-info/SOURCES.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        1 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/bib_lookup.egg-info/dependency_links.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    14823 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/bib_lookup.egg-info/PKG-INFO
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       52 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/bib_lookup.egg-info/entry_points.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      124 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/bib_lookup.egg-info/requires.txt
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/test/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      409 2022-04-07 15:03:53.000000 bib_lookup-0.0.9/test/test_checking.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1211 2022-04-06 02:15:52.000000 bib_lookup-0.0.9/test/test_io.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2634 2022-04-06 02:15:52.000000 bib_lookup-0.0.9/test/test_doi_bib_lookup.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1564 2022-04-06 02:15:52.000000 bib_lookup-0.0.9/test/test_arxiv_bib_lookup.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2866 2022-04-06 02:15:52.000000 bib_lookup-0.0.9/test/test_pubmed_bib_lookup.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-04-12 06:28:48.000000 bib_lookup-0.0.9/bib_lookup/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     7000 2022-04-10 03:19:08.000000 bib_lookup-0.0.9/bib_lookup/utils.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      119 2022-03-31 03:40:32.000000 bib_lookup-0.0.9/bib_lookup/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    31083 2022-04-12 04:08:23.000000 bib_lookup-0.0.9/bib_lookup/bib_lookup.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    19610 2022-04-10 15:19:57.000000 bib_lookup-0.0.9/bib_lookup/_bib.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       22 2022-04-12 06:27:22.000000 bib_lookup-0.0.9/bib_lookup/version.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4981 2022-04-07 15:03:53.000000 bib_lookup-0.0.9/bib_lookup/cli.py
```

### Comparing `bib_lookup-0.0.8/setup.py` & `bib_lookup-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `bib_lookup-0.0.8/test/test_io.py` & `bib_lookup-0.0.9/test/test_io.py`

 * *Files identical despite different names*

### Comparing `bib_lookup-0.0.8/test/test_doi_bib_lookup.py` & `bib_lookup-0.0.9/test/test_doi_bib_lookup.py`

 * *Files identical despite different names*

### Comparing `bib_lookup-0.0.8/test/test_arxiv_bib_lookup.py` & `bib_lookup-0.0.9/test/test_arxiv_bib_lookup.py`

 * *Files identical despite different names*

### Comparing `bib_lookup-0.0.8/test/test_pubmed_bib_lookup.py` & `bib_lookup-0.0.9/test/test_pubmed_bib_lookup.py`

 * *Files identical despite different names*

### Comparing `bib_lookup-0.0.8/bib_lookup/utils.py` & `bib_lookup-0.0.9/bib_lookup/utils.py`

 * *Files identical despite different names*

### Comparing `bib_lookup-0.0.8/bib_lookup/bib_lookup.py` & `bib_lookup-0.0.9/bib_lookup/bib_lookup.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,27 +107,27 @@
     """
 
     __name__ = "BibLookup"
 
     def __init__(
         self,
         align: str = "middle",
-        ignore_fields: Sequence[str] = ["url"],
+        ignore_fields: Union[str, Sequence[str]] = ["url"],
         output_file: Optional[Union[str, Path]] = None,
         email: Optional[str] = None,
         **kwargs,
     ) -> NoReturn:
         """
 
         Parameters
         ----------
         align: str, default "middle",
             alignment of the final output, case insensitive,
             can be one of "middle", "left", "left-middle", "left_middle"
-        ignore_fields: sequence of str, default ["url"],
+        ignore_fields: str or sequence of str, default ["url"],
             fields to be ignored in the final output,
             case insensitive
         output_file: str or Path, optional,
             the file to save the lookup results,
             append mode is used if the file exists
         email: str, optional,
             email for querying PubMed publications
@@ -152,15 +152,18 @@
         if self.output_file is not None:
             assert (
                 self.output_file.suffix == ".bib"
             ), f"output_file must be a .bib file, but got {self.output_file}"
             self.output_file.parent.mkdir(parents=True, exist_ok=True)
         self.__cached_lookup_results = OrderedDict()
         self.email = email
-        self._ignore_fields = [k.lower() for k in ignore_fields]
+        if isinstance(ignore_fields, str):
+            self._ignore_fields = [ignore_fields.lower()]
+        else:
+            self._ignore_fields = [k.lower() for k in ignore_fields]
         assert self.align in [
             "middle",
             "left",
             "left-middle",
             "left_middle",
         ]
         colon = "[\\s]*:[\\s]*"
@@ -190,58 +193,66 @@
             f"((?:(?:(?:https?:\\/\\/)?arxiv.org\\/)?abs\\/)|(arxiv{colon}))"
         )
         self.__arxiv_pattern = f"^(?:{self.__arxiv_pattern_prefix})?(?:([\\w\\-]+\\/\\d+)|(\\d+\\.\\d+(v(\\d+))?))$"
         # self.__arxiv_pattern_old = f"^(?:{self.__arxiv_pattern_prefix})?[\\w\\-]+\\/\\d+$"
         self.__default_err = "Not Found"
         self.__header_pattern = "^@(?P<entry_type>\\w+)\\{(?P<label>[^,]+)"
 
+        self._arxiv2doi = kwargs.get("arxiv2doi", False)
         self.verbose = kwargs.get("verbose", 0)
         self._ordering = kwargs.get(
             "ordering", ["author", "title", "journal", "booktitle"]
         )
         self._ordering = [k.lower() for k in self._ordering]
         self._comment_pattern = re.compile(r"^%")
 
         self.__info_color = "blue"
         self.__err_color = "red"
         self.__err_fontsize = "large"
 
     def __call__(
-        self, identifier: Union[Path, str, Sequence[str]], align: Optional[str] = None
+        self,
+        identifier: Union[Path, str, Sequence[str]],
+        align: Optional[str] = None,
+        ignore_fields: Optional[Union[str, Sequence[str]]] = None,
     ) -> str:
         """
 
         Parameters
         ----------
         identifier: Path or str or sequence of str,
             identifier of a publication,
             can be DOI, PMID (or url), PMCID (or url), arXiv id, etc.
         align: str, optional,
             alignment of the final output, case insensitive,
             if specified, `self.align` is ignored
+        ignore_fields: str or sequence of str, optional,
+            fields to be ignored in the final output,
+            case insensitive,
+            if specified, `self._ignore_fields` is ignored
 
         Returns
         -------
         res: str,
             the final output in the `str` format
 
         """
         if isinstance(identifier, Path):
             identifier = [
                 line for line in identifier.read_text().splitlines() if len(line) > 0
             ]
-            return self(identifier, align)
+            return self(identifier, align, ignore_fields)
         if isinstance(identifier, str):
             if Path(identifier).exists():
-                return self(Path(identifier), align)
+                return self(Path(identifier), align, ignore_fields)
         elif isinstance(identifier, Sequence):
             assert all(
                 [isinstance(i, str) for i in identifier]
             ), f"identifier must be a string or a sequence of strings, but got {identifier}"
-            return "\n".join(self(item, align) for item in identifier)
+            return "\n".join(self(item, align, ignore_fields) for item in identifier)
         else:
             raise TypeError(
                 f"identifier must be a string or a sequence of strings, but got {identifier}"
             )
 
         category, feed_content, idtf = self._obtain_feed_content(identifier)
         if category == "doi":
@@ -250,24 +261,24 @@
             res = self._handle_pm(feed_content)
         elif category == "arxiv":
             res = self._handle_arxiv(feed_content)
         elif category == "error":
             res = self.default_err
 
         if res != self.default_err:
-            res = self._to_bib_item(res, idtf, align)
+            res = self._to_bib_item(res, idtf, align, ignore_fields)
             self.__cached_lookup_results[identifier] = res
 
         if self.verbose >= 1:
             if res == self.default_err:
                 print_func(
                     process_text(res, self.__err_color, font_size=self.__err_fontsize)
                 )
             else:
-                print_func(res)
+                print(res)
 
         return str(res)
 
     def _obtain_feed_content(self, identifier: str) -> Tuple[str, dict, str]:
         """
 
         Parameters
@@ -320,14 +331,17 @@
                 idtf,
             ).strip("/")
             url = "http://export.arxiv.org/api/query?id_list=" + idtf
             fc = {
                 "url": url,
             }
             category = "arxiv"
+            if self._arxiv2doi:
+                idtf = f"10.48550/arXiv.{idtf}"
+                return self._obtain_feed_content(idtf)
         else:
             warnings.warn(
                 "unrecognized indentifier (none of doi, pmid, pmcid, pmurl, arxiv)"
             )
             category, fc = "error", {}
         if self.verbose > 1:
             print_func(f"category = {process_text(category, self.__info_color)}")
@@ -351,16 +365,18 @@
         -------
         res: str,
             decoded query result
 
         """
         r = requests.post(**feed_content)
         res = r.content.decode("utf-8")
-        if self.verbose > 1:
+        if self.verbose > 3:
             print_func(res)
+        if "DOI Not Found" in res:
+            return self.default_err
         return res
 
     def _handle_pm(self, feed_content: dict) -> str:
         """
 
         handle a PubMed query using POST
 
@@ -376,15 +392,15 @@
 
         """
         r = requests.post(**feed_content)
         if self.verbose > 1:
             print_func(r.json())
         mid_res = r.json()["records"][0]
         doi = mid_res.get("doi", "")
-        if self.verbose > 1:
+        if self.verbose > 3:
             print_func(f"doi = {doi}")
         if doi:
             _, feed_content, _ = self._obtain_feed_content(doi)
             res = self._handle_doi(feed_content)
         else:
             res = self.default_err
         return res
@@ -403,29 +419,23 @@
         -------
         res: dict,
             decoded and parsed query result
 
         """
         r = requests.get(**feed_content)
         parsed = feedparser.parse(r.content.decode("utf-8")).entries[0]
-        if self.verbose > 1:
+        if self.verbose > 3:
             print_func(parsed)
         title = re.sub("[\\s]+", " ", parsed["title"])  # sometimes this field has "\n"
         if title == "Error":
             res = self.default_err
             return res
         arxiv_id = parsed["id"].split("arxiv.org/abs/")[-1]
         year = parsed["published_parsed"].tm_year
         res = {"title": title}
-        # authors = []
-        # for item in parsed["authors"]:
-        #     a = item["name"].split(" ")
-        #     if len(a) > 1:
-        #         a[-2] = a[-2] + ","
-        #     authors.append(" ".join(a))
         # it seems that surnames are put in the last position of full names by arXiv
         authors = [item["name"] for item in parsed["authors"]]
         res["author"] = " and ".join(authors)
         res["year"] = year
         res["month"] = parsed["published_parsed"].tm_mon
         res["journal"] = f"arXiv preprint arXiv:{arxiv_id}"
         res[
@@ -435,14 +445,15 @@
         return res
 
     def _to_bib_item(
         self,
         res: Union[str, Dict[str, str]],
         identifier: Optional[str] = None,
         align: Optional[str] = None,
+        ignore_fields: Optional[Union[str, Sequence[str]]] = None,
     ) -> BibItem:
         """
 
         Parameters
         ----------
         res: str or dict,
             result obtained via GET or POST,
@@ -450,21 +461,31 @@
         identifier: str, optional,
             identifier of a publication,
             can be DOI, PMID (or url), PMCID (or url), arXiv id, etc.
             if not provided, "label" from the result will be used as `identifier`
         align: str, optional,
             alignment of the final output, case insensitive,
             if specified, `self.align` is ignored
+        ignore_fields: str or sequence of str, optional,
+            fields to be ignored in the final output,
+            case insensitive,
+            if specified, `self._ignore_fields` is ignored
 
         Returns
         -------
         bib_item: BibItem,
             a BibItem instance converted from `res`
 
         """
+        if ignore_fields is None:
+            _ignore_fields = self.ignore_fields
+        elif isinstance(ignore_fields, str):
+            _ignore_fields = [ignore_fields.lower()]
+        else:
+            _ignore_fields = [k.lower() for k in ignore_fields]
         _align = (align or self.align).lower()
         assert _align in [
             "middle",
             "left",
             "left-middle",
             "left_middle",
         ], f"align must be one of 'middle', 'left', 'left-middle', 'left_middle', but got {_align}"
@@ -492,20 +513,26 @@
                 {
                     k.strip(): str(v).strip(", ")
                     for k, v in res.items()
                     if k not in ["entry_type", "label"]
                 }
             )
 
+        # replace the "_" in title with "\_"
+        if "title" in field_dict:
+            field_dict["title"] = (
+                field_dict["title"].replace("_", r"\_").replace(r"\\_", r"\_")
+            )
+
         # all field names to lower case,
-        # and ignore the fields in the list `self.ignore_fields`
+        # and ignore the fields in the list `_ignore_fields`
         field_dict = {
             k.lower(): v
             for k, v in field_dict.items()
-            if k.lower() not in self.ignore_fields
+            if k.lower() not in _ignore_fields
         }
 
         # re-order the fields according to the list `self.ordering`
         _ordering = self.ordering + [k for k in field_dict if k not in self.ordering]
         _ordering = [k for k in _ordering if k in field_dict]
         field_dict = OrderedDict((k, field_dict[k]) for k in _ordering)
```

### Comparing `bib_lookup-0.0.8/bib_lookup/_bib.py` & `bib_lookup-0.0.9/bib_lookup/_bib.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,16 @@
         }
         >>> bib_item == bl[bl[0]]
         False
         >>> bib_item.__eq__(bl[bl[0]], strict=True)
         True
 
         """
+        if type(other) != type(self):
+            return False
         if self.entry_type != other.entry_type:
             return False
         if not strict:
             if self.label != other.label:
                 return False
             else:
                 return True
```

### Comparing `bib_lookup-0.0.8/bib_lookup/cli.py` & `bib_lookup-0.0.9/bib_lookup/cli.py`

 * *Files identical despite different names*

