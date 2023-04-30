# Comparing `tmp/cthreepo-0.1.2.tar.gz` & `tmp/cthreepo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cthreepo-0.1.2.tar", last modified: Fri Oct 16 17:30:48 2020, max compression
+gzip compressed data, was "cthreepo-0.1.3.tar", last modified: Sun Apr 30 17:59:18 2023, max compression
```

## Comparing `cthreepo-0.1.2.tar` & `cthreepo-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vamsi     (1000) vamsi     (1000)        0 2020-10-16 17:30:48.057955 cthreepo-0.1.2/
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)     3211 2020-10-16 17:30:48.053955 cthreepo-0.1.2/PKG-INFO
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)     2443 2020-10-16 17:30:15.000000 cthreepo-0.1.2/README.md
-drwxrwxr-x   0 vamsi     (1000) vamsi     (1000)        0 2020-10-16 17:30:48.053955 cthreepo-0.1.2/cthreepo/
--rwxrwxr-x   0 vamsi     (1000) vamsi     (1000)     7042 2020-10-16 17:30:15.000000 cthreepo-0.1.2/cthreepo/__init__.py
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    10045 2020-10-16 17:30:15.000000 cthreepo-0.1.2/cthreepo/converters.py
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)     1496 2020-10-16 17:30:15.000000 cthreepo-0.1.2/cthreepo/fetch_assm_report.py
-drwxrwxr-x   0 vamsi     (1000) vamsi     (1000)        0 2020-10-16 17:30:48.053955 cthreepo-0.1.2/cthreepo/mapfiles/
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    28760 2020-10-16 17:30:15.000000 cthreepo-0.1.2/cthreepo/mapfiles/h37.map
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    70144 2020-10-16 17:30:15.000000 cthreepo-0.1.2/cthreepo/mapfiles/h38.map
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    28217 2020-10-16 17:30:15.000000 cthreepo-0.1.2/cthreepo/mapfiles/m37.map
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    24313 2020-10-16 17:30:15.000000 cthreepo-0.1.2/cthreepo/mapfiles/m38.map
-drwxrwxr-x   0 vamsi     (1000) vamsi     (1000)        0 2020-10-16 17:30:48.053955 cthreepo-0.1.2/cthreepo.egg-info/
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)     3211 2020-10-16 17:30:47.000000 cthreepo-0.1.2/cthreepo.egg-info/PKG-INFO
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)      421 2020-10-16 17:30:48.000000 cthreepo-0.1.2/cthreepo.egg-info/SOURCES.txt
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)        1 2020-10-16 17:30:47.000000 cthreepo-0.1.2/cthreepo.egg-info/dependency_links.txt
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)       44 2020-10-16 17:30:47.000000 cthreepo-0.1.2/cthreepo.egg-info/entry_points.txt
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)        1 2020-10-16 17:30:47.000000 cthreepo-0.1.2/cthreepo.egg-info/not-zip-safe
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)        9 2020-10-16 17:30:47.000000 cthreepo-0.1.2/cthreepo.egg-info/requires.txt
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)        9 2020-10-16 17:30:47.000000 cthreepo-0.1.2/cthreepo.egg-info/top_level.txt
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)       38 2020-10-16 17:30:48.057955 cthreepo-0.1.2/setup.cfg
--rw-rw-r--   0 vamsi     (1000) vamsi     (1000)      683 2020-10-16 17:30:15.000000 cthreepo-0.1.2/setup.py
+drwxrwxr-x   0 vamsi     (1000) vamsi     (1000)        0 2023-04-30 17:59:18.771682 cthreepo-0.1.3/
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)     3087 2023-04-30 17:59:18.771682 cthreepo-0.1.3/PKG-INFO
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)     2798 2023-04-30 17:58:19.000000 cthreepo-0.1.3/README.md
+drwxrwxr-x   0 vamsi     (1000) vamsi     (1000)        0 2023-04-30 17:59:18.771682 cthreepo-0.1.3/cthreepo/
+-rwxrwxr-x   0 vamsi     (1000) vamsi     (1000)     7647 2023-04-30 17:58:19.000000 cthreepo-0.1.3/cthreepo/__init__.py
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    10045 2023-04-30 17:58:19.000000 cthreepo-0.1.3/cthreepo/converters.py
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)     1496 2023-04-30 17:58:19.000000 cthreepo-0.1.3/cthreepo/fetch_assm_report.py
+drwxrwxr-x   0 vamsi     (1000) vamsi     (1000)        0 2023-04-30 17:59:18.771682 cthreepo-0.1.3/cthreepo/mapfiles/
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    28760 2023-04-30 17:58:19.000000 cthreepo-0.1.3/cthreepo/mapfiles/h37.map
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    70144 2023-04-30 17:58:19.000000 cthreepo-0.1.3/cthreepo/mapfiles/h38.map
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    28217 2023-04-30 17:58:19.000000 cthreepo-0.1.3/cthreepo/mapfiles/m37.map
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)    24313 2023-04-30 17:58:19.000000 cthreepo-0.1.3/cthreepo/mapfiles/m38.map
+drwxrwxr-x   0 vamsi     (1000) vamsi     (1000)        0 2023-04-30 17:59:18.771682 cthreepo-0.1.3/cthreepo.egg-info/
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)     3087 2023-04-30 17:59:18.000000 cthreepo-0.1.3/cthreepo.egg-info/PKG-INFO
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)      421 2023-04-30 17:59:18.000000 cthreepo-0.1.3/cthreepo.egg-info/SOURCES.txt
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)        1 2023-04-30 17:59:18.000000 cthreepo-0.1.3/cthreepo.egg-info/dependency_links.txt
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)       43 2023-04-30 17:59:18.000000 cthreepo-0.1.3/cthreepo.egg-info/entry_points.txt
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)        1 2023-04-30 17:59:18.000000 cthreepo-0.1.3/cthreepo.egg-info/not-zip-safe
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)        9 2023-04-30 17:59:18.000000 cthreepo-0.1.3/cthreepo.egg-info/requires.txt
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)        9 2023-04-30 17:59:18.000000 cthreepo-0.1.3/cthreepo.egg-info/top_level.txt
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)       38 2023-04-30 17:59:18.771682 cthreepo-0.1.3/setup.cfg
+-rw-rw-r--   0 vamsi     (1000) vamsi     (1000)      683 2023-04-30 17:58:19.000000 cthreepo-0.1.3/setup.py
```

### Comparing `cthreepo-0.1.2/PKG-INFO` & `cthreepo-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,81 @@
 Metadata-Version: 2.1
 Name: cthreepo
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python tool to interconvert seq-ids in gff3, gtf, bed and other files.
 Home-page: http://github.com/vkkodali/cthreepo
 Author: Vamsi Kodali
 Author-email: vkkodali@gmail.com
 License: MIT
-Description: # cthreepo
-        A python script to interconvert seq-ids in gff3, gtf, bed and other files.
-        ---
-        ## Quick start for the impatient
-        1. Clone the repository
-        2. Run the following to install: 
-        ```
-        python3 setup.py install
-        ```
-        3. Execute as follows:
-        ```
-        ## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
-        ## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
-        cthreepo -i <input.gff3> -if rs -it uc -f gff3 -m h38 -o <output.gff3>
-        ```
-        ---
-        ## Introduction
-        NCBI RefSeq, UCSC and Ensembl use different identifiers for chromosomes in annotation and other files such as GFF3, GTF, etc. Users interested in using a mix of files downloaded from different sources and use them in a single pipeline may end up with seq-id mismatch related errors. This script converts seq-ids from one style to the other in order to make the files compatible with each other.
-        
-        ## Installation and Usage
-        Python3 is required for this script to work. With that requirement satisfied, download/clone the repository, install and run the script `cthreepo.py` as shown below.
-        ```
-        ## installation
-        python3 setup.py install
-        
-        ## help
-        cthreepo --help 
-        
-        ## usage
-        ## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
-        ## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
-        cthreepo \
-            --infile <input.gff3> \
-            --id_from rs \
-            --id_to uc \
-            --format gff3 \
-            --mapfile h38 \
-            --outfile <output.gff3>
-        ```
-        
-        ## File formats supported
-        1. GFF3 (default)
-        2. GTF
-        3. BedGraph
-        4. BED
-        5. SAM
-        6. VCF
-        7. WIG
-        8. TSV
-        
-        ## Mapping files
-        `cthreepo` needs a `mapfile` that it uses to figure out how seq-ids map from one style to the other. 
-        * Use the built-in shortcuts -- `h38`, `h37`, `m38` and `m37` for GRCh38/hg38, GRCh37/hg19, MGSCv37/mm9 and GRCm38/mm10 respectively. I try to keep these files up-to-date but if they don't work as expected, I suggest using the latest file by following one of the two options described below.
-        * Provide NCBI assembly accession using the `-a` parameter. A complete, legal accession.version such as GCF_000001405.39 should be provided. 
-        * Provide an NCBI assembly report file. For a given assembly it can be downloaded from the [NCBI Assembly](https://www.ncbi.nlm.nih.gov/assembly) website. If the 'Download' button is used, this file is called 'Assembly structure report'. On the [NCBI Genomes FTP](https://ftp.ncbi.nlm.nih.gov/genomes/all/) site, these files have the suffix `assembly_report.txt`. 
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# cthreepo
+[![PyPI version](https://badge.fury.io/py/cthreepo.svg)](https://badge.fury.io/py/cthreepo)
+[![Conda](https://img.shields.io/conda/dn/bioconda/cthreepo?label=bioconda-install&style=flat)](https://anaconda.org/bioconda/cthreepo)
+
+A python script to interconvert seq-ids in gff3, gtf, bed and other files.
+
+---
+## Quick start for the impatient
+1. Install using conda 
+```
+conda install -c bioconda cthreepo 
+```
+2. Execute as follows:
+```
+## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
+## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
+cthreepo -i <input.gff3> -if rs -it uc -f gff3 -m h38 -o <output.gff3>
+```
+---
+
+## Introduction
+NCBI RefSeq, UCSC and Ensembl use different identifiers for chromosomes in annotation and other files such as GFF3, GTF, etc. Users interested in using a mix of files downloaded from different sources and use them in a single pipeline may end up with seq-id mismatch related errors. This script converts seq-ids from one style to the other in order to make the files compatible with each other.
+
+## Installation and Usage
+Python3 is required for this script to work. With that requirement satisfied, you can install as shown below:
+### Install using conda 
+```
+conda install -c bioconda cthreepo 
+```
+### Install using pip
+```
+pip install cthreepo
+```
+### Install from this repository
+First, download/clone the repository. Then run: 
+```
+python3 setup.py install
+```
+### Usage
+```
+## help
+cthreepo --help 
+
+## usage
+## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
+## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
+cthreepo \
+    --infile <input.gff3> \
+    --id_from rs \
+    --id_to uc \
+    --format gff3 \
+    --mapfile h38 \
+    --outfile <output.gff3>
+```
+
+## File formats supported
+1. GFF3 (default)
+2. GTF
+3. BedGraph
+4. BED
+5. SAM
+6. VCF
+7. WIG
+8. TSV
+
+## Mapping files
+`cthreepo` needs a `mapfile` that it uses to figure out how seq-ids map from one style to the other. 
+* Use the built-in shortcuts -- `h38`, `h37`, `m38` and `m37` for GRCh38/hg38, GRCh37/hg19, MGSCv37/mm9 and GRCm38/mm10 respectively. I try to keep these files up-to-date but if they don't work as expected, I suggest using the latest file by following one of the two options described below.
+* Provide NCBI assembly accession using the `-a` parameter. A complete, legal accession.version such as GCF_000001405.39 should be provided. 
+* Provide an NCBI assembly report file. For a given assembly it can be downloaded from the [NCBI Assembly](https://www.ncbi.nlm.nih.gov/assembly) website. If the 'Download' button is used, this file is called 'Assembly structure report'. On the [NCBI Genomes FTP](https://ftp.ncbi.nlm.nih.gov/genomes/all/) site, these files have the suffix `assembly_report.txt`. 
+
```

### Comparing `cthreepo-0.1.2/README.md` & `cthreepo-0.1.3/cthreepo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,57 @@
+Metadata-Version: 2.1
+Name: cthreepo
+Version: 0.1.3
+Summary: A python tool to interconvert seq-ids in gff3, gtf, bed and other files.
+Home-page: http://github.com/vkkodali/cthreepo
+Author: Vamsi Kodali
+Author-email: vkkodali@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+
 # cthreepo
+[![PyPI version](https://badge.fury.io/py/cthreepo.svg)](https://badge.fury.io/py/cthreepo)
+[![Conda](https://img.shields.io/conda/dn/bioconda/cthreepo?label=bioconda-install&style=flat)](https://anaconda.org/bioconda/cthreepo)
+
 A python script to interconvert seq-ids in gff3, gtf, bed and other files.
+
 ---
 ## Quick start for the impatient
-1. Clone the repository
-2. Run the following to install: 
+1. Install using conda 
 ```
-python3 setup.py install
+conda install -c bioconda cthreepo 
 ```
-3. Execute as follows:
+2. Execute as follows:
 ```
 ## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
 ## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
 cthreepo -i <input.gff3> -if rs -it uc -f gff3 -m h38 -o <output.gff3>
 ```
 ---
+
 ## Introduction
 NCBI RefSeq, UCSC and Ensembl use different identifiers for chromosomes in annotation and other files such as GFF3, GTF, etc. Users interested in using a mix of files downloaded from different sources and use them in a single pipeline may end up with seq-id mismatch related errors. This script converts seq-ids from one style to the other in order to make the files compatible with each other.
 
 ## Installation and Usage
-Python3 is required for this script to work. With that requirement satisfied, download/clone the repository, install and run the script `cthreepo.py` as shown below.
+Python3 is required for this script to work. With that requirement satisfied, you can install as shown below:
+### Install using conda 
+```
+conda install -c bioconda cthreepo 
+```
+### Install using pip
+```
+pip install cthreepo
+```
+### Install from this repository
+First, download/clone the repository. Then run: 
 ```
-## installation
 python3 setup.py install
-
+```
+### Usage
+```
 ## help
 cthreepo --help 
 
 ## usage
 ## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
 ## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
 cthreepo \
```

### Comparing `cthreepo-0.1.2/cthreepo/__init__.py` & `cthreepo-0.1.3/cthreepo/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                 'gb': 4,
                 'rs': 6,
                 'uc': 9,
                 'ensembl': 0,
                 'genbank': 4,
                 'refseq': 6,
                 'ucsc': 9,
+                'any': 99,
                 }
     format_dict = {
                 'gff3'     : convgxf,
                 'gtf'      : convgxf,
                 'vcf'      : convgxf,
                 'bed'      : convbed,
                 'bedgraph' : convbed,
@@ -96,64 +97,82 @@
 
 def create_maptbl(mapfile):
     with open(mapfile, 'r') as f:
         maptbl = f.readlines()
     return maptbl
 
 def chrnamedict(maptbl, id_from, id_to, p):
-    """
-    create a mapping dict that will be used swap seq-ids in the input file
-    ## params
-    mapfile : path to NCBI assembly_report.txt format file
-    id_from : column number of the seq-id format in input file
-    id_to   : column number of the seq-id format to convert to
-    ## returns
-    chrmap  : a dict object with id_from:id_to
-    """
     chrmap = {}
-    tbl = csv.reader(maptbl, delimiter = '\t')
-    if p == 'F' and id_from == 0:
-        for line in tbl:
-            if not line[0].startswith('#') and line[id_to] != 'na':
-                chrmap[line[id_from]] = line[id_to]
-                # to deal with ens using gb seq-ids in their GTF
-                chrmap[line[4]] = line[id_to]
-                # to deal with ens prepending CHR to their patches, etc
-                chrmap['CHR_'+line[id_from]] = line[id_to]
-    if p == 'F' and id_from != 0:
-        for line in tbl:
-            if not line[0].startswith('#') and line[id_to] != 'na':
-                    chrmap[line[id_from]] = line[id_to]
-    elif p == 'T':
-        for line in tbl:
-            if not line[0].startswith('#') and line[0] == '1':
-                au = line[7]
-                print(au, file=sys.stderr)
-                chrmap[line[id_from]] = line[id_to]
-                break
-        for line in tbl:
-            if not line[0].startswith('#') and line[7] == au:
-                chrmap[line[id_from]] = line[id_to]
+    ## add all seq-ids to the dict
+    ## maptbl is just a list but csv reader still works
+    tbl = csv.reader(maptbl, delimiter='\t')
+    for line in tbl:
+        if line[0].startswith('#'): continue
+        if line[id_to] == 'na': continue
+        if id_from == 0:
+            chrmap[line[id_from]] = line[id_to]
+            chrmap[line[4]] = line[id_to] # to deal with ens using gb seq-ids in their GTF
+            if 'CHR' in line[id_from]:
+                chrmap['CHR_'+line[id_from]] = line[id_to] # to deal with ens prepending CHR to their patches, etc
+            if line[id_from] == 'MT':
+                chrmap['chrMT'] = line[id_to] # to deal with chrMT corner case
+        if id_from in [4, 6, 9]:
+            chrmap[line[id_from]] = line[id_to]
+        if id_from == 99:
+            cols = [0, 4, 6, 9]
+            cols.remove(id_to)
+            for col in cols:
+                chrmap[line[col]] = line[id_to]
+                if 'CHR' in line[col]:
+                    chrmap['CHR_'+line[col]] = line[id_to] # to deal with ens prepending CHR to their patches, etc
+                if line[col] == 'MT':
+                    chrmap['chrMT'] = line[id_to] # to deal with chrMT corner case
+
+    chrmap.pop('na', None)
+
+    ## if -p option is set, remove non-primary accs from dict
+    if p == 'T':
+        for line in maptbl:
+            if line.startswith('#'): continue 
+            line = line.split('\t')
+            au = line[7]
+            break
+
+        priassm_accs = set()
+        for line in maptbl:
+            if line.startswith('#'): continue
+            line = line.split('\t')
+            if line[7] == au:
+                for i in [0, 4, 6, 9]:
+                    priassm_accs.add(line[i])
+        priassm_accs.discard('na')
+
+        print(f'Restricting translation to "{au}" only ({len(priassm_accs)} seq-ids)', 
+              file=sys.stderr)            
+
+        for k in set(chrmap) - priassm_accs:
+            del chrmap[k]
+
     return chrmap
 
 def main():
     parser = argparse.ArgumentParser(description ="""This script parses input
                 file and converts the seq-id name from one kind to the other""")
     parser.add_argument('-i', '--infile', help="input file")
     parser.add_argument('-o', '--outfile', help="output file")
     mapgroup = parser.add_mutually_exclusive_group(required=True)
     mapgroup.add_argument('-m', '--mapfile',
                         help = "NCBI style assembly_report file for mapping")
     mapgroup.add_argument('-a', '--accn',
                         help = "NCBI Assembly Accession with version")
-    parser.add_argument('-if', '--id_from', default = 'uc',
-                        choices = ['uc', 'rs', 'gb', 'ens'],
+    parser.add_argument('-if', '--id_from', default = 'any',
+                        choices = ['any', 'uc', 'rs', 'gb', 'ens'],
                         type = lambda s: s.lower().strip(),
                         help = "seq-id format in the input file; can be \
-                            `ens`, `uc`, `gb`, or `rs`; default is `uc`")
+                            `any`, `ens`, `uc`, `gb`, or `rs`; default is `any`")
     parser.add_argument('-it', '--id_to', default = 'rs', 
                         choices = ['uc', 'rs', 'gb', 'ens'],
                         type = lambda s: s.lower().strip(),
                         help = "seq-id format in the output file; can be \
                             `ens`, `uc`, `gb`, or `rs`; default is `rs`")
     parser.add_argument('-ku', '--keep_unmapped', action='store_true',
                         help = "keep lines that don't have seq-id matches")
```

### Comparing `cthreepo-0.1.2/cthreepo/converters.py` & `cthreepo-0.1.3/cthreepo/converters.py`

 * *Files identical despite different names*

### Comparing `cthreepo-0.1.2/cthreepo/fetch_assm_report.py` & `cthreepo-0.1.3/cthreepo/fetch_assm_report.py`

 * *Files identical despite different names*

### Comparing `cthreepo-0.1.2/cthreepo/mapfiles/h37.map` & `cthreepo-0.1.3/cthreepo/mapfiles/h37.map`

 * *Files identical despite different names*

### Comparing `cthreepo-0.1.2/cthreepo/mapfiles/h38.map` & `cthreepo-0.1.3/cthreepo/mapfiles/h38.map`

 * *Files identical despite different names*

### Comparing `cthreepo-0.1.2/cthreepo/mapfiles/m37.map` & `cthreepo-0.1.3/cthreepo/mapfiles/m37.map`

 * *Files identical despite different names*

### Comparing `cthreepo-0.1.2/cthreepo/mapfiles/m38.map` & `cthreepo-0.1.3/cthreepo/mapfiles/m38.map`

 * *Files identical despite different names*

### Comparing `cthreepo-0.1.2/cthreepo.egg-info/PKG-INFO` & `cthreepo-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,71 @@
-Metadata-Version: 2.1
-Name: cthreepo
-Version: 0.1.2
-Summary: A python tool to interconvert seq-ids in gff3, gtf, bed and other files.
-Home-page: http://github.com/vkkodali/cthreepo
-Author: Vamsi Kodali
-Author-email: vkkodali@gmail.com
-License: MIT
-Description: # cthreepo
-        A python script to interconvert seq-ids in gff3, gtf, bed and other files.
-        ---
-        ## Quick start for the impatient
-        1. Clone the repository
-        2. Run the following to install: 
-        ```
-        python3 setup.py install
-        ```
-        3. Execute as follows:
-        ```
-        ## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
-        ## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
-        cthreepo -i <input.gff3> -if rs -it uc -f gff3 -m h38 -o <output.gff3>
-        ```
-        ---
-        ## Introduction
-        NCBI RefSeq, UCSC and Ensembl use different identifiers for chromosomes in annotation and other files such as GFF3, GTF, etc. Users interested in using a mix of files downloaded from different sources and use them in a single pipeline may end up with seq-id mismatch related errors. This script converts seq-ids from one style to the other in order to make the files compatible with each other.
-        
-        ## Installation and Usage
-        Python3 is required for this script to work. With that requirement satisfied, download/clone the repository, install and run the script `cthreepo.py` as shown below.
-        ```
-        ## installation
-        python3 setup.py install
-        
-        ## help
-        cthreepo --help 
-        
-        ## usage
-        ## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
-        ## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
-        cthreepo \
-            --infile <input.gff3> \
-            --id_from rs \
-            --id_to uc \
-            --format gff3 \
-            --mapfile h38 \
-            --outfile <output.gff3>
-        ```
-        
-        ## File formats supported
-        1. GFF3 (default)
-        2. GTF
-        3. BedGraph
-        4. BED
-        5. SAM
-        6. VCF
-        7. WIG
-        8. TSV
-        
-        ## Mapping files
-        `cthreepo` needs a `mapfile` that it uses to figure out how seq-ids map from one style to the other. 
-        * Use the built-in shortcuts -- `h38`, `h37`, `m38` and `m37` for GRCh38/hg38, GRCh37/hg19, MGSCv37/mm9 and GRCm38/mm10 respectively. I try to keep these files up-to-date but if they don't work as expected, I suggest using the latest file by following one of the two options described below.
-        * Provide NCBI assembly accession using the `-a` parameter. A complete, legal accession.version such as GCF_000001405.39 should be provided. 
-        * Provide an NCBI assembly report file. For a given assembly it can be downloaded from the [NCBI Assembly](https://www.ncbi.nlm.nih.gov/assembly) website. If the 'Download' button is used, this file is called 'Assembly structure report'. On the [NCBI Genomes FTP](https://ftp.ncbi.nlm.nih.gov/genomes/all/) site, these files have the suffix `assembly_report.txt`. 
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# cthreepo
+[![PyPI version](https://badge.fury.io/py/cthreepo.svg)](https://badge.fury.io/py/cthreepo)
+[![Conda](https://img.shields.io/conda/dn/bioconda/cthreepo?label=bioconda-install&style=flat)](https://anaconda.org/bioconda/cthreepo)
+
+A python script to interconvert seq-ids in gff3, gtf, bed and other files.
+
+---
+## Quick start for the impatient
+1. Install using conda 
+```
+conda install -c bioconda cthreepo 
+```
+2. Execute as follows:
+```
+## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
+## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
+cthreepo -i <input.gff3> -if rs -it uc -f gff3 -m h38 -o <output.gff3>
+```
+---
+
+## Introduction
+NCBI RefSeq, UCSC and Ensembl use different identifiers for chromosomes in annotation and other files such as GFF3, GTF, etc. Users interested in using a mix of files downloaded from different sources and use them in a single pipeline may end up with seq-id mismatch related errors. This script converts seq-ids from one style to the other in order to make the files compatible with each other.
+
+## Installation and Usage
+Python3 is required for this script to work. With that requirement satisfied, you can install as shown below:
+### Install using conda 
+```
+conda install -c bioconda cthreepo 
+```
+### Install using pip
+```
+pip install cthreepo
+```
+### Install from this repository
+First, download/clone the repository. Then run: 
+```
+python3 setup.py install
+```
+### Usage
+```
+## help
+cthreepo --help 
+
+## usage
+## convert seq-ids in <input.gff3> from refseq format (NC_000001.11)
+## to UCSC format (chr1) using the Human GRCh38 mapping dictionary
+cthreepo \
+    --infile <input.gff3> \
+    --id_from rs \
+    --id_to uc \
+    --format gff3 \
+    --mapfile h38 \
+    --outfile <output.gff3>
+```
+
+## File formats supported
+1. GFF3 (default)
+2. GTF
+3. BedGraph
+4. BED
+5. SAM
+6. VCF
+7. WIG
+8. TSV
+
+## Mapping files
+`cthreepo` needs a `mapfile` that it uses to figure out how seq-ids map from one style to the other. 
+* Use the built-in shortcuts -- `h38`, `h37`, `m38` and `m37` for GRCh38/hg38, GRCh37/hg19, MGSCv37/mm9 and GRCm38/mm10 respectively. I try to keep these files up-to-date but if they don't work as expected, I suggest using the latest file by following one of the two options described below.
+* Provide NCBI assembly accession using the `-a` parameter. A complete, legal accession.version such as GCF_000001405.39 should be provided. 
+* Provide an NCBI assembly report file. For a given assembly it can be downloaded from the [NCBI Assembly](https://www.ncbi.nlm.nih.gov/assembly) website. If the 'Download' button is used, this file is called 'Assembly structure report'. On the [NCBI Genomes FTP](https://ftp.ncbi.nlm.nih.gov/genomes/all/) site, these files have the suffix `assembly_report.txt`. 
+
```

### Comparing `cthreepo-0.1.2/setup.py` & `cthreepo-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='cthreepo',
-    version='0.1.2',
+    version='0.1.3',
     author='Vamsi Kodali',
     author_email='vkkodali@gmail.com',
     description='A python tool to interconvert seq-ids in gff3, gtf, bed and other files.',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url='http://github.com/vkkodali/cthreepo',
     license='MIT',
```

