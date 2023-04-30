# Comparing `tmp/blitzgsea-1.3.3.tar.gz` & `tmp/blitzgsea-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blitzgsea-1.3.3.tar", last modified: Sat Apr 29 19:45:11 2023, max compression
+gzip compressed data, was "blitzgsea-1.3.4.tar", last modified: Sun Apr 30 01:06:55 2023, max compression
```

## Comparing `blitzgsea-1.3.3.tar` & `blitzgsea-1.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-29 19:45:11.125198 blitzgsea-1.3.3/
--rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-07-24 15:38:47.000000 blitzgsea-1.3.3/LICENSE
--rw-r--r--   0 maayanlab   (501) staff       (20)     9725 2023-04-29 19:45:11.125000 blitzgsea-1.3.3/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)     9167 2023-04-28 00:28:45.000000 blitzgsea-1.3.3/README.md
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-29 19:45:11.123472 blitzgsea-1.3.3/blitzgsea/
--rw-r--r--   0 maayanlab   (501) staff       (20)    15508 2023-04-29 01:49:21.000000 blitzgsea-1.3.3/blitzgsea/__init__.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2768 2023-04-28 02:23:48.000000 blitzgsea-1.3.3/blitzgsea/enrichr.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     7316 2022-07-24 15:38:47.000000 blitzgsea-1.3.3/blitzgsea/plot.py
--rw-r--r--   0 maayanlab   (501) staff       (20)     2594 2022-07-24 15:38:47.000000 blitzgsea-1.3.3/blitzgsea/shuffle.py
-drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-29 19:45:11.124723 blitzgsea-1.3.3/blitzgsea.egg-info/
--rw-r--r--   0 maayanlab   (501) staff       (20)     9725 2023-04-29 19:45:11.000000 blitzgsea-1.3.3/blitzgsea.egg-info/PKG-INFO
--rw-r--r--   0 maayanlab   (501) staff       (20)      272 2023-04-29 19:45:11.000000 blitzgsea-1.3.3/blitzgsea.egg-info/SOURCES.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-04-29 19:45:11.000000 blitzgsea-1.3.3/blitzgsea.egg-info/dependency_links.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)      128 2023-04-29 19:45:11.000000 blitzgsea-1.3.3/blitzgsea.egg-info/requires.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       10 2023-04-29 19:45:11.000000 blitzgsea-1.3.3/blitzgsea.egg-info/top_level.txt
--rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-04-29 19:45:11.125254 blitzgsea-1.3.3/setup.cfg
--rw-r--r--   0 maayanlab   (501) staff       (20)     1083 2023-04-29 01:49:27.000000 blitzgsea-1.3.3/setup.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:06:55.149342 blitzgsea-1.3.4/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11357 2022-07-24 15:38:47.000000 blitzgsea-1.3.4/LICENSE
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11988 2023-04-30 01:06:55.149126 blitzgsea-1.3.4/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11430 2023-04-30 01:04:00.000000 blitzgsea-1.3.4/README.md
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:06:55.148006 blitzgsea-1.3.4/blitzgsea/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    15508 2023-04-29 01:49:21.000000 blitzgsea-1.3.4/blitzgsea/__init__.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2768 2023-04-28 02:23:48.000000 blitzgsea-1.3.4/blitzgsea/enrichr.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     7316 2022-07-24 15:38:47.000000 blitzgsea-1.3.4/blitzgsea/plot.py
+-rw-r--r--   0 maayanlab   (501) staff       (20)     2594 2022-07-24 15:38:47.000000 blitzgsea-1.3.4/blitzgsea/shuffle.py
+drwxr-xr-x   0 maayanlab   (501) staff       (20)        0 2023-04-30 01:06:55.148881 blitzgsea-1.3.4/blitzgsea.egg-info/
+-rw-r--r--   0 maayanlab   (501) staff       (20)    11988 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/PKG-INFO
+-rw-r--r--   0 maayanlab   (501) staff       (20)      272 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/SOURCES.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)        1 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/dependency_links.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)      128 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/requires.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       10 2023-04-30 01:06:55.000000 blitzgsea-1.3.4/blitzgsea.egg-info/top_level.txt
+-rw-r--r--   0 maayanlab   (501) staff       (20)       38 2023-04-30 01:06:55.149398 blitzgsea-1.3.4/setup.cfg
+-rw-r--r--   0 maayanlab   (501) staff       (20)     1083 2023-04-30 00:23:09.000000 blitzgsea-1.3.4/setup.py
```

### Comparing `blitzgsea-1.3.3/LICENSE` & `blitzgsea-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.3/PKG-INFO` & `blitzgsea-1.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blitzgsea
-Version: 1.3.3
+Version: 1.3.4
 Summary: Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea
 Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,34 +12,59 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/bgsea_small.png" width=200>
 
+[Installation](#installation) | [Example](#python-example) | [Optional Parameters](#optional-parameters) | [Speed-up](#speeding-up-enrichment-calculations) | [Plotting](#plotting-enrichment-results) | [Attribution](#attribution) | [References](#references)
+
 # blitzGSEA Introduction
 
 This Python package provides a computationally performant <b>G</b>ene <b>S</b>et <b>E</b>nrichment <b>A</b>nalysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy was used as the reference for the running sum and enrichment score calculation [2]. The algorithm estimates the enrichment score (ES) distribution of the null model by fitting data to gamma distibutions instead of calculating permutations for each gene set. blitzGSEA calculates p-values with much higher accuracy than other reference implementations available in Python.
 
 Gene set libraries can directly be loaded from Enrichr (<a href="https://maayanlab.cloud/Enrichr" target="_blank">https://maayanlab.cloud/Enrichr</a>). For this use the `blitzgsea.enrichr.get_library()` function. All libraries can also be listed with `blitzgsea.enrichr.print_libraries()`.
 
 blitzGSEA provides plotting functions to generate publication ready figures similar to the original GSEA-P software. `blitzgsea.plot.running_sum()` plots an enrichment plot for a single gene set and `blitzgsea.plot.top_table()` plots the top `n` gene sets in a compact table. 
 
 # Installation
 
 blitzGSEA is currently only available as a Python package in this GitHub repository. You can install the blitzGSEA Python package and its dependencies through pip by using the following command:
 
 ```
-$ pip install git+https://github.com/MaayanLab/blitzgsea.git
+$ pip install blitzgsea
 ```
 
 # Run enrichment analysis using blitzGSEA
 
 blitzGSEA depends on two input files. 1) a gene signature and 2) a gene set library. The gene set library is a dictionary with the name of the gene set as key and a list of gene ids as values. Gene set libraries can be loaded directly from Enrichr. The signature should be a pandas dataframe with two columns [0,1]. The first column should contain the gene ids (matching the gene ids in the gene set library).
 
+### Python example
+
+This short example will download two files (signature and gene set library). The gene set library consists of KEGG pathways and the signature is an example signature of differential gene expression of muscle samples from young and old donors. Differential gene expression was computed with Limma Voom.
+
+```python
+import blitzgsea as blitz
+import pandas as pd
+
+# read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
+
+# list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries()
+
+# use enrichr submodule to retrieve gene set library
+library = blitz.enrichr.get_library("KEGG_2021_Human")
+
+# run enrichment analysis
+result = blitz.gsea(signature, library)
+```
+
+### Example Input
+
 | index | 0	| 1 |
 |:-----|:-------------:|------:|
 | 1	| ADO	| -7.833439 |
 | 2	| CHUK	| -7.800920 |
 | 3	| GOLGA4	| -7.78722 |
 | ... | ... | ... |
 
@@ -61,55 +86,63 @@
                                                  'LILRB2',
                                                  ...
                                                 ],
 ...
 }
 ```
 
-### Python example
-
-This short example will download two files (signature and gene set library). The gene set library consists of KEGG pathways and the signature is an example signature of differential gene expression of muscle samples from young and old donors. Differential gene expression was computed with Limma Voom.
-
-```python
-import blitzgsea as blitz
-import pandas as pd
-
-# read signature as pandas dataframe
-signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
-
-# list available gene set libraries in Enrichr
-blitz.enrichr.print_libraries()
-
-# use enrichr submodule to retrieve gene set library
-library = blitz.enrichr.get_library("KEGG_2021_Human")
-
-# run enrichment analysis
-result = blitz.gsea(signature, library)
-```
-
 ### Optional Parameters
 
 The main function of `blitzgsea.gsea()` supports several optional parameters. The default parameters should work well for most use cases. 
 
 | parameter name | type | default	| description |
 |:-----|:---------|:-------------|:------|
 | `permutations`	| int | 2000	| Number of randomized permutations to estimate ES distributions. |
 | `min_size` | int | 5 | Minimum number of genes in geneset. |
 | `max_size` | int | 4000 | Maximal number of genes in gene set. |
 | `anchors`	| int | 20 | Number of gene set size distributions calculated. Remaining are interpolated. |
 | `processes`	| int | 4	| Number of parallel threads. Not much gain after 4 threads. |
 | `symmetric` | bool | False | Use same distribution parameters for negative and positive ES. If `False` estimate them separately. |
-| `signature_cache` | bool | True | Use precomputed anchor parameters. |
-| `shared_null` | bool | False | Use same null for all signatures (Only computes calibration once). |
+| `signature_cache` | bool | True | Cache precomputed anchor parameters in memory for later reuse. |
+| `shared_null` | bool | False | Use same null for signatures if a compatible model already exists. (uses KL-divergence test). |
+| `kl_threshold`| float | 0.3 | Controls how similar signature value distributions have to be for reuse. |
+| `kl_bins`| int | 200 | Number of bins in PDF representation of distributions for KL test. |
 | `plotting`| bool | False | Plot estimated anchor parametes. |
 | `verbose` | bool | False | Toggle additonal output. |
 | `progress` | bool | False | Toggle progress bar. |
 | `seed` | int | 0 | Random seed. Same seed will result in identical result. If seed equal `-1` generate random seed. |
 | `add_noise` | bool | False | Add small random noise to signature. The noise is a fraction of the expression values. |
 
+### Speeding up enrichment calculations
+
+blitzGSEA is currently the fastest GSEA implementation. The most time-consuming step of blitzGSEA is the generation of a robust null distribution to compute p-values. Since the null distribution depends on the value distribution of the input signature, blitzGSEA will, by default, compute a new null for each new input signature. blitzGSEA can compute the similarity between input signatures using Kullback–Leibler divergence to identify similar signatures to share null models. A cached null model is used if a previous signature has a similar value distribution. The relevant parameters of the `blitzgsea.gsea()` function are shown below:
+
+| parameter name | type | default	| description |
+|:-----|:---------|:-------------|:------|
+| `signature_cache` | bool | True | Cache precomputed anchor parameters in memory for later reuse. |
+| `shared_null` | bool | False | Use same null for signatures if a compatible model already exists. (uses KL-divergence test). |
+| `kl_threshold`| float | 0.3 | Controls how similar signature value distributions have to be for reuse. The smaller the more conservative. |
+| `kl_bins`| int | 200 | Number of bins in PDF representation of distributions for KL test. |
+
+### Example
+```python
+
+import blitzgsea as blitz
+import pandas as pd
+
+# read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
+
+# list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries()
+
+# run enrichment analysis
+result = blitz.gsea(signature, library, shared_null=True)
+```
+
 ### Plotting enrichment results
 
 blitzGSEA supports several plotting functions. `blitzgsea.plot.running_sum()` and `blitzgsea.plot.top_table()` can be used after enrichment has been performed. `blitzgsea.plot.running_sum()` shows the running sum of an individual gene set. It has a `compact` mode in which the image will be more readable if small. `blitzgsea.plot.top_table()` shows the top `n` enriched gene sets and displays the results in a table, with normalized enrichment score (NES) and the distribution of hits relative to the gene ranking of the signature.
 
 ### Example
 ```python
 
@@ -153,32 +186,32 @@
 
 #### top_table.pdf
 <img title="a title" alt="blitzGSEA sunning_sum" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/top_table.png" width=300>
 
 ### Sample shuffling
 This is the sample shuffling algorithm from GSEApy. It performs a t-test to build signatures for phenotype shuffled groups. The input is a gene expression dataframe, which should be normalized for library size. `groups` is a list containing 0 or 1 describing the corresponding group for the samples in `exprs`. The index of `exprs` are the gene ids matching the gene set library. 
 
-```
+```python
 blitz.shuffle.gsea(exprs, library, groups, permutations=50, seed=1)
 ```
 
 | parameter name | type | default	| description |
 |:-----|:---------|:-------------|:------|
 | `exprs`	| pd.DataFrame | NA	| Normalized gene expression matrix. |
 | `library` | dictionary | NA | Gene set library. |
 | `groups` | list | NA | Phenotype group labels of samples. Labels are 0 or 1. |
 | `permutations` | int | 1000 | Number of permutations. |
 | `seed`	| int | 1 | Random state seed. |
 
 # Dependencies
 Python 3.6+
 
-# Citation
+# Attribution
 
-When using blitzgsea please cite the following reference:
+The statistical tool was developed by the [Ma'ayan Laboratory]([https://www.google.com](https://labs.icahn.mssm.edu/maayanlab/)). When using blitzgsea please cite the following reference:
 
 Lachmann, Alexander, Zhuorui Xie, and Avi Ma’ayan. "blitzGSEA: efficient computation of gene set enrichment analysis through gamma distribution approximation." Bioinformatics (2022).
 https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btac076/6526383?login=false
 
 # References
 
 [1] Lachmann, Alexander, Zhuorui Xie, and Avi Ma’ayan. "blitzGSEA: efficient computation of gene set enrichment analysis through gamma distribution approximation." Bioinformatics (2022).
```

#### html2text {}

```diff
@@ -1,114 +1,143 @@
-Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.3 Summary: Package for fast
+Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.4 Summary: Package for fast
 calculation of GSEA similar to prerank using gamma distribution approximation.
 Home-page: https://github.com/maayanlab/blitzgsea Author: Alexander Lachmann
 Author-email: alexander.lachmann@mssm.edu License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE [blitzGSEA] # blitzGSEA Introduction This Python package
-provides a computationally performant Gene Set Enrichment Analysis (GSEA)
-implementation of the pre-rank algorithm [1]. GSEApy was used as the reference
-for the running sum and enrichment score calculation [2]. The algorithm
-estimates the enrichment score (ES) distribution of the null model by fitting
-data to gamma distibutions instead of calculating permutations for each gene
-set. blitzGSEA calculates p-values with much higher accuracy than other
-reference implementations available in Python. Gene set libraries can directly
-be loaded from Enrichr (https://maayanlab.cloud/Enrichr). For this use the
-`blitzgsea.enrichr.get_library()` function. All libraries can also be listed
-with `blitzgsea.enrichr.print_libraries()`. blitzGSEA provides plotting
+License-File: LICENSE [blitzGSEA] [Installation](#installation) | [Example]
+(#python-example) | [Optional Parameters](#optional-parameters) | [Speed-up]
+(#speeding-up-enrichment-calculations) | [Plotting](#plotting-enrichment-
+results) | [Attribution](#attribution) | [References](#references) # blitzGSEA
+Introduction This Python package provides a computationally performant Gene Set
+Enrichment Analysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy
+was used as the reference for the running sum and enrichment score calculation
+[2]. The algorithm estimates the enrichment score (ES) distribution of the null
+model by fitting data to gamma distibutions instead of calculating permutations
+for each gene set. blitzGSEA calculates p-values with much higher accuracy than
+other reference implementations available in Python. Gene set libraries can
+directly be loaded from Enrichr (https://maayanlab.cloud/Enrichr). For this use
+the `blitzgsea.enrichr.get_library()` function. All libraries can also be
+listed with `blitzgsea.enrichr.print_libraries()`. blitzGSEA provides plotting
 functions to generate publication ready figures similar to the original GSEA-
 P software. `blitzgsea.plot.running_sum()` plots an enrichment plot for a
 single gene set and `blitzgsea.plot.top_table()` plots the top `n` gene sets in
 a compact table. # Installation blitzGSEA is currently only available as a
 Python package in this GitHub repository. You can install the blitzGSEA Python
 package and its dependencies through pip by using the following command: ``` $
-pip install git+https://github.com/MaayanLab/blitzgsea.git ``` # Run enrichment
-analysis using blitzGSEA blitzGSEA depends on two input files. 1) a gene
-signature and 2) a gene set library. The gene set library is a dictionary with
-the name of the gene set as key and a list of gene ids as values. Gene set
-libraries can be loaded directly from Enrichr. The signature should be a pandas
-dataframe with two columns [0,1]. The first column should contain the gene ids
-(matching the gene ids in the gene set library). | index | 0 | 1 | |:-----|:---
-----------:|------:| | 1 | ADO | -7.833439 | | 2 | CHUK | -7.800920 | | 3 |
-GOLGA4 | -7.78722 | | ... | ... | ... | The gene set library is a dictionary
-with the gene set names as key and lists of gene ids as values. ```python
-{ 'ERBB2 SIGNALING PATHWAY (GO:0038128)': ['CDC37', 'PTPN12', 'PIK3CA', 'SOS1',
-'CPNE3', 'EGF', ... ], 'HETEROTYPIC CELL-CELL ADHESION (GO:0034113)': ['DSC2',
-'ITGAV', 'ITGAD', 'LILRB2', ... ], ... } ``` ### Python example This short
-example will download two files (signature and gene set library). The gene set
-library consists of KEGG pathways and the signature is an example signature of
-differential gene expression of muscle samples from young and old donors.
-Differential gene expression was computed with Limma Voom. ```python import
-blitzgsea as blitz import pandas as pd # read signature as pandas dataframe
-signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/
-testing/ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
-blitz.enrichr.print_libraries() # use enrichr submodule to retrieve gene set
-library library = blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment
-analysis result = blitz.gsea(signature, library) ``` ### Optional Parameters
-The main function of `blitzgsea.gsea()` supports several optional parameters.
-The default parameters should work well for most use cases. | parameter name |
-type | default | description | |:-----|:---------|:-------------|:------| |
-`permutations` | int | 2000 | Number of randomized permutations to estimate ES
-distributions. | | `min_size` | int | 5 | Minimum number of genes in geneset. |
-| `max_size` | int | 4000 | Maximal number of genes in gene set. | | `anchors`
-| int | 20 | Number of gene set size distributions calculated. Remaining are
-interpolated. | | `processes` | int | 4 | Number of parallel threads. Not much
-gain after 4 threads. | | `symmetric` | bool | False | Use same distribution
-parameters for negative and positive ES. If `False` estimate them separately. |
-| `signature_cache` | bool | True | Use precomputed anchor parameters. | |
-`shared_null` | bool | False | Use same null for all signatures (Only computes
-calibration once). | | `plotting`| bool | False | Plot estimated anchor
-parametes. | | `verbose` | bool | False | Toggle additonal output. | |
-`progress` | bool | False | Toggle progress bar. | | `seed` | int | 0 | Random
-seed. Same seed will result in identical result. If seed equal `-1` generate
-random seed. | | `add_noise` | bool | False | Add small random noise to
-signature. The noise is a fraction of the expression values. | ### Plotting
-enrichment results blitzGSEA supports several plotting functions.
-`blitzgsea.plot.running_sum()` and `blitzgsea.plot.top_table()` can be used
-after enrichment has been performed. `blitzgsea.plot.running_sum()` shows the
-running sum of an individual gene set. It has a `compact` mode in which the
-image will be more readable if small. `blitzgsea.plot.top_table()` shows the
-top `n` enriched gene sets and displays the results in a table, with normalized
-enrichment score (NES) and the distribution of hits relative to the gene
-ranking of the signature. ### Example ```python import blitzgsea as blitz
+pip install blitzgsea ``` # Run enrichment analysis using blitzGSEA blitzGSEA
+depends on two input files. 1) a gene signature and 2) a gene set library. The
+gene set library is a dictionary with the name of the gene set as key and a
+list of gene ids as values. Gene set libraries can be loaded directly from
+Enrichr. The signature should be a pandas dataframe with two columns [0,1]. The
+first column should contain the gene ids (matching the gene ids in the gene set
+library). ### Python example This short example will download two files
+(signature and gene set library). The gene set library consists of KEGG
+pathways and the signature is an example signature of differential gene
+expression of muscle samples from young and old donors. Differential gene
+expression was computed with Limma Voom. ```python import blitzgsea as blitz
 import pandas as pd # read signature as pandas dataframe signature =
 pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/
 ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
 blitz.enrichr.print_libraries() # use enrichr submodule to retrieve gene set
 library library = blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment
-analysis result = blitz.gsea(signature, library) # plot the enrichment results
-and save to pdf fig = blitz.plot.running_sum(signature, "CELL ADHESION
-MOLECULES", library, result=result, compact=False) fig.savefig
-("running_sum.png", bbox_inches='tight') fig_compact = blitz.plot.running_sum
-(signature, "CELL ADHESION MOLECULES", library, result=result, compact=True)
-fig_compact.savefig("running_sum_compact.png", bbox_inches='tight') fig_table =
+analysis result = blitz.gsea(signature, library) ``` ### Example Input | index
+| 0 | 1 | |:-----|:-------------:|------:| | 1 | ADO | -7.833439 | | 2 | CHUK |
+-7.800920 | | 3 | GOLGA4 | -7.78722 | | ... | ... | ... | The gene set library
+is a dictionary with the gene set names as key and lists of gene ids as values.
+```python { 'ERBB2 SIGNALING PATHWAY (GO:0038128)': ['CDC37', 'PTPN12',
+'PIK3CA', 'SOS1', 'CPNE3', 'EGF', ... ], 'HETEROTYPIC CELL-CELL ADHESION (GO:
+0034113)': ['DSC2', 'ITGAV', 'ITGAD', 'LILRB2', ... ], ... } ``` ### Optional
+Parameters The main function of `blitzgsea.gsea()` supports several optional
+parameters. The default parameters should work well for most use cases. |
+parameter name | type | default | description | |:-----|:---------|:-----------
+--|:------| | `permutations` | int | 2000 | Number of randomized permutations
+to estimate ES distributions. | | `min_size` | int | 5 | Minimum number of
+genes in geneset. | | `max_size` | int | 4000 | Maximal number of genes in gene
+set. | | `anchors` | int | 20 | Number of gene set size distributions
+calculated. Remaining are interpolated. | | `processes` | int | 4 | Number of
+parallel threads. Not much gain after 4 threads. | | `symmetric` | bool | False
+| Use same distribution parameters for negative and positive ES. If `False`
+estimate them separately. | | `signature_cache` | bool | True | Cache
+precomputed anchor parameters in memory for later reuse. | | `shared_null` |
+bool | False | Use same null for signatures if a compatible model already
+exists. (uses KL-divergence test). | | `kl_threshold`| float | 0.3 | Controls
+how similar signature value distributions have to be for reuse. | | `kl_bins`|
+int | 200 | Number of bins in PDF representation of distributions for KL test.
+| | `plotting`| bool | False | Plot estimated anchor parametes. | | `verbose` |
+bool | False | Toggle additonal output. | | `progress` | bool | False | Toggle
+progress bar. | | `seed` | int | 0 | Random seed. Same seed will result in
+identical result. If seed equal `-1` generate random seed. | | `add_noise` |
+bool | False | Add small random noise to signature. The noise is a fraction of
+the expression values. | ### Speeding up enrichment calculations blitzGSEA is
+currently the fastest GSEA implementation. The most time-consuming step of
+blitzGSEA is the generation of a robust null distribution to compute p-values.
+Since the null distribution depends on the value distribution of the input
+signature, blitzGSEA will, by default, compute a new null for each new input
+signature. blitzGSEA can compute the similarity between input signatures using
+KullbackâLeibler divergence to identify similar signatures to share null
+models. A cached null model is used if a previous signature has a similar value
+distribution. The relevant parameters of the `blitzgsea.gsea()` function are
+shown below: | parameter name | type | default | description | |:-----|:-------
+--|:-------------|:------| | `signature_cache` | bool | True | Cache
+precomputed anchor parameters in memory for later reuse. | | `shared_null` |
+bool | False | Use same null for signatures if a compatible model already
+exists. (uses KL-divergence test). | | `kl_threshold`| float | 0.3 | Controls
+how similar signature value distributions have to be for reuse. The smaller the
+more conservative. | | `kl_bins`| int | 200 | Number of bins in PDF
+representation of distributions for KL test. | ### Example ```python import
+blitzgsea as blitz import pandas as pd # read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/
+testing/ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries() # run enrichment analysis result = blitz.gsea
+(signature, library, shared_null=True) ``` ### Plotting enrichment results
+blitzGSEA supports several plotting functions. `blitzgsea.plot.running_sum()`
+and `blitzgsea.plot.top_table()` can be used after enrichment has been
+performed. `blitzgsea.plot.running_sum()` shows the running sum of an
+individual gene set. It has a `compact` mode in which the image will be more
+readable if small. `blitzgsea.plot.top_table()` shows the top `n` enriched gene
+sets and displays the results in a table, with normalized enrichment score
+(NES) and the distribution of hits relative to the gene ranking of the
+signature. ### Example ```python import blitzgsea as blitz import pandas as pd
+# read signature as pandas dataframe signature = pd.read_csv("https://
+github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv") # list
+available gene set libraries in Enrichr blitz.enrichr.print_libraries() # use
+enrichr submodule to retrieve gene set library library =
+blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment analysis result =
+blitz.gsea(signature, library) # plot the enrichment results and save to pdf
+fig = blitz.plot.running_sum(signature, "CELL ADHESION MOLECULES", library,
+result=result, compact=False) fig.savefig("running_sum.png",
+bbox_inches='tight') fig_compact = blitz.plot.running_sum(signature, "CELL
+ADHESION MOLECULES", library, result=result, compact=True) fig_compact.savefig
+("running_sum_compact.png", bbox_inches='tight') fig_table =
 blitz.plot.top_table(signature, library, result, n=15) fig_table.savefig
 ("top_table.png", bbox_inches='tight') ``` The resulting plots will look like
 the examples below: #### running_sum.pdf
 [blitzGSEA sunning_sum]
 #### running_sum_compact.pdf [blitzGSEA sunning_sum] #### top_table.pdf
 [blitzGSEA sunning_sum] ### Sample shuffling This is the sample shuffling
 algorithm from GSEApy. It performs a t-test to build signatures for phenotype
 shuffled groups. The input is a gene expression dataframe, which should be
 normalized for library size. `groups` is a list containing 0 or 1 describing
 the corresponding group for the samples in `exprs`. The index of `exprs` are
-the gene ids matching the gene set library. ``` blitz.shuffle.gsea(exprs,
+the gene ids matching the gene set library. ```python blitz.shuffle.gsea(exprs,
 library, groups, permutations=50, seed=1) ``` | parameter name | type | default
 | description | |:-----|:---------|:-------------|:------| | `exprs` |
 pd.DataFrame | NA | Normalized gene expression matrix. | | `library` |
 dictionary | NA | Gene set library. | | `groups` | list | NA | Phenotype group
 labels of samples. Labels are 0 or 1. | | `permutations` | int | 1000 | Number
 of permutations. | | `seed` | int | 1 | Random state seed. | # Dependencies
-Python 3.6+ # Citation When using blitzgsea please cite the following
-reference: Lachmann, Alexander, Zhuorui Xie, and Avi Maâayan. "blitzGSEA:
-efficient computation of gene set enrichment analysis through gamma
-distribution approximation." Bioinformatics (2022). https://academic.oup.com/
-bioinformatics/advance-article/doi/10.1093/bioinformatics/btac076/
-6526383?login=false # References [1] Lachmann, Alexander, Zhuorui Xie, and Avi
-Maâayan. "blitzGSEA: efficient computation of gene set enrichment analysis
-through gamma distribution approximation." Bioinformatics (2022). [2]
-Subramanian, Aravind, Heidi Kuehn, Joshua Gould, Pablo Tamayo, and Jill P.
-Mesirov. "GSEA-P: a desktop application for Gene Set Enrichment Analysis."
-Bioinformatics 23, no. 23 (2007): 3251-3253. [3] Fang, Zhuoqing, Xinyuan Liu,
-and Gary Peltz. "GSEApy: a comprehensive package for performing gene set
-enrichment analysis in Python." Bioinformatics (2022).
+Python 3.6+ # Attribution The statistical tool was developed by the [Ma'ayan
+Laboratory]([https://www.google.com](https://labs.icahn.mssm.edu/maayanlab/)).
+When using blitzgsea please cite the following reference: Lachmann, Alexander,
+Zhuorui Xie, and Avi Maâayan. "blitzGSEA: efficient computation of gene set
+enrichment analysis through gamma distribution approximation." Bioinformatics
+(2022). https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/
+bioinformatics/btac076/6526383?login=false # References [1] Lachmann,
+Alexander, Zhuorui Xie, and Avi Maâayan. "blitzGSEA: efficient computation of
+gene set enrichment analysis through gamma distribution approximation."
+Bioinformatics (2022). [2] Subramanian, Aravind, Heidi Kuehn, Joshua Gould,
+Pablo Tamayo, and Jill P. Mesirov. "GSEA-P: a desktop application for Gene Set
+Enrichment Analysis." Bioinformatics 23, no. 23 (2007): 3251-3253. [3] Fang,
+Zhuoqing, Xinyuan Liu, and Gary Peltz. "GSEApy: a comprehensive package for
+performing gene set enrichment analysis in Python." Bioinformatics (2022).
```

### Comparing `blitzgsea-1.3.3/README.md` & `blitzgsea-1.3.4/blitzgsea.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,70 @@
+Metadata-Version: 2.1
+Name: blitzgsea
+Version: 1.3.4
+Summary: Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.
+Home-page: https://github.com/maayanlab/blitzgsea
+Author: Alexander Lachmann
+Author-email: alexander.lachmann@mssm.edu
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/bgsea_small.png" width=200>
 
+[Installation](#installation) | [Example](#python-example) | [Optional Parameters](#optional-parameters) | [Speed-up](#speeding-up-enrichment-calculations) | [Plotting](#plotting-enrichment-results) | [Attribution](#attribution) | [References](#references)
+
 # blitzGSEA Introduction
 
 This Python package provides a computationally performant <b>G</b>ene <b>S</b>et <b>E</b>nrichment <b>A</b>nalysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy was used as the reference for the running sum and enrichment score calculation [2]. The algorithm estimates the enrichment score (ES) distribution of the null model by fitting data to gamma distibutions instead of calculating permutations for each gene set. blitzGSEA calculates p-values with much higher accuracy than other reference implementations available in Python.
 
 Gene set libraries can directly be loaded from Enrichr (<a href="https://maayanlab.cloud/Enrichr" target="_blank">https://maayanlab.cloud/Enrichr</a>). For this use the `blitzgsea.enrichr.get_library()` function. All libraries can also be listed with `blitzgsea.enrichr.print_libraries()`.
 
 blitzGSEA provides plotting functions to generate publication ready figures similar to the original GSEA-P software. `blitzgsea.plot.running_sum()` plots an enrichment plot for a single gene set and `blitzgsea.plot.top_table()` plots the top `n` gene sets in a compact table. 
 
 # Installation
 
 blitzGSEA is currently only available as a Python package in this GitHub repository. You can install the blitzGSEA Python package and its dependencies through pip by using the following command:
 
 ```
-$ pip install git+https://github.com/MaayanLab/blitzgsea.git
+$ pip install blitzgsea
 ```
 
 # Run enrichment analysis using blitzGSEA
 
 blitzGSEA depends on two input files. 1) a gene signature and 2) a gene set library. The gene set library is a dictionary with the name of the gene set as key and a list of gene ids as values. Gene set libraries can be loaded directly from Enrichr. The signature should be a pandas dataframe with two columns [0,1]. The first column should contain the gene ids (matching the gene ids in the gene set library).
 
+### Python example
+
+This short example will download two files (signature and gene set library). The gene set library consists of KEGG pathways and the signature is an example signature of differential gene expression of muscle samples from young and old donors. Differential gene expression was computed with Limma Voom.
+
+```python
+import blitzgsea as blitz
+import pandas as pd
+
+# read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
+
+# list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries()
+
+# use enrichr submodule to retrieve gene set library
+library = blitz.enrichr.get_library("KEGG_2021_Human")
+
+# run enrichment analysis
+result = blitz.gsea(signature, library)
+```
+
+### Example Input
+
 | index | 0	| 1 |
 |:-----|:-------------:|------:|
 | 1	| ADO	| -7.833439 |
 | 2	| CHUK	| -7.800920 |
 | 3	| GOLGA4	| -7.78722 |
 | ... | ... | ... |
 
@@ -45,55 +86,63 @@
                                                  'LILRB2',
                                                  ...
                                                 ],
 ...
 }
 ```
 
-### Python example
-
-This short example will download two files (signature and gene set library). The gene set library consists of KEGG pathways and the signature is an example signature of differential gene expression of muscle samples from young and old donors. Differential gene expression was computed with Limma Voom.
-
-```python
-import blitzgsea as blitz
-import pandas as pd
-
-# read signature as pandas dataframe
-signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
-
-# list available gene set libraries in Enrichr
-blitz.enrichr.print_libraries()
-
-# use enrichr submodule to retrieve gene set library
-library = blitz.enrichr.get_library("KEGG_2021_Human")
-
-# run enrichment analysis
-result = blitz.gsea(signature, library)
-```
-
 ### Optional Parameters
 
 The main function of `blitzgsea.gsea()` supports several optional parameters. The default parameters should work well for most use cases. 
 
 | parameter name | type | default	| description |
 |:-----|:---------|:-------------|:------|
 | `permutations`	| int | 2000	| Number of randomized permutations to estimate ES distributions. |
 | `min_size` | int | 5 | Minimum number of genes in geneset. |
 | `max_size` | int | 4000 | Maximal number of genes in gene set. |
 | `anchors`	| int | 20 | Number of gene set size distributions calculated. Remaining are interpolated. |
 | `processes`	| int | 4	| Number of parallel threads. Not much gain after 4 threads. |
 | `symmetric` | bool | False | Use same distribution parameters for negative and positive ES. If `False` estimate them separately. |
-| `signature_cache` | bool | True | Use precomputed anchor parameters. |
-| `shared_null` | bool | False | Use same null for all signatures (Only computes calibration once). |
+| `signature_cache` | bool | True | Cache precomputed anchor parameters in memory for later reuse. |
+| `shared_null` | bool | False | Use same null for signatures if a compatible model already exists. (uses KL-divergence test). |
+| `kl_threshold`| float | 0.3 | Controls how similar signature value distributions have to be for reuse. |
+| `kl_bins`| int | 200 | Number of bins in PDF representation of distributions for KL test. |
 | `plotting`| bool | False | Plot estimated anchor parametes. |
 | `verbose` | bool | False | Toggle additonal output. |
 | `progress` | bool | False | Toggle progress bar. |
 | `seed` | int | 0 | Random seed. Same seed will result in identical result. If seed equal `-1` generate random seed. |
 | `add_noise` | bool | False | Add small random noise to signature. The noise is a fraction of the expression values. |
 
+### Speeding up enrichment calculations
+
+blitzGSEA is currently the fastest GSEA implementation. The most time-consuming step of blitzGSEA is the generation of a robust null distribution to compute p-values. Since the null distribution depends on the value distribution of the input signature, blitzGSEA will, by default, compute a new null for each new input signature. blitzGSEA can compute the similarity between input signatures using Kullback–Leibler divergence to identify similar signatures to share null models. A cached null model is used if a previous signature has a similar value distribution. The relevant parameters of the `blitzgsea.gsea()` function are shown below:
+
+| parameter name | type | default	| description |
+|:-----|:---------|:-------------|:------|
+| `signature_cache` | bool | True | Cache precomputed anchor parameters in memory for later reuse. |
+| `shared_null` | bool | False | Use same null for signatures if a compatible model already exists. (uses KL-divergence test). |
+| `kl_threshold`| float | 0.3 | Controls how similar signature value distributions have to be for reuse. The smaller the more conservative. |
+| `kl_bins`| int | 200 | Number of bins in PDF representation of distributions for KL test. |
+
+### Example
+```python
+
+import blitzgsea as blitz
+import pandas as pd
+
+# read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
+
+# list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries()
+
+# run enrichment analysis
+result = blitz.gsea(signature, library, shared_null=True)
+```
+
 ### Plotting enrichment results
 
 blitzGSEA supports several plotting functions. `blitzgsea.plot.running_sum()` and `blitzgsea.plot.top_table()` can be used after enrichment has been performed. `blitzgsea.plot.running_sum()` shows the running sum of an individual gene set. It has a `compact` mode in which the image will be more readable if small. `blitzgsea.plot.top_table()` shows the top `n` enriched gene sets and displays the results in a table, with normalized enrichment score (NES) and the distribution of hits relative to the gene ranking of the signature.
 
 ### Example
 ```python
 
@@ -137,36 +186,38 @@
 
 #### top_table.pdf
 <img title="a title" alt="blitzGSEA sunning_sum" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/top_table.png" width=300>
 
 ### Sample shuffling
 This is the sample shuffling algorithm from GSEApy. It performs a t-test to build signatures for phenotype shuffled groups. The input is a gene expression dataframe, which should be normalized for library size. `groups` is a list containing 0 or 1 describing the corresponding group for the samples in `exprs`. The index of `exprs` are the gene ids matching the gene set library. 
 
-```
+```python
 blitz.shuffle.gsea(exprs, library, groups, permutations=50, seed=1)
 ```
 
 | parameter name | type | default	| description |
 |:-----|:---------|:-------------|:------|
 | `exprs`	| pd.DataFrame | NA	| Normalized gene expression matrix. |
 | `library` | dictionary | NA | Gene set library. |
 | `groups` | list | NA | Phenotype group labels of samples. Labels are 0 or 1. |
 | `permutations` | int | 1000 | Number of permutations. |
 | `seed`	| int | 1 | Random state seed. |
 
 # Dependencies
 Python 3.6+
 
-# Citation
+# Attribution
 
-When using blitzgsea please cite the following reference:
+The statistical tool was developed by the [Ma'ayan Laboratory]([https://www.google.com](https://labs.icahn.mssm.edu/maayanlab/)). When using blitzgsea please cite the following reference:
 
 Lachmann, Alexander, Zhuorui Xie, and Avi Ma’ayan. "blitzGSEA: efficient computation of gene set enrichment analysis through gamma distribution approximation." Bioinformatics (2022).
 https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btac076/6526383?login=false
 
 # References
 
 [1] Lachmann, Alexander, Zhuorui Xie, and Avi Ma’ayan. "blitzGSEA: efficient computation of gene set enrichment analysis through gamma distribution approximation." Bioinformatics (2022).
 
 [2] Subramanian, Aravind, Heidi Kuehn, Joshua Gould, Pablo Tamayo, and Jill P. Mesirov. "GSEA-P: a desktop application for Gene Set Enrichment Analysis." Bioinformatics 23, no. 23 (2007): 3251-3253.
 
 [3] Fang, Zhuoqing, Xinyuan Liu, and Gary Peltz. "GSEApy: a comprehensive package for performing gene set enrichment analysis in Python." Bioinformatics (2022).
+
+
```

#### html2text {}

```diff
@@ -1,107 +1,143 @@
-[blitzGSEA] # blitzGSEA Introduction This Python package provides a
-computationally performant Gene Set Enrichment Analysis (GSEA) implementation
-of the pre-rank algorithm [1]. GSEApy was used as the reference for the running
-sum and enrichment score calculation [2]. The algorithm estimates the
-enrichment score (ES) distribution of the null model by fitting data to gamma
-distibutions instead of calculating permutations for each gene set. blitzGSEA
-calculates p-values with much higher accuracy than other reference
-implementations available in Python. Gene set libraries can directly be loaded
-from Enrichr (https://maayanlab.cloud/Enrichr). For this use the
-`blitzgsea.enrichr.get_library()` function. All libraries can also be listed
-with `blitzgsea.enrichr.print_libraries()`. blitzGSEA provides plotting
+Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.4 Summary: Package for fast
+calculation of GSEA similar to prerank using gamma distribution approximation.
+Home-page: https://github.com/maayanlab/blitzgsea Author: Alexander Lachmann
+Author-email: alexander.lachmann@mssm.edu License: UNKNOWN Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
+License-File: LICENSE [blitzGSEA] [Installation](#installation) | [Example]
+(#python-example) | [Optional Parameters](#optional-parameters) | [Speed-up]
+(#speeding-up-enrichment-calculations) | [Plotting](#plotting-enrichment-
+results) | [Attribution](#attribution) | [References](#references) # blitzGSEA
+Introduction This Python package provides a computationally performant Gene Set
+Enrichment Analysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy
+was used as the reference for the running sum and enrichment score calculation
+[2]. The algorithm estimates the enrichment score (ES) distribution of the null
+model by fitting data to gamma distibutions instead of calculating permutations
+for each gene set. blitzGSEA calculates p-values with much higher accuracy than
+other reference implementations available in Python. Gene set libraries can
+directly be loaded from Enrichr (https://maayanlab.cloud/Enrichr). For this use
+the `blitzgsea.enrichr.get_library()` function. All libraries can also be
+listed with `blitzgsea.enrichr.print_libraries()`. blitzGSEA provides plotting
 functions to generate publication ready figures similar to the original GSEA-
 P software. `blitzgsea.plot.running_sum()` plots an enrichment plot for a
 single gene set and `blitzgsea.plot.top_table()` plots the top `n` gene sets in
 a compact table. # Installation blitzGSEA is currently only available as a
 Python package in this GitHub repository. You can install the blitzGSEA Python
 package and its dependencies through pip by using the following command: ``` $
-pip install git+https://github.com/MaayanLab/blitzgsea.git ``` # Run enrichment
-analysis using blitzGSEA blitzGSEA depends on two input files. 1) a gene
-signature and 2) a gene set library. The gene set library is a dictionary with
-the name of the gene set as key and a list of gene ids as values. Gene set
-libraries can be loaded directly from Enrichr. The signature should be a pandas
-dataframe with two columns [0,1]. The first column should contain the gene ids
-(matching the gene ids in the gene set library). | index | 0 | 1 | |:-----|:---
-----------:|------:| | 1 | ADO | -7.833439 | | 2 | CHUK | -7.800920 | | 3 |
-GOLGA4 | -7.78722 | | ... | ... | ... | The gene set library is a dictionary
-with the gene set names as key and lists of gene ids as values. ```python
-{ 'ERBB2 SIGNALING PATHWAY (GO:0038128)': ['CDC37', 'PTPN12', 'PIK3CA', 'SOS1',
-'CPNE3', 'EGF', ... ], 'HETEROTYPIC CELL-CELL ADHESION (GO:0034113)': ['DSC2',
-'ITGAV', 'ITGAD', 'LILRB2', ... ], ... } ``` ### Python example This short
-example will download two files (signature and gene set library). The gene set
-library consists of KEGG pathways and the signature is an example signature of
-differential gene expression of muscle samples from young and old donors.
-Differential gene expression was computed with Limma Voom. ```python import
-blitzgsea as blitz import pandas as pd # read signature as pandas dataframe
-signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/
-testing/ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
-blitz.enrichr.print_libraries() # use enrichr submodule to retrieve gene set
-library library = blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment
-analysis result = blitz.gsea(signature, library) ``` ### Optional Parameters
-The main function of `blitzgsea.gsea()` supports several optional parameters.
-The default parameters should work well for most use cases. | parameter name |
-type | default | description | |:-----|:---------|:-------------|:------| |
-`permutations` | int | 2000 | Number of randomized permutations to estimate ES
-distributions. | | `min_size` | int | 5 | Minimum number of genes in geneset. |
-| `max_size` | int | 4000 | Maximal number of genes in gene set. | | `anchors`
-| int | 20 | Number of gene set size distributions calculated. Remaining are
-interpolated. | | `processes` | int | 4 | Number of parallel threads. Not much
-gain after 4 threads. | | `symmetric` | bool | False | Use same distribution
-parameters for negative and positive ES. If `False` estimate them separately. |
-| `signature_cache` | bool | True | Use precomputed anchor parameters. | |
-`shared_null` | bool | False | Use same null for all signatures (Only computes
-calibration once). | | `plotting`| bool | False | Plot estimated anchor
-parametes. | | `verbose` | bool | False | Toggle additonal output. | |
-`progress` | bool | False | Toggle progress bar. | | `seed` | int | 0 | Random
-seed. Same seed will result in identical result. If seed equal `-1` generate
-random seed. | | `add_noise` | bool | False | Add small random noise to
-signature. The noise is a fraction of the expression values. | ### Plotting
-enrichment results blitzGSEA supports several plotting functions.
-`blitzgsea.plot.running_sum()` and `blitzgsea.plot.top_table()` can be used
-after enrichment has been performed. `blitzgsea.plot.running_sum()` shows the
-running sum of an individual gene set. It has a `compact` mode in which the
-image will be more readable if small. `blitzgsea.plot.top_table()` shows the
-top `n` enriched gene sets and displays the results in a table, with normalized
-enrichment score (NES) and the distribution of hits relative to the gene
-ranking of the signature. ### Example ```python import blitzgsea as blitz
+pip install blitzgsea ``` # Run enrichment analysis using blitzGSEA blitzGSEA
+depends on two input files. 1) a gene signature and 2) a gene set library. The
+gene set library is a dictionary with the name of the gene set as key and a
+list of gene ids as values. Gene set libraries can be loaded directly from
+Enrichr. The signature should be a pandas dataframe with two columns [0,1]. The
+first column should contain the gene ids (matching the gene ids in the gene set
+library). ### Python example This short example will download two files
+(signature and gene set library). The gene set library consists of KEGG
+pathways and the signature is an example signature of differential gene
+expression of muscle samples from young and old donors. Differential gene
+expression was computed with Limma Voom. ```python import blitzgsea as blitz
 import pandas as pd # read signature as pandas dataframe signature =
 pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/
 ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
 blitz.enrichr.print_libraries() # use enrichr submodule to retrieve gene set
 library library = blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment
-analysis result = blitz.gsea(signature, library) # plot the enrichment results
-and save to pdf fig = blitz.plot.running_sum(signature, "CELL ADHESION
-MOLECULES", library, result=result, compact=False) fig.savefig
-("running_sum.png", bbox_inches='tight') fig_compact = blitz.plot.running_sum
-(signature, "CELL ADHESION MOLECULES", library, result=result, compact=True)
-fig_compact.savefig("running_sum_compact.png", bbox_inches='tight') fig_table =
+analysis result = blitz.gsea(signature, library) ``` ### Example Input | index
+| 0 | 1 | |:-----|:-------------:|------:| | 1 | ADO | -7.833439 | | 2 | CHUK |
+-7.800920 | | 3 | GOLGA4 | -7.78722 | | ... | ... | ... | The gene set library
+is a dictionary with the gene set names as key and lists of gene ids as values.
+```python { 'ERBB2 SIGNALING PATHWAY (GO:0038128)': ['CDC37', 'PTPN12',
+'PIK3CA', 'SOS1', 'CPNE3', 'EGF', ... ], 'HETEROTYPIC CELL-CELL ADHESION (GO:
+0034113)': ['DSC2', 'ITGAV', 'ITGAD', 'LILRB2', ... ], ... } ``` ### Optional
+Parameters The main function of `blitzgsea.gsea()` supports several optional
+parameters. The default parameters should work well for most use cases. |
+parameter name | type | default | description | |:-----|:---------|:-----------
+--|:------| | `permutations` | int | 2000 | Number of randomized permutations
+to estimate ES distributions. | | `min_size` | int | 5 | Minimum number of
+genes in geneset. | | `max_size` | int | 4000 | Maximal number of genes in gene
+set. | | `anchors` | int | 20 | Number of gene set size distributions
+calculated. Remaining are interpolated. | | `processes` | int | 4 | Number of
+parallel threads. Not much gain after 4 threads. | | `symmetric` | bool | False
+| Use same distribution parameters for negative and positive ES. If `False`
+estimate them separately. | | `signature_cache` | bool | True | Cache
+precomputed anchor parameters in memory for later reuse. | | `shared_null` |
+bool | False | Use same null for signatures if a compatible model already
+exists. (uses KL-divergence test). | | `kl_threshold`| float | 0.3 | Controls
+how similar signature value distributions have to be for reuse. | | `kl_bins`|
+int | 200 | Number of bins in PDF representation of distributions for KL test.
+| | `plotting`| bool | False | Plot estimated anchor parametes. | | `verbose` |
+bool | False | Toggle additonal output. | | `progress` | bool | False | Toggle
+progress bar. | | `seed` | int | 0 | Random seed. Same seed will result in
+identical result. If seed equal `-1` generate random seed. | | `add_noise` |
+bool | False | Add small random noise to signature. The noise is a fraction of
+the expression values. | ### Speeding up enrichment calculations blitzGSEA is
+currently the fastest GSEA implementation. The most time-consuming step of
+blitzGSEA is the generation of a robust null distribution to compute p-values.
+Since the null distribution depends on the value distribution of the input
+signature, blitzGSEA will, by default, compute a new null for each new input
+signature. blitzGSEA can compute the similarity between input signatures using
+KullbackâLeibler divergence to identify similar signatures to share null
+models. A cached null model is used if a previous signature has a similar value
+distribution. The relevant parameters of the `blitzgsea.gsea()` function are
+shown below: | parameter name | type | default | description | |:-----|:-------
+--|:-------------|:------| | `signature_cache` | bool | True | Cache
+precomputed anchor parameters in memory for later reuse. | | `shared_null` |
+bool | False | Use same null for signatures if a compatible model already
+exists. (uses KL-divergence test). | | `kl_threshold`| float | 0.3 | Controls
+how similar signature value distributions have to be for reuse. The smaller the
+more conservative. | | `kl_bins`| int | 200 | Number of bins in PDF
+representation of distributions for KL test. | ### Example ```python import
+blitzgsea as blitz import pandas as pd # read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/
+testing/ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries() # run enrichment analysis result = blitz.gsea
+(signature, library, shared_null=True) ``` ### Plotting enrichment results
+blitzGSEA supports several plotting functions. `blitzgsea.plot.running_sum()`
+and `blitzgsea.plot.top_table()` can be used after enrichment has been
+performed. `blitzgsea.plot.running_sum()` shows the running sum of an
+individual gene set. It has a `compact` mode in which the image will be more
+readable if small. `blitzgsea.plot.top_table()` shows the top `n` enriched gene
+sets and displays the results in a table, with normalized enrichment score
+(NES) and the distribution of hits relative to the gene ranking of the
+signature. ### Example ```python import blitzgsea as blitz import pandas as pd
+# read signature as pandas dataframe signature = pd.read_csv("https://
+github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv") # list
+available gene set libraries in Enrichr blitz.enrichr.print_libraries() # use
+enrichr submodule to retrieve gene set library library =
+blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment analysis result =
+blitz.gsea(signature, library) # plot the enrichment results and save to pdf
+fig = blitz.plot.running_sum(signature, "CELL ADHESION MOLECULES", library,
+result=result, compact=False) fig.savefig("running_sum.png",
+bbox_inches='tight') fig_compact = blitz.plot.running_sum(signature, "CELL
+ADHESION MOLECULES", library, result=result, compact=True) fig_compact.savefig
+("running_sum_compact.png", bbox_inches='tight') fig_table =
 blitz.plot.top_table(signature, library, result, n=15) fig_table.savefig
 ("top_table.png", bbox_inches='tight') ``` The resulting plots will look like
 the examples below: #### running_sum.pdf
 [blitzGSEA sunning_sum]
 #### running_sum_compact.pdf [blitzGSEA sunning_sum] #### top_table.pdf
 [blitzGSEA sunning_sum] ### Sample shuffling This is the sample shuffling
 algorithm from GSEApy. It performs a t-test to build signatures for phenotype
 shuffled groups. The input is a gene expression dataframe, which should be
 normalized for library size. `groups` is a list containing 0 or 1 describing
 the corresponding group for the samples in `exprs`. The index of `exprs` are
-the gene ids matching the gene set library. ``` blitz.shuffle.gsea(exprs,
+the gene ids matching the gene set library. ```python blitz.shuffle.gsea(exprs,
 library, groups, permutations=50, seed=1) ``` | parameter name | type | default
 | description | |:-----|:---------|:-------------|:------| | `exprs` |
 pd.DataFrame | NA | Normalized gene expression matrix. | | `library` |
 dictionary | NA | Gene set library. | | `groups` | list | NA | Phenotype group
 labels of samples. Labels are 0 or 1. | | `permutations` | int | 1000 | Number
 of permutations. | | `seed` | int | 1 | Random state seed. | # Dependencies
-Python 3.6+ # Citation When using blitzgsea please cite the following
-reference: Lachmann, Alexander, Zhuorui Xie, and Avi Maâayan. "blitzGSEA:
-efficient computation of gene set enrichment analysis through gamma
-distribution approximation." Bioinformatics (2022). https://academic.oup.com/
-bioinformatics/advance-article/doi/10.1093/bioinformatics/btac076/
-6526383?login=false # References [1] Lachmann, Alexander, Zhuorui Xie, and Avi
-Maâayan. "blitzGSEA: efficient computation of gene set enrichment analysis
-through gamma distribution approximation." Bioinformatics (2022). [2]
-Subramanian, Aravind, Heidi Kuehn, Joshua Gould, Pablo Tamayo, and Jill P.
-Mesirov. "GSEA-P: a desktop application for Gene Set Enrichment Analysis."
-Bioinformatics 23, no. 23 (2007): 3251-3253. [3] Fang, Zhuoqing, Xinyuan Liu,
-and Gary Peltz. "GSEApy: a comprehensive package for performing gene set
-enrichment analysis in Python." Bioinformatics (2022).
+Python 3.6+ # Attribution The statistical tool was developed by the [Ma'ayan
+Laboratory]([https://www.google.com](https://labs.icahn.mssm.edu/maayanlab/)).
+When using blitzgsea please cite the following reference: Lachmann, Alexander,
+Zhuorui Xie, and Avi Maâayan. "blitzGSEA: efficient computation of gene set
+enrichment analysis through gamma distribution approximation." Bioinformatics
+(2022). https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/
+bioinformatics/btac076/6526383?login=false # References [1] Lachmann,
+Alexander, Zhuorui Xie, and Avi Maâayan. "blitzGSEA: efficient computation of
+gene set enrichment analysis through gamma distribution approximation."
+Bioinformatics (2022). [2] Subramanian, Aravind, Heidi Kuehn, Joshua Gould,
+Pablo Tamayo, and Jill P. Mesirov. "GSEA-P: a desktop application for Gene Set
+Enrichment Analysis." Bioinformatics 23, no. 23 (2007): 3251-3253. [3] Fang,
+Zhuoqing, Xinyuan Liu, and Gary Peltz. "GSEApy: a comprehensive package for
+performing gene set enrichment analysis in Python." Bioinformatics (2022).
```

### Comparing `blitzgsea-1.3.3/blitzgsea/__init__.py` & `blitzgsea-1.3.4/blitzgsea/__init__.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.3/blitzgsea/enrichr.py` & `blitzgsea-1.3.4/blitzgsea/enrichr.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.3/blitzgsea/plot.py` & `blitzgsea-1.3.4/blitzgsea/plot.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.3/blitzgsea/shuffle.py` & `blitzgsea-1.3.4/blitzgsea/shuffle.py`

 * *Files identical despite different names*

### Comparing `blitzgsea-1.3.3/blitzgsea.egg-info/PKG-INFO` & `blitzgsea-1.3.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,54 @@
-Metadata-Version: 2.1
-Name: blitzgsea
-Version: 1.3.3
-Summary: Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.
-Home-page: https://github.com/maayanlab/blitzgsea
-Author: Alexander Lachmann
-Author-email: alexander.lachmann@mssm.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img title="a title" alt="blitzGSEA" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/bgsea_small.png" width=200>
 
+[Installation](#installation) | [Example](#python-example) | [Optional Parameters](#optional-parameters) | [Speed-up](#speeding-up-enrichment-calculations) | [Plotting](#plotting-enrichment-results) | [Attribution](#attribution) | [References](#references)
+
 # blitzGSEA Introduction
 
 This Python package provides a computationally performant <b>G</b>ene <b>S</b>et <b>E</b>nrichment <b>A</b>nalysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy was used as the reference for the running sum and enrichment score calculation [2]. The algorithm estimates the enrichment score (ES) distribution of the null model by fitting data to gamma distibutions instead of calculating permutations for each gene set. blitzGSEA calculates p-values with much higher accuracy than other reference implementations available in Python.
 
 Gene set libraries can directly be loaded from Enrichr (<a href="https://maayanlab.cloud/Enrichr" target="_blank">https://maayanlab.cloud/Enrichr</a>). For this use the `blitzgsea.enrichr.get_library()` function. All libraries can also be listed with `blitzgsea.enrichr.print_libraries()`.
 
 blitzGSEA provides plotting functions to generate publication ready figures similar to the original GSEA-P software. `blitzgsea.plot.running_sum()` plots an enrichment plot for a single gene set and `blitzgsea.plot.top_table()` plots the top `n` gene sets in a compact table. 
 
 # Installation
 
 blitzGSEA is currently only available as a Python package in this GitHub repository. You can install the blitzGSEA Python package and its dependencies through pip by using the following command:
 
 ```
-$ pip install git+https://github.com/MaayanLab/blitzgsea.git
+$ pip install blitzgsea
 ```
 
 # Run enrichment analysis using blitzGSEA
 
 blitzGSEA depends on two input files. 1) a gene signature and 2) a gene set library. The gene set library is a dictionary with the name of the gene set as key and a list of gene ids as values. Gene set libraries can be loaded directly from Enrichr. The signature should be a pandas dataframe with two columns [0,1]. The first column should contain the gene ids (matching the gene ids in the gene set library).
 
+### Python example
+
+This short example will download two files (signature and gene set library). The gene set library consists of KEGG pathways and the signature is an example signature of differential gene expression of muscle samples from young and old donors. Differential gene expression was computed with Limma Voom.
+
+```python
+import blitzgsea as blitz
+import pandas as pd
+
+# read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
+
+# list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries()
+
+# use enrichr submodule to retrieve gene set library
+library = blitz.enrichr.get_library("KEGG_2021_Human")
+
+# run enrichment analysis
+result = blitz.gsea(signature, library)
+```
+
+### Example Input
+
 | index | 0	| 1 |
 |:-----|:-------------:|------:|
 | 1	| ADO	| -7.833439 |
 | 2	| CHUK	| -7.800920 |
 | 3	| GOLGA4	| -7.78722 |
 | ... | ... | ... |
 
@@ -61,55 +70,63 @@
                                                  'LILRB2',
                                                  ...
                                                 ],
 ...
 }
 ```
 
-### Python example
-
-This short example will download two files (signature and gene set library). The gene set library consists of KEGG pathways and the signature is an example signature of differential gene expression of muscle samples from young and old donors. Differential gene expression was computed with Limma Voom.
-
-```python
-import blitzgsea as blitz
-import pandas as pd
-
-# read signature as pandas dataframe
-signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
-
-# list available gene set libraries in Enrichr
-blitz.enrichr.print_libraries()
-
-# use enrichr submodule to retrieve gene set library
-library = blitz.enrichr.get_library("KEGG_2021_Human")
-
-# run enrichment analysis
-result = blitz.gsea(signature, library)
-```
-
 ### Optional Parameters
 
 The main function of `blitzgsea.gsea()` supports several optional parameters. The default parameters should work well for most use cases. 
 
 | parameter name | type | default	| description |
 |:-----|:---------|:-------------|:------|
 | `permutations`	| int | 2000	| Number of randomized permutations to estimate ES distributions. |
 | `min_size` | int | 5 | Minimum number of genes in geneset. |
 | `max_size` | int | 4000 | Maximal number of genes in gene set. |
 | `anchors`	| int | 20 | Number of gene set size distributions calculated. Remaining are interpolated. |
 | `processes`	| int | 4	| Number of parallel threads. Not much gain after 4 threads. |
 | `symmetric` | bool | False | Use same distribution parameters for negative and positive ES. If `False` estimate them separately. |
-| `signature_cache` | bool | True | Use precomputed anchor parameters. |
-| `shared_null` | bool | False | Use same null for all signatures (Only computes calibration once). |
+| `signature_cache` | bool | True | Cache precomputed anchor parameters in memory for later reuse. |
+| `shared_null` | bool | False | Use same null for signatures if a compatible model already exists. (uses KL-divergence test). |
+| `kl_threshold`| float | 0.3 | Controls how similar signature value distributions have to be for reuse. |
+| `kl_bins`| int | 200 | Number of bins in PDF representation of distributions for KL test. |
 | `plotting`| bool | False | Plot estimated anchor parametes. |
 | `verbose` | bool | False | Toggle additonal output. |
 | `progress` | bool | False | Toggle progress bar. |
 | `seed` | int | 0 | Random seed. Same seed will result in identical result. If seed equal `-1` generate random seed. |
 | `add_noise` | bool | False | Add small random noise to signature. The noise is a fraction of the expression values. |
 
+### Speeding up enrichment calculations
+
+blitzGSEA is currently the fastest GSEA implementation. The most time-consuming step of blitzGSEA is the generation of a robust null distribution to compute p-values. Since the null distribution depends on the value distribution of the input signature, blitzGSEA will, by default, compute a new null for each new input signature. blitzGSEA can compute the similarity between input signatures using Kullback–Leibler divergence to identify similar signatures to share null models. A cached null model is used if a previous signature has a similar value distribution. The relevant parameters of the `blitzgsea.gsea()` function are shown below:
+
+| parameter name | type | default	| description |
+|:-----|:---------|:-------------|:------|
+| `signature_cache` | bool | True | Cache precomputed anchor parameters in memory for later reuse. |
+| `shared_null` | bool | False | Use same null for signatures if a compatible model already exists. (uses KL-divergence test). |
+| `kl_threshold`| float | 0.3 | Controls how similar signature value distributions have to be for reuse. The smaller the more conservative. |
+| `kl_bins`| int | 200 | Number of bins in PDF representation of distributions for KL test. |
+
+### Example
+```python
+
+import blitzgsea as blitz
+import pandas as pd
+
+# read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv")
+
+# list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries()
+
+# run enrichment analysis
+result = blitz.gsea(signature, library, shared_null=True)
+```
+
 ### Plotting enrichment results
 
 blitzGSEA supports several plotting functions. `blitzgsea.plot.running_sum()` and `blitzgsea.plot.top_table()` can be used after enrichment has been performed. `blitzgsea.plot.running_sum()` shows the running sum of an individual gene set. It has a `compact` mode in which the image will be more readable if small. `blitzgsea.plot.top_table()` shows the top `n` enriched gene sets and displays the results in a table, with normalized enrichment score (NES) and the distribution of hits relative to the gene ranking of the signature.
 
 ### Example
 ```python
 
@@ -153,38 +170,36 @@
 
 #### top_table.pdf
 <img title="a title" alt="blitzGSEA sunning_sum" src="https://github.com/MaayanLab/blitzgsea/blob/main/icon/top_table.png" width=300>
 
 ### Sample shuffling
 This is the sample shuffling algorithm from GSEApy. It performs a t-test to build signatures for phenotype shuffled groups. The input is a gene expression dataframe, which should be normalized for library size. `groups` is a list containing 0 or 1 describing the corresponding group for the samples in `exprs`. The index of `exprs` are the gene ids matching the gene set library. 
 
-```
+```python
 blitz.shuffle.gsea(exprs, library, groups, permutations=50, seed=1)
 ```
 
 | parameter name | type | default	| description |
 |:-----|:---------|:-------------|:------|
 | `exprs`	| pd.DataFrame | NA	| Normalized gene expression matrix. |
 | `library` | dictionary | NA | Gene set library. |
 | `groups` | list | NA | Phenotype group labels of samples. Labels are 0 or 1. |
 | `permutations` | int | 1000 | Number of permutations. |
 | `seed`	| int | 1 | Random state seed. |
 
 # Dependencies
 Python 3.6+
 
-# Citation
+# Attribution
 
-When using blitzgsea please cite the following reference:
+The statistical tool was developed by the [Ma'ayan Laboratory]([https://www.google.com](https://labs.icahn.mssm.edu/maayanlab/)). When using blitzgsea please cite the following reference:
 
 Lachmann, Alexander, Zhuorui Xie, and Avi Ma’ayan. "blitzGSEA: efficient computation of gene set enrichment analysis through gamma distribution approximation." Bioinformatics (2022).
 https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btac076/6526383?login=false
 
 # References
 
 [1] Lachmann, Alexander, Zhuorui Xie, and Avi Ma’ayan. "blitzGSEA: efficient computation of gene set enrichment analysis through gamma distribution approximation." Bioinformatics (2022).
 
 [2] Subramanian, Aravind, Heidi Kuehn, Joshua Gould, Pablo Tamayo, and Jill P. Mesirov. "GSEA-P: a desktop application for Gene Set Enrichment Analysis." Bioinformatics 23, no. 23 (2007): 3251-3253.
 
 [3] Fang, Zhuoqing, Xinyuan Liu, and Gary Peltz. "GSEApy: a comprehensive package for performing gene set enrichment analysis in Python." Bioinformatics (2022).
-
-
```

#### html2text {}

```diff
@@ -1,114 +1,136 @@
-Metadata-Version: 2.1 Name: blitzgsea Version: 1.3.3 Summary: Package for fast
-calculation of GSEA similar to prerank using gamma distribution approximation.
-Home-page: https://github.com/maayanlab/blitzgsea Author: Alexander Lachmann
-Author-email: alexander.lachmann@mssm.edu License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE [blitzGSEA] # blitzGSEA Introduction This Python package
-provides a computationally performant Gene Set Enrichment Analysis (GSEA)
-implementation of the pre-rank algorithm [1]. GSEApy was used as the reference
-for the running sum and enrichment score calculation [2]. The algorithm
-estimates the enrichment score (ES) distribution of the null model by fitting
-data to gamma distibutions instead of calculating permutations for each gene
-set. blitzGSEA calculates p-values with much higher accuracy than other
-reference implementations available in Python. Gene set libraries can directly
-be loaded from Enrichr (https://maayanlab.cloud/Enrichr). For this use the
-`blitzgsea.enrichr.get_library()` function. All libraries can also be listed
-with `blitzgsea.enrichr.print_libraries()`. blitzGSEA provides plotting
+[blitzGSEA] [Installation](#installation) | [Example](#python-example) |
+[Optional Parameters](#optional-parameters) | [Speed-up](#speeding-up-
+enrichment-calculations) | [Plotting](#plotting-enrichment-results) |
+[Attribution](#attribution) | [References](#references) # blitzGSEA
+Introduction This Python package provides a computationally performant Gene Set
+Enrichment Analysis (GSEA) implementation of the pre-rank algorithm [1]. GSEApy
+was used as the reference for the running sum and enrichment score calculation
+[2]. The algorithm estimates the enrichment score (ES) distribution of the null
+model by fitting data to gamma distibutions instead of calculating permutations
+for each gene set. blitzGSEA calculates p-values with much higher accuracy than
+other reference implementations available in Python. Gene set libraries can
+directly be loaded from Enrichr (https://maayanlab.cloud/Enrichr). For this use
+the `blitzgsea.enrichr.get_library()` function. All libraries can also be
+listed with `blitzgsea.enrichr.print_libraries()`. blitzGSEA provides plotting
 functions to generate publication ready figures similar to the original GSEA-
 P software. `blitzgsea.plot.running_sum()` plots an enrichment plot for a
 single gene set and `blitzgsea.plot.top_table()` plots the top `n` gene sets in
 a compact table. # Installation blitzGSEA is currently only available as a
 Python package in this GitHub repository. You can install the blitzGSEA Python
 package and its dependencies through pip by using the following command: ``` $
-pip install git+https://github.com/MaayanLab/blitzgsea.git ``` # Run enrichment
-analysis using blitzGSEA blitzGSEA depends on two input files. 1) a gene
-signature and 2) a gene set library. The gene set library is a dictionary with
-the name of the gene set as key and a list of gene ids as values. Gene set
-libraries can be loaded directly from Enrichr. The signature should be a pandas
-dataframe with two columns [0,1]. The first column should contain the gene ids
-(matching the gene ids in the gene set library). | index | 0 | 1 | |:-----|:---
-----------:|------:| | 1 | ADO | -7.833439 | | 2 | CHUK | -7.800920 | | 3 |
-GOLGA4 | -7.78722 | | ... | ... | ... | The gene set library is a dictionary
-with the gene set names as key and lists of gene ids as values. ```python
-{ 'ERBB2 SIGNALING PATHWAY (GO:0038128)': ['CDC37', 'PTPN12', 'PIK3CA', 'SOS1',
-'CPNE3', 'EGF', ... ], 'HETEROTYPIC CELL-CELL ADHESION (GO:0034113)': ['DSC2',
-'ITGAV', 'ITGAD', 'LILRB2', ... ], ... } ``` ### Python example This short
-example will download two files (signature and gene set library). The gene set
-library consists of KEGG pathways and the signature is an example signature of
-differential gene expression of muscle samples from young and old donors.
-Differential gene expression was computed with Limma Voom. ```python import
-blitzgsea as blitz import pandas as pd # read signature as pandas dataframe
-signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/
-testing/ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
-blitz.enrichr.print_libraries() # use enrichr submodule to retrieve gene set
-library library = blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment
-analysis result = blitz.gsea(signature, library) ``` ### Optional Parameters
-The main function of `blitzgsea.gsea()` supports several optional parameters.
-The default parameters should work well for most use cases. | parameter name |
-type | default | description | |:-----|:---------|:-------------|:------| |
-`permutations` | int | 2000 | Number of randomized permutations to estimate ES
-distributions. | | `min_size` | int | 5 | Minimum number of genes in geneset. |
-| `max_size` | int | 4000 | Maximal number of genes in gene set. | | `anchors`
-| int | 20 | Number of gene set size distributions calculated. Remaining are
-interpolated. | | `processes` | int | 4 | Number of parallel threads. Not much
-gain after 4 threads. | | `symmetric` | bool | False | Use same distribution
-parameters for negative and positive ES. If `False` estimate them separately. |
-| `signature_cache` | bool | True | Use precomputed anchor parameters. | |
-`shared_null` | bool | False | Use same null for all signatures (Only computes
-calibration once). | | `plotting`| bool | False | Plot estimated anchor
-parametes. | | `verbose` | bool | False | Toggle additonal output. | |
-`progress` | bool | False | Toggle progress bar. | | `seed` | int | 0 | Random
-seed. Same seed will result in identical result. If seed equal `-1` generate
-random seed. | | `add_noise` | bool | False | Add small random noise to
-signature. The noise is a fraction of the expression values. | ### Plotting
-enrichment results blitzGSEA supports several plotting functions.
-`blitzgsea.plot.running_sum()` and `blitzgsea.plot.top_table()` can be used
-after enrichment has been performed. `blitzgsea.plot.running_sum()` shows the
-running sum of an individual gene set. It has a `compact` mode in which the
-image will be more readable if small. `blitzgsea.plot.top_table()` shows the
-top `n` enriched gene sets and displays the results in a table, with normalized
-enrichment score (NES) and the distribution of hits relative to the gene
-ranking of the signature. ### Example ```python import blitzgsea as blitz
+pip install blitzgsea ``` # Run enrichment analysis using blitzGSEA blitzGSEA
+depends on two input files. 1) a gene signature and 2) a gene set library. The
+gene set library is a dictionary with the name of the gene set as key and a
+list of gene ids as values. Gene set libraries can be loaded directly from
+Enrichr. The signature should be a pandas dataframe with two columns [0,1]. The
+first column should contain the gene ids (matching the gene ids in the gene set
+library). ### Python example This short example will download two files
+(signature and gene set library). The gene set library consists of KEGG
+pathways and the signature is an example signature of differential gene
+expression of muscle samples from young and old donors. Differential gene
+expression was computed with Limma Voom. ```python import blitzgsea as blitz
 import pandas as pd # read signature as pandas dataframe signature =
 pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/testing/
 ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
 blitz.enrichr.print_libraries() # use enrichr submodule to retrieve gene set
 library library = blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment
-analysis result = blitz.gsea(signature, library) # plot the enrichment results
-and save to pdf fig = blitz.plot.running_sum(signature, "CELL ADHESION
-MOLECULES", library, result=result, compact=False) fig.savefig
-("running_sum.png", bbox_inches='tight') fig_compact = blitz.plot.running_sum
-(signature, "CELL ADHESION MOLECULES", library, result=result, compact=True)
-fig_compact.savefig("running_sum_compact.png", bbox_inches='tight') fig_table =
+analysis result = blitz.gsea(signature, library) ``` ### Example Input | index
+| 0 | 1 | |:-----|:-------------:|------:| | 1 | ADO | -7.833439 | | 2 | CHUK |
+-7.800920 | | 3 | GOLGA4 | -7.78722 | | ... | ... | ... | The gene set library
+is a dictionary with the gene set names as key and lists of gene ids as values.
+```python { 'ERBB2 SIGNALING PATHWAY (GO:0038128)': ['CDC37', 'PTPN12',
+'PIK3CA', 'SOS1', 'CPNE3', 'EGF', ... ], 'HETEROTYPIC CELL-CELL ADHESION (GO:
+0034113)': ['DSC2', 'ITGAV', 'ITGAD', 'LILRB2', ... ], ... } ``` ### Optional
+Parameters The main function of `blitzgsea.gsea()` supports several optional
+parameters. The default parameters should work well for most use cases. |
+parameter name | type | default | description | |:-----|:---------|:-----------
+--|:------| | `permutations` | int | 2000 | Number of randomized permutations
+to estimate ES distributions. | | `min_size` | int | 5 | Minimum number of
+genes in geneset. | | `max_size` | int | 4000 | Maximal number of genes in gene
+set. | | `anchors` | int | 20 | Number of gene set size distributions
+calculated. Remaining are interpolated. | | `processes` | int | 4 | Number of
+parallel threads. Not much gain after 4 threads. | | `symmetric` | bool | False
+| Use same distribution parameters for negative and positive ES. If `False`
+estimate them separately. | | `signature_cache` | bool | True | Cache
+precomputed anchor parameters in memory for later reuse. | | `shared_null` |
+bool | False | Use same null for signatures if a compatible model already
+exists. (uses KL-divergence test). | | `kl_threshold`| float | 0.3 | Controls
+how similar signature value distributions have to be for reuse. | | `kl_bins`|
+int | 200 | Number of bins in PDF representation of distributions for KL test.
+| | `plotting`| bool | False | Plot estimated anchor parametes. | | `verbose` |
+bool | False | Toggle additonal output. | | `progress` | bool | False | Toggle
+progress bar. | | `seed` | int | 0 | Random seed. Same seed will result in
+identical result. If seed equal `-1` generate random seed. | | `add_noise` |
+bool | False | Add small random noise to signature. The noise is a fraction of
+the expression values. | ### Speeding up enrichment calculations blitzGSEA is
+currently the fastest GSEA implementation. The most time-consuming step of
+blitzGSEA is the generation of a robust null distribution to compute p-values.
+Since the null distribution depends on the value distribution of the input
+signature, blitzGSEA will, by default, compute a new null for each new input
+signature. blitzGSEA can compute the similarity between input signatures using
+KullbackâLeibler divergence to identify similar signatures to share null
+models. A cached null model is used if a previous signature has a similar value
+distribution. The relevant parameters of the `blitzgsea.gsea()` function are
+shown below: | parameter name | type | default | description | |:-----|:-------
+--|:-------------|:------| | `signature_cache` | bool | True | Cache
+precomputed anchor parameters in memory for later reuse. | | `shared_null` |
+bool | False | Use same null for signatures if a compatible model already
+exists. (uses KL-divergence test). | | `kl_threshold`| float | 0.3 | Controls
+how similar signature value distributions have to be for reuse. The smaller the
+more conservative. | | `kl_bins`| int | 200 | Number of bins in PDF
+representation of distributions for KL test. | ### Example ```python import
+blitzgsea as blitz import pandas as pd # read signature as pandas dataframe
+signature = pd.read_csv("https://github.com/MaayanLab/blitzgsea/raw/main/
+testing/ageing_muscle_gtex.tsv") # list available gene set libraries in Enrichr
+blitz.enrichr.print_libraries() # run enrichment analysis result = blitz.gsea
+(signature, library, shared_null=True) ``` ### Plotting enrichment results
+blitzGSEA supports several plotting functions. `blitzgsea.plot.running_sum()`
+and `blitzgsea.plot.top_table()` can be used after enrichment has been
+performed. `blitzgsea.plot.running_sum()` shows the running sum of an
+individual gene set. It has a `compact` mode in which the image will be more
+readable if small. `blitzgsea.plot.top_table()` shows the top `n` enriched gene
+sets and displays the results in a table, with normalized enrichment score
+(NES) and the distribution of hits relative to the gene ranking of the
+signature. ### Example ```python import blitzgsea as blitz import pandas as pd
+# read signature as pandas dataframe signature = pd.read_csv("https://
+github.com/MaayanLab/blitzgsea/raw/main/testing/ageing_muscle_gtex.tsv") # list
+available gene set libraries in Enrichr blitz.enrichr.print_libraries() # use
+enrichr submodule to retrieve gene set library library =
+blitz.enrichr.get_library("KEGG_2021_Human") # run enrichment analysis result =
+blitz.gsea(signature, library) # plot the enrichment results and save to pdf
+fig = blitz.plot.running_sum(signature, "CELL ADHESION MOLECULES", library,
+result=result, compact=False) fig.savefig("running_sum.png",
+bbox_inches='tight') fig_compact = blitz.plot.running_sum(signature, "CELL
+ADHESION MOLECULES", library, result=result, compact=True) fig_compact.savefig
+("running_sum_compact.png", bbox_inches='tight') fig_table =
 blitz.plot.top_table(signature, library, result, n=15) fig_table.savefig
 ("top_table.png", bbox_inches='tight') ``` The resulting plots will look like
 the examples below: #### running_sum.pdf
 [blitzGSEA sunning_sum]
 #### running_sum_compact.pdf [blitzGSEA sunning_sum] #### top_table.pdf
 [blitzGSEA sunning_sum] ### Sample shuffling This is the sample shuffling
 algorithm from GSEApy. It performs a t-test to build signatures for phenotype
 shuffled groups. The input is a gene expression dataframe, which should be
 normalized for library size. `groups` is a list containing 0 or 1 describing
 the corresponding group for the samples in `exprs`. The index of `exprs` are
-the gene ids matching the gene set library. ``` blitz.shuffle.gsea(exprs,
+the gene ids matching the gene set library. ```python blitz.shuffle.gsea(exprs,
 library, groups, permutations=50, seed=1) ``` | parameter name | type | default
 | description | |:-----|:---------|:-------------|:------| | `exprs` |
 pd.DataFrame | NA | Normalized gene expression matrix. | | `library` |
 dictionary | NA | Gene set library. | | `groups` | list | NA | Phenotype group
 labels of samples. Labels are 0 or 1. | | `permutations` | int | 1000 | Number
 of permutations. | | `seed` | int | 1 | Random state seed. | # Dependencies
-Python 3.6+ # Citation When using blitzgsea please cite the following
-reference: Lachmann, Alexander, Zhuorui Xie, and Avi Maâayan. "blitzGSEA:
-efficient computation of gene set enrichment analysis through gamma
-distribution approximation." Bioinformatics (2022). https://academic.oup.com/
-bioinformatics/advance-article/doi/10.1093/bioinformatics/btac076/
-6526383?login=false # References [1] Lachmann, Alexander, Zhuorui Xie, and Avi
-Maâayan. "blitzGSEA: efficient computation of gene set enrichment analysis
-through gamma distribution approximation." Bioinformatics (2022). [2]
-Subramanian, Aravind, Heidi Kuehn, Joshua Gould, Pablo Tamayo, and Jill P.
-Mesirov. "GSEA-P: a desktop application for Gene Set Enrichment Analysis."
-Bioinformatics 23, no. 23 (2007): 3251-3253. [3] Fang, Zhuoqing, Xinyuan Liu,
-and Gary Peltz. "GSEApy: a comprehensive package for performing gene set
-enrichment analysis in Python." Bioinformatics (2022).
+Python 3.6+ # Attribution The statistical tool was developed by the [Ma'ayan
+Laboratory]([https://www.google.com](https://labs.icahn.mssm.edu/maayanlab/)).
+When using blitzgsea please cite the following reference: Lachmann, Alexander,
+Zhuorui Xie, and Avi Maâayan. "blitzGSEA: efficient computation of gene set
+enrichment analysis through gamma distribution approximation." Bioinformatics
+(2022). https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/
+bioinformatics/btac076/6526383?login=false # References [1] Lachmann,
+Alexander, Zhuorui Xie, and Avi Maâayan. "blitzGSEA: efficient computation of
+gene set enrichment analysis through gamma distribution approximation."
+Bioinformatics (2022). [2] Subramanian, Aravind, Heidi Kuehn, Joshua Gould,
+Pablo Tamayo, and Jill P. Mesirov. "GSEA-P: a desktop application for Gene Set
+Enrichment Analysis." Bioinformatics 23, no. 23 (2007): 3251-3253. [3] Fang,
+Zhuoqing, Xinyuan Liu, and Gary Peltz. "GSEApy: a comprehensive package for
+performing gene set enrichment analysis in Python." Bioinformatics (2022).
```

### Comparing `blitzgsea-1.3.3/setup.py` & `blitzgsea-1.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="blitzgsea",
-    version="1.3.3",
+    version="1.3.4",
     author="Alexander Lachmann",
     author_email="alexander.lachmann@mssm.edu",
     description="Package for fast calculation of GSEA similar to prerank using gamma distribution approximation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maayanlab/blitzgsea",
     packages=setuptools.find_packages(),
```

