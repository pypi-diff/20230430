# Comparing `tmp/cellmap-1.0.1.dev202304300542-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304300650-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 19251 bytes, number of entries: 5
+Zip file size: 19253 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   108732 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304300542.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304300542.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304300542.dist-info/RECORD
-5 files, 111146 bytes uncompressed, 18497 bytes compressed:  83.4%
+-rw-r--r--  2.0 unx   108718 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304300650.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304300650.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304300650.dist-info/RECORD
+5 files, 111132 bytes uncompressed, 18499 bytes compressed:  83.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304300542.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304300650.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304300542.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304300650.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304300542.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304300650.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -2004,15 +2004,15 @@
         idx_ = adata.var['expressed_'+name_i_]
         gene_list_ = adata.var.index[idx_].values
         e_ += sum(idx_)
         txt_ = gene_list_ + '<br>' + target_clusters[i]+'<br>cluster '+ np.array(clusters_[s_:e_]+1,dtype=str)#+ '<br><img src="'+image_+'" width="200">'
         texts_= np.append(texts_,txt_)
         index_ = np.append(index_,source_cluster + '_' + target_clusters[i] + '_' + gene_list_)
         adata.var['clusters_'+name_i_] = -np.ones(adata.shape[1],dtype=int)
-        adata.var['clusters_'+name_i_][idx_] = adata.uns['gene_atlas']['clusters'][s_:e_]
+        adata.var['clusters_'+name_i_][idx_] = clusters_['clusters'][s_:e_]
         s_ += sum(idx_)
 
     adata.uns[gene_atlas_key] = {
         'index':index_,
         'texts':texts_,
         'dynamics':gene_dynamics_all_,
         'dynamics_norm':gene_dynamics_all_norm_,
```

## Comparing `cellmap-1.0.1.dev202304300542.dist-info/METADATA` & `cellmap-1.0.1.dev202304300650.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304300542
+Version: 1.0.1.dev202304300650
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

