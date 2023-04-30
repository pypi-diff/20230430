# Comparing `tmp/dnadb-0.2.7.tar.gz` & `tmp/dnadb-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.2.7.tar", last modified: Mon Apr 17 03:05:38 2023, max compression
+gzip compressed data, was "dnadb-0.2.8.tar", last modified: Sun Apr 30 03:43:18 2023, max compression
```

## Comparing `dnadb-0.2.7.tar` & `dnadb-0.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.366622 dnadb-0.2.7/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.7/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-17 03:05:38.366622 dnadb-0.2.7/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.7/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-17 03:04:57.000000 dnadb-0.2.7/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-17 03:05:38.366622 dnadb-0.2.7/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.362621 dnadb-0.2.7/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.362621 dnadb-0.2.7/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-17 03:05:03.000000 dnadb-0.2.7/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.366622 dnadb-0.2.7/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.7/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.7/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.7/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.366622 dnadb-0.2.7/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.7/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.7/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      999 2023-04-12 05:30:41.000000 dnadb-0.2.7/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.7/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4773 2023-04-14 00:18:43.000000 dnadb-0.2.7/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6096 2023-04-14 00:19:30.000000 dnadb-0.2.7/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    15111 2023-04-17 02:55:42.000000 dnadb-0.2.7/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.7/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-17 03:05:38.362621 dnadb-0.2.7/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-17 03:05:38.000000 dnadb-0.2.7/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.8/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-30 03:43:18.608556 dnadb-0.2.8/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.8/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-21 06:50:34.000000 dnadb-0.2.8/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-30 03:43:18.608556 dnadb-0.2.8/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-17 03:05:03.000000 dnadb-0.2.8/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.8/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.8/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.8/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.8/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.8/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1163 2023-04-30 03:41:17.000000 dnadb-0.2.8/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.8/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4998 2023-04-21 05:23:34.000000 dnadb-0.2.8/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6967 2023-04-21 05:23:31.000000 dnadb-0.2.8/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    15313 2023-04-21 05:23:29.000000 dnadb-0.2.8/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.8/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.2.7/LICENSE` & `dnadb-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.7/PKG-INFO` & `dnadb-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.2.7/pyproject.toml` & `dnadb-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.2.7/src/dnadb/datasets/dataset.py` & `dnadb-0.2.8/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.7/src/dnadb/datasets/greengenes.py` & `dnadb-0.2.8/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.7/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.2.8/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.7/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.2.8/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.7/src/dnadb/db.py` & `dnadb-0.2.8/src/dnadb/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,27 +9,34 @@
     def __init__(self, path: Union[str, Path], chunk_size: int = 10000):
         self.path = Path(path)
         if self.path.suffix != ".db":
             self.path = Path(str(self.path) + ".db")
         self.db = Lmdb.open(str(self.path), "n", lock=True)
         self.buffer: dict[Union[str, bytes], bytes] = {}
         self.chunk_size = chunk_size
+        self.is_closed = False
 
     def flush(self):
         self.db.update(self.buffer)
         self.buffer.clear()
 
     def write(self, key: Union[str, bytes], value: bytes):
         self.buffer[key] = value
         if len(self.buffer) >= self.chunk_size:
             self.flush()
 
-    def close(self):
+    def before_close(self):
         self.flush()
+
+    def close(self):
+        if self.is_closed:
+            return
+        self.before_close()
         self.db.close()
+        self.is_closed = True
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
```

### Comparing `dnadb-0.2.7/src/dnadb/dna.py` & `dnadb-0.2.8/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.7/src/dnadb/fasta.py` & `dnadb-0.2.8/src/dnadb/fasta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from functools import singledispatchmethod
+import io
 from lmdbm import Lmdb
 import numpy as np
 from pathlib import Path
-from typing import Generator, Iterable, TextIO, Tuple, Union
+from typing import Generator, Iterable, Tuple, Union
 
 from .db import DbFactory
 from .taxonomy import TaxonomyEntry
 from .utils import open_file
 
 class FastaEntry:
     """
@@ -39,14 +40,19 @@
     def serialize(self) -> bytes:
         return "\x00".join((self.identifier, self.sequence, self.extra)).encode()
 
     def __str__(self):
         header_line = f"{self.identifier} {self.extra}".rstrip()
         return f">{header_line}\n{self.sequence}"
 
+    def __eq__(self, other):
+        return self.identifier == other.identifier \
+            and self.sequence == other.sequence \
+            and self.extra == other.extra
+
     def __repr__(self):
         return str(self)
 
 
 class FastaDbFactory(DbFactory):
     """
     A factory for creating LMDB-backed databases of FASTA entries.
@@ -64,17 +70,17 @@
         self.write(str(self.num_entries), entry.serialize())
         self.num_entries += 1
 
     def write_entries(self, entries: Iterable[FastaEntry]):
         for entry in entries:
             self.write_entry(entry)
 
-    def close(self):
+    def before_close(self):
         self.write("length", self.num_entries.tobytes())
-        super().close()
+        super().before_close()
 
 
 class FastaDb:
     """
     An LMDB-backed database of FASTA entries.
     """
     def __init__(self, fasta_db_path: Union[str, Path]):
@@ -92,22 +98,24 @@
 
     @__getitem__.register
     def _(self, sequence_id: str) -> FastaEntry:
         index = np.frombuffer(self.db[f"id_{sequence_id}"], dtype=np.int32, count=1)[0]
         return self[index]
 
 
-def entries(sequences: Union[TextIO, Iterable[FastaEntry], str, Path]) -> Iterable[FastaEntry]:
+def entries(
+    sequences: Union[io.TextIOBase, Iterable[FastaEntry], str, Path]
+) -> Iterable[FastaEntry]:
     """
     Create an iterator over a FASTA file or iterable of FASTA entries.
     """
     if isinstance(sequences, (str, Path)):
         with open_file(sequences, 'r') as buffer:
             yield from read(buffer)
-    elif isinstance(sequences, TextIO):
+    elif isinstance(sequences, io.TextIOBase):
         yield from read(sequences)
     else:
         yield from sequences
 
 
 def entries_with_taxonomy(
     sequences: Iterable[FastaEntry],
@@ -124,29 +132,29 @@
             taxonomy = next(taxonomy_iterator)
             labels[taxonomy.identifier] = taxonomy
         taxonomy = labels[sequence.identifier]
         del labels[sequence.identifier]
         yield sequence, taxonomy
 
 
-def read(buffer: TextIO) -> Generator[FastaEntry, None, None]:
+def read(buffer: io.TextIOBase) -> Generator[FastaEntry, None, None]:
     """
     Read entries from a FASTA file buffer.
     """
     entry_str = buffer.readline()
     for line in buffer:
         if line.startswith('>'):
             yield FastaEntry.from_str(entry_str)
             entry_str = ""
         entry_str += line
     if len(entry_str) > 0:
         yield FastaEntry.from_str(entry_str)
 
 
-def write(buffer: TextIO, entries: Iterable[FastaEntry]) -> int:
+def write(buffer: io.TextIOBase, entries: Iterable[FastaEntry]) -> int:
     """
     Write entries to a FASTA file.
     """
     bytes_written = 0
     for entry in entries:
         bytes_written += buffer.write(str(entry) + '\n')
     return bytes_written
```

### Comparing `dnadb-0.2.7/src/dnadb/taxonomy.py` & `dnadb-0.2.8/src/dnadb/taxonomy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import cached_property
+import io
 import json
 from lmdbm import Lmdb
 import numpy as np
 from pathlib import Path
 import re
-from typing import Dict, Generator, Iterable, List, Optional, TextIO, Tuple, TypedDict, Set, Union
+from typing import Dict, Generator, Iterable, List, Optional, Tuple, TypedDict, Set, Union
 
 from .db import DbFactory
 from .utils import open_file
 
 TAXON_LEVEL_NAMES = ("Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species")
 TAXON_PREFIXES = ''.join(name[0] for name in TAXON_LEVEL_NAMES).lower()
 
@@ -318,24 +319,28 @@
     def from_str(cls, entry: str) -> "TaxonomyEntry":
         """
         Create a taxonomy entry from a string
         """
         identifier, taxonomy = entry.rstrip().split('\t')
         return cls(identifier, taxonomy)
 
-    def __init__(self, identifier, label):
+    def __init__(self, identifier: str, label: str):
         self.identifier = identifier
         self.label = label
 
     def taxons(self, depth: int = 7) -> Tuple[str, ...]:
         return split_taxonomy(self.label, depth)
 
     def serialize(self) -> bytes:
         return str(self).encode()
 
+    def __eq__(self, other: "TaxonomyEntry"):
+        return self.identifier == other.identifier \
+            and self.label == other.label
+
     def __repr__(self):
         return str(self)
 
     def __str__(self):
         return f"{self.identifier}\t{self.label}"
 
 
@@ -356,18 +361,18 @@
         self.write(entry.identifier, entry.serialize())
         self.num_entries += 1
 
     def write_entries(self, entries: Iterable[TaxonomyEntry]):
         for entry in entries:
             self.write_entry(entry)
 
-    def close(self):
+    def before_close(self):
         self.write("hierarchy", self.hierarchy.serialize())
         self.write("length", self.num_entries.tobytes())
-        super().close()
+        super().before_close()
 
 
 class TaxonomyDb:
     def __init__(self, taxonomy_db_path: Union[str, Path]):
         self.path = Path(taxonomy_db_path).absolute()
         self.db = Lmdb.open(str(self.path), lock=False)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
@@ -379,35 +384,37 @@
     def hierarchy(self):
         return TaxonomyHierarchy.deserialize(self.db["hierarchy"])
 
     def __getitem__(self, sequence_id: str) -> TaxonomyEntry:
         return TaxonomyEntry.deserialize(self.db[sequence_id])
 
 
-def entries(taxonomy: Union[TextIO, Iterable[TaxonomyEntry], str, Path]) -> Iterable[TaxonomyEntry]:
+def entries(
+    taxonomy: Union[io.TextIOBase, Iterable[TaxonomyEntry], str, Path]
+) -> Iterable[TaxonomyEntry]:
     """
     Create an iterator over a taxonomy file or iterable of taxonomy entries.
     """
     if isinstance(taxonomy, (str, Path)):
         with open_file(taxonomy, 'r') as buffer:
             yield from read(buffer)
-    elif isinstance(taxonomy, TextIO):
+    elif isinstance(taxonomy, io.TextIOBase):
         yield from read(taxonomy)
     else:
         yield from taxonomy
 
 
-def read(buffer: TextIO) -> Generator[TaxonomyEntry, None, None]:
+def read(buffer: io.TextIOBase) -> Generator[TaxonomyEntry, None, None]:
     """
     Read taxonomies from a tab-separated file (TSV)
     """
     for line in buffer:
         identifier, taxonomy = line.rstrip().split('\t')
         yield TaxonomyEntry(identifier, taxonomy)
 
 
-def write(buffer: TextIO, entries: Iterable[TaxonomyEntry]):
+def write(buffer: io.TextIOBase, entries: Iterable[TaxonomyEntry]):
     """
     Write taxonomy entries to a tab-separate file (TSV)
     """
     for entry in entries:
         buffer.write(f"{entry.identifier}\t{entry.label}\n")
```

### Comparing `dnadb-0.2.7/src/dnadb/utils.py` & `dnadb-0.2.8/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.7/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.2.8/src/dnadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

