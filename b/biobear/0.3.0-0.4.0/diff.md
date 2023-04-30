# Comparing `tmp/biobear-0.3.0.tar.gz` & `tmp/biobear-0.4.0.tar.gz`

## Comparing `biobear-0.3.0.tar` & `biobear-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,59 @@
--rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 biobear-0.3.0/Cargo.toml
--rw-r--r--   0     1001      123     2566 2023-04-27 14:22:00.000000 biobear-0.3.0/.github/workflows/release.yml
--rw-r--r--   0     1001      123      865 2023-04-27 14:22:00.000000 biobear-0.3.0/.github/workflows/smoke-test.yml
--rw-r--r--   0     1001      123      107 2023-04-27 14:22:00.000000 biobear-0.3.0/.github/workflows/smoketest.py
--rw-r--r--   0     1001      123      891 2023-04-27 14:22:00.000000 biobear-0.3.0/.github/workflows/test.yml
--rw-r--r--   0     1001      123     4135 2023-04-27 14:22:00.000000 biobear-0.3.0/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-27 14:22:00.000000 biobear-0.3.0/LICENSE
--rw-r--r--   0     1001      123       71 2023-04-27 14:22:00.000000 biobear-0.3.0/Makefile
--rw-r--r--   0     1001      123    17139 2023-04-27 14:22:00.000000 biobear-0.3.0/README.md
--rw-r--r--   0     1001      123      186 2023-04-27 14:22:00.000000 biobear-0.3.0/cz.json
--rw-r--r--   0     1001      123      238 2023-04-27 14:22:00.000000 biobear-0.3.0/docs.bash
--rw-r--r--   0     1001      123      565 2023-04-27 14:22:00.000000 biobear-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123      482 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/__init__.py
--rw-r--r--   0     1001      123     2270 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123      720 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/compression.py
--rw-r--r--   0     1001      123     1369 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123     1463 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123     1229 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/gff_reader.py
--rw-r--r--   0     1001      123     2175 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123     6152 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      123     7608 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      123     1749 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/file.vcf
--rw-r--r--   0     1001      123     8296 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      123      212 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      123       41 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.fasta
--rw-r--r--   0     1001      123       58 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      123      286 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      134 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      123      112 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.gff
--rw-r--r--   0     1001      123       91 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.gff.gz
--rw-r--r--   0     1001      123     4302 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      123     1669 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      123      254 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      123      800 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      123     1205 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123     1154 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123      919 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      123      898 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      123       20 2023-04-27 14:22:00.000000 biobear-0.3.0/requirements-dev.txt
--rw-r--r--   0     1001      123     6470 2023-04-27 14:22:00.000000 biobear-0.3.0/src/bam_reader/bam_batch.rs
--rw-r--r--   0     1001      123     6442 2023-04-27 14:22:00.000000 biobear-0.3.0/src/bam_reader.rs
--rw-r--r--   0     1001      123      565 2023-04-27 14:22:00.000000 biobear-0.3.0/src/batch.rs
--rw-r--r--   0     1001      123     3635 2023-04-27 14:22:00.000000 biobear-0.3.0/src/fasta_reader/fasta_batch.rs
--rw-r--r--   0     1001      123     3673 2023-04-27 14:22:00.000000 biobear-0.3.0/src/fasta_reader.rs
--rw-r--r--   0     1001      123     3365 2023-04-27 14:22:00.000000 biobear-0.3.0/src/fastq_reader/fastq_batch.rs
--rw-r--r--   0     1001      123     3360 2023-04-27 14:22:00.000000 biobear-0.3.0/src/fastq_reader.rs
--rw-r--r--   0     1001      123     5084 2023-04-27 14:22:00.000000 biobear-0.3.0/src/gff_reader/gff_batch.rs
--rw-r--r--   0     1001      123     3294 2023-04-27 14:22:00.000000 biobear-0.3.0/src/gff_reader.rs
--rw-r--r--   0     1001      123      720 2023-04-27 14:22:00.000000 biobear-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123      938 2023-04-27 14:22:00.000000 biobear-0.3.0/src/to_arrow.rs
--rw-r--r--   0     1001      123     5804 2023-04-27 14:22:00.000000 biobear-0.3.0/src/vcf_reader/vcf_batch.rs
--rw-r--r--   0     1001      123     4941 2023-04-27 14:22:00.000000 biobear-0.3.0/src/vcf_reader.rs
--rw-r--r--   0     1001      123    37575 2023-04-27 14:23:06.000000 biobear-0.3.0/Cargo.lock
--rw-r--r--   0        0        0    17587 1970-01-01 00:00:00.000000 biobear-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 biobear-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      123     2566 2023-04-30 14:45:04.000000 biobear-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      865 2023-04-30 14:45:04.000000 biobear-0.4.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      123      107 2023-04-30 14:45:04.000000 biobear-0.4.0/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      123      891 2023-04-30 14:45:04.000000 biobear-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     4135 2023-04-30 14:45:04.000000 biobear-0.4.0/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-30 14:45:04.000000 biobear-0.4.0/LICENSE
+-rw-r--r--   0     1001      123       71 2023-04-30 14:45:04.000000 biobear-0.4.0/Makefile
+-rw-r--r--   0     1001      123    18156 2023-04-30 14:45:04.000000 biobear-0.4.0/README.md
+-rw-r--r--   0     1001      123      186 2023-04-30 14:45:04.000000 biobear-0.4.0/cz.json
+-rw-r--r--   0     1001      123      238 2023-04-30 14:45:04.000000 biobear-0.4.0/docs.bash
+-rw-r--r--   0     1001      123      565 2023-04-30 14:45:04.000000 biobear-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123      552 2023-04-30 14:45:04.000000 biobear-0.4.0/python/biobear/__init__.py
+-rw-r--r--   0     1001      123     2270 2023-04-30 14:45:04.000000 biobear-0.4.0/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123      720 2023-04-30 14:45:04.000000 biobear-0.4.0/python/biobear/compression.py
+-rw-r--r--   0     1001      123     1369 2023-04-30 14:45:04.000000 biobear-0.4.0/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123     1463 2023-04-30 14:45:04.000000 biobear-0.4.0/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123      989 2023-04-30 14:45:04.000000 biobear-0.4.0/python/biobear/genbank_reader.py
+-rw-r--r--   0     1001      123     1229 2023-04-30 14:45:04.000000 biobear-0.4.0/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123     2175 2023-04-30 14:45:04.000000 biobear-0.4.0/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123   124562 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/BGC0000404.gbk
+-rw-r--r--   0     1001      123     6152 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     8296 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      212 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123       41 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/test.fasta
+-rw-r--r--   0     1001      123       58 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      123      286 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      134 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      123      112 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/test.gff
+-rw-r--r--   0     1001      123       91 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      123     4302 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123      800 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123     1205 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123     1154 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      421 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/test_genbank_reader.py
+-rw-r--r--   0     1001      123     1241 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123      898 2023-04-30 14:45:04.000000 biobear-0.4.0/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123       20 2023-04-30 14:45:04.000000 biobear-0.4.0/requirements-dev.txt
+-rw-r--r--   0     1001      123     6470 2023-04-30 14:45:04.000000 biobear-0.4.0/src/bam_reader/bam_batch.rs
+-rw-r--r--   0     1001      123     6442 2023-04-30 14:45:04.000000 biobear-0.4.0/src/bam_reader.rs
+-rw-r--r--   0     1001      123      565 2023-04-30 14:45:04.000000 biobear-0.4.0/src/batch.rs
+-rw-r--r--   0     1001      123     3635 2023-04-30 14:45:04.000000 biobear-0.4.0/src/fasta_reader/fasta_batch.rs
+-rw-r--r--   0     1001      123     3673 2023-04-30 14:45:04.000000 biobear-0.4.0/src/fasta_reader.rs
+-rw-r--r--   0     1001      123     3365 2023-04-30 14:45:04.000000 biobear-0.4.0/src/fastq_reader/fastq_batch.rs
+-rw-r--r--   0     1001      123     3360 2023-04-30 14:45:04.000000 biobear-0.4.0/src/fastq_reader.rs
+-rw-r--r--   0     1001      123     9756 2023-04-30 14:45:04.000000 biobear-0.4.0/src/genbank_reader/genbank_batch.rs
+-rw-r--r--   0     1001      123     1822 2023-04-30 14:45:04.000000 biobear-0.4.0/src/genbank_reader.rs
+-rw-r--r--   0     1001      123     5430 2023-04-30 14:45:04.000000 biobear-0.4.0/src/gff_reader/gff_batch.rs
+-rw-r--r--   0     1001      123     3294 2023-04-30 14:45:04.000000 biobear-0.4.0/src/gff_reader.rs
+-rw-r--r--   0     1001      123      794 2023-04-30 14:45:04.000000 biobear-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123      938 2023-04-30 14:45:04.000000 biobear-0.4.0/src/to_arrow.rs
+-rw-r--r--   0     1001      123     5804 2023-04-30 14:45:04.000000 biobear-0.4.0/src/vcf_reader/vcf_batch.rs
+-rw-r--r--   0     1001      123     4941 2023-04-30 14:45:04.000000 biobear-0.4.0/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    43636 2023-04-30 14:46:10.000000 biobear-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0    18604 1970-01-01 00:00:00.000000 biobear-0.4.0/PKG-INFO
```

### Comparing `biobear-0.3.0/.github/workflows/release.yml` & `biobear-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/.github/workflows/smoke-test.yml` & `biobear-0.4.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/.github/workflows/test.yml` & `biobear-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/.gitignore` & `biobear-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/LICENSE` & `biobear-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/README.md` & `biobear-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-# biobear (v0.3.0)
+Metadata-Version: 2.1
+Name: biobear
+Version: 0.4.0
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: polars[pyarrow]>=0.17.0
+License-File: LICENSE
+Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+
+# biobear (v0.4.0)
 
 biobear is a Python library designed for reading and searching bioinformatic file formats, using Rust as its backend and producing Arrow or Polars DataFrames as its output.
 
 The python package has minimal dependencies and only requires Polars. Biobear can be used to read various bioinformatic file formats, including FASTA, FASTQ, VCF, BAM, and GFF. It can also query some indexed file formats, including VCF and BAM.
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Similar Packages](#similar-packages)
 - [API Documentation](#api-documentation)
   - [vcf\_reader](#vcf_reader)
     - [VCFReader](#vcfreader)
     - [VCFIndexedReader](#vcfindexedreader)
+  - [genbank\_reader](#genbank_reader)
+    - [GenbankReader](#genbankreader)
   - [fasta\_reader](#fasta_reader)
     - [FastaReader](#fastareader)
   - [compression](#compression)
     - [Compression](#compression-1)
-  - [\_\_init\_\_](#__init__-3)
+  - [\_\_init\_\_](#__init__-4)
   - [bam\_reader](#bam_reader)
     - [BamReader](#bamreader)
     - [BamIndexedReader](#bamindexedreader)
   - [fastq\_reader](#fastq_reader)
     - [FastqReader](#fastqreader)
   - [gff\_reader](#gff_reader)
     - [GFFReader](#gffreader)
@@ -242,14 +256,72 @@
 
 Query the VCF file and return a polars DataFrame.
 
 **Arguments**:
 
 - `region` _str_ - The region to query.
 
+<a id="genbank_reader"></a>
+
+### genbank\_reader
+
+Genbank file reader.
+
+<a id="genbank_reader.GenbankReader"></a>
+
+#### GenbankReader
+
+```python
+class GenbankReader()
+```
+
+<a id="genbank_reader.GenbankReader.__init__"></a>
+
+##### \_\_init\_\_
+
+```python
+def __init__(path: Path)
+```
+
+Read a fasta file.
+
+**Arguments**:
+
+- `path` _Path_ - Path to the fasta file.
+
+<a id="genbank_reader.GenbankReader.read"></a>
+
+##### read
+
+```python
+def read() -> pl.DataFrame
+```
+
+Read the fasta file and return a polars DataFrame.
+
+<a id="genbank_reader.GenbankReader.to_arrow_scanner"></a>
+
+##### to\_arrow\_scanner
+
+```python
+def to_arrow_scanner() -> ds.Scanner
+```
+
+Convert the fasta reader to an arrow scanner.
+
+<a id="genbank_reader.GenbankReader.to_arrow_record_batch_reader"></a>
+
+##### to\_arrow\_record\_batch\_reader
+
+```python
+def to_arrow_record_batch_reader() -> pa.RecordBatchReader
+```
+
+Convert the fasta reader to an arrow batch reader.
+
 <a id="fasta_reader"></a>
 
 ### fasta\_reader
 
 FASTA file reader.
 
 <a id="fasta_reader.FastaReader"></a>
@@ -600,7 +672,8 @@
 ##### to\_arrow\_scanner
 
 ```python
 def to_arrow_scanner() -> ds.Scanner
 ```
 
 Convert the GFF reader to an arrow scanner.
+
```

### Comparing `biobear-0.3.0/pyproject.toml` & `biobear-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/biobear/bam_reader.py` & `biobear-0.4.0/python/biobear/bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/biobear/compression.py` & `biobear-0.4.0/python/biobear/compression.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/biobear/fasta_reader.py` & `biobear-0.4.0/python/biobear/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/biobear/fastq_reader.py` & `biobear-0.4.0/python/biobear/fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/biobear/gff_reader.py` & `biobear-0.4.0/python/biobear/gff_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/biobear/vcf_reader.py` & `biobear-0.4.0/python/biobear/vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/data/bedcov.bam` & `biobear-0.4.0/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/data/bedcov.bam.bai` & `biobear-0.4.0/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/data/file.vcf` & `biobear-0.4.0/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/data/index.vcf.gz` & `biobear-0.4.0/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/data/vcf_file.vcf` & `biobear-0.4.0/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/data/vcf_file.vcf.gz` & `biobear-0.4.0/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/test_bam_reader.py` & `biobear-0.4.0/python/tests/test_bam_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/test_fasta_reader.py` & `biobear-0.4.0/python/tests/test_fasta_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/test_fastq_reader.py` & `biobear-0.4.0/python/tests/test_fastq_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/python/tests/test_vcf_reader.py` & `biobear-0.4.0/python/tests/test_vcf_reader.py`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/bam_reader/bam_batch.rs` & `biobear-0.4.0/src/bam_reader/bam_batch.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/bam_reader.rs` & `biobear-0.4.0/src/bam_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/batch.rs` & `biobear-0.4.0/src/batch.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/fasta_reader/fasta_batch.rs` & `biobear-0.4.0/src/fasta_reader/fasta_batch.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/fasta_reader.rs` & `biobear-0.4.0/src/fasta_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/fastq_reader/fastq_batch.rs` & `biobear-0.4.0/src/fastq_reader/fastq_batch.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/fastq_reader.rs` & `biobear-0.4.0/src/fastq_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/gff_reader/gff_batch.rs` & `biobear-0.4.0/src/gff_reader/gff_batch.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 use std::{io::BufRead, str::FromStr, sync::Arc};
 
 use arrow::{
-    array::{Float32Builder, GenericStringBuilder, Int64Builder},
+    array::{Float32Builder, GenericStringBuilder, Int64Builder, MapBuilder},
     datatypes::{DataType, Field, Schema},
     error::ArrowError,
     record_batch::RecordBatch,
 };
 use noodles::gff::Line;
 
 use crate::batch::BearRecordBatch;
 
 pub trait GFFSchemaTrait {
     fn gff_schema(&self) -> Schema {
+        let attribute_key_field = Field::new("keys", DataType::Utf8, false);
+        let attribute_value_field = Field::new("values", DataType::Utf8, true);
+
         Schema::new(vec![
             Field::new("seqname", DataType::Utf8, false),
             Field::new("source", DataType::Utf8, true),
             Field::new("feature", DataType::Utf8, false),
             Field::new("start", DataType::Int64, false),
             Field::new("end", DataType::Int64, false),
             Field::new("score", DataType::Float32, true),
             Field::new("strand", DataType::Utf8, false),
             Field::new("phase", DataType::Utf8, true),
-            Field::new("attributes", DataType::Utf8, true),
+            Field::new_map(
+                "attributes",
+                "entries",
+                attribute_key_field,
+                attribute_value_field,
+                false,
+                true,
+            ),
         ])
     }
 }
 
 pub struct GFFBatch {
     seqnames: GenericStringBuilder<i32>,
     sources: GenericStringBuilder<i32>,
     feature_types: GenericStringBuilder<i32>,
     starts: Int64Builder,
     ends: Int64Builder,
     scores: Float32Builder,
     strands: GenericStringBuilder<i32>,
     phases: GenericStringBuilder<i32>,
-    attributes: GenericStringBuilder<i32>,
+    attributes: MapBuilder<GenericStringBuilder<i32>, GenericStringBuilder<i32>>,
 }
 
 impl GFFSchemaTrait for GFFBatch {}
 
 impl GFFBatch {
     pub fn new() -> Self {
         Self {
@@ -47,39 +57,39 @@
             sources: GenericStringBuilder::<i32>::new(),
             feature_types: GenericStringBuilder::<i32>::new(),
             starts: Int64Builder::new(),
             ends: Int64Builder::new(),
             scores: Float32Builder::new(),
             strands: GenericStringBuilder::<i32>::new(),
             phases: GenericStringBuilder::<i32>::new(),
-            attributes: GenericStringBuilder::<i32>::new(),
+            attributes: MapBuilder::new(
+                None,
+                GenericStringBuilder::<i32>::new(),
+                GenericStringBuilder::<i32>::new(),
+            ),
         }
     }
 
     pub fn add(&mut self, record: noodles::gff::Record) {
         self.seqnames.append_value(record.reference_sequence_name());
         self.sources.append_value(record.source());
         self.feature_types.append_value(record.ty());
         self.starts.append_value(record.start().get() as i64);
         self.ends.append_value(record.end().get() as i64);
         self.scores.append_option(record.score());
         self.strands.append_value(record.strand().to_string());
         self.phases
             .append_option(record.phase().map(|p| p.to_string()));
 
-        let attrs = record.attributes();
-        if attrs.is_empty() {
-            self.attributes.append_null();
-        } else {
-            let mut attr_str = String::new();
-            for entry in attrs.into_iter() {
-                attr_str.push_str(&format!("{}={};", entry.key(), entry.value()));
-            }
-            self.attributes.append_value(&attr_str);
+        for entry in record.attributes().iter() {
+            self.attributes.keys().append_value(entry.key());
+            self.attributes.values().append_value(entry.value());
         }
+
+        self.attributes.append(true).unwrap();
     }
 }
 
 impl BearRecordBatch for GFFBatch {
     fn to_batch(&mut self) -> RecordBatch {
         let seqnames = self.seqnames.finish();
         let sources = self.sources.finish();
```

### Comparing `biobear-0.3.0/src/gff_reader.rs` & `biobear-0.4.0/src/gff_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/lib.rs` & `biobear-0.4.0/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use pyo3::prelude::*;
 
 mod bam_reader;
 mod batch;
 mod fasta_reader;
 mod fastq_reader;
+mod genbank_reader;
 mod gff_reader;
 mod to_arrow;
 mod vcf_reader;
 
 #[pymodule]
 fn biobear(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<fasta_reader::FastaReader>()?;
@@ -21,9 +22,11 @@
 
     m.add_class::<bam_reader::BamReader>()?;
     m.add_class::<bam_reader::BamIndexedReader>()?;
 
     m.add_class::<vcf_reader::VCFReader>()?;
     m.add_class::<vcf_reader::VCFIndexedReader>()?;
 
+    m.add_class::<genbank_reader::GenbankReader>()?;
+
     Ok(())
 }
```

### Comparing `biobear-0.3.0/src/to_arrow.rs` & `biobear-0.4.0/src/to_arrow.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/vcf_reader/vcf_batch.rs` & `biobear-0.4.0/src/vcf_reader/vcf_batch.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/src/vcf_reader.rs` & `biobear-0.4.0/src/vcf_reader.rs`

 * *Files identical despite different names*

### Comparing `biobear-0.3.0/Cargo.lock` & `biobear-0.4.0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
  "cfg-if",
  "const-random",
  "getrandom",
  "once_cell",
- "version_check",
+ "version_check 0.9.4",
 ]
 
 [[package]]
 name = "aho-corasick"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
@@ -255,18 +255,19 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "biobear"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
  "arrow",
  "flate2",
+ "gb-io",
  "noodles",
  "pyo3",
 ]
 
 [[package]]
 name = "bit-vec"
 version = "0.6.3"
@@ -324,14 +325,20 @@
  "iana-time-zone",
  "num-integer",
  "num-traits",
  "winapi",
 ]
 
 [[package]]
+name = "circular"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fc239e0f6cb375d2402d48afb92f76f5404fd1df208a41930ec81eda078bea"
+
+[[package]]
 name = "codespan-reporting"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
@@ -461,34 +468,71 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
+name = "either"
+version = "1.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+
+[[package]]
+name = "err-derive"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c34a887c8df3ed90498c1c437ce21f211c8e27672921a8ffa293cb8d6d4caa9e"
+dependencies = [
+ "proc-macro-error",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn 1.0.109",
+ "synstructure",
+]
+
+[[package]]
 name = "flatbuffers"
 version = "23.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77f5399c2c9c50ae9418e522842ad362f61ee48b346ac106807bd355a8a7c619"
 dependencies = [
  "bitflags 1.3.2",
  "rustc_version",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "gb-io"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "387616b1e67a2c326231a86f1a62fb98e94f1da7c089817a00e332a96c2dbc21"
+dependencies = [
+ "circular",
+ "err-derive",
+ "itertools",
+ "log",
+ "nom 4.2.3",
+ "serde",
+ "serde_bytes",
+ "string_cache",
+ "string_cache_codegen",
+]
+
+[[package]]
 name = "getrandom"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
@@ -554,14 +598,23 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "itertools"
+version = "0.10.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
@@ -701,22 +754,38 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
+name = "new_debug_unreachable"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
+
+[[package]]
+name = "nom"
+version = "4.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2ad2a91a8e869eeb30b9cb3119ae87773a8f4ae617f41b1eb9c154b2905f7bd6"
+dependencies = [
+ "memchr",
+ "version_check 0.1.5",
+]
+
+[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
@@ -871,15 +940,15 @@
 name = "noodles-vcf"
 version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4be4406c87ddefbec64fe0b398aeb41e926d8ac302438258e3b1cc6d5ccb5f4"
 dependencies = [
  "indexmap",
  "memchr",
- "nom",
+ "nom 7.1.3",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "noodles-tabix",
  "percent-encoding",
 ]
 
@@ -992,14 +1061,69 @@
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
+name = "phf_generator"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5d5285893bb5eb82e6aaf5d59ee909a06a16737a8970984dd7746ba9283498d6"
+dependencies = [
+ "phf_shared",
+ "rand",
+]
+
+[[package]]
+name = "phf_shared"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6796ad771acdc0123d2a88dc428b5e38ef24456743ddb1744ed628f9815c096"
+dependencies = [
+ "siphasher",
+]
+
+[[package]]
+name = "ppv-lite86"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+
+[[package]]
+name = "precomputed-hash"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
+
+[[package]]
+name = "proc-macro-error"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
+dependencies = [
+ "proc-macro-error-attr",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "version_check 0.9.4",
+]
+
+[[package]]
+name = "proc-macro-error-attr"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "version_check 0.9.4",
+]
+
+[[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
@@ -1076,14 +1200,44 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "libc",
+ "rand_chacha",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -1117,14 +1271,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
+name = "rustversion"
+version = "1.0.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+
+[[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "scopeguard"
@@ -1145,39 +1305,94 @@
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
 version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+dependencies = [
+ "serde_derive",
+]
+
+[[package]]
+name = "serde_bytes"
+version = "0.11.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "serde_derive"
+version = "1.0.160"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "siphasher"
+version = "0.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
+name = "string_cache"
+version = "0.8.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f91138e76242f575eb1d3b38b4f1362f10d3a43f47d182a5b359af488a02293b"
+dependencies = [
+ "new_debug_unreachable",
+ "once_cell",
+ "parking_lot",
+ "phf_shared",
+ "precomputed-hash",
+ "serde",
+]
+
+[[package]]
+name = "string_cache_codegen"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6bb30289b722be4ff74a408c3cc27edeaad656e06cb1fe8fa9231fa59c728988"
+dependencies = [
+ "phf_generator",
+ "phf_shared",
+ "proc-macro2",
+ "quote",
+]
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -1192,14 +1407,26 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "synstructure"
+version = "0.12.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "unicode-xid",
+]
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "termcolor"
@@ -1228,21 +1455,33 @@
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
 [[package]]
+name = "unicode-xid"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
+
+[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "version_check"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "914b1a6776c4c929a602fafd8bc742e06365d4bcbe48c30f9cca5824f70dc9dd"
+
+[[package]]
+name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
```

### Comparing `biobear-0.3.0/PKG-INFO` & `biobear-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,27 @@
-Metadata-Version: 2.1
-Name: biobear
-Version: 0.3.0
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: polars[pyarrow]>=0.17.0
-License-File: LICENSE
-Author-email: WHERE TRUE devs <thauck+biobear@wheretrue.com>
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
-# biobear (v0.3.0)
+# biobear (v0.4.0)
 
 biobear is a Python library designed for reading and searching bioinformatic file formats, using Rust as its backend and producing Arrow or Polars DataFrames as its output.
 
 The python package has minimal dependencies and only requires Polars. Biobear can be used to read various bioinformatic file formats, including FASTA, FASTQ, VCF, BAM, and GFF. It can also query some indexed file formats, including VCF and BAM.
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Similar Packages](#similar-packages)
 - [API Documentation](#api-documentation)
   - [vcf\_reader](#vcf_reader)
     - [VCFReader](#vcfreader)
     - [VCFIndexedReader](#vcfindexedreader)
+  - [genbank\_reader](#genbank_reader)
+    - [GenbankReader](#genbankreader)
   - [fasta\_reader](#fasta_reader)
     - [FastaReader](#fastareader)
   - [compression](#compression)
     - [Compression](#compression-1)
-  - [\_\_init\_\_](#__init__-3)
+  - [\_\_init\_\_](#__init__-4)
   - [bam\_reader](#bam_reader)
     - [BamReader](#bamreader)
     - [BamIndexedReader](#bamindexedreader)
   - [fastq\_reader](#fastq_reader)
     - [FastqReader](#fastqreader)
   - [gff\_reader](#gff_reader)
     - [GFFReader](#gffreader)
@@ -254,14 +244,72 @@
 
 Query the VCF file and return a polars DataFrame.
 
 **Arguments**:
 
 - `region` _str_ - The region to query.
 
+<a id="genbank_reader"></a>
+
+### genbank\_reader
+
+Genbank file reader.
+
+<a id="genbank_reader.GenbankReader"></a>
+
+#### GenbankReader
+
+```python
+class GenbankReader()
+```
+
+<a id="genbank_reader.GenbankReader.__init__"></a>
+
+##### \_\_init\_\_
+
+```python
+def __init__(path: Path)
+```
+
+Read a fasta file.
+
+**Arguments**:
+
+- `path` _Path_ - Path to the fasta file.
+
+<a id="genbank_reader.GenbankReader.read"></a>
+
+##### read
+
+```python
+def read() -> pl.DataFrame
+```
+
+Read the fasta file and return a polars DataFrame.
+
+<a id="genbank_reader.GenbankReader.to_arrow_scanner"></a>
+
+##### to\_arrow\_scanner
+
+```python
+def to_arrow_scanner() -> ds.Scanner
+```
+
+Convert the fasta reader to an arrow scanner.
+
+<a id="genbank_reader.GenbankReader.to_arrow_record_batch_reader"></a>
+
+##### to\_arrow\_record\_batch\_reader
+
+```python
+def to_arrow_record_batch_reader() -> pa.RecordBatchReader
+```
+
+Convert the fasta reader to an arrow batch reader.
+
 <a id="fasta_reader"></a>
 
 ### fasta\_reader
 
 FASTA file reader.
 
 <a id="fasta_reader.FastaReader"></a>
@@ -612,8 +660,7 @@
 ##### to\_arrow\_scanner
 
 ```python
 def to_arrow_scanner() -> ds.Scanner
 ```
 
 Convert the GFF reader to an arrow scanner.
-
```

