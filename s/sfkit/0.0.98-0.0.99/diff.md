# Comparing `tmp/sfkit-0.0.98-py3-none-any.whl.zip` & `tmp/sfkit-0.0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 617902 bytes, number of entries: 36
+Zip file size: 617905 bytes, number of entries: 36
 -rw-r--r--  2.0 unx     6148 b- defN 20-Feb-02 00:00 sfkit/.DS_Store
 -rw-r--r--  2.0 unx      939 b- defN 20-Feb-02 00:00 sfkit/api.py
 -rw-r--r--  2.0 unx     1055 b- defN 20-Feb-02 00:00 sfkit/cli.py
 -rw-r--r--  2.0 unx     1832 b- defN 20-Feb-02 00:00 sfkit/parser.py
 -rw-r--r--  2.0 unx     1088 b- defN 20-Feb-02 00:00 sfkit/auth/auth.py
 -rw-r--r--  2.0 unx     1840 b- defN 20-Feb-02 00:00 sfkit/auth/setup_networking.py
 -rw-r--r--  2.0 unx     6148 b- defN 20-Feb-02 00:00 sfkit/encryption/.DS_Store
@@ -22,17 +22,17 @@
 -rw-r--r--  2.0 unx    10000 b- defN 20-Feb-02 00:00 sfkit/encryption/mpc/test_data/input_data2/cov.txt
 -rw-r--r--  2.0 unx  1000000 b- defN 20-Feb-02 00:00 sfkit/encryption/mpc/test_data/input_data2/geno.txt
 -rw-r--r--  2.0 unx     1000 b- defN 20-Feb-02 00:00 sfkit/encryption/mpc/test_data/input_data2/pheno.txt
 -rw-r--r--  2.0 unx    12000 b- defN 20-Feb-02 00:00 sfkit/encryption/mpc/test_data/input_data2/pos.txt
 -rw-r--r--  2.0 unx     4702 b- defN 20-Feb-02 00:00 sfkit/protocol/register_data.py
 -rw-r--r--  2.0 unx     2080 b- defN 20-Feb-02 00:00 sfkit/protocol/run_protocol.py
 -rw-r--r--  2.0 unx      407 b- defN 20-Feb-02 00:00 sfkit/protocol/utils/constants.py
--rw-r--r--  2.0 unx     8633 b- defN 20-Feb-02 00:00 sfkit/protocol/utils/gwas_protocol.py
+-rw-r--r--  2.0 unx     8666 b- defN 20-Feb-02 00:00 sfkit/protocol/utils/gwas_protocol.py
 -rw-r--r--  2.0 unx      452 b- defN 20-Feb-02 00:00 sfkit/protocol/utils/helper_functions.py
 -rw-r--r--  2.0 unx     1508 b- defN 20-Feb-02 00:00 sfkit/protocol/utils/pca_protocol.py
 -rw-r--r--  2.0 unx    10318 b- defN 20-Feb-02 00:00 sfkit/protocol/utils/sfgwas_protocol.py
-?rw-r--r--  2.0 unx     2077 b- defN 20-Feb-02 00:00 sfkit-0.0.98.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sfkit-0.0.98.dist-info/WHEEL
-?rw-r--r--  2.0 unx       41 b- defN 20-Feb-02 00:00 sfkit-0.0.98.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 sfkit-0.0.98.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     3362 b- defN 20-Feb-02 00:00 sfkit-0.0.98.dist-info/RECORD
-36 files, 4150615 bytes uncompressed, 612428 bytes compressed:  85.3%
+?rw-r--r--  2.0 unx     2077 b- defN 20-Feb-02 00:00 sfkit-0.0.99.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sfkit-0.0.99.dist-info/WHEEL
+?rw-r--r--  2.0 unx       41 b- defN 20-Feb-02 00:00 sfkit-0.0.99.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 sfkit-0.0.99.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     3362 b- defN 20-Feb-02 00:00 sfkit-0.0.99.dist-info/RECORD
+36 files, 4150648 bytes uncompressed, 612431 bytes compressed:  85.3%
```

## zipnote {}

```diff
@@ -87,23 +87,23 @@
 
 Filename: sfkit/protocol/utils/pca_protocol.py
 Comment: 
 
 Filename: sfkit/protocol/utils/sfgwas_protocol.py
 Comment: 
 
-Filename: sfkit-0.0.98.dist-info/METADATA
+Filename: sfkit-0.0.99.dist-info/METADATA
 Comment: 
 
-Filename: sfkit-0.0.98.dist-info/WHEEL
+Filename: sfkit-0.0.99.dist-info/WHEEL
 Comment: 
 
-Filename: sfkit-0.0.98.dist-info/entry_points.txt
+Filename: sfkit-0.0.99.dist-info/entry_points.txt
 Comment: 
 
-Filename: sfkit-0.0.98.dist-info/licenses/LICENSE
+Filename: sfkit-0.0.99.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: sfkit-0.0.98.dist-info/RECORD
+Filename: sfkit-0.0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sfkit/protocol/utils/gwas_protocol.py

```diff
@@ -88,26 +88,26 @@
     pars["NUM_INDS_SP_1"] = doc_ref_dict["personal_parameters"][doc_ref_dict["participants"][1]]["NUM_INDS"]
     pars["NUM_INDS_SP_2"] = doc_ref_dict["personal_parameters"][doc_ref_dict["participants"][2]]["NUM_INDS"]
     pars["NUM_INDS"] = {"value": ""}
     pars["NUM_INDS"]["value"] = str(int(pars["NUM_INDS_SP_1"]["value"]) + int(pars["NUM_INDS_SP_2"]["value"]))
 
     # num threads = num_cpus = $(nproc)
     num_cpus = str(multiprocessing.cpu_count())
-    pars["NUM_THREADS"] = num_cpus
+    pars["NUM_THREADS"] = {"value": num_cpus}
     update_firestore(f"update_firestore::NUM_THREADS={num_cpus}")
     update_firestore(f"update_firestore::NUM_CPUS={num_cpus}")
 
     # update pars with ipaddresses and ports
     for i in range(3):
         ip = doc_ref_dict["personal_parameters"][doc_ref_dict["participants"][i]]["IP_ADDRESS"]["value"]
-        pars[f"IP_ADDR_P{i}"] = ip
+        pars[f"IP_ADDR_P{i}"] = {"value": ip}
 
         ports = doc_ref_dict["personal_parameters"][doc_ref_dict["participants"][i]]["PORTS"]["value"]
         for j in range(i + 1, 3):
-            pars[f"PORT_P{i}_P{j}"] = ports.split(",")[j]
+            pars[f"PORT_P{i}_P{j}"] = {"value": ports.split(",")[j]}
 
     for line in fileinput.input(f"secure-gwas/par/test.par.{role}.txt", inplace=True):
         key = str(line).split(" ")[0]
         if key in pars:
             line = f"{key} " + str(pars[key]["value"]) + "\n"
         print(line, end="")
```

## Comparing `sfkit-0.0.98.dist-info/METADATA` & `sfkit-0.0.99.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfkit
-Version: 0.0.98
+Version: 0.0.99
 Summary: Some CLI Tools For The Secure Multi-party Genomic Analysis Website
 Project-URL: Website, https://secure-gwas-website-bhj5a4wkqa-uc.a.run.app/
 Project-URL: Github, https://github.com/simonjmendelsohn/secure-gwas-keys-and-encryption
 Author-email: Simon Mendelsohn <smendels@broadinstitute.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `sfkit-0.0.98.dist-info/licenses/LICENSE` & `sfkit-0.0.99.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `sfkit-0.0.98.dist-info/RECORD` & `sfkit-0.0.99.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 sfkit/encryption/mpc/test_data/input_data2/cov.txt,sha256=sOtLarBoT7DwIEjybIkhIODceLtfyA_d6VwEMsCmT0o,10000
 sfkit/encryption/mpc/test_data/input_data2/geno.txt,sha256=j-Q5bE5QhpQ9YdrErd1q3LIxXxoIs-Zy_v3N5q9QTC4,1000000
 sfkit/encryption/mpc/test_data/input_data2/pheno.txt,sha256=BEuzGzDWLPPGBKtc2Q8FKBEkwZN4iks-SNR_3WgCll8,1000
 sfkit/encryption/mpc/test_data/input_data2/pos.txt,sha256=UO4tAji81yVr3uYn-1HXLbjOjsENKKnZqfQD94Y86x0,12000
 sfkit/protocol/register_data.py,sha256=bsLaPmvCdvBTDNW8ir378bAqr8Pf4cc5ATS12e7hcfU,4702
 sfkit/protocol/run_protocol.py,sha256=GSrf0YAhtSqgPAtjuyi6V9yd3JiYTpk8fEm71GMopII,2080
 sfkit/protocol/utils/constants.py,sha256=daRLURnSGQzJrIAoT85HlM7fm7rcXMQ09zAbrPns6U8,407
-sfkit/protocol/utils/gwas_protocol.py,sha256=rRmYmp1jXrFRwLaHUq7_KzPJ1XQQ9vQfZMScbi1MR78,8633
+sfkit/protocol/utils/gwas_protocol.py,sha256=CUbiJYA-zXDq_J-f5p34abRDY5ZPDig9nZcC1tsWHQ0,8666
 sfkit/protocol/utils/helper_functions.py,sha256=-sQTS7spoYT8kp70hymrDaz2Q0Af0VsyMKmAi6TrVeE,452
 sfkit/protocol/utils/pca_protocol.py,sha256=QZFF5PxZhgUOdGUHkQWRUzlWmajqBCgzntF-QiUByng,1508
 sfkit/protocol/utils/sfgwas_protocol.py,sha256=xSHKi3pSSIVwww4M7JxSVb_09Qz7W4QLwKWMXzt3HSA,10318
-sfkit-0.0.98.dist-info/METADATA,sha256=0vIWGCi4sEgDTYYKvrZPWfQ16iioZkdtvnWCy8BPnXw,2077
-sfkit-0.0.98.dist-info/WHEEL,sha256=NaLmgHHW_f9jTvv_wRh9vcK7c7EK9o5fwsIXMOzoGgM,87
-sfkit-0.0.98.dist-info/entry_points.txt,sha256=Vvw2Pp_elCGEt1l_kxS5XxrzrLLKvdikFqIpxVqGVpw,41
-sfkit-0.0.98.dist-info/licenses/LICENSE,sha256=naooNWwcBzutWZZhLJciH5mzmsj3-AeWRojIR9TZtzE,1073
-sfkit-0.0.98.dist-info/RECORD,,
+sfkit-0.0.99.dist-info/METADATA,sha256=qZiFu7wj0nNBxz-4awplqv4Tk-OCZma90ygJlSg9T-U,2077
+sfkit-0.0.99.dist-info/WHEEL,sha256=NaLmgHHW_f9jTvv_wRh9vcK7c7EK9o5fwsIXMOzoGgM,87
+sfkit-0.0.99.dist-info/entry_points.txt,sha256=Vvw2Pp_elCGEt1l_kxS5XxrzrLLKvdikFqIpxVqGVpw,41
+sfkit-0.0.99.dist-info/licenses/LICENSE,sha256=naooNWwcBzutWZZhLJciH5mzmsj3-AeWRojIR9TZtzE,1073
+sfkit-0.0.99.dist-info/RECORD,,
```

