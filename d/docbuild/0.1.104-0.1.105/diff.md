# Comparing `tmp/docbuild-0.1.104.tar.gz` & `tmp/docbuild-0.1.105.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.104.tar", last modified: Sun Apr 30 08:43:50 2023, max compression
+gzip compressed data, was "docbuild-0.1.105.tar", last modified: Sun Apr 30 11:58:07 2023, max compression
```

## Comparing `docbuild-0.1.104.tar` & `docbuild-0.1.105.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 08:43:50.971772 docbuild-0.1.104/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-30 08:43:50.971573 docbuild-0.1.104/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.104/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 08:43:50.967685 docbuild-0.1.104/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-30 08:43:40.000000 docbuild-0.1.104/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.104/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.104/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.104/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7054 2023-04-29 18:09:32.000000 docbuild-0.1.104/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 08:43:50.970125 docbuild-0.1.104/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.104/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.104/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.104/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.104/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.104/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     5805 2023-04-30 08:43:31.000000 docbuild-0.1.104/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.104/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 08:43:50.971205 docbuild-0.1.104/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.104/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12474 2023-04-27 10:55:27.000000 docbuild-0.1.104/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      193 2023-04-27 11:06:55.000000 docbuild-0.1.104/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16325 2023-04-30 05:58:58.000000 docbuild-0.1.104/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 08:43:50.968601 docbuild-0.1.104/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-30 08:43:50.000000 docbuild-0.1.104/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-30 08:43:50.000000 docbuild-0.1.104/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-30 08:43:50.000000 docbuild-0.1.104/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-30 08:43:50.000000 docbuild-0.1.104/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-30 08:43:50.000000 docbuild-0.1.104/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-30 08:43:50.971820 docbuild-0.1.104/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      832 2023-04-30 08:43:45.000000 docbuild-0.1.104/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.555246 docbuild-0.1.105/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-30 11:58:07.554589 docbuild-0.1.105/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.105/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.543852 docbuild-0.1.105/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-04-30 11:57:46.000000 docbuild-0.1.105/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.105/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.105/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.105/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7054 2023-04-29 18:09:32.000000 docbuild-0.1.105/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.549383 docbuild-0.1.105/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.105/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.105/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.105/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.105/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.105/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     5805 2023-04-30 08:43:31.000000 docbuild-0.1.105/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.105/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.553007 docbuild-0.1.105/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.105/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    12923 2023-04-30 11:56:34.000000 docbuild-0.1.105/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      218 2023-04-30 11:54:41.000000 docbuild-0.1.105/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16325 2023-04-30 05:58:58.000000 docbuild-0.1.105/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-04-30 11:58:07.546627 docbuild-0.1.105/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      741 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       83 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-04-30 11:58:07.000000 docbuild-0.1.105/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-04-30 11:58:07.555300 docbuild-0.1.105/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      832 2023-04-30 11:57:59.000000 docbuild-0.1.105/setup.py
```

### Comparing `docbuild-0.1.104/PKG-INFO` & `docbuild-0.1.105/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.104
+Version: 0.1.105
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.104/docbuild/graph.py` & `docbuild-0.1.105/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild/hocr_parser.py` & `docbuild-0.1.105/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild/page_creator.py` & `docbuild-0.1.105/docbuild/page_creator.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.105/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.105/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.105/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild/textract_parser.py` & `docbuild-0.1.105/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild/utils.py` & `docbuild-0.1.105/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.105/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 import attr
 import numpy as np
 
 from docstruct import Word, TableCell, Table, BoundingBox, Segment, VisLine, VisLineOrientation
 from ..graph import Node, Graph, BipartiteGraph
-from .constants import GRID_COVER_RATIO_THRESHOLD
+from .constants import GRID_COVER_RATIO_THRESHOLD, IS_GRID_THRESHOLD
 
 
 @attr.s(auto_attribs=True)
 class CellOfLines:
     left: VisLine
     right: VisLine
     top: VisLine
@@ -187,15 +187,16 @@
         for lines in grouped_lines:
             axis = VisLine.get_weighted_average_axis(lines)
             axis_values.append(axis)
         return axis_values
 
     def fill_lines_grid(
         self, axis_values, all_lines_grouped: list[list[VisLine]], is_hor: bool
-    ):
+    ):  
+        
         for k in range(len(all_lines_grouped)):
             segments = [
                 Segment(left=line.start, right=line.end)
                 for line in all_lines_grouped[k]
             ]
             for l in range(len(axis_values) - 1):
                 grid_segment = Segment(
@@ -302,15 +303,24 @@
                         row_index=i,
                         col_index=j,
                         row_span=1,
                         col_span=1,
                     )
                     cells.append(cell)
         return cells
-
+    
+    @staticmethod
+    def truth_ratio(matrix: np.ndarray) -> float:
+        return np.count_nonzero(matrix) / matrix.size
+    
+    def is_grid(self):
+        hor_cover = TableGrid.truth_ratio(self.hor_lines_grid)
+        ver_cover = TableGrid.truth_ratio(self.ver_lines_grid)
+        return hor_cover > IS_GRID_THRESHOLD and ver_cover > IS_GRID_THRESHOLD
+    
     def detect_table(
         self,
         all_hor_lines: list[VisLine],
         all_ver_lines: list[VisLine],
         hor_threshold: float,
         ver_threshold: float,
     ) -> Optional[Table]:
@@ -320,12 +330,14 @@
         )
         all_ver_lines_grouped = self.group_lines_by_axis_values(
             self.ver_axis_values, all_ver_lines, ver_threshold
         )
         
         self.fill_lines_grid(self.ver_axis_values, all_hor_lines_grouped, is_hor=True)
         self.fill_lines_grid(self.hor_axis_values, all_ver_lines_grouped, is_hor=False)
+        if not self.is_grid():
+            return None
         graph = self.get_graph()
         cells = self.get_cells(graph)
         if len(cells) <= 1:
             return None
         return Table(cells=cells)
```

### Comparing `docbuild-0.1.104/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.105/docbuild/visual_detection/vis_line_detection.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.105/docbuild.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.104
+Version: 0.1.105
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.104/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.105/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.104/setup.py` & `docbuild-0.1.105/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.104",
+    version="0.1.105",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

