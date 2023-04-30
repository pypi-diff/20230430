# Comparing `tmp/napatrackmater-3.3.9.tar.gz` & `tmp/napatrackmater-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-ttt3b2mp/napatrackmater-3.3.9.tar", last modified: Sun Apr 30 11:21:44 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-n_v27yyh/napatrackmater-3.4.0.tar", last modified: Sun Apr 30 13:06:40 2023, max compression
```

## Comparing `napatrackmater-3.3.9.tar` & `napatrackmater-3.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 11:21:44.106428 napatrackmater-3.3.9/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.3.9/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-04-30 11:21:44.097821 napatrackmater-3.3.9/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.3.9/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 11:21:43.735334 napatrackmater-3.3.9/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.3.9/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.3.9/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   109528 2023-04-30 11:03:51.000000 napatrackmater-3.3.9/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.3.9/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.3.9/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.3.9/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.3.9/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.3.9/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.3.9/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-30 11:20:54.000000 napatrackmater-3.3.9/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 11:21:44.038261 napatrackmater-3.3.9/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-04-30 11:21:43.000000 napatrackmater-3.3.9/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-04-30 11:21:44.108713 napatrackmater-3.3.9/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.3.9/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 13:06:40.292935 napatrackmater-3.4.0/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.4.0/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-04-30 13:06:40.286154 napatrackmater-3.4.0/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.4.0/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 13:06:39.983011 napatrackmater-3.4.0/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.4.0/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.4.0/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   108412 2023-04-30 13:05:31.000000 napatrackmater-3.4.0/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.4.0/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.4.0/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.4.0/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.4.0/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.4.0/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.4.0/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-30 13:05:38.000000 napatrackmater-3.4.0/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 13:06:40.236339 napatrackmater-3.4.0/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-04-30 13:06:39.000000 napatrackmater-3.4.0/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-04-30 13:06:39.000000 napatrackmater-3.4.0/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-30 13:06:39.000000 napatrackmater-3.4.0/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-04-30 13:06:39.000000 napatrackmater-3.4.0/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-04-30 13:06:39.000000 napatrackmater-3.4.0/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-04-30 13:06:39.000000 napatrackmater-3.4.0/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-04-30 13:06:40.295934 napatrackmater-3.4.0/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.4.0/setup.py
```

### Comparing `napatrackmater-3.3.9/LICENSE` & `napatrackmater-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/PKG-INFO` & `napatrackmater-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.3.9
+Version: 3.4.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.3.9/README.md` & `napatrackmater-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.4.0/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.4.0/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater/Trackmate.py` & `napatrackmater-3.4.0/napatrackmater/Trackmate.py`

 * *Files 1% similar despite different names*

```diff
@@ -3191,3656 +3191,3586 @@
 0000c760: 2e7a 6361 6c69 6272 6174 696f 6e0d 0a20  .zcalibration.. 
 0000c770: 2020 2020 2020 2020 2020 2064 6973 7461             dista
 0000c780: 6e63 655f 6365 6c6c 5f6d 6173 6b2c 206d  nce_cell_mask, m
 0000c790: 6173 6b63 656e 7472 6f69 6420 3d20 7365  askcentroid = se
 0000c7a0: 6c66 2e5f 6765 745f 626f 756e 6461 7279  lf._get_boundary
 0000c7b0: 5f64 6973 7428 6672 616d 652c 206c 6f63  _dist(frame, loc
 0000c7c0: 6174 696f 6e2c 2052 4144 4955 5329 0d0a  ation, RADIUS)..
-0000c7d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c7e0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000c7f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000c800: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
-0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c820: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
-0000c830: 793a 2069 6e74 2863 656c 6c5f 6964 292c  y: int(cell_id),
-0000c840: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000c850: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
-0000c860: 6569 645f 6b65 7920 3a20 696e 7428 666c  eid_key : int(fl
-0000c870: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000c880: 6574 2873 656c 662e 6672 616d 6569 645f  et(self.frameid_
-0000c890: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
-0000c8a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c8b0: 662e 7a70 6f73 6964 5f6b 6579 203a 2066  f.zposid_key : f
-0000c8c0: 6c6f 6174 2863 656e 7472 6f69 6473 5b69  loat(centroids[i
-0000c8d0: 6e64 6578 5d5b 305d 292c 0d0a 2020 2020  ndex][0]),..    
-0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8f0: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
-0000c900: 3a20 666c 6f61 7428 6365 6e74 726f 6964  : float(centroid
-0000c910: 735b 696e 6465 785d 5b31 5d29 2c0d 0a20  s[index][1]),.. 
-0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c930: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
-0000c940: 6579 203a 2066 6c6f 6174 2863 656e 7472  ey : float(centr
-0000c950: 6f69 6473 5b69 6e64 6578 5d5b 325d 292c  oids[index][2]),
-0000c960: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000c970: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-0000c980: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-0000c990: 203a 2028 666c 6f61 7428 696e 7465 6e73   : (float(intens
-0000c9a0: 6974 795f 746f 7461 6c5b 696e 6465 785d  ity_total[index]
-0000c9b0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000c9c0: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
-0000c9d0: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
-0000c9e0: 203a 2028 666c 6f61 7428 696e 7465 6e73   : (float(intens
-0000c9f0: 6974 795f 6d65 616e 5b69 6e64 6578 5d29  ity_mean[index])
-0000ca00: 292c 0d0a 0d0a 2020 2020 2020 2020 2020  ),....          
-0000ca10: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000ca20: 6164 6975 735f 6b65 7920 3a20 2866 6c6f  adius_key : (flo
-0000ca30: 6174 2852 4144 4955 5329 292c 0d0a 2020  at(RADIUS)),..  
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca50: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
-0000ca60: 6579 203a 2028 666c 6f61 7428 5155 414c  ey : (float(QUAL
-0000ca70: 4954 5929 292c 0d0a 2020 2020 2020 2020  ITY)),..        
-0000ca80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ca90: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-0000caa0: 6173 6b5f 6b65 793a 2066 6c6f 6174 2864  ask_key: float(d
-0000cab0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-0000cac0: 6b29 2c0d 0a20 2020 2020 2020 2020 2020  k),..           
-0000cad0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000cae0: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
-0000caf0: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
-0000cb00: 726f 6964 5b30 5d29 2c0d 0a20 2020 2020  roid[0]),..     
-0000cb10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000cb20: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-0000cb30: 5f79 5f6b 6579 3a20 666c 6f61 7428 6d61  _y_key: float(ma
-0000cb40: 736b 6365 6e74 726f 6964 5b31 5d29 2c0d  skcentroid[1]),.
-0000cb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cb60: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
-0000cb70: 6e74 726f 6964 5f78 5f6b 6579 3a20 666c  ntroid_x_key: fl
-0000cb80: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
-0000cb90: 5b32 5d29 200d 0a0d 0a20 2020 2020 2020  [2]) ....       
-0000cba0: 2020 2020 207d 200d 0a20 2020 2020 2020       } ..       
+0000c7d0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0000c7e0: 6973 7420 3c3d 2032 202a 2076 6574 6f5f  ist <= 2 * veto_
+0000c7f0: 7261 6469 7573 3a0d 0a20 2020 2020 2020  radius:..       
+0000c800: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+0000c810: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+0000c820: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+0000c830: 6c5f 6964 5d20 3d20 7b0d 0a20 2020 2020  l_id] = {..     
+0000c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c850: 2020 2073 656c 662e 6365 6c6c 6964 5f6b     self.cellid_k
+0000c860: 6579 3a20 696e 7428 6365 6c6c 5f69 6429  ey: int(cell_id)
+0000c870: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+0000c880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c890: 2e66 7261 6d65 6964 5f6b 6579 203a 2069  .frameid_key : i
+0000c8a0: 6e74 2866 6c6f 6174 2853 706f 746f 626a  nt(float(Spotobj
+0000c8b0: 6563 742e 6765 7428 7365 6c66 2e66 7261  ect.get(self.fra
+0000c8c0: 6d65 6964 5f6b 6579 2929 292c 0d0a 2020  meid_key))),..  
+0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8e0: 2020 2020 2020 7365 6c66 2e7a 706f 7369        self.zposi
+0000c8f0: 645f 6b65 7920 3a20 666c 6f61 7428 6365  d_key : float(ce
+0000c900: 6e74 726f 6964 735b 696e 6465 785d 5b30  ntroids[index][0
+0000c910: 5d29 2c0d 0a20 2020 2020 2020 2020 2020  ]),..           
+0000c920: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c930: 662e 7970 6f73 6964 5f6b 6579 203a 2066  f.yposid_key : f
+0000c940: 6c6f 6174 2863 656e 7472 6f69 6473 5b69  loat(centroids[i
+0000c950: 6e64 6578 5d5b 315d 292c 0d0a 2020 2020  ndex][1]),..    
+0000c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c970: 2020 2020 7365 6c66 2e78 706f 7369 645f      self.xposid_
+0000c980: 6b65 7920 3a20 666c 6f61 7428 6365 6e74  key : float(cent
+0000c990: 726f 6964 735b 696e 6465 785d 5b32 5d29  roids[index][2])
+0000c9a0: 2c0d 0a0d 0a20 2020 2020 2020 2020 2020  ,....           
+0000c9b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c9c0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000c9d0: 795f 6b65 7920 3a20 2866 6c6f 6174 2869  y_key : (float(i
+0000c9e0: 6e74 656e 7369 7479 5f74 6f74 616c 5b69  ntensity_total[i
+0000c9f0: 6e64 6578 5d29 292c 0d0a 2020 2020 2020  ndex])),..      
+0000ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca10: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
+0000ca20: 6e73 6974 795f 6b65 7920 3a20 2866 6c6f  nsity_key : (flo
+0000ca30: 6174 2869 6e74 656e 7369 7479 5f6d 6561  at(intensity_mea
+0000ca40: 6e5b 696e 6465 785d 2929 2c0d 0a0d 0a20  n[index])),.... 
+0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca60: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+0000ca70: 7573 5f6b 6579 203a 2028 666c 6f61 7428  us_key : (float(
+0000ca80: 5241 4449 5553 2929 2c0d 0a20 2020 2020  RADIUS)),..     
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caa0: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
+0000cab0: 6b65 7920 3a20 2866 6c6f 6174 2851 5541  key : (float(QUA
+0000cac0: 4c49 5459 2929 2c0d 0a20 2020 2020 2020  LITY)),..       
+0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cae0: 2073 656c 662e 6469 7374 616e 6365 5f63   self.distance_c
+0000caf0: 656c 6c5f 6d61 736b 5f6b 6579 3a20 666c  ell_mask_key: fl
+0000cb00: 6f61 7428 6469 7374 616e 6365 5f63 656c  oat(distance_cel
+0000cb10: 6c5f 6d61 736b 292c 0d0a 2020 2020 2020  l_mask),..      
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb30: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+0000cb40: 6f69 645f 7a5f 6b65 793a 2066 6c6f 6174  oid_z_key: float
+0000cb50: 286d 6173 6b63 656e 7472 6f69 645b 305d  (maskcentroid[0]
+0000cb60: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000cb70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cb80: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
+0000cb90: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
+0000cba0: 656e 7472 6f69 645b 315d 292c 0d0a 2020  entroid[1]),..  
 0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbc0: 200d 0a0d 0a20 2020 2064 6566 205f 6765   ....    def _ge
-0000cbd0: 745f 6d61 7374 6572 5f78 6d6c 5f64 6174  t_master_xml_dat
-0000cbe0: 6128 7365 6c66 293a 0d0a 2020 2020 2020  a(self):..      
-0000cbf0: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-0000cc00: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
-0000cc10: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc30: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-0000cc40: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
-0000cc50: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
-0000cc60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cc70: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
-0000cc80: 7472 6565 203d 2065 742e 7061 7273 6528  tree = et.parse(
-0000cc90: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
-0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccb0: 2020 2020 2020 7365 6c66 2e78 6d6c 5f72        self.xml_r
-0000ccc0: 6f6f 7420 3d20 7365 6c66 2e78 6d6c 5f74  oot = self.xml_t
-0000ccd0: 7265 652e 6765 7472 6f6f 7428 290d 0a20  ree.getroot().. 
+0000cbc0: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
+0000cbd0: 656e 7472 6f69 645f 785f 6b65 793a 2066  entroid_x_key: f
+0000cbe0: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
+0000cbf0: 645b 325d 2920 0d0a 0d0a 2020 2020 2020  d[2]) ....      
+0000cc00: 2020 2020 2020 2020 2020 7d20 0d0a 2020            } ..  
+0000cc10: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000cc20: 6627 666f 756e 6420 7b6c 656e 2873 656c  f'found {len(sel
+0000cc30: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000cc40: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000cc50: 297d 206d 6174 6368 696e 6720 7370 6f74  )} matching spot
+0000cc60: 7327 2920 2020 200d 0a20 2020 2020 2020  s')    ..       
+0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc80: 200d 0a0d 0a20 2020 2064 6566 205f 6765   ....    def _ge
+0000cc90: 745f 6d61 7374 6572 5f78 6d6c 5f64 6174  t_master_xml_dat
+0000cca0: 6128 7365 6c66 293a 0d0a 2020 2020 2020  a(self):..      
+0000ccb0: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
+0000ccc0: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
+0000ccd0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
 0000cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccf0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-0000cd00: 6c5f 786d 6c5f 6e61 6d65 203d 2027 7365  l_xml_name = 'se
-0000cd10: 636f 6e64 5f63 6861 6e6e 656c 5f27 202b  cond_channel_' +
-0000cd20: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-0000cd30: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
-0000cd40: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
-0000cd50: 2929 5b30 5d20 2b20 272e 786d 6c27 0d0a  ))[0] + '.xml'..
+0000ccf0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+0000cd00: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
+0000cd10: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
+0000cd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd30: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
+0000cd40: 7472 6565 203d 2065 742e 7061 7273 6528  tree = et.parse(
+0000cd50: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
 0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
-0000cd80: 656c 5f78 6d6c 5f70 6174 6820 3d20 6f73  el_xml_path = os
-0000cd90: 2e70 6174 682e 6469 726e 616d 6528 7365  .path.dirname(se
-0000cda0: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdc0: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
-0000cdd0: 5f63 6861 6e6e 656c 5f74 7265 6528 290d  _channel_tree().
-0000cde0: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
-0000cdf0: 656c 662e 756e 6971 7565 5f6f 626a 6563  elf.unique_objec
-0000ce00: 7473 203d 207b 7d0d 0a20 2020 2020 2020  ts = {}..       
-0000ce10: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000ce20: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-0000ce30: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000ce40: 6c66 2e41 6c6c 5472 6163 6b49 6473 203d  lf.AllTrackIds =
-0000ce50: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-0000ce60: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-0000ce70: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
-0000ce80: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
-0000ce90: 726d 616c 5472 6163 6b49 6473 203d 205b  rmalTrackIds = [
-0000cea0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-0000ceb0: 656c 662e 616c 6c5f 7472 6163 6b5f 7072  elf.all_track_pr
-0000cec0: 6f70 6572 7469 6573 203d 205b 5d0d 0a20  operties = [].. 
-0000ced0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cee0: 7370 6c69 745f 706f 696e 7473 5f74 696d  split_points_tim
-0000cef0: 6573 203d 205b 5d0d 0a0d 0a20 2020 2020  es = []....     
-0000cf00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000cf10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000cf20: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-0000cf30: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
-0000cf40: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000cf50: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
-0000cf60: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
-0000cf70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000cf80: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000cf90: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
-0000cfa0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000cfb0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-0000cfc0: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
-0000cfd0: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
-0000cfe0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0000cff0: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
-0000d000: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
-0000d010: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
-0000d020: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d030: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
-0000d040: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
-0000d050: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
-0000d060: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000d070: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d080: 7365 6c66 2e53 706f 746f 626a 6563 7473  self.Spotobjects
-0000d090: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000d0a0: 656e 742e 6669 6e64 2827 4d6f 6465 6c27  ent.find('Model'
-0000d0b0: 292e 6669 6e64 2827 416c 6c53 706f 7473  ).find('AllSpots
-0000d0c0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-0000d0d0: 2320 4578 7472 6163 7420 7468 6520 7472  # Extract the tr
-0000d0e0: 6163 6b73 2066 726f 6d20 786d 6c0d 0a20  acks from xml.. 
-0000d0f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d100: 7472 6163 6b73 203d 2073 656c 662e 786d  tracks = self.xm
-0000d110: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
-0000d120: 4d6f 6465 6c22 292e 6669 6e64 2822 416c  Model").find("Al
-0000d130: 6c54 7261 636b 7322 290d 0a20 2020 2020  lTracks")..     
-0000d140: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000d150: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
-0000d160: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
-0000d170: 7474 696e 6773 2229 2e66 696e 6428 2249  ttings").find("I
-0000d180: 6d61 6765 4461 7461 2229 0d0a 2020 2020  mageData")..    
-0000d190: 2020 2020 2020 2020 7365 6c66 2e78 6361          self.xca
-0000d1a0: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
-0000d1b0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
-0000d1c0: 6765 7428 2270 6978 656c 7769 6474 6822  get("pixelwidth"
-0000d1d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000d1e0: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
-0000d1f0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
-0000d200: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
-0000d210: 656c 6865 6967 6874 2229 290d 0a20 2020  elheight"))..   
-0000d220: 2020 2020 2020 2020 2073 656c 662e 7a63           self.zc
-0000d230: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
-0000d240: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
-0000d250: 2e67 6574 2822 766f 7865 6c64 6570 7468  .get("voxeldepth
-0000d260: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
-0000d270: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
-0000d280: 6f6e 203d 2069 6e74 2866 6c6f 6174 2873  on = int(float(s
-0000d290: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000d2a0: 2822 7469 6d65 696e 7465 7276 616c 2229  ("timeinterval")
-0000d2b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000d2c0: 7365 6c66 2e64 6574 6563 746f 7273 6574  self.detectorset
-0000d2d0: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
-0000d2e0: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
-0000d2f0: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
-0000d300: 4465 7465 6374 6f72 5365 7474 696e 6773  DetectorSettings
-0000d310: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000d320: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
-0000d330: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
-0000d340: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
-0000d350: 696e 6773 2229 2e66 696e 6428 2242 6173  ings").find("Bas
-0000d360: 6963 5365 7474 696e 6773 2229 0d0a 2020  icSettings")..  
-0000d370: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000d380: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
-0000d390: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
-0000d3a0: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
-0000d3b0: 2e67 6574 2822 5441 5247 4554 5f43 4841  .get("TARGET_CHA
-0000d3c0: 4e4e 454c 2229 2929 0d0a 2020 2020 2020  NNEL")))..      
-0000d3d0: 2020 2020 2020 7365 6c66 2e74 7374 6172        self.tstar
-0000d3e0: 7420 3d20 696e 7428 666c 6f61 7428 7365  t = int(float(se
-0000d3f0: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
-0000d400: 2e67 6574 2822 7473 7461 7274 2229 2929  .get("tstart")))
-0000d410: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d420: 6c66 2e74 656e 6420 3d20 696e 7428 666c  lf.tend = int(fl
-0000d430: 6f61 7428 7365 6c66 2e62 6173 6963 7365  oat(self.basicse
-0000d440: 7474 696e 6773 2e67 6574 2822 7465 6e64  ttings.get("tend
-0000d450: 2229 2929 2020 2020 2020 0d0a 0d0a 2020  ")))      ....  
-0000d460: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000d470: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
-0000d480: 7370 6f74 7320 696e 2066 7261 6d65 2729  spots in frame')
-0000d490: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d4a0: 6c66 2e63 6f75 6e74 203d 2030 0d0a 2020  lf.count = 0..  
-0000d4b0: 2020 2020 2020 2020 2020 6675 7475 7265            future
-0000d4c0: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-0000d4d0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
-0000d4e0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
-0000d4f0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
-0000d500: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
-0000d510: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
-0000d520: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
-0000d530: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000d540: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000d550: 6f72 2066 7261 6d65 2069 6e20 7365 6c66  or frame in self
-0000d560: 2e53 706f 746f 626a 6563 7473 2e66 696e  .Spotobjects.fin
-0000d570: 6461 6c6c 2827 5370 6f74 7349 6e46 7261  dall('SpotsInFra
-0000d580: 6d65 2729 3a0d 0a20 2020 2020 2020 2020  me'):..         
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
-0000d5b0: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
-0000d5c0: 7428 7365 6c66 2e5f 6d61 7374 6572 5f73  t(self._master_s
-0000d5d0: 706f 745f 636f 6d70 7574 6572 2c20 6672  pot_computer, fr
-0000d5e0: 616d 6529 290d 0a20 2020 2020 2020 2020  ame))..         
-0000d5f0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000d600: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000d610: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d630: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d660: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-0000d670: 6265 6c20 3d20 2243 6f6c 6c65 6374 696e  bel = "Collectin
-0000d680: 6720 5370 6f74 7322 0d0a 2020 2020 2020  g Spots"..      
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6a0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000d6b0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
-0000d6c0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
-0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 2020 2020 7365 6c66 2e78 6d6c 5f72        self.xml_r
+0000cd80: 6f6f 7420 3d20 7365 6c66 2e78 6d6c 5f74  oot = self.xml_t
+0000cd90: 7265 652e 6765 7472 6f6f 7428 290d 0a20  ree.getroot().. 
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+0000cdc0: 6c5f 786d 6c5f 6e61 6d65 203d 2027 7365  l_xml_name = 'se
+0000cdd0: 636f 6e64 5f63 6861 6e6e 656c 5f27 202b  cond_channel_' +
+0000cde0: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+0000cdf0: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
+0000ce00: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
+0000ce10: 2929 5b30 5d20 2b20 272e 786d 6c27 0d0a  ))[0] + '.xml'..
+0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce30: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
+0000ce40: 656c 5f78 6d6c 5f70 6174 6820 3d20 6f73  el_xml_path = os
+0000ce50: 2e70 6174 682e 6469 726e 616d 6528 7365  .path.dirname(se
+0000ce60: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
+0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce80: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
+0000ce90: 5f63 6861 6e6e 656c 5f74 7265 6528 290d  _channel_tree().
+0000cea0: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
+0000ceb0: 656c 662e 756e 6971 7565 5f6f 626a 6563  elf.unique_objec
+0000cec0: 7473 203d 207b 7d0d 0a20 2020 2020 2020  ts = {}..       
+0000ced0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+0000cee0: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+0000cef0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000cf00: 6c66 2e41 6c6c 5472 6163 6b49 6473 203d  lf.AllTrackIds =
+0000cf10: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000cf20: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
+0000cf30: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
+0000cf40: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
+0000cf50: 726d 616c 5472 6163 6b49 6473 203d 205b  rmalTrackIds = [
+0000cf60: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+0000cf70: 656c 662e 616c 6c5f 7472 6163 6b5f 7072  elf.all_track_pr
+0000cf80: 6f70 6572 7469 6573 203d 205b 5d0d 0a20  operties = [].. 
+0000cf90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cfa0: 7370 6c69 745f 706f 696e 7473 5f74 696d  split_points_tim
+0000cfb0: 6573 203d 205b 5d0d 0a0d 0a20 2020 2020  es = []....     
+0000cfc0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000cfd0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000cfe0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+0000cff0: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
+0000d000: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d010: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
+0000d020: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
+0000d030: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d040: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+0000d050: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
+0000d060: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000d070: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+0000d080: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
+0000d090: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
+0000d0a0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000d0b0: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
+0000d0c0: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
+0000d0d0: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
+0000d0e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d0f0: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
+0000d100: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
+0000d110: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
+0000d120: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d130: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d140: 7365 6c66 2e53 706f 746f 626a 6563 7473  self.Spotobjects
+0000d150: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
+0000d160: 656e 742e 6669 6e64 2827 4d6f 6465 6c27  ent.find('Model'
+0000d170: 292e 6669 6e64 2827 416c 6c53 706f 7473  ).find('AllSpots
+0000d180: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+0000d190: 2320 4578 7472 6163 7420 7468 6520 7472  # Extract the tr
+0000d1a0: 6163 6b73 2066 726f 6d20 786d 6c0d 0a20  acks from xml.. 
+0000d1b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d1c0: 7472 6163 6b73 203d 2073 656c 662e 786d  tracks = self.xm
+0000d1d0: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
+0000d1e0: 4d6f 6465 6c22 292e 6669 6e64 2822 416c  Model").find("Al
+0000d1f0: 6c54 7261 636b 7322 290d 0a20 2020 2020  lTracks")..     
+0000d200: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000d210: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
+0000d220: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
+0000d230: 7474 696e 6773 2229 2e66 696e 6428 2249  ttings").find("I
+0000d240: 6d61 6765 4461 7461 2229 0d0a 2020 2020  mageData")..    
+0000d250: 2020 2020 2020 2020 7365 6c66 2e78 6361          self.xca
+0000d260: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
+0000d270: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000d280: 6765 7428 2270 6978 656c 7769 6474 6822  get("pixelwidth"
+0000d290: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000d2a0: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+0000d2b0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000d2c0: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
+0000d2d0: 656c 6865 6967 6874 2229 290d 0a20 2020  elheight"))..   
+0000d2e0: 2020 2020 2020 2020 2073 656c 662e 7a63           self.zc
+0000d2f0: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
+0000d300: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000d310: 2e67 6574 2822 766f 7865 6c64 6570 7468  .get("voxeldepth
+0000d320: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+0000d330: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
+0000d340: 6f6e 203d 2069 6e74 2866 6c6f 6174 2873  on = int(float(s
+0000d350: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000d360: 2822 7469 6d65 696e 7465 7276 616c 2229  ("timeinterval")
+0000d370: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000d380: 7365 6c66 2e64 6574 6563 746f 7273 6574  self.detectorset
+0000d390: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
+0000d3a0: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
+0000d3b0: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
+0000d3c0: 4465 7465 6374 6f72 5365 7474 696e 6773  DetectorSettings
+0000d3d0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000d3e0: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
+0000d3f0: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
+0000d400: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
+0000d410: 696e 6773 2229 2e66 696e 6428 2242 6173  ings").find("Bas
+0000d420: 6963 5365 7474 696e 6773 2229 0d0a 2020  icSettings")..  
+0000d430: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000d440: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
+0000d450: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
+0000d460: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
+0000d470: 2e67 6574 2822 5441 5247 4554 5f43 4841  .get("TARGET_CHA
+0000d480: 4e4e 454c 2229 2929 0d0a 2020 2020 2020  NNEL")))..      
+0000d490: 2020 2020 2020 7365 6c66 2e74 7374 6172        self.tstar
+0000d4a0: 7420 3d20 696e 7428 666c 6f61 7428 7365  t = int(float(se
+0000d4b0: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
+0000d4c0: 2e67 6574 2822 7473 7461 7274 2229 2929  .get("tstart")))
+0000d4d0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d4e0: 6c66 2e74 656e 6420 3d20 696e 7428 666c  lf.tend = int(fl
+0000d4f0: 6f61 7428 7365 6c66 2e62 6173 6963 7365  oat(self.basicse
+0000d500: 7474 696e 6773 2e67 6574 2822 7465 6e64  ttings.get("tend
+0000d510: 2229 2929 2020 2020 2020 0d0a 0d0a 2020  ")))      ....  
+0000d520: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000d530: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
+0000d540: 7370 6f74 7320 696e 2066 7261 6d65 2729  spots in frame')
+0000d550: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d560: 6c66 2e63 6f75 6e74 203d 2030 0d0a 2020  lf.count = 0..  
+0000d570: 2020 2020 2020 2020 2020 6675 7475 7265            future
+0000d580: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+0000d590: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
+0000d5a0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
+0000d5b0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
+0000d5c0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
+0000d5d0: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
+0000d5e0: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
+0000d5f0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d610: 6f72 2066 7261 6d65 2069 6e20 7365 6c66  or frame in self
+0000d620: 2e53 706f 746f 626a 6563 7473 2e66 696e  .Spotobjects.fin
+0000d630: 6461 6c6c 2827 5370 6f74 7349 6e46 7261  dall('SpotsInFra
+0000d640: 6d65 2729 3a0d 0a20 2020 2020 2020 2020  me'):..         
+0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d660: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
+0000d670: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
+0000d680: 7428 7365 6c66 2e5f 6d61 7374 6572 5f73  t(self._master_s
+0000d690: 706f 745f 636f 6d70 7574 6572 2c20 6672  pot_computer, fr
+0000d6a0: 616d 6529 290d 0a20 2020 2020 2020 2020  ame))..         
+0000d6b0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+0000d6c0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+0000d6d0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d710: 2020 206c 656e 2866 7574 7572 6573 292c     len(futures),
-0000d720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d740: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+0000d710: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d720: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+0000d730: 6265 6c20 3d20 2243 6f6c 6c65 6374 696e  bel = "Collectin
+0000d740: 6720 5370 6f74 7322 0d0a 2020 2020 2020  g Spots"..      
 0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000d770: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
-0000d780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d790: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
-0000d7a0: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
-0000d7b0: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
-0000d7c0: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
-0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7e0: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-0000d7f0: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
-0000d800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d760: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000d770: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+0000d780: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7a0: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
+0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7d0: 2020 206c 656e 2866 7574 7572 6573 292c     len(futures),
+0000d7e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d800: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
 0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-0000d830: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-0000d840: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d860: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000d870: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
-0000d880: 203d 2020 7365 6c66 2e63 6f75 6e74 0d0a   =  self.count..
+0000d820: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000d830: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
+0000d840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d850: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
+0000d860: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
+0000d870: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
+0000d880: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
 0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8b0: 722e 7265 7375 6c74 2829 2020 2020 0d0a  r.result()    ..
-0000d8c0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000d8d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000d8e0: 7428 6627 4974 6572 6174 696e 6720 6f76  t(f'Iterating ov
-0000d8f0: 6572 2074 7261 636b 7320 7b6c 656e 2873  er tracks {len(s
-0000d900: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
-0000d910: 636b 5f69 6473 297d 2729 2020 0d0a 2020  ck_ids)}')  ..  
-0000d920: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000d930: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
-0000d940: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
-0000d950: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000d960: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
-0000d970: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
-0000d980: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
-0000d990: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
-0000d9a0: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
-0000d9b0: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
-0000d9c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000d9d0: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
-0000d9e0: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
-0000d9f0: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
-0000da00: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000da10: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da30: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-0000da40: 3d20 696e 7428 7472 6163 6b2e 6765 7428  = int(track.get(
-0000da50: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-0000da60: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000da70: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0000da80: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
-0000da90: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000daa0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dac0: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
-0000dad0: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
-0000dae0: 6d69 7428 7365 6c66 2e5f 6d61 7374 6572  mit(self._master
-0000daf0: 5f74 7261 636b 5f63 6f6d 7075 7465 722c  _track_computer,
-0000db00: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
-0000db10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000db20: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-0000db30: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-0000db40: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000d8a0: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000d8b0: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+0000d8c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8e0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000d8f0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000d900: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d920: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000d930: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+0000d940: 203d 2020 7365 6c66 2e63 6f75 6e74 0d0a   =  self.count..
+0000d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d970: 722e 7265 7375 6c74 2829 2020 2020 0d0a  r.result()    ..
+0000d980: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000d990: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000d9a0: 7428 6627 4974 6572 6174 696e 6720 6f76  t(f'Iterating ov
+0000d9b0: 6572 2074 7261 636b 7320 7b6c 656e 2873  er tracks {len(s
+0000d9c0: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000d9d0: 636b 5f69 6473 297d 2729 2020 0d0a 2020  ck_ids)}')  ..  
+0000d9e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000d9f0: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+0000da00: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
+0000da10: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+0000da20: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
+0000da30: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
+0000da40: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
+0000da50: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
+0000da60: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
+0000da70: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
+0000da80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000da90: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
+0000daa0: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
+0000dab0: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
+0000dac0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+0000dad0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daf0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+0000db00: 3d20 696e 7428 7472 6163 6b2e 6765 7428  = int(track.get(
+0000db10: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+0000db20: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000db30: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+0000db40: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
+0000db50: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+0000db60: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
 0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000db90: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-0000dba0: 203d 2022 436f 6c6c 6563 7469 6e67 2054   = "Collecting T
-0000dbb0: 7261 636b 7322 0d0a 2020 2020 2020 2020  racks"..        
-0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbd0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000dbe0: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
-0000dbf0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc10: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
-0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db80: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
+0000db90: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
+0000dba0: 6d69 7428 7365 6c66 2e5f 6d61 7374 6572  mit(self._master
+0000dbb0: 5f74 7261 636b 5f63 6f6d 7075 7465 722c  _track_computer,
+0000dbc0: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
+0000dbd0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000dbe0: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+0000dbf0: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+0000dc00: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc20: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc40: 206c 656e 2873 656c 662e 6669 6c74 6572   len(self.filter
-0000dc50: 6564 5f74 7261 636b 5f69 6473 292c 0d0a  ed_track_ids),..
-0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dca0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000dcb0: 5f62 6172 2e73 686f 7728 290d 0a0d 0a0d  _bar.show().....
-0000dcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dcd0: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
-0000dce0: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
-0000dcf0: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
-0000dd00: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
-0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd20: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-0000dd30: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
-0000dd40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dc40: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000dc50: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+0000dc60: 203d 2022 436f 6c6c 6563 7469 6e67 2054   = "Collecting T
+0000dc70: 7261 636b 7322 0d0a 2020 2020 2020 2020  racks"..        
+0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc90: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000dca0: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
+0000dcb0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcd0: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd00: 206c 656e 2873 656c 662e 6669 6c74 6572   len(self.filter
+0000dd10: 6564 5f74 7261 636b 5f69 6473 292c 0d0a  ed_track_ids),..
+0000dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd60: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-0000dd70: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-0000dd80: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dda0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000ddb0: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
-0000ddc0: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
+0000dd60: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000dd70: 5f62 6172 2e73 686f 7728 290d 0a0d 0a0d  _bar.show().....
+0000dd80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd90: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
+0000dda0: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
+0000ddb0: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
+0000ddc0: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
 0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dde0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000ddf0: 2e72 6573 756c 7428 290d 0a20 2020 2020  .result()..     
-0000de00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000de10: 2020 2020 2069 6620 7365 6c66 2e63 6861       if self.cha
-0000de20: 6e6e 656c 5f73 6567 5f69 6d61 6765 2069  nnel_seg_image i
-0000de30: 7320 6e6f 7420 4e6f 6e65 3a20 200d 0a20  s not None:  .. 
-0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000de60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000de70: 656c 662e 5f63 7265 6174 655f 7365 636f  elf._create_seco
-0000de80: 6e64 5f63 6861 6e6e 656c 5f78 6d6c 2829  nd_channel_xml()
-0000de90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dea0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-0000deb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000dec0: 286b 2c76 2920 696e 2073 656c 662e 6772  (k,v) in self.gr
-0000ded0: 6170 685f 7370 6c69 742e 6974 656d 7328  aph_split.items(
-0000dee0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000def0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000df00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df10: 2020 2020 2020 2020 2020 2020 2064 6175               dau
-0000df20: 6768 7465 725f 7472 6163 6b5f 6964 203d  ghter_track_id =
-0000df30: 2020 696e 7428 666c 6f61 7428 7374 7228    int(float(str(
-0000df40: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-0000df50: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-0000df60: 666c 6f61 7428 6b29 295d 5b73 656c 662e  float(k))][self.
-0000df70: 756e 6971 7565 6964 5f6b 6579 5d29 2929  uniqueid_key])))
-0000df80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000df90: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000dfa0: 7265 6e74 5f74 7261 636b 5f69 6420 3d20  rent_track_id = 
-0000dfb0: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
-0000dfc0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-0000dfd0: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
-0000dfe0: 6f61 7428 7629 295d 5b73 656c 662e 756e  oat(v))][self.un
-0000dff0: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
-0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e020: 2e67 7261 7068 5f74 7261 636b 735b 6461  .graph_tracks[da
-0000e030: 7567 6874 6572 5f74 7261 636b 5f69 645d  ughter_track_id]
-0000e040: 203d 2070 6172 656e 745f 7472 6163 6b5f   = parent_track_
-0000e050: 6964 0d0a 0d0a 2020 2020 2020 2020 2020  id....          
-0000e060: 2020 7072 696e 7428 2767 6574 7469 6e67    print('getting
-0000e070: 2061 7474 7269 6275 7465 7327 2920 2020   attributes')   
-0000e080: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000e090: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e0a0: 5f67 6574 5f61 7474 7269 6275 7465 7328  _get_attributes(
-0000e0b0: 290d 0a20 2020 2020 2020 2020 2020 0d0a  )..           ..
-0000e0c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e0d0: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
-0000e0e0: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
-0000e0f0: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
-0000e100: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
-0000e110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e130: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000e140: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
-0000e150: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e180: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000e190: 6172 2e6c 6162 656c 203d 2022 4a75 7374  ar.label = "Just
-0000e1a0: 206f 6e65 206d 6f72 6520 7468 696e 6722   one more thing"
-0000e1b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000e1e0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
-0000e1f0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
-0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e220: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
+0000dde0: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000ddf0: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+0000de00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000de30: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000de40: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de60: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000de70: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+0000de80: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
+0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dea0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000deb0: 2e72 6573 756c 7428 290d 0a20 2020 2020  .result()..     
+0000dec0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000ded0: 2020 2020 2069 6620 7365 6c66 2e63 6861       if self.cha
+0000dee0: 6e6e 656c 5f73 6567 5f69 6d61 6765 2069  nnel_seg_image i
+0000def0: 7320 6e6f 7420 4e6f 6e65 3a20 200d 0a20  s not None:  .. 
+0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000df20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000df30: 656c 662e 5f63 7265 6174 655f 7365 636f  elf._create_seco
+0000df40: 6e64 5f63 6861 6e6e 656c 5f78 6d6c 2829  nd_channel_xml()
+0000df50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000df60: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+0000df70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000df80: 286b 2c76 2920 696e 2073 656c 662e 6772  (k,v) in self.gr
+0000df90: 6170 685f 7370 6c69 742e 6974 656d 7328  aph_split.items(
+0000dfa0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000dfc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dfd0: 2020 2020 2020 2020 2020 2020 2064 6175               dau
+0000dfe0: 6768 7465 725f 7472 6163 6b5f 6964 203d  ghter_track_id =
+0000dff0: 2020 696e 7428 666c 6f61 7428 7374 7228    int(float(str(
+0000e000: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+0000e010: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+0000e020: 666c 6f61 7428 6b29 295d 5b73 656c 662e  float(k))][self.
+0000e030: 756e 6971 7565 6964 5f6b 6579 5d29 2929  uniqueid_key])))
+0000e040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e050: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000e060: 7265 6e74 5f74 7261 636b 5f69 6420 3d20  rent_track_id = 
+0000e070: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
+0000e080: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+0000e090: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
+0000e0a0: 6f61 7428 7629 295d 5b73 656c 662e 756e  oat(v))][self.un
+0000e0b0: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
+0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e0e0: 2e67 7261 7068 5f74 7261 636b 735b 6461  .graph_tracks[da
+0000e0f0: 7567 6874 6572 5f74 7261 636b 5f69 645d  ughter_track_id]
+0000e100: 203d 2070 6172 656e 745f 7472 6163 6b5f   = parent_track_
+0000e110: 6964 0d0a 0d0a 2020 2020 2020 2020 2020  id....          
+0000e120: 2020 7072 696e 7428 2767 6574 7469 6e67    print('getting
+0000e130: 2061 7474 7269 6275 7465 7327 2920 2020   attributes')   
+0000e140: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000e150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e160: 5f67 6574 5f61 7474 7269 6275 7465 7328  _get_attributes(
+0000e170: 290d 0a20 2020 2020 2020 2020 2020 0d0a  )..           ..
+0000e180: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e190: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
+0000e1a0: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
+0000e1b0: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
+0000e1c0: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
+0000e1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000e200: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000e210: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e250: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
-0000e260: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
-0000e270: 636b 5f69 6473 292c 0d0a 2020 2020 2020  ck_ids),..      
+0000e240: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000e250: 6172 2e6c 6162 656c 203d 2022 4a75 7374  ar.label = "Just
+0000e260: 206f 6e65 206d 6f72 6520 7468 696e 6722   one more thing"
+0000e270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2a0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e290: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000e2a0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+0000e2b0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
 0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2d0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000e2e0: 6172 2e73 686f 7728 290d 0a20 2020 2020  ar.show()..     
+0000e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2e0: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
 0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e310: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-0000e320: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
-0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e310: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
+0000e320: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000e330: 636b 5f69 6473 292c 0d0a 2020 2020 2020  ck_ids),..      
 0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000e360: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
-0000e370: 3d20 7365 6c66 2e63 6f75 6e74 0d0a 2020  = self.count..  
+0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e360: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3a0: 2020 7365 6c66 2e5f 6669 6e61 6c5f 7472    self._final_tr
-0000e3b0: 6163 6b73 2874 7261 636b 5f69 6429 200d  acks(track_id) .
-0000e3c0: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-0000e3d0: 6620 7365 6c66 2e66 6f75 7269 6572 3a0d  f self.fourier:.
-0000e3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e3f0: 2020 2020 7072 696e 7428 2763 6f6d 7075      print('compu
-0000e400: 7469 6e67 2046 6f75 7269 6572 2729 0d0a  ting Fourier')..
-0000e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e420: 2020 2073 656c 662e 5f63 6f6d 7075 7465     self._compute
-0000e430: 5f70 6865 6e6f 7479 7065 7328 2920 2020  _phenotypes()   
+0000e390: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000e3a0: 6172 2e73 686f 7728 290d 0a20 2020 2020  ar.show()..     
+0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3d0: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+0000e3e0: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e410: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000e420: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
+0000e430: 3d20 7365 6c66 2e63 6f75 6e74 0d0a 2020  = self.count..  
 0000e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e450: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000e460: 2020 2073 656c 662e 5f74 656d 706f 7261     self._tempora
-0000e470: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
-0000e480: 6528 2920 2020 2020 2020 200d 0a0d 0a0d  e()        .....
-0000e490: 0a20 2020 2064 6566 205f 6372 6561 7465  .    def _create
-0000e4a0: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
-0000e4b0: 786d 6c28 7365 6c66 293a 0d0a 2020 2020  xml(self):..    
-0000e4c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000e4d0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-0000e4e0: 6e6e 656c 5f66 696c 7465 7265 645f 7472  nnel_filtered_tr
-0000e4f0: 6163 6b73 203d 205b 5d20 2020 200d 0a20  acks = []    .. 
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e460: 2020 7365 6c66 2e5f 6669 6e61 6c5f 7472    self._final_tr
+0000e470: 6163 6b73 2874 7261 636b 5f69 6429 200d  acks(track_id) .
+0000e480: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0000e490: 6620 7365 6c66 2e66 6f75 7269 6572 3a0d  f self.fourier:.
+0000e4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e4b0: 2020 2020 7072 696e 7428 2763 6f6d 7075      print('compu
+0000e4c0: 7469 6e67 2046 6f75 7269 6572 2729 0d0a  ting Fourier')..
+0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4e0: 2020 2073 656c 662e 5f63 6f6d 7075 7465     self._compute
+0000e4f0: 5f70 6865 6e6f 7479 7065 7328 2920 2020  _phenotypes()   
 0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e510: 2020 2070 7269 6e74 2827 5472 616e 7366     print('Transf
-0000e520: 6572 7269 6e67 2058 4d4c 2729 2020 2020  erring XML')    
-0000e530: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e550: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
-0000e560: 696e 2073 656c 662e 786d 6c5f 726f 6f74  in self.xml_root
-0000e570: 2e69 7465 7228 2753 706f 7427 293a 0d0a  .iter('Spot'):..
-0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e590: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-0000e5a0: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
-0000e5b0: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
-0000e5c0: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
-0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5e0: 2020 2020 2020 2020 6966 2063 656c 6c5f          if cell_
-0000e5f0: 6964 2069 6e20 7365 6c66 2e63 6861 6e6e  id in self.chann
-0000e600: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-0000e610: 726f 7065 7274 6965 732e 6b65 7973 2829  roperties.keys()
-0000e620: 3a20 2020 2020 2020 200d 0a20 2020 2020  :        ..     
-0000e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e640: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e660: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000e670: 5f70 6f73 6974 696f 6e78 203d 2020 7365  _positionx =  se
-0000e680: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-0000e690: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000e6a0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
-0000e6b0: 7870 6f73 6964 5f6b 6579 5d0d 0a20 2020  xposid_key]..   
+0000e510: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e520: 2020 2073 656c 662e 5f74 656d 706f 7261     self._tempora
+0000e530: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
+0000e540: 6528 2920 2020 2020 2020 200d 0a0d 0a0d  e()        .....
+0000e550: 0a20 2020 2064 6566 205f 6372 6561 7465  .    def _create
+0000e560: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
+0000e570: 786d 6c28 7365 6c66 293a 0d0a 2020 2020  xml(self):..    
+0000e580: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000e590: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0000e5a0: 6e74 2827 5472 616e 7366 6572 7269 6e67  nt('Transferring
+0000e5b0: 2058 4d4c 2729 2020 2020 2020 2020 2020   XML')          
+0000e5c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e5d0: 2020 2020 2020 2020 2020 2066 6f72 2053             for S
+0000e5e0: 706f 746f 626a 6563 7420 696e 2073 656c  potobject in sel
+0000e5f0: 662e 786d 6c5f 726f 6f74 2e69 7465 7228  f.xml_root.iter(
+0000e600: 2753 706f 7427 293a 0d0a 2020 2020 2020  'Spot'):..      
+0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e620: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
+0000e630: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
+0000e640: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
+0000e650: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e670: 2020 6966 2063 656c 6c5f 6964 2069 6e20    if cell_id in 
+0000e680: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+0000e690: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000e6a0: 6965 732e 6b65 7973 2829 3a20 2020 2020  ies.keys():     
+0000e6b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 0000e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6e0: 206e 6577 5f70 6f73 6974 696f 6e79 203d   new_positiony =
-0000e6f0: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
-0000e700: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000e710: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
-0000e720: 656c 662e 7970 6f73 6964 5f6b 6579 5d0d  elf.yposid_key].
-0000e730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 2020 2020 206e 6577 5f70 6f73 6974 696f       new_positio
-0000e760: 6e7a 203d 2020 7365 6c66 2e63 6861 6e6e  nz =  self.chann
-0000e770: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-0000e780: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-0000e790: 645d 5b73 656c 662e 7a70 6f73 6964 5f6b  d][self.zposid_k
-0000e7a0: 6579 5d0d 0a0d 0a20 2020 2020 2020 2020  ey]....         
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2020 2020 2020 2020 2020 206e 6577 5f74             new_t
-0000e7d0: 6f74 616c 5f69 6e74 656e 7369 7479 203d  otal_intensity =
-0000e7e0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000e7f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e800: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000e810: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000e820: 7479 5f6b 6579 5d0d 0a20 2020 2020 2020  ty_key]..       
-0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e840: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000e850: 5f6d 6561 6e5f 696e 7465 6e73 6974 7920  _mean_intensity 
-0000e860: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f75  = self.channel_u
-0000e870: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000e880: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
-0000e890: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-0000e8a0: 7479 5f6b 6579 5d0d 0a0d 0a20 2020 2020  ty_key]....     
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000e8d0: 6577 5f72 6164 6975 7320 3d20 7365 6c66  ew_radius = self
-0000e8e0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000e8f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000e900: 6365 6c6c 5f69 645d 5b73 656c 662e 7261  cell_id][self.ra
-0000e910: 6469 7573 5f6b 6579 5d0d 0a20 2020 2020  dius_key]..     
-0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e930: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000e940: 6577 5f71 7561 6c69 7479 203d 2073 656c  ew_quality = sel
-0000e950: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000e960: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000e970: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e71  [cell_id][self.q
-0000e980: 7561 6c69 7479 5f6b 6579 5d0d 0a20 2020  uality_key]..   
-0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 206e 6577 5f64 6973 7461 6e63 655f 6365   new_distance_ce
-0000e9c0: 6c6c 5f6d 6173 6b20 3d20 7365 6c66 2e63  ll_mask = self.c
-0000e9d0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-0000e9e0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-0000e9f0: 6c6c 5f69 645d 5b73 656c 662e 6469 7374  ll_id][self.dist
-0000ea00: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
-0000ea10: 6579 5d0d 0a0d 0a20 2020 2020 2020 2020  ey]....         
+0000e6d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6f0: 2020 2020 2020 206e 6577 5f70 6f73 6974         new_posit
+0000e700: 696f 6e78 203d 2020 7365 6c66 2e63 6861  ionx =  self.cha
+0000e710: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000e720: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000e730: 5f69 645d 5b73 656c 662e 7870 6f73 6964  _id][self.xposid
+0000e740: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
+0000e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e760: 2020 2020 2020 2020 2020 206e 6577 5f70             new_p
+0000e770: 6f73 6974 696f 6e79 203d 2020 7365 6c66  ositiony =  self
+0000e780: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000e790: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000e7a0: 6365 6c6c 5f69 645d 5b73 656c 662e 7970  cell_id][self.yp
+0000e7b0: 6f73 6964 5f6b 6579 5d0d 0a20 2020 2020  osid_key]..     
+0000e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e7e0: 6577 5f70 6f73 6974 696f 6e7a 203d 2020  ew_positionz =  
+0000e7f0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+0000e800: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000e810: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
+0000e820: 662e 7a70 6f73 6964 5f6b 6579 5d0d 0a0d  f.zposid_key]...
+0000e830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e850: 2020 2020 206e 6577 5f74 6f74 616c 5f69       new_total_i
+0000e860: 6e74 656e 7369 7479 203d 2073 656c 662e  ntensity = self.
+0000e870: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+0000e880: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+0000e890: 656c 6c5f 6964 5d5b 7365 6c66 2e74 6f74  ell_id][self.tot
+0000e8a0: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
+0000e8b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8d0: 2020 2020 2020 206e 6577 5f6d 6561 6e5f         new_mean_
+0000e8e0: 696e 7465 6e73 6974 7920 3d20 7365 6c66  intensity = self
+0000e8f0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000e900: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000e910: 6365 6c6c 5f69 645d 5b73 656c 662e 6d65  cell_id][self.me
+0000e920: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
+0000e930: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e950: 2020 2020 2020 2020 206e 6577 5f72 6164           new_rad
+0000e960: 6975 7320 3d20 7365 6c66 2e63 6861 6e6e  ius = self.chann
+0000e970: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000e980: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+0000e990: 645d 5b73 656c 662e 7261 6469 7573 5f6b  d][self.radius_k
+0000e9a0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9c0: 2020 2020 2020 2020 206e 6577 5f71 7561           new_qua
+0000e9d0: 6c69 7479 203d 2073 656c 662e 6368 616e  lity = self.chan
+0000e9e0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000e9f0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+0000ea00: 6964 5d5b 7365 6c66 2e71 7561 6c69 7479  id][self.quality
+0000ea10: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
 0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
-0000ea40: 626a 6563 742e 7365 7428 7365 6c66 2e78  bject.set(self.x
-0000ea50: 706f 7369 645f 6b65 792c 2073 7472 286e  posid_key, str(n
-0000ea60: 6577 5f70 6f73 6974 696f 6e78 2929 2020  ew_positionx))  
-0000ea70: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea90: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
-0000eaa0: 6563 742e 7365 7428 7365 6c66 2e79 706f  ect.set(self.ypo
-0000eab0: 7369 645f 6b65 792c 2073 7472 286e 6577  sid_key, str(new
-0000eac0: 5f70 6f73 6974 696f 6e79 2929 0d0a 2020  _positiony))..  
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
-0000eb00: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
-0000eb10: 2c20 7374 7228 6e65 775f 706f 7369 7469  , str(new_positi
-0000eb20: 6f6e 7a29 290d 0a0d 0a20 2020 2020 2020  onz))....       
-0000eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb40: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
-0000eb50: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
-0000eb60: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
-0000eb70: 5f6b 6579 2c20 7374 7228 6e65 775f 746f  _key, str(new_to
-0000eb80: 7461 6c5f 696e 7465 6e73 6974 7929 2920  tal_intensity)) 
-0000eb90: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000eba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebb0: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
-0000ebc0: 6a65 6374 2e73 6574 2873 656c 662e 6d65  ject.set(self.me
-0000ebd0: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
-0000ebe0: 2c20 7374 7228 6e65 775f 6d65 616e 5f69  , str(new_mean_i
-0000ebf0: 6e74 656e 7369 7479 2929 0d0a 0d0a 2020  ntensity))....  
-0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec20: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
-0000ec30: 2873 656c 662e 7261 6469 7573 5f6b 6579  (self.radius_key
-0000ec40: 2c20 7374 7228 6e65 775f 7261 6469 7573  , str(new_radius
-0000ec50: 2929 2020 2020 200d 0a20 2020 2020 2020  ))     ..       
-0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec70: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
-0000ec80: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
-0000ec90: 2e71 7561 6c69 7479 5f6b 6579 2c20 7374  .quality_key, st
-0000eca0: 7228 6e65 775f 7175 616c 6974 7929 290d  r(new_quality)).
-0000ecb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecd0: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-0000ece0: 7365 7428 7365 6c66 2e64 6973 7461 6e63  set(self.distanc
-0000ecf0: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 792c  e_cell_mask_key,
-0000ed00: 2073 7472 286e 6577 5f64 6973 7461 6e63   str(new_distanc
-0000ed10: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
-0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed40: 2020 2069 6620 7365 6c66 2e74 7261 636b     if self.track
-0000ed50: 6964 5f6b 6579 2069 6e20 7365 6c66 2e75  id_key in self.u
-0000ed60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000ed70: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-0000ed80: 6429 5d2e 6b65 7973 2829 3a0d 0a20 2020  d)].keys():..   
-0000ed90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edb0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000ede0: 7261 636b 5f69 6420 3d20 7365 6c66 2e75  rack_id = self.u
-0000edf0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000ee00: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-0000ee10: 6429 5d5b 7365 6c66 2e74 7261 636b 6964  d)][self.trackid
-0000ee20: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
+0000ea30: 2020 2020 2020 2020 2020 206e 6577 5f64             new_d
+0000ea40: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0000ea50: 6b20 3d20 7365 6c66 2e63 6861 6e6e 656c  k = self.channel
+0000ea60: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000ea70: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000ea80: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
+0000ea90: 656c 6c5f 6d61 736b 5f6b 6579 5d0d 0a0d  ell_mask_key]...
+0000eaa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
+0000ead0: 7365 7428 7365 6c66 2e78 706f 7369 645f  set(self.xposid_
+0000eae0: 6b65 792c 2073 7472 286e 6577 5f70 6f73  key, str(new_pos
+0000eaf0: 6974 696f 6e78 2929 2020 2020 200d 0a20  itionx))     .. 
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb20: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
+0000eb30: 7428 7365 6c66 2e79 706f 7369 645f 6b65  t(self.yposid_ke
+0000eb40: 792c 2073 7472 286e 6577 5f70 6f73 6974  y, str(new_posit
+0000eb50: 696f 6e79 2929 0d0a 2020 2020 2020 2020  iony))..        
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb70: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+0000eb80: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+0000eb90: 7a70 6f73 6964 5f6b 6579 2c20 7374 7228  zposid_key, str(
+0000eba0: 6e65 775f 706f 7369 7469 6f6e 7a29 290d  new_positionz)).
+0000ebb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebd0: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
+0000ebe0: 742e 7365 7428 7365 6c66 2e74 6f74 616c  t.set(self.total
+0000ebf0: 5f69 6e74 656e 7369 7479 5f6b 6579 2c20  _intensity_key, 
+0000ec00: 7374 7228 6e65 775f 746f 7461 6c5f 696e  str(new_total_in
+0000ec10: 7465 6e73 6974 7929 2920 2020 2020 0d0a  tensity))     ..
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec40: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000ec50: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
+0000ec60: 656e 7369 7479 5f6b 6579 2c20 7374 7228  ensity_key, str(
+0000ec70: 6e65 775f 6d65 616e 5f69 6e74 656e 7369  new_mean_intensi
+0000ec80: 7479 2929 0d0a 0d0a 2020 2020 2020 2020  ty))....        
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eca0: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+0000ecb0: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+0000ecc0: 7261 6469 7573 5f6b 6579 2c20 7374 7228  radius_key, str(
+0000ecd0: 6e65 775f 7261 6469 7573 2929 2020 2020  new_radius))    
+0000ece0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed00: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
+0000ed10: 742e 7365 7428 7365 6c66 2e71 7561 6c69  t.set(self.quali
+0000ed20: 7479 5f6b 6579 2c20 7374 7228 6e65 775f  ty_key, str(new_
+0000ed30: 7175 616c 6974 7929 290d 0a20 2020 2020  quality))..     
+0000ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed50: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000ed60: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
+0000ed70: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+0000ed80: 5f6d 6173 6b5f 6b65 792c 2073 7472 286e  _mask_key, str(n
+0000ed90: 6577 5f64 6973 7461 6e63 655f 6365 6c6c  ew_distance_cell
+0000eda0: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+0000edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edc0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ede0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000edf0: 2020 2020 2020 2020 2066 6f72 2070 6172           for par
+0000ee00: 656e 7420 696e 2073 656c 662e 786d 6c5f  ent in self.xml_
+0000ee10: 726f 6f74 2e66 696e 6461 6c6c 2827 4d6f  root.findall('Mo
+0000ee20: 6465 6c27 293a 0d0a 2020 2020 2020 2020  del'):..        
 0000ee30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000ee50: 6861 6e6e 656c 5f66 696c 7465 7265 645f  hannel_filtered_
-0000ee60: 7472 6163 6b73 2e61 7070 656e 6428 7472  tracks.append(tr
-0000ee70: 6163 6b5f 6964 290d 0a20 2020 2020 2020  ack_id)..       
-0000ee80: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000ee90: 2070 6172 656e 7420 696e 2073 656c 662e   parent in self.
-0000eea0: 786d 6c5f 726f 6f74 2e66 696e 6461 6c6c  xml_root.findall
-0000eeb0: 2827 4d6f 6465 6c27 293a 0d0a 2020 2020  ('Model'):..    
+0000ee40: 666f 7220 6669 7273 7463 6869 6c64 2069  for firstchild i
+0000ee50: 6e20 7061 7265 6e74 2e66 696e 6461 6c6c  n parent.findall
+0000ee60: 2827 416c 6c54 7261 636b 7327 293a 0d0a  ('AllTracks'):..
+0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000ee90: 7365 636f 6e64 6368 696c 6420 696e 2066  secondchild in f
+0000eea0: 6972 7374 6368 696c 642e 6669 6e64 616c  irstchild.findal
+0000eeb0: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
 0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eed0: 2020 2020 666f 7220 6669 7273 7463 6869      for firstchi
-0000eee0: 6c64 2069 6e20 7061 7265 6e74 2e66 696e  ld in parent.fin
-0000eef0: 6461 6c6c 2827 416c 6c54 7261 636b 7327  dall('AllTracks'
-0000ef00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000eed0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000eee0: 2045 6467 656f 626a 6563 7420 696e 2073   Edgeobject in s
+0000eef0: 6563 6f6e 6463 6869 6c64 2e66 696e 6461  econdchild.finda
+0000ef00: 6c6c 2827 4564 6765 2729 3a0d 0a20 2020  ll('Edge'):..   
 0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef20: 666f 7220 7365 636f 6e64 6368 696c 6420  for secondchild 
-0000ef30: 696e 2066 6972 7374 6368 696c 642e 6669  in firstchild.fi
-0000ef40: 6e64 616c 6c28 2754 7261 636b 2729 3a0d  ndall('Track'):.
-0000ef50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef70: 2074 7261 636b 5f69 6420 3d20 696e 7428   track_id = int(
-0000ef80: 7365 636f 6e64 6368 696c 642e 6765 7428  secondchild.get(
-0000ef90: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-0000efa0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efc0: 2020 2020 6966 2074 7261 636b 5f69 6420      if track_id 
-0000efd0: 6e6f 7420 696e 2063 6861 6e6e 656c 5f66  not in channel_f
-0000efe0: 696c 7465 7265 645f 7472 6163 6b73 3a20  iltered_tracks: 
-0000eff0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ef20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef30: 2020 2020 2073 706f 745f 736f 7572 6365       spot_source
+0000ef40: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
+0000ef50: 4564 6765 6f62 6a65 6374 2e67 6574 2873  Edgeobject.get(s
+0000ef60: 656c 662e 7370 6f74 5f73 6f75 7263 655f  elf.spot_source_
+0000ef70: 6964 5f6b 6579 2929 2920 200d 0a20 2020  id_key)))  ..   
+0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efa0: 2020 2020 2073 706f 745f 7461 7267 6574       spot_target
+0000efb0: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
+0000efc0: 4564 6765 6f62 6a65 6374 2e67 6574 2873  Edgeobject.get(s
+0000efd0: 656c 662e 7370 6f74 5f74 6172 6765 745f  elf.spot_target_
+0000efe0: 6964 5f6b 6579 2929 2920 2020 2020 200d  id_key)))      .
+0000eff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f010: 2020 2020 2020 2020 2066 6972 7374 6368           firstch
-0000f020: 696c 642e 7265 6d6f 7665 2873 6563 6f6e  ild.remove(secon
-0000f030: 6463 6869 6c64 290d 0a20 2020 2020 2020  dchild)..       
-0000f040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f050: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000f060: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000f070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f080: 2020 2020 2066 6f72 2070 6172 656e 7420       for parent 
-0000f090: 696e 2073 656c 662e 786d 6c5f 726f 6f74  in self.xml_root
-0000f0a0: 2e66 696e 6461 6c6c 2827 4d6f 6465 6c27  .findall('Model'
-0000f0b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000f0c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000f0d0: 6669 7273 7463 6869 6c64 2069 6e20 7061  firstchild in pa
-0000f0e0: 7265 6e74 2e66 696e 6461 6c6c 2827 416c  rent.findall('Al
-0000f0f0: 6c54 7261 636b 7327 293a 0d0a 2020 2020  lTracks'):..    
-0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f110: 2020 2020 2020 2020 666f 7220 7365 636f          for seco
-0000f120: 6e64 6368 696c 6420 696e 2066 6972 7374  ndchild in first
-0000f130: 6368 696c 642e 6669 6e64 616c 6c28 2754  child.findall('T
-0000f140: 7261 636b 2729 3a0d 0a20 2020 2020 2020  rack'):..       
-0000f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f160: 2020 2020 2020 2020 2066 6f72 2045 6467           for Edg
-0000f170: 656f 626a 6563 7420 696e 2073 6563 6f6e  eobject in secon
-0000f180: 6463 6869 6c64 2e66 696e 6461 6c6c 2827  dchild.findall('
-0000f190: 4564 6765 2729 3a0d 0a20 2020 2020 2020  Edge'):..       
-0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1c0: 2073 706f 745f 736f 7572 6365 5f69 6420   spot_source_id 
-0000f1d0: 3d20 696e 7428 666c 6f61 7428 4564 6765  = int(float(Edge
-0000f1e0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000f1f0: 7370 6f74 5f73 6f75 7263 655f 6964 5f6b  spot_source_id_k
-0000f200: 6579 2929 2920 200d 0a20 2020 2020 2020  ey)))  ..       
+0000f010: 2020 2020 2020 2020 2069 6620 7370 6f74           if spot
+0000f020: 5f73 6f75 7263 655f 6964 206e 6f74 2069  _source_id not i
+0000f030: 6e20 7365 6c66 2e63 6861 6e6e 656c 5f75  n self.channel_u
+0000f040: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000f050: 7274 6965 732e 6b65 7973 2829 2061 6e64  rties.keys() and
+0000f060: 2073 706f 745f 7461 7267 6574 5f69 6420   spot_target_id 
+0000f070: 6e6f 7420 696e 2073 656c 662e 6368 616e  not in self.chan
+0000f080: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000f090: 7072 6f70 6572 7469 6573 2e6b 6579 7328  properties.keys(
+0000f0a0: 293a 2020 2020 200d 0a20 2020 2020 2020  ):     ..       
+0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0e0: 2020 2020 2073 6563 6f6e 6463 6869 6c64       secondchild
+0000f0f0: 2e72 656d 6f76 6528 4564 6765 6f62 6a65  .remove(Edgeobje
+0000f100: 6374 2920 200d 0a0d 0a20 2020 2020 2020  ct)  ....       
+0000f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f130: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f150: 7365 6c66 2e78 6d6c 5f74 7265 652e 7772  self.xml_tree.wr
+0000f160: 6974 6528 6f73 2e70 6174 682e 6a6f 696e  ite(os.path.join
+0000f170: 2873 656c 662e 6368 616e 6e65 6c5f 786d  (self.channel_xm
+0000f180: 6c5f 7061 7468 2c20 7365 6c66 2e63 6861  l_path, self.cha
+0000f190: 6e6e 656c 5f78 6d6c 5f6e 616d 6529 2920  nnel_xml_name)) 
+0000f1a0: 0d0a 0d0a 2020 2020 6465 6620 5f67 6574  ....    def _get
+0000f1b0: 5f78 6d6c 5f64 6174 6128 7365 6c66 293a  _xml_data(self):
+0000f1c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000f1d0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0000f1e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f1f0: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
+0000f200: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
 0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f230: 2073 706f 745f 7461 7267 6574 5f69 6420   spot_target_id 
-0000f240: 3d20 696e 7428 666c 6f61 7428 4564 6765  = int(float(Edge
-0000f250: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000f260: 7370 6f74 5f74 6172 6765 745f 6964 5f6b  spot_target_id_k
-0000f270: 6579 2929 2920 2020 2020 200d 0a20 2020  ey)))      ..   
-0000f280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2a0: 2020 2020 2069 6620 7370 6f74 5f73 6f75       if spot_sou
-0000f2b0: 7263 655f 6964 206e 6f74 2069 6e20 7365  rce_id not in se
-0000f2c0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-0000f2d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000f2e0: 732e 6b65 7973 2829 2061 6e64 2073 706f  s.keys() and spo
-0000f2f0: 745f 7461 7267 6574 5f69 6420 6e6f 7420  t_target_id not 
-0000f300: 696e 2073 656c 662e 6368 616e 6e65 6c5f  in self.channel_
-0000f310: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000f320: 6572 7469 6573 2e6b 6579 7328 293a 2020  erties.keys():  
-0000f330: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f370: 2073 6563 6f6e 6463 6869 6c64 2e72 656d   secondchild.rem
-0000f380: 6f76 6528 4564 6765 6f62 6a65 6374 2920  ove(Edgeobject) 
-0000f390: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0000f3a0: 2020 2020 2020 2020 2066 6f72 2070 6172           for par
-0000f3b0: 656e 7420 696e 2073 656c 662e 786d 6c5f  ent in self.xml_
-0000f3c0: 726f 6f74 2e66 696e 6461 6c6c 2827 4d6f  root.findall('Mo
-0000f3d0: 6465 6c27 293a 0d0a 2020 2020 2020 2020  del'):..        
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3f0: 666f 7220 6669 7273 7463 6869 6c64 2069  for firstchild i
-0000f400: 6e20 7061 7265 6e74 2e66 696e 6461 6c6c  n parent.findall
-0000f410: 2827 4669 6c74 6572 6564 5472 6163 6b73  ('FilteredTracks
-0000f420: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f440: 2066 6f72 2073 6563 6f6e 6463 6869 6c64   for secondchild
-0000f450: 2069 6e20 6669 7273 7463 6869 6c64 2e66   in firstchild.f
-0000f460: 696e 6461 6c6c 2827 5472 6163 6b49 4427  indall('TrackID'
-0000f470: 293a 200d 0a20 2020 2020 2020 2020 2020  ): ..           
-0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f490: 2020 2020 2020 2020 2066 696c 7465 725f           filter_
-0000f4a0: 7472 6163 6b5f 6964 203d 2069 6e74 2873  track_id = int(s
-0000f4b0: 6563 6f6e 6463 6869 6c64 2e67 6574 2873  econdchild.get(s
-0000f4c0: 656c 662e 7472 6163 6b69 645f 6b65 7929  elf.trackid_key)
-0000f4d0: 2920 200d 0a20 2020 2020 2020 2020 2020  )  ..           
-0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4f0: 2020 2020 2020 2020 2069 6620 6669 6c74           if filt
-0000f500: 6572 5f74 7261 636b 5f69 6420 6e6f 7420  er_track_id not 
-0000f510: 696e 2063 6861 6e6e 656c 5f66 696c 7465  in channel_filte
-0000f520: 7265 645f 7472 6163 6b73 3a0d 0a20 2020  red_tracks:..   
-0000f530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f550: 2020 2020 2020 2020 2066 6972 7374 6368           firstch
-0000f560: 696c 642e 7265 6d6f 7665 2873 6563 6f6e  ild.remove(secon
-0000f570: 6463 6869 6c64 2920 2020 2020 2020 2020  dchild)         
-0000f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f590: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000f5a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f5b0: 2e78 6d6c 5f74 7265 652e 7772 6974 6528  .xml_tree.write(
-0000f5c0: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-0000f5d0: 662e 6368 616e 6e65 6c5f 786d 6c5f 7061  f.channel_xml_pa
-0000f5e0: 7468 2c20 7365 6c66 2e63 6861 6e6e 656c  th, self.channel
-0000f5f0: 5f78 6d6c 5f6e 616d 6529 2920 0d0a 0d0a  _xml_name)) ....
-0000f600: 2020 2020 6465 6620 5f67 6574 5f78 6d6c      def _get_xml
-0000f610: 5f64 6174 6128 7365 6c66 293a 0d0a 0d0a  _data(self):....
-0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f630: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000f640: 2020 2020 6966 2073 656c 662e 6368 616e      if self.chan
-0000f650: 6e65 6c5f 7365 675f 696d 6167 6520 6973  nel_seg_image is
-0000f660: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f680: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
-0000f690: 6d6c 5f63 6f6e 7465 6e74 203d 2073 656c  ml_content = sel
-0000f6a0: 662e 786d 6c5f 636f 6e74 656e 740d 0a20  f.xml_content.. 
-0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 2020 2020 2073 656c 662e 786d 6c5f 7472       self.xml_tr
-0000f6d0: 6565 203d 2065 742e 7061 7273 6528 7365  ee = et.parse(se
-0000f6e0: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 2020 2020 7365 6c66 2e78 6d6c 5f72 6f6f      self.xml_roo
-0000f710: 7420 3d20 7365 6c66 2e78 6d6c 5f74 7265  t = self.xml_tre
-0000f720: 652e 6765 7472 6f6f 7428 290d 0a20 2020  e.getroot()..   
-0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f740: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
-0000f750: 786d 6c5f 6e61 6d65 203d 2027 7365 636f  xml_name = 'seco
-0000f760: 6e64 5f63 6861 6e6e 656c 5f27 202b 206f  nd_channel_' + o
-0000f770: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
-0000f780: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
-0000f790: 2873 656c 662e 786d 6c5f 7061 7468 2929  (self.xml_path))
-0000f7a0: 5b30 5d20 2b20 272e 786d 6c27 0d0a 2020  [0] + '.xml'..  
-0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7c0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-0000f7d0: 5f78 6d6c 5f70 6174 6820 3d20 6f73 2e70  _xml_path = os.p
-0000f7e0: 6174 682e 6469 726e 616d 6528 7365 6c66  ath.dirname(self
-0000f7f0: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
-0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f810: 2020 7365 6c66 2e5f 6372 6561 7465 5f63    self._create_c
-0000f820: 6861 6e6e 656c 5f74 7265 6528 290d 0a20  hannel_tree().. 
-0000f830: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f840: 6620 7365 6c66 2e63 6c75 7374 6572 5f6d  f self.cluster_m
-0000f850: 6f64 656c 2069 7320 6e6f 7420 4e6f 6e65  odel is not None
-0000f860: 2061 6e64 2073 656c 662e 7365 675f 696d   and self.seg_im
-0000f870: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-0000f880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f890: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000f8a0: 7374 6572 5f78 6d6c 5f63 6f6e 7465 6e74  ster_xml_content
-0000f8b0: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000f8c0: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
-0000f8d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f8e0: 2e6d 6173 7465 725f 786d 6c5f 7472 6565  .master_xml_tree
-0000f8f0: 203d 2065 742e 7061 7273 6528 7365 6c66   = et.parse(self
-0000f900: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
-0000f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f920: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
-0000f930: 6d6c 5f72 6f6f 7420 3d20 7365 6c66 2e6d  ml_root = self.m
-0000f940: 6173 7465 725f 786d 6c5f 7472 6565 2e67  aster_xml_tree.g
-0000f950: 6574 726f 6f74 2829 0d0a 2020 2020 2020  etroot()..      
-0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f970: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
-0000f980: 5f6e 616d 6520 3d20 276d 6173 7465 725f  _name = 'master_
-0000f990: 2720 2b20 7365 6c66 2e6d 6173 7465 725f  ' + self.master_
-0000f9a0: 6578 7472 615f 6e61 6d65 2020 2b20 6f73  extra_name  + os
-0000f9b0: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
-0000f9c0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0000f9d0: 7365 6c66 2e78 6d6c 5f70 6174 6829 295b  self.xml_path))[
-0000f9e0: 305d 202b 2027 2e78 6d6c 270d 0a20 2020  0] + '.xml'..   
-0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa00: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
-0000fa10: 786d 6c5f 7061 7468 203d 206f 732e 7061  xml_path = os.pa
-0000fa20: 7468 2e64 6972 6e61 6d65 2873 656c 662e  th.dirname(self.
-0000fa30: 786d 6c5f 7061 7468 2920 2020 2020 200d  xml_path)      .
-0000fa40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fa50: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000fa60: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000fa70: 6e69 7175 655f 6f62 6a65 6374 7320 3d20  nique_objects = 
-0000fa80: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-0000fa90: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-0000faa0: 7072 6f70 6572 7469 6573 203d 207b 7d0d  properties = {}.
-0000fab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fac0: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-0000fad0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000fae0: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
-0000faf0: 6964 696e 6754 7261 636b 4964 7320 3d20  idingTrackIds = 
-0000fb00: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000fb10: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
-0000fb20: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
-0000fb30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fb40: 6c66 2e61 6c6c 5f74 7261 636b 5f70 726f  lf.all_track_pro
-0000fb50: 7065 7274 6965 7320 3d20 5b5d 0d0a 2020  perties = []..  
-0000fb60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fb70: 6c66 2e73 706c 6974 5f70 6f69 6e74 735f  lf.split_points_
-0000fb80: 7469 6d65 7320 3d20 5b5d 0d0a 0d0a 2020  times = []....  
-0000fb90: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fbc0: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
-0000fbd0: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
-0000fbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fbf0: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-0000fc00: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000fc10: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000fc20: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
-0000fc30: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000fc40: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000fc50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000fc60: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
-0000fc70: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-0000fc80: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
-0000fc90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fca0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000fcb0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000fcc0: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
-0000fcd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fce0: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
-0000fcf0: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
-0000fd00: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
-0000fd10: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000fd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd30: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000fd40: 2020 2073 656c 662e 5370 6f74 6f62 6a65     self.Spotobje
-0000fd50: 6374 7320 3d20 7365 6c66 2e78 6d6c 5f63  cts = self.xml_c
-0000fd60: 6f6e 7465 6e74 2e66 696e 6428 274d 6f64  ontent.find('Mod
-0000fd70: 656c 2729 2e66 696e 6428 2741 6c6c 5370  el').find('AllSp
-0000fd80: 6f74 7327 290d 0a20 2020 2020 2020 2020  ots')..         
-0000fd90: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
-0000fda0: 2074 6865 2074 7261 636b 7320 6672 6f6d   the tracks from
-0000fdb0: 2078 6d6c 0d0a 2020 2020 2020 2020 2020   xml..          
-0000fdc0: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-0000fdd0: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000fde0: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
-0000fdf0: 2229 2e66 696e 6428 2241 6c6c 5472 6163  ").find("AllTrac
-0000fe00: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-0000fe10: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000fe20: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
-0000fe30: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
-0000fe40: 7469 6e67 7322 292e 6669 6e64 2822 496d  tings").find("Im
-0000fe50: 6167 6544 6174 6122 290d 0a20 2020 2020  ageData")..     
-0000fe60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fe70: 7863 616c 6962 7261 7469 6f6e 203d 2066  xcalibration = f
-0000fe80: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000fe90: 6773 2e67 6574 2822 7069 7865 6c77 6964  gs.get("pixelwid
-0000fea0: 7468 2229 290d 0a20 2020 2020 2020 2020  th"))..         
-0000feb0: 2020 2020 2020 2073 656c 662e 7963 616c         self.ycal
-0000fec0: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
-0000fed0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
-0000fee0: 6574 2822 7069 7865 6c68 6569 6768 7422  et("pixelheight"
-0000fef0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000ff00: 2020 2020 7365 6c66 2e7a 6361 6c69 6272      self.zcalibr
-0000ff10: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
-0000ff20: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000ff30: 2276 6f78 656c 6465 7074 6822 2929 0d0a  "voxeldepth"))..
-0000ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff50: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
-0000ff60: 6e20 3d20 696e 7428 666c 6f61 7428 7365  n = int(float(se
-0000ff70: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000ff80: 2274 696d 6569 6e74 6572 7661 6c22 2929  "timeinterval"))
-0000ff90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ffa0: 2020 2073 656c 662e 6465 7465 6374 6f72     self.detector
-0000ffb0: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
-0000ffc0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
-0000ffd0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
-0000ffe0: 6428 2244 6574 6563 746f 7253 6574 7469  d("DetectorSetti
-0000fff0: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
-00010000: 2020 2020 2020 2073 656c 662e 6261 7369         self.basi
-00010010: 6373 6574 7469 6e67 7320 3d20 7365 6c66  csettings = self
-00010020: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-00010030: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
-00010040: 6e64 2822 4261 7369 6353 6574 7469 6e67  nd("BasicSetting
-00010050: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-00010060: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
-00010070: 6f72 6368 616e 6e65 6c20 3d20 696e 7428  orchannel = int(
-00010080: 666c 6f61 7428 7365 6c66 2e64 6574 6563  float(self.detec
-00010090: 746f 7273 6574 7469 6e67 732e 6765 7428  torsettings.get(
-000100a0: 2254 4152 4745 545f 4348 414e 4e45 4c22  "TARGET_CHANNEL"
-000100b0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-000100c0: 2020 2020 2073 656c 662e 7473 7461 7274       self.tstart
-000100d0: 203d 2069 6e74 2866 6c6f 6174 2873 656c   = int(float(sel
-000100e0: 662e 6261 7369 6373 6574 7469 6e67 732e  f.basicsettings.
-000100f0: 6765 7428 2274 7374 6172 7422 2929 290d  get("tstart"))).
-00010100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010110: 2073 656c 662e 7465 6e64 203d 2069 6e74   self.tend = int
-00010120: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
-00010130: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
-00010140: 656e 6422 2929 290d 0a20 2020 2020 2020  end")))..       
-00010150: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
-00010160: 6574 5f62 6f75 6e64 6172 795f 706f 696e  et_boundary_poin
-00010170: 7473 2829 0d0a 2020 2020 2020 2020 2020  ts()..          
-00010180: 2020 2020 2020 7072 696e 7428 2749 7465        print('Ite
-00010190: 7261 7469 6e67 206f 7665 7220 7370 6f74  rating over spot
-000101a0: 7320 696e 2066 7261 6d65 2729 0d0a 2020  s in frame')..  
-000101b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000101c0: 6c66 2e63 6f75 6e74 203d 2030 0d0a 2020  lf.count = 0..  
-000101d0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-000101e0: 7475 7265 7320 3d20 5b5d 0d0a 0d0a 2020  tures = []....  
-000101f0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00010200: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
-00010210: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
-00010220: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
-00010230: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
-00010240: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
-00010250: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00010260: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00010270: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00010280: 6f72 2066 7261 6d65 2069 6e20 7365 6c66  or frame in self
-00010290: 2e53 706f 746f 626a 6563 7473 2e66 696e  .Spotobjects.fin
-000102a0: 6461 6c6c 2827 5370 6f74 7349 6e46 7261  dall('SpotsInFra
-000102b0: 6d65 2729 3a0d 0a20 2020 2020 2020 2020  me'):..         
-000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102d0: 2020 2020 6675 7475 7265 732e 6170 7065      futures.appe
-000102e0: 6e64 2865 7865 6375 746f 722e 7375 626d  nd(executor.subm
-000102f0: 6974 2873 656c 662e 5f73 706f 745f 636f  it(self._spot_co
-00010300: 6d70 7574 6572 2c20 6672 616d 6529 290d  mputer, frame)).
-00010310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010320: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-00010330: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-00010340: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010360: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000f220: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
+0000f230: 656c 5f78 6d6c 5f63 6f6e 7465 6e74 203d  el_xml_content =
+0000f240: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
+0000f250: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+0000f260: 2020 2020 2020 2020 2073 656c 662e 786d           self.xm
+0000f270: 6c5f 7472 6565 203d 2065 742e 7061 7273  l_tree = et.pars
+0000f280: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
+0000f290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f2a0: 2020 2020 2020 2020 7365 6c66 2e78 6d6c          self.xml
+0000f2b0: 5f72 6f6f 7420 3d20 7365 6c66 2e78 6d6c  _root = self.xml
+0000f2c0: 5f74 7265 652e 6765 7472 6f6f 7428 290d  _tree.getroot().
+0000f2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f2e0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+0000f2f0: 6e65 6c5f 786d 6c5f 6e61 6d65 203d 2027  nel_xml_name = '
+0000f300: 7365 636f 6e64 5f63 6861 6e6e 656c 5f27  second_channel_'
+0000f310: 202b 206f 732e 7061 7468 2e73 706c 6974   + os.path.split
+0000f320: 6578 7428 6f73 2e70 6174 682e 6261 7365  ext(os.path.base
+0000f330: 6e61 6d65 2873 656c 662e 786d 6c5f 7061  name(self.xml_pa
+0000f340: 7468 2929 5b30 5d20 2b20 272e 786d 6c27  th))[0] + '.xml'
+0000f350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f360: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+0000f370: 6e6e 656c 5f78 6d6c 5f70 6174 6820 3d20  nnel_xml_path = 
+0000f380: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+0000f390: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3b0: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
+0000f3c0: 7465 5f63 6861 6e6e 656c 5f74 7265 6528  te_channel_tree(
+0000f3d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f3e0: 2020 2069 6620 7365 6c66 2e63 6c75 7374     if self.clust
+0000f3f0: 6572 5f6d 6f64 656c 2069 7320 6e6f 7420  er_model is not 
+0000f400: 4e6f 6e65 2061 6e64 2073 656c 662e 7365  None and self.se
+0000f410: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+0000f420: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000f430: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f440: 662e 6d61 7374 6572 5f78 6d6c 5f63 6f6e  f.master_xml_con
+0000f450: 7465 6e74 203d 2073 656c 662e 786d 6c5f  tent = self.xml_
+0000f460: 636f 6e74 656e 740d 0a20 2020 2020 2020  content..       
+0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f480: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+0000f490: 7472 6565 203d 2065 742e 7061 7273 6528  tree = et.parse(
+0000f4a0: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
+0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4c0: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
+0000f4d0: 6572 5f78 6d6c 5f72 6f6f 7420 3d20 7365  er_xml_root = se
+0000f4e0: 6c66 2e6d 6173 7465 725f 786d 6c5f 7472  lf.master_xml_tr
+0000f4f0: 6565 2e67 6574 726f 6f74 2829 0d0a 2020  ee.getroot()..  
+0000f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f510: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+0000f520: 5f78 6d6c 5f6e 616d 6520 3d20 276d 6173  _xml_name = 'mas
+0000f530: 7465 725f 2720 2b20 7365 6c66 2e6d 6173  ter_' + self.mas
+0000f540: 7465 725f 6578 7472 615f 6e61 6d65 2020  ter_extra_name  
+0000f550: 2b20 6f73 2e70 6174 682e 7370 6c69 7465  + os.path.splite
+0000f560: 7874 286f 732e 7061 7468 2e62 6173 656e  xt(os.path.basen
+0000f570: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
+0000f580: 6829 295b 305d 202b 2027 2e78 6d6c 270d  h))[0] + '.xml'.
+0000f590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f5a0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+0000f5b0: 7465 725f 786d 6c5f 7061 7468 203d 206f  ter_xml_path = o
+0000f5c0: 732e 7061 7468 2e64 6972 6e61 6d65 2873  s.path.dirname(s
+0000f5d0: 656c 662e 786d 6c5f 7061 7468 2920 2020  elf.xml_path)   
+0000f5e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f5f0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000f600: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f610: 6c66 2e75 6e69 7175 655f 6f62 6a65 6374  lf.unique_object
+0000f620: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+0000f630: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+0000f640: 7175 655f 7072 6f70 6572 7469 6573 203d  que_properties =
+0000f650: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+0000f660: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+0000f670: 636b 4964 7320 3d20 5b5d 0d0a 2020 2020  ckIds = []..    
+0000f680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f690: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
+0000f6a0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000f6b0: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
+0000f6c0: 6d61 6c54 7261 636b 4964 7320 3d20 5b5d  malTrackIds = []
+0000f6d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f6e0: 2020 7365 6c66 2e61 6c6c 5f74 7261 636b    self.all_track
+0000f6f0: 5f70 726f 7065 7274 6965 7320 3d20 5b5d  _properties = []
+0000f700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f710: 2020 7365 6c66 2e73 706c 6974 5f70 6f69    self.split_poi
+0000f720: 6e74 735f 7469 6d65 7320 3d20 5b5d 0d0a  nts_times = []..
+0000f730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f740: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000f750: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000f760: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
+0000f770: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
+0000f780: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
+0000f790: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+0000f7a0: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+0000f7b0: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
+0000f7c0: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
+0000f7d0: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
+0000f7e0: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
+0000f7f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000f800: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f810: 662e 416c 6c54 7261 636b 4964 732e 6170  f.AllTrackIds.ap
+0000f820: 7065 6e64 2873 656c 662e 5472 6163 6b69  pend(self.Tracki
+0000f830: 6442 6f78 290d 0a20 2020 2020 2020 2020  dBox)..         
+0000f840: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
+0000f850: 6469 6e67 5472 6163 6b49 6473 2e61 7070  dingTrackIds.app
+0000f860: 656e 6428 7365 6c66 2e54 7261 636b 6964  end(self.Trackid
+0000f870: 426f 7829 0d0a 2020 2020 2020 2020 2020  Box)..          
+0000f880: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000f890: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000f8a0: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
+0000f8b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f8c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f8d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f8e0: 2020 2020 2020 2073 656c 662e 5370 6f74         self.Spot
+0000f8f0: 6f62 6a65 6374 7320 3d20 7365 6c66 2e78  objects = self.x
+0000f900: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
+0000f910: 274d 6f64 656c 2729 2e66 696e 6428 2741  'Model').find('A
+0000f920: 6c6c 5370 6f74 7327 290d 0a20 2020 2020  llSpots')..     
+0000f930: 2020 2020 2020 2020 2020 2023 2045 7874             # Ext
+0000f940: 7261 6374 2074 6865 2074 7261 636b 7320  ract the tracks 
+0000f950: 6672 6f6d 2078 6d6c 0d0a 2020 2020 2020  from xml..      
+0000f960: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000f970: 7261 636b 7320 3d20 7365 6c66 2e78 6d6c  racks = self.xml
+0000f980: 5f63 6f6e 7465 6e74 2e66 696e 6428 224d  _content.find("M
+0000f990: 6f64 656c 2229 2e66 696e 6428 2241 6c6c  odel").find("All
+0000f9a0: 5472 6163 6b73 2229 0d0a 2020 2020 2020  Tracks")..      
+0000f9b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000f9c0: 6574 7469 6e67 7320 3d20 7365 6c66 2e78  ettings = self.x
+0000f9d0: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
+0000f9e0: 2253 6574 7469 6e67 7322 292e 6669 6e64  "Settings").find
+0000f9f0: 2822 496d 6167 6544 6174 6122 290d 0a20  ("ImageData").. 
+0000fa00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fa10: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+0000fa20: 203d 2066 6c6f 6174 2873 656c 662e 7365   = float(self.se
+0000fa30: 7474 696e 6773 2e67 6574 2822 7069 7865  ttings.get("pixe
+0000fa40: 6c77 6964 7468 2229 290d 0a20 2020 2020  lwidth"))..     
+0000fa50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fa60: 7963 616c 6962 7261 7469 6f6e 203d 2066  ycalibration = f
+0000fa70: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+0000fa80: 6773 2e67 6574 2822 7069 7865 6c68 6569  gs.get("pixelhei
+0000fa90: 6768 7422 2929 0d0a 2020 2020 2020 2020  ght"))..        
+0000faa0: 2020 2020 2020 2020 7365 6c66 2e7a 6361          self.zca
+0000fab0: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
+0000fac0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000fad0: 6765 7428 2276 6f78 656c 6465 7074 6822  get("voxeldepth"
+0000fae0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000faf0: 2020 2020 7365 6c66 2e74 6361 6c69 6272      self.tcalibr
+0000fb00: 6174 696f 6e20 3d20 696e 7428 666c 6f61  ation = int(floa
+0000fb10: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000fb20: 6765 7428 2274 696d 6569 6e74 6572 7661  get("timeinterva
+0000fb30: 6c22 2929 290d 0a20 2020 2020 2020 2020  l")))..         
+0000fb40: 2020 2020 2020 2073 656c 662e 6465 7465         self.dete
+0000fb50: 6374 6f72 7365 7474 696e 6773 203d 2073  ctorsettings = s
+0000fb60: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000fb70: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
+0000fb80: 2e66 696e 6428 2244 6574 6563 746f 7253  .find("DetectorS
+0000fb90: 6574 7469 6e67 7322 290d 0a20 2020 2020  ettings")..     
+0000fba0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fbb0: 6261 7369 6373 6574 7469 6e67 7320 3d20  basicsettings = 
+0000fbc0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000fbd0: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000fbe0: 292e 6669 6e64 2822 4261 7369 6353 6574  ).find("BasicSet
+0000fbf0: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
+0000fc00: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+0000fc10: 7465 6374 6f72 6368 616e 6e65 6c20 3d20  tectorchannel = 
+0000fc20: 696e 7428 666c 6f61 7428 7365 6c66 2e64  int(float(self.d
+0000fc30: 6574 6563 746f 7273 6574 7469 6e67 732e  etectorsettings.
+0000fc40: 6765 7428 2254 4152 4745 545f 4348 414e  get("TARGET_CHAN
+0000fc50: 4e45 4c22 2929 290d 0a20 2020 2020 2020  NEL")))..       
+0000fc60: 2020 2020 2020 2020 2073 656c 662e 7473           self.ts
+0000fc70: 7461 7274 203d 2069 6e74 2866 6c6f 6174  tart = int(float
+0000fc80: 2873 656c 662e 6261 7369 6373 6574 7469  (self.basicsetti
+0000fc90: 6e67 732e 6765 7428 2274 7374 6172 7422  ngs.get("tstart"
+0000fca0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000fcb0: 2020 2020 2073 656c 662e 7465 6e64 203d       self.tend =
+0000fcc0: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
+0000fcd0: 6261 7369 6373 6574 7469 6e67 732e 6765  basicsettings.ge
+0000fce0: 7428 2274 656e 6422 2929 290d 0a20 2020  t("tend")))..   
+0000fcf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fd00: 662e 5f67 6574 5f62 6f75 6e64 6172 795f  f._get_boundary_
+0000fd10: 706f 696e 7473 2829 0d0a 2020 2020 2020  points()..      
+0000fd20: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000fd30: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
+0000fd40: 7370 6f74 7320 696e 2066 7261 6d65 2729  spots in frame')
+0000fd50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fd60: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
+0000fd70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fd80: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
+0000fd90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fda0: 2020 7769 7468 2063 6f6e 6375 7272 656e    with concurren
+0000fdb0: 742e 6675 7475 7265 732e 5468 7265 6164  t.futures.Thread
+0000fdc0: 506f 6f6c 4578 6563 7574 6f72 286d 6178  PoolExecutor(max
+0000fdd0: 5f77 6f72 6b65 7273 203d 206f 732e 6370  _workers = os.cp
+0000fde0: 755f 636f 756e 7428 2929 2061 7320 6578  u_count()) as ex
+0000fdf0: 6563 7574 6f72 3a0d 0a20 2020 2020 2020  ecutor:..       
+0000fe00: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe20: 2020 2066 6f72 2066 7261 6d65 2069 6e20     for frame in 
+0000fe30: 7365 6c66 2e53 706f 746f 626a 6563 7473  self.Spotobjects
+0000fe40: 2e66 696e 6461 6c6c 2827 5370 6f74 7349  .findall('SpotsI
+0000fe50: 6e46 7261 6d65 2729 3a0d 0a20 2020 2020  nFrame'):..     
+0000fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe70: 2020 2020 2020 2020 6675 7475 7265 732e          futures.
+0000fe80: 6170 7065 6e64 2865 7865 6375 746f 722e  append(executor.
+0000fe90: 7375 626d 6974 2873 656c 662e 5f73 706f  submit(self._spo
+0000fea0: 745f 636f 6d70 7574 6572 2c20 6672 616d  t_computer, fram
+0000feb0: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+0000fec0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000fed0: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
+0000fee0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff00: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff30: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000ff40: 5f62 6172 2e6c 6162 656c 203d 2022 436f  _bar.label = "Co
+0000ff50: 6c6c 6563 7469 6e67 2053 706f 7473 220d  llecting Spots".
+0000ff60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff80: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000ff90: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+0000ffa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffc0: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
+0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fff0: 2020 2020 2020 6c65 6e28 6675 7475 7265        len(future
+00010000: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
+00010010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010020: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010050: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00010060: 722e 7368 6f77 2829 0d0a 0d0a 2020 2020  r.show()....    
+00010070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010080: 666f 7220 7220 696e 2063 6f6e 6375 7272  for r in concurr
+00010090: 656e 742e 6675 7475 7265 732e 6173 5f63  ent.futures.as_c
+000100a0: 6f6d 706c 6574 6564 2866 7574 7572 6573  ompleted(futures
+000100b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000100c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100d0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+000100e0: 6e74 203d 2073 656c 662e 636f 756e 7420  nt = self.count 
+000100f0: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
+00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010110: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00010120: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
+00010130: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010160: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00010170: 6261 722e 7661 6c75 6520 3d20 2073 656c  bar.value =  sel
+00010180: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
+00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101a0: 2020 2020 2020 2020 2020 2020 2072 2e72               r.r
+000101b0: 6573 756c 7428 290d 0a0d 0a20 2020 2020  esult()....     
+000101c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000101d0: 2866 2749 7465 7261 7469 6e67 206f 7665  (f'Iterating ove
+000101e0: 7220 7472 6163 6b73 207b 6c65 6e28 7365  r tracks {len(se
+000101f0: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
+00010200: 6b5f 6964 7329 7d27 2920 200d 0a20 2020  k_ids)}')  ..   
+00010210: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010220: 662e 636f 756e 7420 3d20 300d 0a20 2020  f.count = 0..   
+00010230: 2020 2020 2020 2020 2020 2020 2066 7574               fut
+00010240: 7572 6573 203d 205b 5d0d 0a20 2020 2020  ures = []..     
+00010250: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00010260: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+00010270: 6573 2e54 6872 6561 6450 6f6f 6c45 7865  es.ThreadPoolExe
+00010280: 6375 746f 7228 6d61 785f 776f 726b 6572  cutor(max_worker
+00010290: 7320 3d20 6f73 2e63 7075 5f63 6f75 6e74  s = os.cpu_count
+000102a0: 2829 2920 6173 2065 7865 6375 746f 723a  ()) as executor:
+000102b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000102c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000102d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000102e0: 7472 6163 6b20 696e 2073 656c 662e 7472  track in self.tr
+000102f0: 6163 6b73 2e66 696e 6461 6c6c 2827 5472  acks.findall('Tr
+00010300: 6163 6b27 293a 0d0a 2020 2020 2020 2020  ack'):..        
+00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010320: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 2020 7472 6163 6b5f 6964 203d 2069 6e74    track_id = int
+00010350: 2874 7261 636b 2e67 6574 2873 656c 662e  (track.get(self.
+00010360: 7472 6163 6b69 645f 6b65 7929 290d 0a20  trackid_key)).. 
 00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010380: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010390: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-000103a0: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
-000103b0: 7469 6e67 2053 706f 7473 220d 0a20 2020  ting Spots"..   
+00010380: 2020 2020 2020 2020 2020 2069 6620 7472             if tr
+00010390: 6163 6b5f 6964 2069 6e20 7365 6c66 2e66  ack_id in self.f
+000103a0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+000103b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
 000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-000103f0: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
-00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010420: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
-00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2020 6c65 6e28 6675 7475 7265 7329 2c0d    len(futures),.
-00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000104b0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-000104c0: 6f77 2829 0d0a 0d0a 2020 2020 2020 2020  ow()....        
-000104d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000104e0: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
-000104f0: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
-00010500: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
+000103d0: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
+000103e0: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
+000103f0: 626d 6974 2873 656c 662e 5f74 7261 636b  bmit(self._track
+00010400: 5f63 6f6d 7075 7465 722c 2074 7261 636b  _computer, track
+00010410: 2c20 7472 6163 6b5f 6964 2929 0d0a 2020  , track_id))..  
+00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010430: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+00010440: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+00010450: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010470: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010490: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000104a0: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+000104b0: 6265 6c20 3d20 2243 6f6c 6c65 6374 696e  bel = "Collectin
+000104c0: 6720 5472 6163 6b73 220d 0a20 2020 2020  g Tracks"..     
+000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000104f0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00010500: 2e72 616e 6765 203d 2028 0d0a 2020 2020  .range = (..    
 00010510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010530: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-00010540: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
-00010550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010570: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-00010580: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-00010590: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000105c0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-000105d0: 7661 6c75 6520 3d20 2073 656c 662e 636f  value =  self.co
-000105e0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 2020 2020 2020 2020 2072 2e72 6573 756c           r.resul
-00010610: 7428 290d 0a0d 0a20 2020 2020 2020 2020  t()....         
-00010620: 2020 2020 2020 2070 7269 6e74 2866 2749         print(f'I
-00010630: 7465 7261 7469 6e67 206f 7665 7220 7472  terating over tr
-00010640: 6163 6b73 207b 6c65 6e28 7365 6c66 2e66  acks {len(self.f
-00010650: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-00010660: 7329 7d27 2920 200d 0a20 2020 2020 2020  s)}')  ..       
-00010670: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00010680: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-00010690: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-000106a0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000106b0: 2020 2020 2020 2077 6974 6820 636f 6e63         with conc
-000106c0: 7572 7265 6e74 2e66 7574 7572 6573 2e54  urrent.futures.T
-000106d0: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
-000106e0: 7228 6d61 785f 776f 726b 6572 7320 3d20  r(max_workers = 
-000106f0: 6f73 2e63 7075 5f63 6f75 6e74 2829 2920  os.cpu_count()) 
-00010700: 6173 2065 7865 6375 746f 723a 0d0a 2020  as executor:..  
+00010530: 2020 2020 302c 0d0a 2020 2020 2020 2020      0,..        
+00010540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010560: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
+00010570: 645f 7472 6163 6b5f 6964 7329 2c0d 0a20  d_track_ids),.. 
+00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105a0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105c0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+000105d0: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
+000105e0: 2829 0d0a 0d0a 0d0a 2020 2020 2020 2020  ()......        
+000105f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010600: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
+00010610: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
+00010620: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
+00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010650: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+00010660: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
+00010670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010690: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
+000106a0: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+000106b0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+000106c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000106e0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+000106f0: 2e76 616c 7565 203d 2073 656c 662e 636f  .value = self.co
+00010700: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
 00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010720: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00010730: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
-00010740: 6b20 696e 2073 656c 662e 7472 6163 6b73  k in self.tracks
-00010750: 2e66 696e 6461 6c6c 2827 5472 6163 6b27  .findall('Track'
-00010760: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00010720: 2020 2020 2020 2020 2072 2e72 6573 756c           r.resul
+00010730: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+00010740: 2020 2020 2069 6620 7365 6c66 2e63 6861       if self.cha
+00010750: 6e6e 656c 5f73 6567 5f69 6d61 6765 2069  nnel_seg_image i
+00010760: 7320 6e6f 7420 4e6f 6e65 3a20 200d 0a20  s not None:  .. 
 00010770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010790: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000107a0: 6163 6b5f 6964 203d 2069 6e74 2874 7261  ack_id = int(tra
-000107b0: 636b 2e67 6574 2873 656c 662e 7472 6163  ck.get(self.trac
-000107c0: 6b69 645f 6b65 7929 290d 0a20 2020 2020  kid_key))..     
-000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107e0: 2020 2020 2020 2069 6620 7472 6163 6b5f         if track_
-000107f0: 6964 2069 6e20 7365 6c66 2e66 696c 7465  id in self.filte
-00010800: 7265 645f 7472 6163 6b5f 6964 733a 0d0a  red_track_ids:..
-00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010830: 2020 6675 7475 7265 732e 6170 7065 6e64    futures.append
-00010840: 2865 7865 6375 746f 722e 7375 626d 6974  (executor.submit
-00010850: 2873 656c 662e 5f74 7261 636b 5f63 6f6d  (self._track_com
-00010860: 7075 7465 722c 2074 7261 636b 2c20 7472  puter, track, tr
-00010870: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
-00010880: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010890: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-000108a0: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
-000108b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00010900: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
-00010910: 3d20 2243 6f6c 6c65 6374 696e 6720 5472  = "Collecting Tr
-00010920: 6163 6b73 220d 0a20 2020 2020 2020 2020  acks"..         
-00010930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010950: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
-00010960: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
-00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109b0: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
-000109c0: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-000109d0: 6163 6b5f 6964 7329 2c0d 0a20 2020 2020  ack_ids),..     
-000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00010a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010780: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
+00010790: 7465 5f73 6563 6f6e 645f 6368 616e 6e65  te_second_channe
+000107a0: 6c5f 786d 6c28 290d 0a20 2020 2020 2020  l_xml()..       
+000107b0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+000107c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000107d0: 2028 6b2c 7629 2069 6e20 7365 6c66 2e67   (k,v) in self.g
+000107e0: 7261 7068 5f73 706c 6974 2e69 7465 6d73  raph_split.items
+000107f0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010820: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00010830: 7567 6874 6572 5f74 7261 636b 5f69 6420  ughter_track_id 
+00010840: 3d20 2069 6e74 2866 6c6f 6174 2873 7472  =  int(float(str
+00010850: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00010860: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00010870: 2866 6c6f 6174 286b 2929 5d5b 7365 6c66  (float(k))][self
+00010880: 2e75 6e69 7175 6569 645f 6b65 795d 2929  .uniqueid_key]))
+00010890: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000108a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000108b0: 6172 656e 745f 7472 6163 6b5f 6964 203d  arent_track_id =
+000108c0: 2069 6e74 2866 6c6f 6174 2873 7472 2873   int(float(str(s
+000108d0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000108e0: 7072 6f70 6572 7469 6573 5b69 6e74 2866  properties[int(f
+000108f0: 6c6f 6174 2876 2929 5d5b 7365 6c66 2e75  loat(v))][self.u
+00010900: 6e69 7175 6569 645f 6b65 795d 2929 290d  niqueid_key]))).
+00010910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010920: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010930: 662e 6772 6170 685f 7472 6163 6b73 5b64  f.graph_tracks[d
+00010940: 6175 6768 7465 725f 7472 6163 6b5f 6964  aughter_track_id
+00010950: 5d20 3d20 7061 7265 6e74 5f74 7261 636b  ] = parent_track
+00010960: 5f69 640d 0a20 2020 2020 2020 2020 2020  _id..           
+00010970: 2020 2020 2073 656c 662e 5f67 6574 5f61       self._get_a
+00010980: 7474 7269 6275 7465 7328 290d 0a20 2020  ttributes()..   
+00010990: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000109a0: 7365 6c66 2e63 6c75 7374 6572 5f6d 6f64  self.cluster_mod
+000109b0: 656c 2061 6e64 2073 656c 662e 7365 675f  el and self.seg_
+000109c0: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+000109d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000109e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000109f0: 5f61 7373 6967 6e5f 636c 7573 7465 725f  _assign_cluster_
+00010a00: 636c 6173 7328 290d 0a20 2020 2020 2020  class()..       
 00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a20: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-00010a30: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
-00010a40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00010a50: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
-00010a60: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-00010a70: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
-00010a80: 2866 7574 7572 6573 293a 0d0a 2020 2020  (futures):..    
-00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 7365 6c66 2e5f 6372 6561 7465 5f6d 6173  self._create_mas
+00010a30: 7465 725f 786d 6c28 290d 0a20 2020 2020  ter_xml()..     
+00010a40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010a50: 636f 756e 7420 3d20 3020 0d0a 2020 2020  count = 0 ..    
+00010a60: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010a70: 7472 6163 6b5f 6964 2069 6e20 7365 6c66  track_id in self
+00010a80: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+00010a90: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
 00010aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ab0: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
-00010ac0: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
-00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ab0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00010ac0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+00010ad0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
 00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010af0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-00010b00: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-00010b10: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010b40: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
-00010b50: 7565 203d 2073 656c 662e 636f 756e 740d  ue = self.count.
-00010b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 2020 2020 2072 2e72 6573 756c 7428 290d       r.result().
-00010b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ba0: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
-00010bb0: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
-00010bc0: 7420 4e6f 6e65 3a20 200d 0a20 2020 2020  t None:  ..     
-00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010be0: 2020 7365 6c66 2e5f 6372 6561 7465 5f73    self._create_s
-00010bf0: 6563 6f6e 645f 6368 616e 6e65 6c5f 786d  econd_channel_xm
-00010c00: 6c28 290d 0a20 2020 2020 2020 2020 2020  l()..           
-00010c10: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-00010c20: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-00010c30: 7629 2069 6e20 7365 6c66 2e67 7261 7068  v) in self.graph
-00010c40: 5f73 706c 6974 2e69 7465 6d73 2829 3a0d  _split.items():.
-00010c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010c60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b00: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00010b10: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
+00010b20: 4a75 7374 206f 6e65 206d 6f72 6520 7468  Just one more th
+00010b30: 696e 6722 0d0a 2020 2020 2020 2020 2020  ing"..          
+00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b50: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010b60: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00010b70: 7261 6e67 6520 3d20 280d 0a20 2020 2020  range = (..     
+00010b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ba0: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
+00010bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00010be0: 656e 2873 656c 662e 6669 6c74 6572 6564  en(self.filtered
+00010bf0: 5f74 7261 636b 5f69 6473 292c 0d0a 2020  _track_ids),..  
+00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c20: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c50: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00010c60: 7373 5f62 6172 2e73 686f 7728 290d 0a20  ss_bar.show().. 
 00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c80: 2020 2020 2020 2020 2020 6461 7567 6874            daught
-00010c90: 6572 5f74 7261 636b 5f69 6420 3d20 2069  er_track_id =  i
-00010ca0: 6e74 2866 6c6f 6174 2873 7472 2873 656c  nt(float(str(sel
-00010cb0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00010cc0: 6f70 6572 7469 6573 5b69 6e74 2866 6c6f  operties[int(flo
-00010cd0: 6174 286b 2929 5d5b 7365 6c66 2e75 6e69  at(k))][self.uni
-00010ce0: 7175 6569 645f 6b65 795d 2929 290d 0a20  queid_key]))).. 
-00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d00: 2020 2020 2020 2020 2020 2070 6172 656e             paren
-00010d10: 745f 7472 6163 6b5f 6964 203d 2069 6e74  t_track_id = int
-00010d20: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
-00010d30: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00010d40: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
-00010d50: 2876 2929 5d5b 7365 6c66 2e75 6e69 7175  (v))][self.uniqu
-00010d60: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
-00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d80: 2020 2020 2020 2020 2073 656c 662e 6772           self.gr
-00010d90: 6170 685f 7472 6163 6b73 5b64 6175 6768  aph_tracks[daugh
-00010da0: 7465 725f 7472 6163 6b5f 6964 5d20 3d20  ter_track_id] = 
-00010db0: 7061 7265 6e74 5f74 7261 636b 5f69 640d  parent_track_id.
-00010dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010dd0: 2073 656c 662e 5f67 6574 5f61 7474 7269   self._get_attri
-00010de0: 6275 7465 7328 290d 0a20 2020 2020 2020  butes()..       
-00010df0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00010e00: 2e63 6c75 7374 6572 5f6d 6f64 656c 2061  .cluster_model a
-00010e10: 6e64 2073 656c 662e 7365 675f 696d 6167  nd self.seg_imag
-00010e20: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
-00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e40: 2020 2020 2020 2073 656c 662e 5f61 7373         self._ass
-00010e50: 6967 6e5f 636c 7573 7465 725f 636c 6173  ign_cluster_clas
-00010e60: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
-00010e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010e80: 2e5f 6372 6561 7465 5f6d 6173 7465 725f  ._create_master_
-00010e90: 786d 6c28 290d 0a20 2020 2020 2020 2020  xml()..         
-00010ea0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
-00010eb0: 7420 3d20 3020 0d0a 2020 2020 2020 2020  t = 0 ..        
-00010ec0: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
-00010ed0: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
-00010ee0: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
-00010ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c90: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+00010ca0: 7420 3d20 7365 6c66 2e63 6f75 6e74 202b  t = self.count +
+00010cb0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010ce0: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
+00010cf0: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
+00010d00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d20: 2020 2020 2020 7365 6c66 2e5f 6669 6e61        self._fina
+00010d30: 6c5f 7472 6163 6b73 2874 7261 636b 5f69  l_tracks(track_i
+00010d40: 6429 200d 0a0d 0a20 2020 2020 2020 2020  d) ....         
+00010d50: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+00010d60: 6f75 7269 6572 3a0d 0a20 2020 2020 2020  ourier:..       
+00010d70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00010d80: 7428 2763 6f6d 7075 7469 6e67 2046 6f75  t('computing Fou
+00010d90: 7269 6572 2729 0d0a 2020 2020 2020 2020  rier')..        
+00010da0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010db0: 5f63 6f6d 7075 7465 5f70 6865 6e6f 7479  _compute_phenoty
+00010dc0: 7065 7328 2920 2020 2020 2020 2020 2020  pes()           
+00010dd0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00010de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010df0: 656c 662e 5f74 656d 706f 7261 6c5f 706c  elf._temporal_pl
+00010e00: 6f74 735f 7472 6163 6b6d 6174 6528 290d  ots_trackmate().
+00010e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e20: 200d 0a0d 0a20 2020 2064 6566 205f 6372   ....    def _cr
+00010e30: 6561 7465 5f6d 6173 7465 725f 786d 6c28  eate_master_xml(
+00010e40: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00010e50: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+00010e60: 2020 2020 2020 2020 2020 666f 7220 5370            for Sp
+00010e70: 6f74 6f62 6a65 6374 2069 6e20 7365 6c66  otobject in self
+00010e80: 2e6d 6173 7465 725f 786d 6c5f 726f 6f74  .master_xml_root
+00010e90: 2e69 7465 7228 2753 706f 7427 293a 0d0a  .iter('Spot'):..
+00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ec0: 6365 6c6c 5f69 6420 3d20 696e 7428 5370  cell_id = int(Sp
+00010ed0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+00010ee0: 662e 7370 6f74 6964 5f6b 6579 2929 0d0a  f.spotid_key))..
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f10: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00010f20: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
-00010f30: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f10: 6966 2063 656c 6c5f 6964 2069 6e20 7365  if cell_id in se
+00010f20: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00010f30: 726f 7065 7274 6965 732e 6b65 7973 2829  roperties.keys()
+00010f40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f60: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00010f70: 6172 2e6c 6162 656c 203d 2022 4a75 7374  ar.label = "Just
-00010f80: 206f 6e65 206d 6f72 6520 7468 696e 6722   one more thing"
-00010f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fb0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010fc0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
-00010fd0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+00010f60: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f90: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
+00010fa0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00010fb0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00010fc0: 2e6b 6579 7328 293a 0d0a 0d0a 2020 2020  .keys():....    
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
-00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
-00011040: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
-00011050: 636b 5f69 6473 292c 0d0a 2020 2020 2020  ck_ids),..      
-00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-000110c0: 6172 2e73 686f 7728 290d 0a20 2020 2020  ar.show()..     
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ff0: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
+00011000: 742e 7365 7428 6b2c 2073 7472 2873 656c  t.set(k, str(sel
+00011010: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00011020: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+00011030: 5d5b 6b5d 2929 2020 200d 0a0d 0a20 2020  ][k]))   ....   
+00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011060: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00011070: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
+00011080: 6c5f 7472 6565 2e77 7269 7465 286f 732e  l_tree.write(os.
+00011090: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e6d  path.join(self.m
+000110a0: 6173 7465 725f 786d 6c5f 7061 7468 2c20  aster_xml_path, 
+000110b0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+000110c0: 6e61 6d65 2929 0d0a 2020 2020 2020 2020  name))..        
+000110d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-00011100: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
+000110f0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00011140: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
-00011150: 3d20 7365 6c66 2e63 6f75 6e74 0d0a 2020  = self.count..  
+00011120: 2020 2020 200d 0a0d 0a20 2020 2064 6566       ....    def
+00011130: 205f 6173 7369 676e 5f63 6c75 7374 6572   _assign_cluster
+00011140: 5f63 6c61 7373 2873 656c 6629 3a0d 0a20  _class(self):.. 
+00011150: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 7365 6c66 2e5f 6669 6e61 6c5f 7472    self._final_tr
-00011190: 6163 6b73 2874 7261 636b 5f69 6429 200d  acks(track_id) .
-000111a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000111b0: 2020 2069 6620 7365 6c66 2e66 6f75 7269     if self.fouri
-000111c0: 6572 3a0d 0a20 2020 2020 2020 2020 2020  er:..           
-000111d0: 2020 2020 2020 2020 7072 696e 7428 2763          print('c
-000111e0: 6f6d 7075 7469 6e67 2046 6f75 7269 6572  omputing Fourier
-000111f0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00011200: 2020 2020 2020 2073 656c 662e 5f63 6f6d         self._com
-00011210: 7075 7465 5f70 6865 6e6f 7479 7065 7328  pute_phenotypes(
-00011220: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-00011230: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00011240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011250: 5f74 656d 706f 7261 6c5f 706c 6f74 735f  _temporal_plots_
-00011260: 7472 6163 6b6d 6174 6528 290d 0a20 2020  trackmate()..   
-00011270: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00011280: 0a20 2020 2064 6566 205f 6372 6561 7465  .    def _create
-00011290: 5f6d 6173 7465 725f 786d 6c28 7365 6c66  _master_xml(self
-000112a0: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
-000112b0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000112c0: 2020 2020 2020 666f 7220 5370 6f74 6f62        for Spotob
-000112d0: 6a65 6374 2069 6e20 7365 6c66 2e6d 6173  ject in self.mas
-000112e0: 7465 725f 786d 6c5f 726f 6f74 2e69 7465  ter_xml_root.ite
-000112f0: 7228 2753 706f 7427 293a 0d0a 2020 2020  r('Spot'):..    
-00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011310: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00011320: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
-00011330: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
-00011340: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
+00011170: 7365 6c66 2e61 7865 7320 3d20 7365 6c66  self.axes = self
+00011180: 2e61 7865 732e 7265 706c 6163 6528 2254  .axes.replace("T
+00011190: 222c 2022 2229 0d0a 2020 2020 2020 2020  ", "")..        
+000111a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111c0: 2020 666f 7220 636f 756e 742c 2074 696d    for count, tim
+000111d0: 655f 6b65 7920 696e 2065 6e75 6d65 7261  e_key in enumera
+000111e0: 7465 2873 656c 662e 5f74 696d 6564 5f63  te(self._timed_c
+000111f0: 656e 7472 6f69 642e 6b65 7973 2829 293a  entroid.keys()):
+00011200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011210: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011230: 2020 2020 2020 2020 2020 7472 6565 2c20            tree, 
+00011240: 7370 6f74 5f63 656e 7472 6f69 6473 203d  spot_centroids =
+00011250: 2073 656c 662e 5f74 696d 6564 5f63 656e   self._timed_cen
+00011260: 7472 6f69 645b 7469 6d65 5f6b 6579 5d0d  troid[time_key].
+00011270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011280: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00011290: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+000112a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000112d0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+000112e0: 2e6c 6162 656c 203d 2022 436f 6d70 7574  .label = "Comput
+000112f0: 696e 6720 636c 7573 7465 7269 6e67 2063  ing clustering c
+00011300: 6c61 7373 6573 220d 0a20 2020 2020 2020  lasses"..       
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00011330: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
+00011340: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
 00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00011370: 656c 6c5f 6964 2069 6e20 7365 6c66 2e75  ell_id in self.u
-00011380: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00011390: 7274 6965 732e 6b65 7973 2829 3a0d 0a20  rties.keys():.. 
+00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011380: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
+00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000113f0: 6f72 206b 2069 6e20 7365 6c66 2e75 6e69  or k in self.uni
-00011400: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00011410: 6965 735b 6365 6c6c 5f69 645d 2e6b 6579  ies[cell_id].key
-00011420: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+000113c0: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
+000113d0: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
+000113e0: 6964 2e6b 6579 7328 2929 202b 2031 2c0d  id.keys()) + 1,.
+000113f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011420: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
 00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011450: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
-00011460: 7428 6b2c 2073 7472 2873 656c 662e 756e  t(k, str(self.un
-00011470: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011480: 7469 6573 5b63 656c 6c5f 6964 5d5b 6b5d  ties[cell_id][k]
-00011490: 2929 2020 200d 0a0d 0a20 2020 2020 2020  ))   ....       
-000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000114c0: 0a0d 0a20 2020 2020 2020 2020 2020 7365  ...           se
-000114d0: 6c66 2e6d 6173 7465 725f 786d 6c5f 7472  lf.master_xml_tr
-000114e0: 6565 2e77 7269 7465 286f 732e 7061 7468  ee.write(os.path
-000114f0: 2e6a 6f69 6e28 7365 6c66 2e6d 6173 7465  .join(self.maste
-00011500: 725f 786d 6c5f 7061 7468 2c20 7365 6c66  r_xml_path, self
-00011510: 2e6d 6173 7465 725f 786d 6c5f 6e61 6d65  .master_xml_name
-00011520: 2929 0d0a 2020 2020 2020 2020 2020 200d  ))..           .
-00011530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011580: 200d 0a0d 0a20 2020 2064 6566 205f 6173   ....    def _as
-00011590: 7369 676e 5f63 6c75 7374 6572 5f63 6c61  sign_cluster_cla
-000115a0: 7373 2873 656c 6629 3a0d 0a20 2020 2020  ss(self):..     
-000115b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000115c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000115d0: 2e61 7865 7320 3d20 7365 6c66 2e61 7865  .axes = self.axe
-000115e0: 732e 7265 706c 6163 6528 2254 222c 2022  s.replace("T", "
-000115f0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00011600: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00011610: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00011620: 7220 636f 756e 742c 2074 696d 655f 6b65  r count, time_ke
-00011630: 7920 696e 2065 6e75 6d65 7261 7465 2873  y in enumerate(s
-00011640: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
-00011650: 6f69 642e 6b65 7973 2829 293a 0d0a 2020  oid.keys()):..  
-00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011670: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011690: 2020 2020 2020 7472 6565 2c20 7370 6f74        tree, spot
-000116a0: 5f63 656e 7472 6f69 6473 203d 2073 656c  _centroids = sel
-000116b0: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
-000116c0: 645b 7469 6d65 5f6b 6579 5d0d 0a20 2020  d[time_key]..   
-000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000116f0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
-00011700: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011720: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011730: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
-00011740: 656c 203d 2022 436f 6d70 7574 696e 6720  el = "Computing 
-00011750: 636c 7573 7465 7269 6e67 2063 6c61 7373  clustering class
-00011760: 6573 220d 0a20 2020 2020 2020 2020 2020  es"..           
+00011450: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00011460: 722e 7661 6c75 6520 3d20 2063 6f75 6e74  r.value =  count
+00011470: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+000114a0: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114c0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
+000114d0: 725f 6576 616c 203d 2043 6c75 7374 6572  r_eval = Cluster
+000114e0: 696e 6728 7365 6c66 2e73 6567 5f69 6d61  ing(self.seg_ima
+000114f0: 6765 5b69 6e74 2874 696d 655f 6b65 7929  ge[int(time_key)
+00011500: 2c3a 5d2c 2020 7365 6c66 2e61 7865 732c  ,:],  self.axes,
+00011510: 2073 656c 662e 6e75 6d5f 706f 696e 7473   self.num_points
+00011520: 2c20 7365 6c66 2e63 6c75 7374 6572 5f6d  , self.cluster_m
+00011530: 6f64 656c 2c20 6b65 7920 3d20 7469 6d65  odel, key = time
+00011540: 5f6b 6579 2c20 7072 6f67 7265 7373 5f62  _key, progress_b
+00011550: 6172 3d73 656c 662e 7072 6f67 7265 7373  ar=self.progress
+00011560: 5f62 6172 2c20 6261 7463 685f 7369 7a65  _bar, batch_size
+00011570: 203d 2073 656c 662e 6261 7463 685f 7369   = self.batch_si
+00011580: 7a65 2920 2020 2020 2020 0d0a 2020 2020  ze)       ..    
+00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115a0: 2020 2020 2020 2063 6c75 7374 6572 5f65         cluster_e
+000115b0: 7661 6c2e 5f63 7265 6174 655f 636c 7573  val._create_clus
+000115c0: 7465 725f 6c61 6265 6c73 2829 0d0a 2020  ter_labels()..  
+000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115e0: 2020 2020 2020 2020 2074 696d 6564 5f63           timed_c
+000115f0: 6c75 7374 6572 5f6c 6162 656c 203d 2063  luster_label = c
+00011600: 6c75 7374 6572 5f65 7661 6c2e 7469 6d65  luster_eval.time
+00011610: 645f 636c 7573 7465 725f 6c61 6265 6c20  d_cluster_label 
+00011620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011630: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00011640: 7075 745f 6c61 6265 6c73 2c20 6f75 7470  put_labels, outp
+00011650: 7574 5f63 6c75 7374 6572 5f73 636f 7265  ut_cluster_score
+00011660: 2c20 6f75 7470 7574 5f63 6c75 7374 6572  , output_cluster
+00011670: 5f63 6c61 7373 2c20 6f75 7470 7574 5f63  _class, output_c
+00011680: 6c75 7374 6572 5f63 656e 7472 6f69 642c  luster_centroid,
+00011690: 206f 7574 7075 745f 636c 6f75 645f 6563   output_cloud_ec
+000116a0: 6365 6e74 7269 6369 7479 2c20 6f75 7470  centricity, outp
+000116b0: 7574 5f6c 6172 6765 7374 5f65 6967 656e  ut_largest_eigen
+000116c0: 7665 6374 6f72 2c20 6f75 7470 7574 5f63  vector, output_c
+000116d0: 6c6f 7564 5f73 7572 6661 6365 5f61 7265  loud_surface_are
+000116e0: 6120 3d20 7469 6d65 645f 636c 7573 7465  a = timed_cluste
+000116f0: 725f 6c61 6265 6c5b 7469 6d65 5f6b 6579  r_label[time_key
+00011700: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00011710: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011730: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00011740: 2069 6e20 7261 6e67 6528 6c65 6e28 6f75   in range(len(ou
+00011750: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
+00011760: 7472 6f69 6429 293a 0d0a 2020 2020 2020  troid)):..      
 00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-00011790: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-000117a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011780: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00011790: 6e74 726f 6964 203d 206f 7574 7075 745f  ntroid = output_
+000117a0: 636c 7573 7465 725f 6365 6e74 726f 6964  cluster_centroid
+000117b0: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
 000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117e0: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117d0: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
+000117e0: 5f63 6c61 7373 203d 206f 7574 7075 745f  _class = output_
+000117f0: 636c 7573 7465 725f 636c 6173 735b 695d  cluster_class[i]
+00011800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011820: 2020 2020 2020 6c65 6e28 7365 6c66 2e5f        len(self._
-00011830: 7469 6d65 645f 6365 6e74 726f 6964 2e6b  timed_centroid.k
-00011840: 6579 7328 2929 202b 2031 2c0d 0a20 2020  eys()) + 1,..   
+00011820: 2020 2020 2020 636c 7573 7465 725f 7363        cluster_sc
+00011830: 6f72 6520 3d20 6f75 7470 7574 5f63 6c75  ore = output_clu
+00011840: 7374 6572 5f73 636f 7265 5b69 5d0d 0a20  ster_score[i].. 
 00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011880: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000118b0: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
-000118c0: 6c75 6520 3d20 2063 6f75 6e74 200d 0a20  lue =  count .. 
-000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000118f0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00011900: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
+00011870: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
+00011880: 636f 6d70 5f66 6972 7374 797a 203d 206f  comp_firstyz = o
+00011890: 7574 7075 745f 636c 6f75 645f 6563 6365  utput_cloud_ecce
+000118a0: 6e74 7269 6369 7479 5b69 5d0d 0a20 2020  ntricity[i]..   
+000118b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118d0: 2063 656c 6c5f 6178 6973 203d 206f 7574   cell_axis = out
+000118e0: 7075 745f 6c61 7267 6573 745f 6569 6765  put_largest_eige
+000118f0: 6e76 6563 746f 725b 695d 0d0a 2020 2020  nvector[i]..    
+00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011920: 2020 2020 2020 636c 7573 7465 725f 6576        cluster_ev
-00011930: 616c 203d 2043 6c75 7374 6572 696e 6728  al = Clustering(
-00011940: 7365 6c66 2e73 6567 5f69 6d61 6765 5b69  self.seg_image[i
-00011950: 6e74 2874 696d 655f 6b65 7929 2c3a 5d2c  nt(time_key),:],
-00011960: 2020 7365 6c66 2e61 7865 732c 2073 656c    self.axes, sel
-00011970: 662e 6e75 6d5f 706f 696e 7473 2c20 7365  f.num_points, se
-00011980: 6c66 2e63 6c75 7374 6572 5f6d 6f64 656c  lf.cluster_model
-00011990: 2c20 6b65 7920 3d20 7469 6d65 5f6b 6579  , key = time_key
-000119a0: 2c20 7072 6f67 7265 7373 5f62 6172 3d73  , progress_bar=s
-000119b0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-000119c0: 2c20 6261 7463 685f 7369 7a65 203d 2073  , batch_size = s
-000119d0: 656c 662e 6261 7463 685f 7369 7a65 2920  elf.batch_size) 
-000119e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00011920: 7375 7266 6163 655f 6172 6561 203d 206f  surface_area = o
+00011930: 7574 7075 745f 636c 6f75 645f 7375 7266  utput_cloud_surf
+00011940: 6163 655f 6172 6561 5b69 5d0d 0a20 2020  ace_area[i]..   
+00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011970: 2064 6973 742c 2069 6e64 6578 203d 2074   dist, index = t
+00011980: 7265 652e 7175 6572 7928 6365 6e74 726f  ree.query(centro
+00011990: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
+000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119b0: 2020 2020 2020 2020 2063 6c6f 7365 7374           closest
+000119c0: 5f63 656e 7472 6f69 6420 3d20 7370 6f74  _centroid = spot
+000119d0: 5f63 656e 7472 6f69 6473 5b69 6e64 6578  _centroids[index
+000119e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
 000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a00: 2020 2063 6c75 7374 6572 5f65 7661 6c2e     cluster_eval.
-00011a10: 5f63 7265 6174 655f 636c 7573 7465 725f  _create_cluster_
-00011a20: 6c61 6265 6c73 2829 0d0a 2020 2020 2020  labels()..      
-00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a40: 2020 2020 2074 696d 6564 5f63 6c75 7374       timed_clust
-00011a50: 6572 5f6c 6162 656c 203d 2063 6c75 7374  er_label = clust
-00011a60: 6572 5f65 7661 6c2e 7469 6d65 645f 636c  er_eval.timed_cl
-00011a70: 7573 7465 725f 6c61 6265 6c20 0d0a 2020  uster_label ..  
+00011a00: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
+00011a10: 745f 6365 6e74 726f 6964 203d 2028 696e  t_centroid = (in
+00011a20: 7428 7469 6d65 5f6b 6579 292c 636c 6f73  t(time_key),clos
+00011a30: 6573 745f 6365 6e74 726f 6964 5b30 5d2c  est_centroid[0],
+00011a40: 2063 6c6f 7365 7374 5f63 656e 7472 6f69   closest_centroi
+00011a50: 645b 315d 2c20 636c 6f73 6573 745f 6365  d[1], closest_ce
+00011a60: 6e74 726f 6964 5b32 5d29 0d0a 2020 2020  ntroid[2])..    
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a90: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-00011aa0: 6c61 6265 6c73 2c20 6f75 7470 7574 5f63  labels, output_c
-00011ab0: 6c75 7374 6572 5f73 636f 7265 2c20 6f75  luster_score, ou
-00011ac0: 7470 7574 5f63 6c75 7374 6572 5f63 6c61  tput_cluster_cla
-00011ad0: 7373 2c20 6f75 7470 7574 5f63 6c75 7374  ss, output_clust
-00011ae0: 6572 5f63 656e 7472 6f69 642c 206f 7574  er_centroid, out
-00011af0: 7075 745f 636c 6f75 645f 6563 6365 6e74  put_cloud_eccent
-00011b00: 7269 6369 7479 2c20 6f75 7470 7574 5f6c  ricity, output_l
-00011b10: 6172 6765 7374 5f65 6967 656e 7665 6374  argest_eigenvect
-00011b20: 6f72 2c20 6f75 7470 7574 5f63 6c6f 7564  or, output_cloud
-00011b30: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
-00011b40: 7469 6d65 645f 636c 7573 7465 725f 6c61  timed_cluster_la
-00011b50: 6265 6c5b 7469 6d65 5f6b 6579 5d0d 0a20  bel[time_key].. 
-00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b70: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00011ba0: 7261 6e67 6528 6c65 6e28 6f75 7470 7574  range(len(output
-00011bb0: 5f63 6c75 7374 6572 5f63 656e 7472 6f69  _cluster_centroi
-00011bc0: 6429 293a 0d0a 2020 2020 2020 2020 2020  d)):..          
-00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011be0: 2020 2020 2020 2020 2020 6365 6e74 726f            centro
-00011bf0: 6964 203d 206f 7574 7075 745f 636c 7573  id = output_clus
-00011c00: 7465 725f 6365 6e74 726f 6964 5b69 5d0d  ter_centroid[i].
-00011c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c30: 2020 2020 2063 6c75 7374 6572 5f63 6c61       cluster_cla
-00011c40: 7373 203d 206f 7574 7075 745f 636c 7573  ss = output_clus
-00011c50: 7465 725f 636c 6173 735b 695d 0d0a 2020  ter_class[i]..  
+00011a90: 636c 6f73 6573 745f 6365 6c6c 5f69 6420  closest_cell_id 
+00011aa0: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+00011ab0: 6f74 5f63 656e 7472 6f69 645b 6672 616d  ot_centroid[fram
+00011ac0: 655f 7370 6f74 5f63 656e 7472 6f69 645d  e_spot_centroid]
+00011ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2020 2020 2020 6d61 736b 5f76 6563 746f        mask_vecto
+00011b00: 7220 3d20 5b20 666c 6f61 7428 7365 6c66  r = [ float(self
+00011b10: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00011b20: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00011b30: 6573 745f 6365 6c6c 5f69 6429 5d5b 7365  est_cell_id)][se
+00011b40: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+00011b50: 785f 6b65 795d 292c 2066 6c6f 6174 2873  x_key]), float(s
+00011b60: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00011b70: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00011b80: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00011b90: 5b73 656c 662e 6d61 736b 6365 6e74 726f  [self.maskcentro
+00011ba0: 6964 5f79 5f6b 6579 5d29 2c20 666c 6f61  id_y_key]), floa
+00011bb0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00011bc0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00011bd0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00011be0: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+00011bf0: 7472 6f69 645f 7a5f 6b65 795d 2920 5d0d  troid_z_key]) ].
+00011c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 2020 2020 2063 656c 6c5f 6178 6973 5f6d       cell_axis_m
+00011c30: 6173 6b20 3d20 616e 6775 6c61 725f 6368  ask = angular_ch
+00011c40: 616e 6765 2863 656c 6c5f 6178 6973 2c20  ange(cell_axis, 
+00011c50: 6d61 736b 5f76 6563 746f 7229 0d0a 2020  mask_vector)..  
 00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c80: 2020 636c 7573 7465 725f 7363 6f72 6520    cluster_score 
-00011c90: 3d20 6f75 7470 7574 5f63 6c75 7374 6572  = output_cluster
-00011ca0: 5f73 636f 7265 5b69 5d0d 0a20 2020 2020  _score[i]..     
-00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cc0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00011cd0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00011ce0: 5f66 6972 7374 797a 203d 206f 7574 7075  _firstyz = outpu
-00011cf0: 745f 636c 6f75 645f 6563 6365 6e74 7269  t_cloud_eccentri
-00011d00: 6369 7479 5b69 5d0d 0a20 2020 2020 2020  city[i]..       
+00011c80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ca0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00011cb0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011cc0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00011cd0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00011ce0: 287b 7365 6c66 2e63 656c 6c61 7869 735f  ({self.cellaxis_
+00011cf0: 6d61 736b 5f6b 6579 203a 2063 656c 6c5f  mask_key : cell_
+00011d00: 6178 6973 5f6d 6173 6b7d 290d 0a20 2020  axis_mask})..   
 00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d20: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00011d30: 6c5f 6178 6973 203d 206f 7574 7075 745f  l_axis = output_
-00011d40: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
-00011d50: 746f 725b 695d 0d0a 2020 2020 2020 2020  tor[i]..        
-00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d70: 2020 2020 2020 2020 2020 2020 7375 7266              surf
-00011d80: 6163 655f 6172 6561 203d 206f 7574 7075  ace_area = outpu
-00011d90: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
-00011da0: 6172 6561 5b69 5d0d 0a20 2020 2020 2020  area[i]..       
-00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dc0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00011dd0: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
-00011de0: 7175 6572 7928 6365 6e74 726f 6964 290d  query(centroid).
-00011df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 2020 2020 2063 6c6f 7365 7374 5f63 656e       closest_cen
-00011e20: 7472 6f69 6420 3d20 7370 6f74 5f63 656e  troid = spot_cen
-00011e30: 7472 6f69 6473 5b69 6e64 6578 5d0d 0a20  troids[index].. 
-00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2020 2066 7261 6d65 5f73 706f 745f 6365     frame_spot_ce
-00011e70: 6e74 726f 6964 203d 2028 696e 7428 7469  ntroid = (int(ti
-00011e80: 6d65 5f6b 6579 292c 636c 6f73 6573 745f  me_key),closest_
-00011e90: 6365 6e74 726f 6964 5b30 5d2c 2063 6c6f  centroid[0], clo
-00011ea0: 7365 7374 5f63 656e 7472 6f69 645b 315d  sest_centroid[1]
-00011eb0: 2c20 636c 6f73 6573 745f 6365 6e74 726f  , closest_centro
-00011ec0: 6964 5b32 5d29 0d0a 2020 2020 2020 2020  id[2])..        
-00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ee0: 2020 2020 2020 2020 2020 2020 636c 6f73              clos
-00011ef0: 6573 745f 6365 6c6c 5f69 6420 3d20 7365  est_cell_id = se
-00011f00: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
-00011f10: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
-00011f20: 6f74 5f63 656e 7472 6f69 645d 0d0a 2020  ot_centroid]..  
-00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f50: 2020 6d61 736b 5f76 6563 746f 7220 3d20    mask_vector = 
-00011f60: 5b20 666c 6f61 7428 7365 6c66 2e75 6e69  [ float(self.uni
-00011f70: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00011f80: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00011f90: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
-00011fa0: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
-00011fb0: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
-00011fc0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00011fd0: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00011fe0: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
-00011ff0: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
-00012000: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
-00012010: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00012020: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00012030: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
-00012040: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-00012050: 645f 7a5f 6b65 795d 2920 5d0d 0a20 2020  d_z_key]) ]..   
-00012060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012080: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
-00012090: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
-000120a0: 2863 656c 6c5f 6178 6973 2c20 6d61 736b  (cell_axis, mask
-000120b0: 5f76 6563 746f 7229 0d0a 2020 2020 2020  _vector)..      
-000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012100: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00012110: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00012120: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00012130: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00012140: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
-00012150: 5f6b 6579 203a 2063 656c 6c5f 6178 6973  _key : cell_axis
-00012160: 5f6d 6173 6b7d 290d 0a20 2020 2020 2020  _mask})..       
-00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012180: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012190: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000121a0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-000121b0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-000121c0: 7064 6174 6528 7b73 656c 662e 636c 7573  pdate({self.clus
-000121d0: 7465 7263 6c61 7373 5f6b 6579 203a 2063  terclass_key : c
-000121e0: 6c75 7374 6572 5f63 6c61 7373 7d29 0d0a  luster_class})..
-000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012210: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00012220: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00012230: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00012240: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00012250: 6c66 2e63 6c75 7374 6572 7363 6f72 655f  lf.clusterscore_
-00012260: 6b65 7920 3a20 636c 7573 7465 725f 7363  key : cluster_sc
-00012270: 6f72 657d 290d 0a20 2020 2020 2020 2020  ore})..         
-00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000122a0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000122b0: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-000122c0: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
-000122d0: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
-000122e0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-000122f0: 746b 6579 203a 2065 6363 656e 7472 6963  tkey : eccentric
-00012300: 6974 795f 636f 6d70 5f66 6972 7374 797a  ity_comp_firstyz
-00012310: 5b30 5d7d 290d 0a20 2020 2020 2020 2020  [0]})..         
-00012320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012340: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00012350: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00012360: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
-00012370: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
-00012380: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00012390: 6e64 6b65 7920 3a20 6563 6365 6e74 7269  ndkey : eccentri
-000123a0: 6369 7479 5f63 6f6d 705f 6669 7273 7479  city_comp_firsty
-000123b0: 7a5b 315d 7d29 0d0a 2020 2020 2020 2020  z[1]})..        
-000123c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000123e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000123f0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-00012400: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
-00012410: 6461 7465 287b 7365 6c66 2e73 7572 6661  date({self.surfa
-00012420: 6365 5f61 7265 615f 6b65 7920 3a20 7375  ce_area_key : su
-00012430: 7266 6163 655f 6172 6561 7d29 0d0a 0d0a  rface_area})....
-00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012460: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00012470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012480: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-00012490: 6c66 2e72 6f6f 745f 7370 6f74 732e 6974  lf.root_spots.it
-000124a0: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000124d0: 6f6f 745f 7370 6f74 735b 6b5d 203d 2073  oot_spots[k] = s
-000124e0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000124f0: 7072 6f70 6572 7469 6573 5b6b 5d20 2020  properties[k]   
-00012500: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00012510: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00012520: 6620 5f63 6f6d 7075 7465 5f70 6865 6e6f  f _compute_pheno
-00012530: 7479 7065 7328 7365 6c66 293a 0d0a 0d0a  types(self):....
-00012540: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
-00012550: 2c76 2920 696e 2073 656c 662e 756e 6971  ,v) in self.uniq
-00012560: 7565 5f74 7261 636b 732e 6974 656d 7328  ue_tracks.items(
-00012570: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00012580: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00012590: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
-000125a0: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
-000125b0: 2020 2020 7472 6163 6b6c 6574 5f70 726f      tracklet_pro
-000125c0: 7065 7274 6965 7320 3d20 7365 6c66 2e75  perties = self.u
-000125d0: 6e69 7175 655f 7472 6163 6b5f 7072 6f70  nique_track_prop
-000125e0: 6572 7469 6573 5b6b 5d0d 0a20 2020 2020  erties[k]..     
-000125f0: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00012600: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
-00012610: 7472 6163 6b73 5b6b 5d0d 0a20 2020 2020  tracks[k]..     
-00012620: 2020 2020 2020 2020 2020 205a 203d 2074             Z = t
-00012630: 7261 636b 735b 3a2c 325d 0d0a 2020 2020  racks[:,2]..    
-00012640: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
-00012650: 7472 6163 6b73 5b3a 2c33 5d0d 0a20 2020  tracks[:,3]..   
-00012660: 2020 2020 2020 2020 2020 2020 2058 203d               X =
-00012670: 2074 7261 636b 735b 3a2c 345d 0d0a 2020   tracks[:,4]..  
-00012680: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00012690: 6d65 203d 2074 7261 636b 6c65 745f 7072  me = tracklet_pr
-000126a0: 6f70 6572 7469 6573 5b3a 2c30 5d0d 0a20  operties[:,0].. 
-000126b0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-000126c0: 6e69 7175 655f 6964 7320 3d20 7472 6163  nique_ids = trac
-000126d0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-000126e0: 3a2c 315d 0d0a 2020 2020 2020 2020 2020  :,1]..          
-000126f0: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
-00012700: 5f73 6574 203d 2073 6574 2875 6e69 7175  _set = set(uniqu
-00012710: 655f 6964 7329 0d0a 2020 2020 2020 2020  e_ids)..        
-00012720: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
-00012730: 6f6e 5f69 6473 203d 2074 7261 636b 6c65  on_ids = trackle
-00012740: 745f 7072 6f70 6572 7469 6573 5b3a 2c32  t_properties[:,2
-00012750: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012760: 2020 2072 6164 6975 7320 3d20 7472 6163     radius = trac
-00012770: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00012780: 3a2c 335d 0d0a 2020 2020 2020 2020 2020  :,3]..          
-00012790: 2020 2020 2020 766f 6c75 6d65 203d 2074        volume = t
-000127a0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-000127b0: 6573 5b3a 2c34 5d0d 0a20 2020 2020 2020  es[:,4]..       
-000127c0: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-000127d0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-000127e0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-000127f0: 6572 7469 6573 5b3a 2c35 5d0d 0a20 2020  erties[:,5]..   
-00012800: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
-00012810: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00012820: 6563 6f6e 6420 3d20 7472 6163 6b6c 6574  econd = tracklet
-00012830: 5f70 726f 7065 7274 6965 735b 3a2c 365d  _properties[:,6]
-00012840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012850: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
-00012860: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00012870: 7469 6573 5b3a 2c37 5d0d 0a20 2020 2020  ties[:,7]..     
-00012880: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
-00012890: 6572 5f63 6c61 7373 203d 2074 7261 636b  er_class = track
-000128a0: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-000128b0: 2c38 5d0d 0a20 2020 2020 2020 2020 2020  ,8]..           
-000128c0: 2020 2020 2063 6c75 7374 6572 5f63 6c61       cluster_cla
-000128d0: 7373 5f73 636f 7265 203d 2074 7261 636b  ss_score = track
-000128e0: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-000128f0: 2c39 5d0d 0a20 2020 2020 2020 2020 2020  ,9]..           
-00012900: 2020 2020 2069 6e74 656e 7369 7479 203d       intensity =
-00012910: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00012920: 7469 6573 5b3a 2c31 305d 0d0a 2020 2020  ties[:,10]..    
-00012930: 2020 2020 2020 2020 2020 2020 7370 6565              spee
-00012940: 6420 3d20 7472 6163 6b6c 6574 5f70 726f  d = tracklet_pro
-00012950: 7065 7274 6965 735b 3a2c 3131 5d0d 0a20  perties[:,11].. 
-00012960: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00012970: 6f74 696f 6e5f 616e 676c 6520 3d20 7472  otion_angle = tr
-00012980: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00012990: 735b 3a2c 3132 5d0d 0a20 2020 2020 2020  s[:,12]..       
-000129a0: 2020 2020 2020 2020 2061 6363 656c 6572           acceler
-000129b0: 6174 696f 6e20 3d20 7472 6163 6b6c 6574  ation = tracklet
-000129c0: 5f70 726f 7065 7274 6965 735b 3a2c 3133  _properties[:,13
-000129d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000129e0: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
-000129f0: 5f6d 6173 6b20 3d20 7472 6163 6b6c 6574  _mask = tracklet
-00012a00: 5f70 726f 7065 7274 6965 735b 3a2c 3134  _properties[:,14
-00012a10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012a20: 2020 2072 6164 6961 6c5f 616e 676c 6520     radial_angle 
-00012a30: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012a40: 7274 6965 735b 3a2c 3135 5d0d 0a20 2020  rties[:,15]..   
-00012a50: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00012a60: 6c5f 6178 6973 5f6d 6173 6b20 3d20 7472  l_axis_mask = tr
-00012a70: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00012a80: 735b 3a2c 3136 5d0d 0a0d 0a0d 0a20 2020  s[:,16]......   
-00012a90: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00012aa0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00012ab0: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
-00012ac0: 7469 6573 5f74 7261 636b 6c65 7420 3d20  ties_tracklet = 
-00012ad0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00012ae0: 2020 2020 756e 6971 7565 5f63 6c75 7374      unique_clust
-00012af0: 6572 5f70 726f 7065 7274 6965 735f 7472  er_properties_tr
-00012b00: 6163 6b6c 6574 203d 207b 7d0d 0a20 2020  acklet = {}..   
-00012b10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012b20: 662e 756e 6971 7565 5f66 6674 5f70 726f  f.unique_fft_pro
-00012b30: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
-00012b40: 5d20 3d20 7b7d 0d0a 2020 2020 2020 2020  ] = {}..        
-00012b50: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00012b60: 7175 655f 636c 7573 7465 725f 7072 6f70  que_cluster_prop
-00012b70: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00012b80: 203d 207b 7d0d 0a0d 0a20 2020 2020 2020   = {}....       
-00012b90: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-00012ba0: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
-00012bb0: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
-00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bd0: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
-00012be0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00012bf0: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
-00012c00: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00012c10: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
-00012c20: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
-00012c30: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00012c40: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00012c50: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
-00012c60: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
-00012c70: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00012c80: 2020 2020 2065 7870 616e 6465 645f 7469       expanded_ti
-00012c90: 6d65 203d 206e 702e 7a65 726f 7328 7365  me = np.zeros(se
-00012ca0: 6c66 2e74 656e 6420 2d20 7365 6c66 2e74  lf.tend - self.t
-00012cb0: 7374 6172 7420 2b20 3129 0d0a 2020 2020  start + 1)..    
-00012cc0: 2020 2020 2020 2020 2020 2020 706f 696e              poin
-00012cd0: 745f 7361 6d70 6c65 203d 2065 7870 616e  t_sample = expan
-00012ce0: 6465 645f 7469 6d65 2e73 6861 7065 5b30  ded_time.shape[0
-00012cf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012d00: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00012d10: 6528 6c65 6e28 6578 7061 6e64 6564 5f74  e(len(expanded_t
-00012d20: 696d 6529 293a 0d0a 2020 2020 2020 2020  ime)):..        
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00012d40: 7870 616e 6465 645f 7469 6d65 5b69 5d20  xpanded_time[i] 
-00012d50: 3d20 6920 0d0a 2020 2020 2020 2020 2020  = i ..          
-00012d60: 2020 2020 2020 666f 7220 6375 7272 656e        for curren
-00012d70: 745f 756e 6971 7565 5f69 6420 696e 2075  t_unique_id in u
-00012d80: 6e69 7175 655f 6964 735f 7365 743a 0d0a  nique_ids_set:..
-00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00012db0: 2020 2020 2020 2020 6578 7061 6e64 6564          expanded
-00012dc0: 5f69 6e74 656e 7369 7479 203d 206e 702e  _intensity = np.
-00012dd0: 7a65 726f 7328 7365 6c66 2e74 656e 6420  zeros(self.tend 
-00012de0: 2d20 7365 6c66 2e74 7374 6172 7420 2b20  - self.tstart + 
-00012df0: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
-00012e00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00012e10: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 2063 7572 7265 6e74 5f74 696d 6520 3d20   current_time = 
-00012e40: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012e50: 2020 2020 2020 2063 7572 7265 6e74 5f7a         current_z
-00012e60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012e70: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012e80: 745f 7920 3d20 5b5d 0d0a 2020 2020 2020  t_y = []..      
-00012e90: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012ea0: 7265 6e74 5f78 203d 205b 5d0d 0a20 2020  rent_x = []..   
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00011d40: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00011d50: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00011d60: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00011d70: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+00011d80: 203a 2063 6c75 7374 6572 5f63 6c61 7373   : cluster_class
+00011d90: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011db0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00011dc0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011dd0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00011de0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00011df0: 287b 7365 6c66 2e63 6c75 7374 6572 7363  ({self.clustersc
+00011e00: 6f72 655f 6b65 7920 3a20 636c 7573 7465  ore_key : cluste
+00011e10: 725f 7363 6f72 657d 290d 0a20 2020 2020  r_score})..     
+00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011e40: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00011e50: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00011e60: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00011e70: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
+00011e80: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00011e90: 6669 7273 746b 6579 203a 2065 6363 656e  firstkey : eccen
+00011ea0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00011eb0: 7374 797a 5b30 5d7d 290d 0a20 2020 2020  styz[0]})..     
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011ee0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00011ef0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00011f00: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00011f10: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
+00011f20: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00011f30: 7365 636f 6e64 6b65 7920 3a20 6563 6365  secondkey : ecce
+00011f40: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00011f50: 7273 7479 7a5b 315d 7d29 0d0a 2020 2020  rstyz[1]})..    
+00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f80: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00011f90: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00011fa0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00011fb0: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
+00011fc0: 7572 6661 6365 5f61 7265 615f 6b65 7920  urface_area_key 
+00011fd0: 3a20 7375 7266 6163 655f 6172 6561 7d29  : surface_area})
+00011fe0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012000: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012020: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
+00012030: 6e20 7365 6c66 2e72 6f6f 745f 7370 6f74  n self.root_spot
+00012040: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012060: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012070: 6c66 2e72 6f6f 745f 7370 6f74 735b 6b5d  lf.root_spots[k]
+00012080: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+00012090: 706f 745f 7072 6f70 6572 7469 6573 5b6b  pot_properties[k
+000120a0: 5d20 2020 2020 2020 2020 0d0a 2020 2020  ]         ..    
+000120b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000120c0: 2020 6465 6620 5f63 6f6d 7075 7465 5f70    def _compute_p
+000120d0: 6865 6e6f 7479 7065 7328 7365 6c66 293a  henotypes(self):
+000120e0: 0d0a 0d0a 2020 2020 2020 2020 2020 666f  ....          fo
+000120f0: 7220 286b 2c76 2920 696e 2073 656c 662e  r (k,v) in self.
+00012100: 756e 6971 7565 5f74 7261 636b 732e 6974  unique_tracks.it
+00012110: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
+00012120: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00012130: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
+00012140: 6964 203d 206b 0d0a 2020 2020 2020 2020  id = k..        
+00012150: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
+00012160: 5f70 726f 7065 7274 6965 7320 3d20 7365  _properties = se
+00012170: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
+00012180: 7072 6f70 6572 7469 6573 5b6b 5d0d 0a20  properties[k].. 
+00012190: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000121a0: 7261 636b 7320 3d20 7365 6c66 2e75 6e69  racks = self.uni
+000121b0: 7175 655f 7472 6163 6b73 5b6b 5d0d 0a20  que_tracks[k].. 
+000121c0: 2020 2020 2020 2020 2020 2020 2020 205a                 Z
+000121d0: 203d 2074 7261 636b 735b 3a2c 325d 0d0a   = tracks[:,2]..
+000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121f0: 5920 3d20 7472 6163 6b73 5b3a 2c33 5d0d  Y = tracks[:,3].
+00012200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012210: 2058 203d 2074 7261 636b 735b 3a2c 345d   X = tracks[:,4]
+00012220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012230: 2020 7469 6d65 203d 2074 7261 636b 6c65    time = trackle
+00012240: 745f 7072 6f70 6572 7469 6573 5b3a 2c30  t_properties[:,0
+00012250: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012260: 2020 2075 6e69 7175 655f 6964 7320 3d20     unique_ids = 
+00012270: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00012280: 6965 735b 3a2c 315d 0d0a 2020 2020 2020  ies[:,1]..      
+00012290: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+000122a0: 5f69 6473 5f73 6574 203d 2073 6574 2875  _ids_set = set(u
+000122b0: 6e69 7175 655f 6964 7329 0d0a 2020 2020  nique_ids)..    
+000122c0: 2020 2020 2020 2020 2020 2020 6765 6e65              gene
+000122d0: 7261 7469 6f6e 5f69 6473 203d 2074 7261  ration_ids = tra
+000122e0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+000122f0: 5b3a 2c32 5d0d 0a20 2020 2020 2020 2020  [:,2]..         
+00012300: 2020 2020 2020 2072 6164 6975 7320 3d20         radius = 
+00012310: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00012320: 6965 735b 3a2c 335d 0d0a 2020 2020 2020  ies[:,3]..      
+00012330: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
+00012340: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00012350: 6572 7469 6573 5b3a 2c34 5d0d 0a20 2020  erties[:,4]..   
+00012360: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+00012370: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00012380: 6972 7374 203d 2074 7261 636b 6c65 745f  irst = tracklet_
+00012390: 7072 6f70 6572 7469 6573 5b3a 2c35 5d0d  properties[:,5].
+000123a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000123b0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+000123c0: 6d70 5f73 6563 6f6e 6420 3d20 7472 6163  mp_second = trac
+000123d0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+000123e0: 3a2c 365d 0d0a 2020 2020 2020 2020 2020  :,6]..          
+000123f0: 2020 2020 2020 7375 7266 6163 655f 6172        surface_ar
+00012400: 6561 203d 2074 7261 636b 6c65 745f 7072  ea = tracklet_pr
+00012410: 6f70 6572 7469 6573 5b3a 2c37 5d0d 0a20  operties[:,7].. 
+00012420: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012430: 6c75 7374 6572 5f63 6c61 7373 203d 2074  luster_class = t
+00012440: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012450: 6573 5b3a 2c38 5d0d 0a20 2020 2020 2020  es[:,8]..       
+00012460: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
+00012470: 5f63 6c61 7373 5f73 636f 7265 203d 2074  _class_score = t
+00012480: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012490: 6573 5b3a 2c39 5d0d 0a20 2020 2020 2020  es[:,9]..       
+000124a0: 2020 2020 2020 2020 2069 6e74 656e 7369           intensi
+000124b0: 7479 203d 2074 7261 636b 6c65 745f 7072  ty = tracklet_pr
+000124c0: 6f70 6572 7469 6573 5b3a 2c31 305d 0d0a  operties[:,10]..
+000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124e0: 7370 6565 6420 3d20 7472 6163 6b6c 6574  speed = tracklet
+000124f0: 5f70 726f 7065 7274 6965 735b 3a2c 3131  _properties[:,11
+00012500: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012510: 2020 206d 6f74 696f 6e5f 616e 676c 6520     motion_angle 
+00012520: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00012530: 7274 6965 735b 3a2c 3132 5d0d 0a20 2020  rties[:,12]..   
+00012540: 2020 2020 2020 2020 2020 2020 2061 6363               acc
+00012550: 656c 6572 6174 696f 6e20 3d20 7472 6163  eleration = trac
+00012560: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012570: 3a2c 3133 5d0d 0a20 2020 2020 2020 2020  :,13]..         
+00012580: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
+00012590: 6365 6c6c 5f6d 6173 6b20 3d20 7472 6163  cell_mask = trac
+000125a0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+000125b0: 3a2c 3134 5d0d 0a20 2020 2020 2020 2020  :,14]..         
+000125c0: 2020 2020 2020 2072 6164 6961 6c5f 616e         radial_an
+000125d0: 676c 6520 3d20 7472 6163 6b6c 6574 5f70  gle = tracklet_p
+000125e0: 726f 7065 7274 6965 735b 3a2c 3135 5d0d  roperties[:,15].
+000125f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012600: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
+00012610: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00012620: 7274 6965 735b 3a2c 3136 5d0d 0a0d 0a0d  rties[:,16].....
+00012630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012640: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012650: 2020 2075 6e69 7175 655f 6666 745f 7072     unique_fft_pr
+00012660: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00012670: 7420 3d20 7b7d 0d0a 2020 2020 2020 2020  t = {}..        
+00012680: 2020 2020 2020 2020 756e 6971 7565 5f63          unique_c
+00012690: 6c75 7374 6572 5f70 726f 7065 7274 6965  luster_propertie
+000126a0: 735f 7472 6163 6b6c 6574 203d 207b 7d0d  s_tracklet = {}.
+000126b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000126c0: 2073 656c 662e 756e 6971 7565 5f66 6674   self.unique_fft
+000126d0: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
+000126e0: 6b5f 6964 5d20 3d20 7b7d 0d0a 2020 2020  k_id] = {}..    
+000126f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012700: 2e75 6e69 7175 655f 636c 7573 7465 725f  .unique_cluster_
+00012710: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
+00012720: 5f69 645d 203d 207b 7d0d 0a0d 0a20 2020  _id] = {}....   
+00012730: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00012740: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
+00012750: 7469 6573 5f74 7261 636b 6c65 7420 3d20  ties_tracklet = 
+00012760: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+00012770: 2020 2020 756e 6971 7565 5f64 796e 616d      unique_dynam
+00012780: 6963 5f70 726f 7065 7274 6965 735f 7472  ic_properties_tr
+00012790: 6163 6b6c 6574 203d 207b 7d0d 0a20 2020  acklet = {}..   
+000127a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000127b0: 662e 756e 6971 7565 5f73 6861 7065 5f70  f.unique_shape_p
+000127c0: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
+000127d0: 6964 5d20 3d20 7b7d 0d0a 2020 2020 2020  id] = {}..      
+000127e0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+000127f0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
+00012800: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
+00012810: 645d 203d 207b 7d0d 0a20 2020 2020 2020  d] = {}..       
+00012820: 2020 2020 2020 2020 2065 7870 616e 6465           expande
+00012830: 645f 7469 6d65 203d 206e 702e 7a65 726f  d_time = np.zero
+00012840: 7328 7365 6c66 2e74 656e 6420 2d20 7365  s(self.tend - se
+00012850: 6c66 2e74 7374 6172 7420 2b20 3129 0d0a  lf.tstart + 1)..
+00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012870: 706f 696e 745f 7361 6d70 6c65 203d 2065  point_sample = e
+00012880: 7870 616e 6465 645f 7469 6d65 2e73 6861  xpanded_time.sha
+00012890: 7065 5b30 5d0d 0a20 2020 2020 2020 2020  pe[0]..         
+000128a0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000128b0: 7261 6e67 6528 6c65 6e28 6578 7061 6e64  range(len(expand
+000128c0: 6564 5f74 696d 6529 293a 0d0a 2020 2020  ed_time)):..    
+000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128e0: 2020 2065 7870 616e 6465 645f 7469 6d65     expanded_time
+000128f0: 5b69 5d20 3d20 6920 0d0a 2020 2020 2020  [i] = i ..      
+00012900: 2020 2020 2020 2020 2020 666f 7220 6375            for cu
+00012910: 7272 656e 745f 756e 6971 7565 5f69 6420  rrent_unique_id 
+00012920: 696e 2075 6e69 7175 655f 6964 735f 7365  in unique_ids_se
+00012930: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00012940: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00012950: 2020 2020 2020 2020 2020 2020 6578 7061              expa
+00012960: 6e64 6564 5f69 6e74 656e 7369 7479 203d  nded_intensity =
+00012970: 206e 702e 7a65 726f 7328 7365 6c66 2e74   np.zeros(self.t
+00012980: 656e 6420 2d20 7365 6c66 2e74 7374 6172  end - self.tstar
+00012990: 7420 2b20 3129 0d0a 2020 2020 2020 2020  t + 1)..        
+000129a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000129d0: 2020 2020 2063 7572 7265 6e74 5f74 696d       current_tim
+000129e0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+000129f0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012a00: 6e74 5f7a 203d 205b 5d0d 0a20 2020 2020  nt_z = []..     
+00012a10: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012a20: 7272 656e 745f 7920 3d20 5b5d 0d0a 2020  rrent_y = []..  
+00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a40: 2063 7572 7265 6e74 5f78 203d 205b 5d0d   current_x = [].
+00012a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a60: 2020 2020 6375 7272 656e 745f 696e 7465      current_inte
+00012a70: 6e73 6974 7920 3d20 5b5d 0d0a 2020 2020  nsity = []..    
+00012a80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012a90: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
+00012aa0: 6c61 7373 203d 205b 5d0d 0a20 2020 2020  lass = []..     
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012ac0: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
+00012ad0: 6173 735f 7363 6f72 6520 3d20 5b5d 0d0a  ass_score = []..
+00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012af0: 2020 2063 7572 7265 6e74 5f72 6164 6975     current_radiu
+00012b00: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00012b10: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012b20: 6e74 5f76 6f6c 756d 6520 3d20 5b5d 0d0a  nt_volume = []..
+00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b40: 2020 2063 7572 7265 6e74 5f73 7065 6564     current_speed
+00012b50: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00012b60: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012b70: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 203d  t_motion_angle =
+00012b80: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00012b90: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012ba0: 6163 6365 6c65 7261 7469 6f6e 203d 205b  acceleration = [
+00012bb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012bc0: 2020 2020 2020 6375 7272 656e 745f 6469        current_di
+00012bd0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00012be0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00012bf0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012c00: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00012c10: 6f6d 705f 6669 7273 7420 3d20 5b5d 0d0a  omp_first = []..
+00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c30: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
+00012c40: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+00012c50: 6f6e 6420 3d20 5b5d 0d0a 2020 2020 2020  ond = []..      
+00012c60: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012c70: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
+00012c80: 6120 3d20 5b5d 0d0a 0d0a 2020 2020 2020  a = []....      
+00012c90: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012ca0: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
+00012cb0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+00012cc0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012cd0: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
+00012ce0: 6b20 3d20 5b5d 200d 0a20 2020 2020 2020  k = [] ..       
+00012cf0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+00012d20: 7469 6d65 2e73 6861 7065 5b30 5d29 3a0d  time.shape[0]):.
+00012d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d40: 2020 2020 2020 2020 2020 2069 6620 6375             if cu
+00012d50: 7272 656e 745f 756e 6971 7565 5f69 6420  rrent_unique_id 
+00012d60: 3d3d 2075 6e69 7175 655f 6964 735b 6a5d  == unique_ids[j]
+00012d70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d90: 2020 2020 6375 7272 656e 745f 7469 6d65      current_time
+00012da0: 2e61 7070 656e 6428 7469 6d65 5b6a 5d29  .append(time[j])
+00012db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012dd0: 2020 2063 7572 7265 6e74 5f7a 2e61 7070     current_z.app
+00012de0: 656e 6428 5a5b 6a5d 290d 0a20 2020 2020  end(Z[j])..     
+00012df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e00: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012e10: 656e 745f 792e 6170 7065 6e64 2859 5b6a  ent_y.append(Y[j
+00012e20: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 2020 2063 7572 7265 6e74 5f78 2e61       current_x.a
+00012e50: 7070 656e 6428 585b 6a5d 290d 0a20 2020  ppend(X[j])..   
+00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e70: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00012e80: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
+00012e90: 5b69 6e74 2874 696d 655b 6a5d 295d 203d  [int(time[j])] =
+00012ea0: 2069 6e74 656e 7369 7479 5b6a 5d0d 0a20   intensity[j].. 
 00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 6375 7272 656e 745f 696e 7465 6e73 6974  current_intensit
-00012ed0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
-00012ee0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012ef0: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00012f00: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012f10: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012f20: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
-00012f30: 7363 6f72 6520 3d20 5b5d 0d0a 2020 2020  score = []..    
-00012f40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012f50: 7572 7265 6e74 5f72 6164 6975 7320 3d20  urrent_radius = 
-00012f60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012f70: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
-00012f80: 6f6c 756d 6520 3d20 5b5d 0d0a 2020 2020  olume = []..    
-00012f90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012fa0: 7572 7265 6e74 5f73 7065 6564 203d 205b  urrent_speed = [
-00012fb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012fc0: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
-00012fd0: 7469 6f6e 5f61 6e67 6c65 203d 205b 5d0d  tion_angle = [].
-00012fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ff0: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
-00013000: 6c65 7261 7469 6f6e 203d 205b 5d0d 0a20  leration = [].. 
-00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013020: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
-00013030: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00013040: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00013050: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
-00013060: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00013070: 6669 7273 7420 3d20 5b5d 0d0a 2020 2020  first = []..    
-00013080: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013090: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-000130a0: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
-000130b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000130c0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000130d0: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
-000130e0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-000130f0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013100: 5f72 6164 6961 6c5f 616e 676c 6520 3d20  _radial_angle = 
-00013110: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00013120: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00013130: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
-00013140: 5b5d 200d 0a20 2020 2020 2020 2020 2020  [] ..           
-00013150: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00013160: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00013170: 206a 2069 6e20 7261 6e67 6528 7469 6d65   j in range(time
-00013180: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
-00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131a0: 2020 2020 2020 2069 6620 6375 7272 656e         if curren
-000131b0: 745f 756e 6971 7565 5f69 6420 3d3d 2075  t_unique_id == u
-000131c0: 6e69 7175 655f 6964 735b 6a5d 3a0d 0a20  nique_ids[j]:.. 
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ed0: 6375 7272 656e 745f 696e 7465 6e73 6974  current_intensit
+00012ee0: 792e 6170 7065 6e64 2869 6e74 656e 7369  y.append(intensi
+00012ef0: 7479 5b6a 5d29 0d0a 2020 2020 2020 2020  ty[j])..        
+00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f10: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012f20: 5f63 6c75 7374 6572 5f63 6c61 7373 2e61  _cluster_class.a
+00012f30: 7070 656e 6428 636c 7573 7465 725f 636c  ppend(cluster_cl
+00012f40: 6173 735b 6a5d 290d 0a20 2020 2020 2020  ass[j])..       
+00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f60: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012f70: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00012f80: 7363 6f72 652e 6170 7065 6e64 2863 6c75  score.append(clu
+00012f90: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
+00012fa0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fc0: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
+00012fd0: 6164 6975 732e 6170 7065 6e64 2872 6164  adius.append(rad
+00012fe0: 6975 735b 6a5d 290d 0a20 2020 2020 2020  ius[j])..       
+00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013000: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013010: 745f 766f 6c75 6d65 2e61 7070 656e 6428  t_volume.append(
+00013020: 766f 6c75 6d65 5b6a 5d29 0d0a 2020 2020  volume[j])..    
+00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013040: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013050: 7265 6e74 5f73 7065 6564 2e61 7070 656e  rent_speed.appen
+00013060: 6428 7370 6565 645b 6a5d 290d 0a20 2020  d(speed[j])..   
+00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013080: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013090: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
+000130a0: 6c65 2e61 7070 656e 6428 6d6f 7469 6f6e  le.append(motion
+000130b0: 5f61 6e67 6c65 5b6a 5d29 0d0a 2020 2020  _angle[j])..    
+000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130d0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000130e0: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
+000130f0: 6e2e 6170 7065 6e64 2861 6363 656c 6572  n.append(acceler
+00013100: 6174 696f 6e5b 6a5d 290d 0a20 2020 2020  ation[j])..     
+00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013120: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013130: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00013140: 6c5f 6d61 736b 2e61 7070 656e 6428 6469  l_mask.append(di
+00013150: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00013160: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00013170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013180: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
+00013190: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+000131a0: 5f66 6972 7374 2e61 7070 656e 6428 6563  _first.append(ec
+000131b0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+000131c0: 6669 7273 745b 6a5d 290d 0a20 2020 2020  first[j])..     
 000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131f0: 6375 7272 656e 745f 7469 6d65 2e61 7070  current_time.app
-00013200: 656e 6428 7469 6d65 5b6a 5d29 0d0a 2020  end(time[j])..  
-00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013230: 7572 7265 6e74 5f7a 2e61 7070 656e 6428  urrent_z.append(
-00013240: 5a5b 6a5d 290d 0a20 2020 2020 2020 2020  Z[j])..         
-00013250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013260: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013270: 792e 6170 7065 6e64 2859 5b6a 5d29 0d0a  y.append(Y[j])..
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131e0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000131f0: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00013200: 5f63 6f6d 705f 7365 636f 6e64 2e61 7070  _comp_second.app
+00013210: 656e 6428 6563 6365 6e74 7269 6369 7479  end(eccentricity
+00013220: 5f63 6f6d 705f 7365 636f 6e64 5b6a 5d29  _comp_second[j])
+00013230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013250: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
+00013260: 6365 5f61 7265 612e 6170 7065 6e64 2873  ce_area.append(s
+00013270: 7572 6661 6365 5f61 7265 615b 6a5d 290d  urface_area[j]).
+00013280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00013290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132a0: 2063 7572 7265 6e74 5f78 2e61 7070 656e   current_x.appen
-000132b0: 6428 585b 6a5d 290d 0a20 2020 2020 2020  d(X[j])..       
-000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132d0: 2020 2020 2020 2020 2020 6578 7061 6e64            expand
-000132e0: 6564 5f69 6e74 656e 7369 7479 5b69 6e74  ed_intensity[int
-000132f0: 2874 696d 655b 6a5d 295d 203d 2069 6e74  (time[j])] = int
-00013300: 656e 7369 7479 5b6a 5d0d 0a20 2020 2020  ensity[j]..     
-00013310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013320: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013330: 656e 745f 696e 7465 6e73 6974 792e 6170  ent_intensity.ap
-00013340: 7065 6e64 2869 6e74 656e 7369 7479 5b6a  pend(intensity[j
-00013350: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000132a0: 2020 6375 7272 656e 745f 7261 6469 616c    current_radial
+000132b0: 5f61 6e67 6c65 2e61 7070 656e 6428 7261  _angle.append(ra
+000132c0: 6469 616c 5f61 6e67 6c65 5b6a 5d29 0d0a  dial_angle[j])..
+000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132f0: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
+00013300: 6973 5f6d 6173 6b2e 6170 7065 6e64 2863  is_mask.append(c
+00013310: 656c 6c5f 6178 6973 5f6d 6173 6b5b 6a5d  ell_axis_mask[j]
+00013320: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013330: 2020 2020 2020 6375 7272 656e 745f 7469        current_ti
+00013340: 6d65 203d 206e 702e 6173 6172 7261 7928  me = np.asarray(
+00013350: 6375 7272 656e 745f 7469 6d65 290d 0a20  current_time).. 
 00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013370: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
-00013380: 7374 6572 5f63 6c61 7373 2e61 7070 656e  ster_class.appen
-00013390: 6428 636c 7573 7465 725f 636c 6173 735b  d(cluster_class[
-000133a0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133c0: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
-000133d0: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
-000133e0: 652e 6170 7065 6e64 2863 6c75 7374 6572  e.append(cluster
-000133f0: 5f63 6c61 7373 5f73 636f 7265 5b6a 5d29  _class_score[j])
-00013400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013420: 2020 2063 7572 7265 6e74 5f72 6164 6975     current_radiu
-00013430: 732e 6170 7065 6e64 2872 6164 6975 735b  s.append(radius[
-00013440: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013460: 2020 2020 2020 6375 7272 656e 745f 766f        current_vo
-00013470: 6c75 6d65 2e61 7070 656e 6428 766f 6c75  lume.append(volu
-00013480: 6d65 5b6a 5d29 0d0a 2020 2020 2020 2020  me[j])..        
-00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013370: 2020 6375 7272 656e 745f 696e 7465 6e73    current_intens
+00013380: 6974 7920 3d20 6e70 2e61 7361 7272 6179  ity = np.asarray
+00013390: 2863 7572 7265 6e74 5f69 6e74 656e 7369  (current_intensi
+000133a0: 7479 290d 0a0d 0a0d 0a20 2020 2020 2020  ty)......       
+000133b0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000133c0: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
+000133d0: 7320 3d20 6e70 2e61 7361 7272 6179 2863  s = np.asarray(c
+000133e0: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
+000133f0: 6c61 7373 290d 0a20 2020 2020 2020 2020  lass)..         
+00013400: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013410: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00013420: 7363 6f72 6520 3d20 6e70 2e61 7361 7272  score = np.asarr
+00013430: 6179 2863 7572 7265 6e74 5f63 6c75 7374  ay(current_clust
+00013440: 6572 5f63 6c61 7373 5f73 636f 7265 2920  er_class_score) 
+00013450: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00013460: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013470: 5f72 6164 6975 7320 3d20 6e70 2e61 7361  _radius = np.asa
+00013480: 7272 6179 2863 7572 7265 6e74 5f72 6164  rray(current_rad
+00013490: 6975 7329 0d0a 2020 2020 2020 2020 2020  ius)..          
 000134a0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000134b0: 5f73 7065 6564 2e61 7070 656e 6428 7370  _speed.append(sp
-000134c0: 6565 645b 6a5d 290d 0a20 2020 2020 2020  eed[j])..       
-000134d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134e0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000134f0: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 2e61  t_motion_angle.a
-00013500: 7070 656e 6428 6d6f 7469 6f6e 5f61 6e67  ppend(motion_ang
-00013510: 6c65 5b6a 5d29 0d0a 2020 2020 2020 2020  le[j])..        
-00013520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013530: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013540: 5f61 6363 656c 6572 6174 696f 6e2e 6170  _acceleration.ap
-00013550: 7065 6e64 2861 6363 656c 6572 6174 696f  pend(acceleratio
-00013560: 6e5b 6a5d 290d 0a20 2020 2020 2020 2020  n[j])..         
-00013570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013580: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013590: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000135a0: 736b 2e61 7070 656e 6428 6469 7374 616e  sk.append(distan
-000135b0: 6365 5f63 656c 6c5f 6d61 736b 5b6a 5d29  ce_cell_mask[j])
-000135c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135e0: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
-000135f0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00013600: 7374 2e61 7070 656e 6428 6563 6365 6e74  st.append(eccent
-00013610: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00013620: 745b 6a5d 290d 0a20 2020 2020 2020 2020  t[j])..         
-00013630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013640: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013650: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00013660: 705f 7365 636f 6e64 2e61 7070 656e 6428  p_second.append(
-00013670: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00013680: 705f 7365 636f 6e64 5b6a 5d29 0d0a 2020  p_second[j])..  
-00013690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000136b0: 7572 7265 6e74 5f73 7572 6661 6365 5f61  urrent_surface_a
-000136c0: 7265 612e 6170 7065 6e64 2873 7572 6661  rea.append(surfa
-000136d0: 6365 5f61 7265 615b 6a5d 290d 0a20 2020  ce_area[j])..   
-000136e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136f0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013700: 7272 656e 745f 7261 6469 616c 5f61 6e67  rrent_radial_ang
-00013710: 6c65 2e61 7070 656e 6428 7261 6469 616c  le.append(radial
-00013720: 5f61 6e67 6c65 5b6a 5d29 0d0a 2020 2020  _angle[j])..    
-00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013740: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013750: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
-00013760: 6173 6b2e 6170 7065 6e64 2863 656c 6c5f  ask.append(cell_
-00013770: 6178 6973 5f6d 6173 6b5b 6a5d 290d 0a20  axis_mask[j]).. 
-00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013790: 2020 6375 7272 656e 745f 7469 6d65 203d    current_time =
-000137a0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-000137b0: 656e 745f 7469 6d65 290d 0a20 2020 2020  ent_time)..     
-000137c0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000137d0: 7272 656e 745f 696e 7465 6e73 6974 7920  rrent_intensity 
-000137e0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-000137f0: 7265 6e74 5f69 6e74 656e 7369 7479 290d  rent_intensity).
-00013800: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00013810: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013820: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
-00013830: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00013840: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00013850: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013860: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
-00013870: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
-00013880: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
-00013890: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
-000138a0: 6c61 7373 5f73 636f 7265 2920 2020 0d0a  lass_score)   ..
-000138b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000138c0: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
-000138d0: 6975 7320 3d20 6e70 2e61 7361 7272 6179  ius = np.asarray
-000138e0: 2863 7572 7265 6e74 5f72 6164 6975 7329  (current_radius)
-000138f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013900: 2020 2020 2063 7572 7265 6e74 5f76 6f6c       current_vol
-00013910: 756d 6520 3d20 6e70 2e61 7361 7272 6179  ume = np.asarray
-00013920: 2863 7572 7265 6e74 5f76 6f6c 756d 6529  (current_volume)
-00013930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013940: 2020 2020 2063 7572 7265 6e74 5f65 6363       current_ecc
-00013950: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00013960: 6972 7374 203d 206e 702e 6173 6172 7261  irst = np.asarra
-00013970: 7928 6375 7272 656e 745f 6563 6365 6e74  y(current_eccent
-00013980: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00013990: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-000139a0: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
-000139b0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000139c0: 5f73 6563 6f6e 6420 3d20 6e70 2e61 7361  _second = np.asa
-000139d0: 7272 6179 2863 7572 7265 6e74 5f65 6363  rray(current_ecc
-000139e0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-000139f0: 6563 6f6e 6429 0d0a 2020 2020 2020 2020  econd)..        
-00013a00: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013a10: 6e74 5f73 7572 6661 6365 5f61 7265 6120  nt_surface_area 
-00013a20: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-00013a30: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
-00013a40: 6129 0d0a 0d0a 2020 2020 2020 2020 2020  a)....          
-00013a50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013a60: 5f73 7065 6564 203d 206e 702e 6173 6172  _speed = np.asar
-00013a70: 7261 7928 6375 7272 656e 745f 7370 6565  ray(current_spee
-00013a80: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00013a90: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
-00013aa0: 6f74 696f 6e5f 616e 676c 6520 3d20 6e70  otion_angle = np
-00013ab0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013ac0: 5f6d 6f74 696f 6e5f 616e 676c 6529 0d0a  _motion_angle)..
-00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ae0: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
-00013af0: 6572 6174 696f 6e20 3d20 6e70 2e61 7361  eration = np.asa
-00013b00: 7272 6179 2863 7572 7265 6e74 5f61 6363  rray(current_acc
-00013b10: 656c 6572 6174 696f 6e29 0d0a 2020 2020  eleration)..    
-00013b20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013b30: 7572 7265 6e74 5f64 6973 7461 6e63 655f  urrent_distance_
-00013b40: 6365 6c6c 5f6d 6173 6b20 3d20 6e70 2e61  cell_mask = np.a
-00013b50: 7361 7272 6179 2863 7572 7265 6e74 5f64  sarray(current_d
-00013b60: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00013b70: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
-00013b80: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
-00013b90: 6164 6961 6c5f 616e 676c 6520 3d20 6e70  adial_angle = np
-00013ba0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013bb0: 5f72 6164 6961 6c5f 616e 676c 6529 0d0a  _radial_angle)..
-00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bd0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00013be0: 6178 6973 5f6d 6173 6b20 3d20 6e70 2e61  axis_mask = np.a
-00013bf0: 7361 7272 6179 2863 7572 7265 6e74 5f63  sarray(current_c
-00013c00: 656c 6c5f 6178 6973 5f6d 6173 6b29 0d0a  ell_axis_mask)..
-00013c10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00013c20: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00013c30: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c50: 2069 6620 706f 696e 745f 7361 6d70 6c65   if point_sample
-00013c60: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c80: 2020 2020 2020 2078 665f 7361 6d70 6c65         xf_sample
-00013c90: 203d 2066 6674 6672 6571 2870 6f69 6e74   = fftfreq(point
-00013ca0: 5f73 616d 706c 652c 2073 656c 662e 7463  _sample, self.tc
-00013cb0: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cd0: 2020 2020 2020 2020 2020 2020 2066 6674               fft
-00013ce0: 7374 7269 705f 7361 6d70 6c65 203d 2066  strip_sample = f
-00013cf0: 6674 2865 7870 616e 6465 645f 696e 7465  ft(expanded_inte
-00013d00: 6e73 6974 7929 0d0a 2020 2020 2020 2020  nsity)..        
-00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d20: 2020 2020 2020 2020 6666 7474 6f74 616c          ffttotal
-00013d30: 5f73 616d 706c 6520 3d20 6e70 2e61 6273  _sample = np.abs
-00013d40: 2866 6674 7374 7269 705f 7361 6d70 6c65  (fftstrip_sample
-00013d50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d70: 2020 2078 665f 7361 6d70 6c65 203d 2078     xf_sample = x
-00013d80: 665f 7361 6d70 6c65 5b30 203a 206c 656e  f_sample[0 : len
-00013d90: 2878 665f 7361 6d70 6c65 2920 2f2f 2032  (xf_sample) // 2
-00013da0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dc0: 2020 2066 6674 746f 7461 6c5f 7361 6d70     ffttotal_samp
-00013dd0: 6c65 203d 2066 6674 746f 7461 6c5f 7361  le = ffttotal_sa
-00013de0: 6d70 6c65 5b30 203a 206c 656e 2866 6674  mple[0 : len(fft
-00013df0: 746f 7461 6c5f 7361 6d70 6c65 2920 2f2f  total_sample) //
-00013e00: 2032 5d0d 0a0d 0a20 2020 2020 2020 2020   2]....         
-00013e10: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00013e20: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
-00013e30: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-00013e40: 5f75 6e69 7175 655f 6964 5d20 3d20 6578  _unique_id] = ex
-00013e50: 7061 6e64 6564 5f74 696d 652c 2065 7870  panded_time, exp
-00013e60: 616e 6465 645f 696e 7465 6e73 6974 792c  anded_intensity,
-00013e70: 2078 665f 7361 6d70 6c65 2c20 6666 7474   xf_sample, fftt
-00013e80: 6f74 616c 5f73 616d 706c 650d 0a20 2020  otal_sample..   
-00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ea0: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
-00013eb0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00013ec0: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
-00013ed0: 655f 6964 5d20 3d20 2063 7572 7265 6e74  e_id] =  current
-00013ee0: 5f74 696d 652c 2063 7572 7265 6e74 5f63  _time, current_c
-00013ef0: 6c75 7374 6572 5f63 6c61 7373 2c20 6375  luster_class, cu
-00013f00: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
-00013f10: 6173 735f 7363 6f72 650d 0a20 2020 2020  ass_score..     
-00013f20: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00013f30: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
-00013f40: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-00013f50: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00013f60: 5d20 3d20 6375 7272 656e 745f 7469 6d65  ] = current_time
-00013f70: 2c20 6375 7272 656e 745f 7a2c 2063 7572  , current_z, cur
-00013f80: 7265 6e74 5f79 2c20 6375 7272 656e 745f  rent_y, current_
-00013f90: 782c 2063 7572 7265 6e74 5f72 6164 6975  x, current_radiu
-00013fa0: 732c 2063 7572 7265 6e74 5f76 6f6c 756d  s, current_volum
-00013fb0: 652c 2063 7572 7265 6e74 5f65 6363 656e  e, current_eccen
-00013fc0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00013fd0: 7374 2c20 6375 7272 656e 745f 6563 6365  st, current_ecce
-00013fe0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00013ff0: 636f 6e64 2c20 6375 7272 656e 745f 7375  cond, current_su
-00014000: 7266 6163 655f 6172 6561 2c20 6375 7272  rface_area, curr
-00014010: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
-00014020: 732c 2063 7572 7265 6e74 5f63 6c75 7374  s, current_clust
-00014030: 6572 5f63 6c61 7373 5f73 636f 7265 0d0a  er_class_score..
-00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014050: 2020 2075 6e69 7175 655f 6479 6e61 6d69     unique_dynami
-00014060: 635f 7072 6f70 6572 7469 6573 5f74 7261  c_properties_tra
-00014070: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
-00014080: 6971 7565 5f69 645d 203d 2063 7572 7265  ique_id] = curre
-00014090: 6e74 5f74 696d 652c 2063 7572 7265 6e74  nt_time, current
-000140a0: 5f73 7065 6564 2c20 6375 7272 656e 745f  _speed, current_
-000140b0: 6d6f 7469 6f6e 5f61 6e67 6c65 2c20 6375  motion_angle, cu
-000140c0: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
-000140d0: 6f6e 2c20 6375 7272 656e 745f 6469 7374  on, current_dist
-000140e0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
-000140f0: 6375 7272 656e 745f 7261 6469 616c 5f61  current_radial_a
-00014100: 6e67 6c65 2c20 6375 7272 656e 745f 6365  ngle, current_ce
-00014110: 6c6c 5f61 7869 735f 6d61 736b 0d0a 2020  ll_axis_mask..  
-00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014130: 2073 656c 662e 756e 6971 7565 5f66 6674   self.unique_fft
-00014140: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
-00014150: 6b5f 6964 5d2e 7570 6461 7465 287b 6375  k_id].update({cu
-00014160: 7272 656e 745f 756e 6971 7565 5f69 643a  rrent_unique_id:
-00014170: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
-00014180: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-00014190: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-000141a0: 5d7d 290d 0a20 2020 2020 2020 2020 2020  ]})..           
-000141b0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000141c0: 7175 655f 636c 7573 7465 725f 7072 6f70  que_cluster_prop
-000141d0: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-000141e0: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
-000141f0: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
-00014200: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
-00014210: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
-00014220: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
-00014230: 7d29 0d0a 0d0a 2020 2020 2020 2020 2020  })....          
-00014240: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00014250: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
-00014260: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
-00014270: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
-00014280: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
-00014290: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
-000142a0: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
-000142b0: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
-000142c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000142d0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000142e0: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
-000142f0: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
-00014300: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
-00014310: 7175 655f 6964 3a75 6e69 7175 655f 6479  que_id:unique_dy
-00014320: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
-00014330: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-00014340: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
-00014350: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014370: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
-00014380: 6469 6374 5f75 7064 6174 6528 7365 6c66  dict_update(self
-00014390: 2c20 756e 6971 7565 5f74 7261 636b 6c65  , unique_trackle
-000143a0: 745f 6964 733a 204c 6973 742c 2020 6365  t_ids: List,  ce
-000143b0: 6c6c 5f69 643a 2069 6e74 2c20 7472 6163  ll_id: int, trac
-000143c0: 6b5f 6964 3a20 696e 742c 2073 6f75 7263  k_id: int, sourc
-000143d0: 655f 6964 3a20 696e 742c 2074 6172 6765  e_id: int, targe
-000143e0: 745f 6964 3a20 696e 7429 3a0d 0a0d 0a20  t_id: int):.... 
-000143f0: 0d0a 2020 2020 2020 2020 6765 6e65 7261  ..        genera
-00014400: 7469 6f6e 5f69 6420 3d20 7365 6c66 2e67  tion_id = self.g
-00014410: 656e 6572 6174 696f 6e5f 6469 6374 5b63  eneration_dict[c
-00014420: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
-00014430: 2074 7261 636b 6c65 745f 6964 203d 2073   tracklet_id = s
-00014440: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
-00014450: 745b 6365 6c6c 5f69 645d 0d0a 0d0a 2020  t[cell_id]....  
-00014460: 2020 2020 2020 756e 6971 7565 5f69 6420        unique_id 
-00014470: 3d20 7374 7228 7472 6163 6b5f 6964 2920  = str(track_id) 
-00014480: 2b20 7374 7228 7365 6c66 2e6d 6178 5f74  + str(self.max_t
-00014490: 7261 636b 5f69 6429 202b 2073 7472 2867  rack_id) + str(g
-000144a0: 656e 6572 6174 696f 6e5f 6964 2920 2b20  eneration_id) + 
-000144b0: 7374 7228 7472 6163 6b6c 6574 5f69 6429  str(tracklet_id)
-000144c0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000144d0: 2020 2020 7665 635f 6d61 736b 203d 205b      vec_mask = [
-000144e0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000144f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014500: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00014510: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-00014520: 645f 785f 6b65 795d 292c 2066 6c6f 6174  d_x_key]), float
-00014530: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00014540: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014550: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00014560: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
-00014570: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
-00014580: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014590: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000145a0: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
-000145b0: 656e 7472 6f69 645f 7a5f 6b65 795d 2920  entroid_z_key]) 
-000145c0: 5d0d 0a0d 0a20 2020 2020 2020 2076 6563  ]....        vec
-000145d0: 5f63 656c 6c20 3d20 5b66 6c6f 6174 2873  _cell = [float(s
-000145e0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000145f0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014600: 656c 6c5f 6964 295d 5b73 656c 662e 7870  ell_id)][self.xp
-00014610: 6f73 6964 5f6b 6579 5d29 202c 200d 0a20  osid_key]) , .. 
-00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014630: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00014640: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00014650: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014660: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00014670: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
-00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014690: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-000146a0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-000146b0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000146c0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-000146d0: 2e7a 706f 7369 645f 6b65 795d 295d 0d0a  .zposid_key])]..
-000146e0: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
-000146f0: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
-00014700: 2876 6563 5f6d 6173 6b2c 2076 6563 5f63  (vec_mask, vec_c
-00014710: 656c 6c29 0d0a 0d0a 2020 2020 2020 2020  ell)....        
-00014720: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014730: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014740: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00014750: 287b 7365 6c66 2e72 6164 6961 6c5f 616e  ({self.radial_an
-00014760: 676c 655f 6b65 7920 3a20 616e 676c 657d  gle_key : angle}
-00014770: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-00014780: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-00014790: 2075 6e69 7175 655f 7472 6163 6b6c 6574   unique_tracklet
-000147a0: 5f69 6473 2e61 7070 656e 6428 7374 7228  _ids.append(str(
-000147b0: 756e 6971 7565 5f69 6429 290d 0a20 2020  unique_id))..   
-000147c0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000147d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000147e0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-000147f0: 7064 6174 6528 7b73 656c 662e 636c 7573  pdate({self.clus
-00014800: 7465 7263 6c61 7373 5f6b 6579 203a 204e  terclass_key : N
-00014810: 6f6e 657d 290d 0a20 2020 2020 2020 2073  one})..        s
-00014820: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014830: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014840: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00014850: 7b73 656c 662e 636c 7573 7465 7273 636f  {self.clustersco
-00014860: 7265 5f6b 6579 203a 2030 7d29 0d0a 2020  re_key : 0})..  
-00014870: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014880: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014890: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-000148a0: 7570 6461 7465 287b 7365 6c66 2e75 6e69  update({self.uni
-000148b0: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
-000148c0: 756e 6971 7565 5f69 6429 7d29 0d0a 2020  unique_id)})..  
-000148d0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000148e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000148f0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00014900: 7570 6461 7465 287b 7365 6c66 2e74 7261  update({self.tra
-00014910: 636b 6c65 7469 645f 6b65 7920 3a20 7374  ckletid_key : st
-00014920: 7228 7472 6163 6b6c 6574 5f69 6429 7d29  r(tracklet_id)})
-00014930: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00014940: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014950: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014960: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00014970: 662e 6765 6e65 7261 7469 6f6e 6964 5f6b  f.generationid_k
-00014980: 6579 203a 2073 7472 2867 656e 6572 6174  ey : str(generat
-00014990: 696f 6e5f 6964 297d 2920 0d0a 2020 2020  ion_id)}) ..    
-000149a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000149b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000149c0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-000149d0: 6461 7465 287b 7365 6c66 2e74 7261 636b  date({self.track
-000149e0: 6964 5f6b 6579 203a 2073 7472 2874 7261  id_key : str(tra
-000149f0: 636b 5f69 6429 7d29 0d0a 2020 2020 2020  ck_id)})..      
-00014a00: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014a10: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014a20: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014a30: 7465 287b 7365 6c66 2e6d 6f74 696f 6e5f  te({self.motion_
-00014a40: 616e 676c 655f 6b65 7920 3a20 302e 307d  angle_key : 0.0}
-00014a50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00014a60: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014a70: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014a80: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00014a90: 662e 7370 6565 645f 6b65 7920 3a20 302e  f.speed_key : 0.
-00014aa0: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
-00014ab0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014ac0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014ad0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014ae0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00014af0: 5f6b 6579 203a 2030 2e30 7d29 0d0a 2020  _key : 0.0})..  
-00014b00: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014b10: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014b20: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00014b30: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-00014b40: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00014b50: 6972 7374 6b65 7920 3a20 4e6f 6e65 7d29  irstkey : None})
-00014b60: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00014b70: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014b80: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014b90: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00014ba0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
-00014bb0: 6d70 5f73 6563 6f6e 646b 6579 203a 204e  mp_secondkey : N
-00014bc0: 6f6e 657d 290d 0a20 2020 2020 2020 2073  one})..        s
-00014bd0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014be0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014bf0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00014c00: 7b73 656c 662e 7375 7266 6163 655f 6172  {self.surface_ar
-00014c10: 6561 5f6b 6579 203a 204e 6f6e 657d 290d  ea_key : None}).
-00014c20: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00014c30: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014c40: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014c50: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014c60: 6365 6c6c 6178 6973 5f6d 6173 6b5f 6b65  cellaxis_mask_ke
-00014c70: 7920 3a20 4e6f 6e65 7d29 0d0a 0d0a 2020  y : None})....  
-00014c80: 2020 2020 2020 6966 2073 6f75 7263 655f        if source_
-00014c90: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0d  id is not None:.
-00014ca0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014cb0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014cc0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014cd0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014ce0: 656c 662e 6265 666f 7265 6964 5f6b 6579  elf.beforeid_key
-00014cf0: 203a 2069 6e74 2873 6f75 7263 655f 6964   : int(source_id
-00014d00: 297d 290d 0a20 2020 2020 2020 2020 2020  )})..           
-00014d10: 2076 6563 5f31 203d 205b 666c 6f61 7428   vec_1 = [float(
-00014d20: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014d30: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014d40: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-00014d50: 706f 7369 645f 6b65 795d 2920 2d20 666c  posid_key]) - fl
-00014d60: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00014d70: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014d80: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
-00014d90: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-00014da0: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
-00014db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014dc0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00014dd0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014de0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014df0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-00014e00: 5d29 202d 2066 6c6f 6174 2873 656c 662e  ]) - float(self.
-00014e10: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014e20: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00014e30: 655f 6964 295d 5b73 656c 662e 7970 6f73  e_id)][self.ypos
-00014e40: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
-00014e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e60: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-00014e70: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014e80: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014e90: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
-00014ea0: 7369 645f 6b65 795d 2920 2d20 2066 6c6f  sid_key]) -  flo
-00014eb0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014ec0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014ed0: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-00014ee0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00014ef0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-00014f00: 7065 6564 203d 206e 702e 7371 7274 286e  peed = np.sqrt(n
-00014f10: 702e 646f 7428 7665 635f 312c 2076 6563  p.dot(vec_1, vec
-00014f20: 5f31 2929 2f73 656c 662e 7463 616c 6962  _1))/self.tcalib
-00014f30: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00014f40: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00014f50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014f60: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00014f70: 6461 7465 287b 7365 6c66 2e73 7065 6564  date({self.speed
-00014f80: 5f6b 6579 203a 2073 7065 6564 7d29 0d0a  _key : speed})..
-00014f90: 0d0a 2020 2020 2020 2020 2020 2020 6d6f  ..            mo
-00014fa0: 7469 6f6e 5f61 6e67 6c65 203d 2061 6e67  tion_angle = ang
-00014fb0: 756c 6172 5f63 6861 6e67 6528 7665 635f  ular_change(vec_
-00014fc0: 6d61 736b 2c20 7665 635f 3129 0d0a 0d0a  mask, vec_1)....
-00014fd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014fe0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014ff0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015000: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015010: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
-00015020: 6b65 7920 3a20 6d6f 7469 6f6e 5f61 6e67  key : motion_ang
-00015030: 6c65 7d29 200d 0a0d 0a20 2020 2020 2020  le}) ....       
-00015040: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
-00015050: 6420 696e 2073 656c 662e 6564 6765 5f73  d in self.edge_s
-00015060: 6f75 7263 655f 6c6f 6f6b 7570 3a0d 0a20  ource_lookup:.. 
-00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015080: 2020 2070 7265 5f73 6f75 7263 655f 6964     pre_source_id
-00015090: 203d 2073 656c 662e 6564 6765 5f73 6f75   = self.edge_sou
-000150a0: 7263 655f 6c6f 6f6b 7570 5b73 6f75 7263  rce_lookup[sourc
-000150b0: 655f 6964 5d0d 0a20 2020 2020 2020 2020  e_id]..         
-000150c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150e0: 2076 6563 5f32 203d 205b 666c 6f61 7428   vec_2 = [float(
-000150f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015100: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015110: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-00015120: 706f 7369 645f 6b65 795d 2920 2d20 3220  posid_key]) - 2 
-00015130: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
-00015140: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015150: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
-00015160: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
-00015170: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
-00015180: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015190: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
-000151a0: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
-000151b0: 6c66 2e78 706f 7369 645f 6b65 795d 292c  lf.xposid_key]),
-000151c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000151d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000151e0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-000151f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015200: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00015210: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00015220: 202d 2032 202a 2066 6c6f 6174 2873 656c   - 2 * float(sel
-00015230: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015240: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
-00015250: 7263 655f 6964 295d 5b73 656c 662e 7970  rce_id)][self.yp
-00015260: 6f73 6964 5f6b 6579 5d29 202b 2066 6c6f  osid_key]) + flo
-00015270: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00015280: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015290: 6e74 2870 7265 5f73 6f75 7263 655f 6964  nt(pre_source_id
-000152a0: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
-000152b0: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
-000152c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152d0: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-000152e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000152f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00015300: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
-00015310: 6b65 795d 2920 2d20 2032 202a 2066 6c6f  key]) -  2 * flo
-00015320: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00015330: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015340: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-00015350: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00015360: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
-00015370: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015380: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
-00015390: 7263 655f 6964 295d 5b73 656c 662e 7a70  rce_id)][self.zp
-000153a0: 6f73 6964 5f6b 6579 5d29 5d0d 0a20 2020  osid_key])]..   
-000153b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153c0: 2061 6363 203d 206e 702e 7371 7274 286e   acc = np.sqrt(n
-000153d0: 702e 646f 7428 7665 635f 322c 2076 6563  p.dot(vec_2, vec
-000153e0: 5f32 2929 2f73 656c 662e 7463 616c 6962  _2))/self.tcalib
-000153f0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00015400: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015420: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00015430: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015440: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00015450: 7465 287b 7365 6c66 2e61 6363 656c 6572  te({self.acceler
-00015460: 6174 696f 6e5f 6b65 7920 3a20 6163 637d  ation_key : acc}
-00015470: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-00015480: 736f 7572 6365 5f69 6420 6973 204e 6f6e  source_id is Non
-00015490: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000154a0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000154b0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000154c0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-000154d0: 287b 7365 6c66 2e62 6566 6f72 6569 645f  ({self.beforeid_
-000154e0: 6b65 7920 3a20 4e6f 6e65 7d29 200d 0a20  key : None}) .. 
-000154f0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-00015500: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00015510: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00015520: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00015530: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015540: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015550: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015560: 7064 6174 6528 7b73 656c 662e 6166 7465  pdate({self.afte
-00015570: 7269 645f 6b65 7920 3a20 696e 7428 7461  rid_key : int(ta
-00015580: 7267 6574 5f69 6429 7d29 200d 0a20 2020  rget_id)}) ..   
-00015590: 2020 2020 2065 6c69 6620 7461 7267 6574       elif target
-000155a0: 5f69 6420 6973 204e 6f6e 653a 0d0a 2020  _id is None:..  
-000155b0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000155c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000155d0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-000155e0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-000155f0: 2e61 6674 6572 6964 5f6b 6579 203a 204e  .afterid_key : N
-00015600: 6f6e 657d 290d 0a20 2020 2020 2020 2020  one})..         
-00015610: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00015620: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015640: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00015650: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00015660: 2020 2020 6465 6620 5f74 656d 706f 7261      def _tempora
-00015670: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
-00015680: 6528 7365 6c66 293a 0d0a 2020 2020 0d0a  e(self):..    ..
-00015690: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
-000156a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000156b0: 2e41 7474 7220 3d20 7b7d 0d0a 2020 2020  .Attr = {}..    
-000156c0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-000156d0: 7474 696d 6520 3d20 696e 7428 6d69 6e28  ttime = int(min(
-000156e0: 7365 6c66 2e41 6c6c 5661 6c75 6573 5b73  self.AllValues[s
-000156f0: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
-00015700: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00015710: 2020 2020 656e 6474 696d 6520 3d20 696e      endtime = in
-00015720: 7428 6d61 7828 7365 6c66 2e41 6c6c 5661  t(max(self.AllVa
-00015730: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
-00015740: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
-00015750: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00015760: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015770: 662e 7469 6d65 203d 205b 5d0d 0a20 2020  f.time = []..   
-00015780: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015790: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-000157a0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-000157b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000157c0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-000157d0: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
-000157e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000157f0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-00015800: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00015810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015820: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-00015830: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
-00015840: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015850: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00015860: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00015870: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015880: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-00015890: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
-000158a0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000158b0: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
-000158c0: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-000158d0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000158e0: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
-000158f0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015900: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015910: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-00015920: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015930: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015940: 7469 635f 7661 725f 7370 6565 6420 3d20  tic_var_speed = 
-00015950: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015960: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00015970: 6963 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ic_mean_acc = []
-00015980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015990: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-000159a0: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
-000159b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000159c0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-000159d0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000159e0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-000159f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015a00: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
-00015a10: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00015a20: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015a30: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00015a40: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
-00015a50: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00015a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015a70: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00015a80: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-00015a90: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-00015aa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015ab0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00015ac0: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
-00015ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ae0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015af0: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
-00015b00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015b10: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00015b20: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
-00015b30: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015b40: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015b50: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-00015b60: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
-00015b70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015b80: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00015b90: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00015ba0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015bb0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00015bc0: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
-00015bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015be0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00015bf0: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
-00015c00: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015c10: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00015c20: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
-00015c30: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015c40: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00015c50: 6e5f 6d69 746f 7469 635f 6d65 616e 5f73  n_mitotic_mean_s
-00015c60: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00015c70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015c80: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00015c90: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
-00015ca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015cb0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00015cc0: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
-00015cd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015ce0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00015cf0: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
-00015d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015d10: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00015d20: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
-00015d30: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
-00015d40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015d50: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00015d60: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00015d70: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
-00015d80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015d90: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00015da0: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00015db0: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00015dc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015dd0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00015de0: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-00015df0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-00015e00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015e10: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
-00015e20: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00015e30: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00015e40: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
-00015e50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015e60: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00015e70: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
-00015e80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015e90: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
-00015ea0: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
-00015eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015ec0: 616c 6c5f 6d65 616e 5f64 6973 705f 7820  all_mean_disp_x 
-00015ed0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015ee0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00015ef0: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
-00015f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015f10: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00015f20: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00015f30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015f40: 662e 616c 6c5f 7661 725f 7261 6469 7573  f.all_var_radius
-00015f50: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015f60: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00015f70: 6c5f 6d65 616e 5f73 7065 6564 203d 205b  l_mean_speed = [
-00015f80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015f90: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00015fa0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
-00015fb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015fc0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 6320  lf.all_mean_acc 
-00015fd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015fe0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00015ff0: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
-00016000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016010: 656c 662e 616c 6c5f 6d65 616e 5f64 6972  elf.all_mean_dir
-00016020: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00016030: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016040: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00016050: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00016060: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
-00016070: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016080: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
-00016090: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-000160a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000160b0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-000160c0: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-000160d0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-000160e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000160f0: 662e 6d69 746f 7469 635f 636c 7573 7465  f.mitotic_cluste
-00016100: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
-00016110: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016120: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f63  lf.non_mitotic_c
-00016130: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
-00016140: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016150: 2020 2073 656c 662e 616c 6c5f 636c 7573     self.all_clus
-00016160: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
-00016170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016180: 2020 616c 6c5f 7370 6f74 735f 7472 6163    all_spots_trac
-00016190: 6b73 203d 207b 7d0d 0a20 2020 2020 2020  ks = {}..       
-000161a0: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-000161b0: 7629 2069 6e20 7365 6c66 2e75 6e69 7175  v) in self.uniqu
-000161c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000161d0: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
-000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00016200: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
-00016210: 6f74 7320 3d20 7365 6c66 2e75 6e69 7175  ots = self.uniqu
-00016220: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016230: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
-00016240: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00016250: 656c 662e 7472 6163 6b69 645f 6b65 7920  elf.trackid_key 
-00016260: 696e 2061 6c6c 5f73 706f 7473 3a0d 0a20  in all_spots:.. 
-00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016280: 2020 2020 2020 2020 2061 6c6c 5f73 706f           all_spo
-00016290: 7473 5f74 7261 636b 735b 6b5d 203d 2061  ts_tracks[k] = a
-000162a0: 6c6c 5f73 706f 7473 0d0a 2020 2020 2020  ll_spots..      
-000162b0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-000162c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000134b0: 5f76 6f6c 756d 6520 3d20 6e70 2e61 7361  _volume = np.asa
+000134c0: 7272 6179 2863 7572 7265 6e74 5f76 6f6c  rray(current_vol
+000134d0: 756d 6529 0d0a 2020 2020 2020 2020 2020  ume)..          
+000134e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000134f0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00013500: 6d70 5f66 6972 7374 203d 206e 702e 6173  mp_first = np.as
+00013510: 6172 7261 7928 6375 7272 656e 745f 6563  array(current_ec
+00013520: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00013530: 6669 7273 7429 0d0a 2020 2020 2020 2020  first)..        
+00013540: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013550: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+00013560: 636f 6d70 5f73 6563 6f6e 6420 3d20 6e70  comp_second = np
+00013570: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013580: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00013590: 6d70 5f73 6563 6f6e 6429 0d0a 2020 2020  mp_second)..    
+000135a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000135b0: 7572 7265 6e74 5f73 7572 6661 6365 5f61  urrent_surface_a
+000135c0: 7265 6120 3d20 6e70 2e61 7361 7272 6179  rea = np.asarray
+000135d0: 2863 7572 7265 6e74 5f73 7572 6661 6365  (current_surface
+000135e0: 5f61 7265 6129 0d0a 0d0a 2020 2020 2020  _area)....      
+000135f0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013600: 7265 6e74 5f73 7065 6564 203d 206e 702e  rent_speed = np.
+00013610: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00013620: 7370 6565 6429 0d0a 2020 2020 2020 2020  speed)..        
+00013630: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013640: 6e74 5f6d 6f74 696f 6e5f 616e 676c 6520  nt_motion_angle 
+00013650: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+00013660: 7265 6e74 5f6d 6f74 696f 6e5f 616e 676c  rent_motion_angl
+00013670: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00013680: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00013690: 6363 656c 6572 6174 696f 6e20 3d20 6e70  cceleration = np
+000136a0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+000136b0: 5f61 6363 656c 6572 6174 696f 6e29 0d0a  _acceleration)..
+000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136d0: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
+000136e0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+000136f0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00013700: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
+00013710: 5f6d 6173 6b29 0d0a 2020 2020 2020 2020  _mask)..        
+00013720: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013730: 6e74 5f72 6164 6961 6c5f 616e 676c 6520  nt_radial_angle 
+00013740: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+00013750: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
+00013760: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00013770: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+00013780: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
+00013790: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+000137a0: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
+000137b0: 6b29 0d0a 0d0a 0d0a 2020 2020 2020 2020  k)......        
+000137c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000137d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000137f0: 2020 2020 2069 6620 706f 696e 745f 7361       if point_sa
+00013800: 6d70 6c65 203e 2030 3a0d 0a20 2020 2020  mple > 0:..     
+00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013820: 2020 2020 2020 2020 2020 2078 665f 7361             xf_sa
+00013830: 6d70 6c65 203d 2066 6674 6672 6571 2870  mple = fftfreq(p
+00013840: 6f69 6e74 5f73 616d 706c 652c 2073 656c  oint_sample, sel
+00013850: 662e 7463 616c 6962 7261 7469 6f6e 290d  f.tcalibration).
+00013860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013880: 2066 6674 7374 7269 705f 7361 6d70 6c65   fftstrip_sample
+00013890: 203d 2066 6674 2865 7870 616e 6465 645f   = fft(expanded_
+000138a0: 696e 7465 6e73 6974 7929 0d0a 2020 2020  intensity)..    
+000138b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138c0: 2020 2020 2020 2020 2020 2020 6666 7474              fftt
+000138d0: 6f74 616c 5f73 616d 706c 6520 3d20 6e70  otal_sample = np
+000138e0: 2e61 6273 2866 6674 7374 7269 705f 7361  .abs(fftstrip_sa
+000138f0: 6d70 6c65 290d 0a20 2020 2020 2020 2020  mple)..         
+00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013910: 2020 2020 2020 2078 665f 7361 6d70 6c65         xf_sample
+00013920: 203d 2078 665f 7361 6d70 6c65 5b30 203a   = xf_sample[0 :
+00013930: 206c 656e 2878 665f 7361 6d70 6c65 2920   len(xf_sample) 
+00013940: 2f2f 2032 5d0d 0a20 2020 2020 2020 2020  // 2]..         
+00013950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013960: 2020 2020 2020 2066 6674 746f 7461 6c5f         ffttotal_
+00013970: 7361 6d70 6c65 203d 2066 6674 746f 7461  sample = ffttota
+00013980: 6c5f 7361 6d70 6c65 5b30 203a 206c 656e  l_sample[0 : len
+00013990: 2866 6674 746f 7461 6c5f 7361 6d70 6c65  (ffttotal_sample
+000139a0: 2920 2f2f 2032 5d0d 0a0d 0a20 2020 2020  ) // 2]....     
+000139b0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+000139c0: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
+000139d0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+000139e0: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
+000139f0: 3d20 6578 7061 6e64 6564 5f74 696d 652c  = expanded_time,
+00013a00: 2065 7870 616e 6465 645f 696e 7465 6e73   expanded_intens
+00013a10: 6974 792c 2078 665f 7361 6d70 6c65 2c20  ity, xf_sample, 
+00013a20: 6666 7474 6f74 616c 5f73 616d 706c 650d  ffttotal_sample.
+00013a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013a40: 2020 2020 756e 6971 7565 5f63 6c75 7374      unique_clust
+00013a50: 6572 5f70 726f 7065 7274 6965 735f 7472  er_properties_tr
+00013a60: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
+00013a70: 6e69 7175 655f 6964 5d20 3d20 2063 7572  nique_id] =  cur
+00013a80: 7265 6e74 5f74 696d 652c 2063 7572 7265  rent_time, curre
+00013a90: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
+00013aa0: 2c20 6375 7272 656e 745f 636c 7573 7465  , current_cluste
+00013ab0: 725f 636c 6173 735f 7363 6f72 650d 0a20  r_class_score.. 
+00013ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ad0: 2020 756e 6971 7565 5f73 6861 7065 5f70    unique_shape_p
+00013ae0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00013af0: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
+00013b00: 655f 6964 5d20 3d20 6375 7272 656e 745f  e_id] = current_
+00013b10: 7469 6d65 2c20 6375 7272 656e 745f 7a2c  time, current_z,
+00013b20: 2063 7572 7265 6e74 5f79 2c20 6375 7272   current_y, curr
+00013b30: 656e 745f 782c 2063 7572 7265 6e74 5f72  ent_x, current_r
+00013b40: 6164 6975 732c 2063 7572 7265 6e74 5f76  adius, current_v
+00013b50: 6f6c 756d 652c 2063 7572 7265 6e74 5f65  olume, current_e
+00013b60: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00013b70: 5f66 6972 7374 2c20 6375 7272 656e 745f  _first, current_
+00013b80: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00013b90: 705f 7365 636f 6e64 2c20 6375 7272 656e  p_second, curren
+00013ba0: 745f 7375 7266 6163 655f 6172 6561 2c20  t_surface_area, 
+00013bb0: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
+00013bc0: 636c 6173 732c 2063 7572 7265 6e74 5f63  class, current_c
+00013bd0: 6c75 7374 6572 5f63 6c61 7373 5f73 636f  luster_class_sco
+00013be0: 7265 0d0a 2020 2020 2020 2020 2020 2020  re..            
+00013bf0: 2020 2020 2020 2075 6e69 7175 655f 6479         unique_dy
+00013c00: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
+00013c10: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00013c20: 745f 756e 6971 7565 5f69 645d 203d 2063  t_unique_id] = c
+00013c30: 7572 7265 6e74 5f74 696d 652c 2063 7572  urrent_time, cur
+00013c40: 7265 6e74 5f73 7065 6564 2c20 6375 7272  rent_speed, curr
+00013c50: 656e 745f 6d6f 7469 6f6e 5f61 6e67 6c65  ent_motion_angle
+00013c60: 2c20 6375 7272 656e 745f 6163 6365 6c65  , current_accele
+00013c70: 7261 7469 6f6e 2c20 6375 7272 656e 745f  ration, current_
+00013c80: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00013c90: 736b 2c20 6375 7272 656e 745f 7261 6469  sk, current_radi
+00013ca0: 616c 5f61 6e67 6c65 2c20 6375 7272 656e  al_angle, curren
+00013cb0: 745f 6365 6c6c 5f61 7869 735f 6d61 736b  t_cell_axis_mask
+00013cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013cd0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00013ce0: 5f66 6674 5f70 726f 7065 7274 6965 735b  _fft_properties[
+00013cf0: 7472 6163 6b5f 6964 5d2e 7570 6461 7465  track_id].update
+00013d00: 287b 6375 7272 656e 745f 756e 6971 7565  ({current_unique
+00013d10: 5f69 643a 756e 6971 7565 5f66 6674 5f70  _id:unique_fft_p
+00013d20: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00013d30: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
+00013d40: 655f 6964 5d7d 290d 0a20 2020 2020 2020  e_id]})..       
+00013d50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013d60: 2e75 6e69 7175 655f 636c 7573 7465 725f  .unique_cluster_
+00013d70: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
+00013d80: 5f69 645d 2e75 7064 6174 6528 7b63 7572  _id].update({cur
+00013d90: 7265 6e74 5f75 6e69 7175 655f 6964 3a75  rent_unique_id:u
+00013da0: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
+00013db0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00013dc0: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00013dd0: 5f69 645d 7d29 0d0a 0d0a 2020 2020 2020  _id]})....      
+00013de0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013df0: 662e 756e 6971 7565 5f73 6861 7065 5f70  f.unique_shape_p
+00013e00: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
+00013e10: 6964 5d2e 7570 6461 7465 287b 6375 7272  id].update({curr
+00013e20: 656e 745f 756e 6971 7565 5f69 643a 756e  ent_unique_id:un
+00013e30: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
+00013e40: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
+00013e50: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00013e60: 5d7d 290d 0a20 2020 2020 2020 2020 2020  ]})..           
+00013e70: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00013e80: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
+00013e90: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
+00013ea0: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
+00013eb0: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
+00013ec0: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
+00013ed0: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
+00013ee0: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
+00013ef0: 7d29 0d0a 0d0a 0d0a 2020 2020 2020 2020  })......        
+00013f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f10: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+00013f20: 6566 205f 6469 6374 5f75 7064 6174 6528  ef _dict_update(
+00013f30: 7365 6c66 2c20 756e 6971 7565 5f74 7261  self, unique_tra
+00013f40: 636b 6c65 745f 6964 733a 204c 6973 742c  cklet_ids: List,
+00013f50: 2020 6365 6c6c 5f69 643a 2069 6e74 2c20    cell_id: int, 
+00013f60: 7472 6163 6b5f 6964 3a20 696e 742c 2073  track_id: int, s
+00013f70: 6f75 7263 655f 6964 3a20 696e 742c 2074  ource_id: int, t
+00013f80: 6172 6765 745f 6964 3a20 696e 7429 3a0d  arget_id: int):.
+00013f90: 0a0d 0a20 0d0a 2020 2020 2020 2020 6765  ... ..        ge
+00013fa0: 6e65 7261 7469 6f6e 5f69 6420 3d20 7365  neration_id = se
+00013fb0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00013fc0: 6374 5b63 656c 6c5f 6964 5d0d 0a20 2020  ct[cell_id]..   
+00013fd0: 2020 2020 2074 7261 636b 6c65 745f 6964       tracklet_id
+00013fe0: 203d 2073 656c 662e 7472 6163 6b6c 6574   = self.tracklet
+00013ff0: 5f64 6963 745b 6365 6c6c 5f69 645d 0d0a  _dict[cell_id]..
+00014000: 0d0a 2020 2020 2020 2020 756e 6971 7565  ..        unique
+00014010: 5f69 6420 3d20 7374 7228 7472 6163 6b5f  _id = str(track_
+00014020: 6964 2920 2b20 7374 7228 7365 6c66 2e6d  id) + str(self.m
+00014030: 6178 5f74 7261 636b 5f69 6429 202b 2073  ax_track_id) + s
+00014040: 7472 2867 656e 6572 6174 696f 6e5f 6964  tr(generation_id
+00014050: 2920 2b20 7374 7228 7472 6163 6b6c 6574  ) + str(tracklet
+00014060: 5f69 6429 0d0a 2020 2020 2020 2020 0d0a  _id)..        ..
+00014070: 2020 2020 2020 2020 7665 635f 6d61 736b          vec_mask
+00014080: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+00014090: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000140a0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000140b0: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+000140c0: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
+000140d0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000140e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000140f0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00014100: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+00014110: 5f79 5f6b 6579 5d29 2c20 666c 6f61 7428  _y_key]), float(
+00014120: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014130: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014140: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00014150: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+00014160: 795d 2920 5d0d 0a0d 0a20 2020 2020 2020  y]) ]....       
+00014170: 2076 6563 5f63 656c 6c20 3d20 5b66 6c6f   vec_cell = [flo
+00014180: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014190: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000141a0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+000141b0: 662e 7870 6f73 6964 5f6b 6579 5d29 202c  f.xposid_key]) ,
+000141c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000141d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000141e0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000141f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014200: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00014210: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+00014220: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00014230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014240: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014250: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014260: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014270: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00014280: 295d 0d0a 0d0a 2020 2020 2020 2020 616e  )]....        an
+00014290: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
+000142a0: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
+000142b0: 6563 5f63 656c 6c29 0d0a 0d0a 2020 2020  ec_cell)....    
+000142c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000142d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000142e0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000142f0: 6461 7465 287b 7365 6c66 2e72 6164 6961  date({self.radia
+00014300: 6c5f 616e 676c 655f 6b65 7920 3a20 616e  l_angle_key : an
+00014310: 676c 657d 2920 2020 2020 2020 2020 2020  gle})           
+00014320: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00014330: 2020 2020 2075 6e69 7175 655f 7472 6163       unique_trac
+00014340: 6b6c 6574 5f69 6473 2e61 7070 656e 6428  klet_ids.append(
+00014350: 7374 7228 756e 6971 7565 5f69 6429 290d  str(unique_id)).
+00014360: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00014370: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014380: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014390: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+000143a0: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+000143b0: 203a 204e 6f6e 657d 290d 0a20 2020 2020   : None})..     
+000143c0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+000143d0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000143e0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+000143f0: 6174 6528 7b73 656c 662e 636c 7573 7465  ate({self.cluste
+00014400: 7273 636f 7265 5f6b 6579 203a 2030 7d29  rscore_key : 0})
+00014410: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00014420: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014430: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014440: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014450: 2e75 6e69 7175 6569 645f 6b65 7920 3a20  .uniqueid_key : 
+00014460: 7374 7228 756e 6971 7565 5f69 6429 7d29  str(unique_id)})
+00014470: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00014480: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014490: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000144a0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+000144b0: 2e74 7261 636b 6c65 7469 645f 6b65 7920  .trackletid_key 
+000144c0: 3a20 7374 7228 7472 6163 6b6c 6574 5f69  : str(tracklet_i
+000144d0: 6429 7d29 200d 0a20 2020 2020 2020 2073  d)}) ..        s
+000144e0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000144f0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014500: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00014510: 7b73 656c 662e 6765 6e65 7261 7469 6f6e  {self.generation
+00014520: 6964 5f6b 6579 203a 2073 7472 2867 656e  id_key : str(gen
+00014530: 6572 6174 696f 6e5f 6964 297d 2920 0d0a  eration_id)}) ..
+00014540: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014550: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014560: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014570: 5d2e 7570 6461 7465 287b 7365 6c66 2e74  ].update({self.t
+00014580: 7261 636b 6964 5f6b 6579 203a 2073 7472  rackid_key : str
+00014590: 2874 7261 636b 5f69 6429 7d29 0d0a 2020  (track_id)})..  
+000145a0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000145b0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000145c0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000145d0: 7570 6461 7465 287b 7365 6c66 2e6d 6f74  update({self.mot
+000145e0: 696f 6e5f 616e 676c 655f 6b65 7920 3a20  ion_angle_key : 
+000145f0: 302e 307d 290d 0a20 2020 2020 2020 2073  0.0})..        s
+00014600: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014610: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014620: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00014630: 7b73 656c 662e 7370 6565 645f 6b65 7920  {self.speed_key 
+00014640: 3a20 302e 307d 290d 0a20 2020 2020 2020  : 0.0})..       
+00014650: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014660: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014670: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014680: 6528 7b73 656c 662e 6163 6365 6c65 7261  e({self.accelera
+00014690: 7469 6f6e 5f6b 6579 203a 2030 2e30 7d29  tion_key : 0.0})
+000146a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000146b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000146c0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000146d0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+000146e0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+000146f0: 6d70 5f66 6972 7374 6b65 7920 3a20 4e6f  mp_firstkey : No
+00014700: 6e65 7d29 0d0a 2020 2020 2020 2020 7365  ne})..        se
+00014710: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014720: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014730: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00014740: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+00014750: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
+00014760: 203a 204e 6f6e 657d 290d 0a20 2020 2020   : None})..     
+00014770: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014780: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014790: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+000147a0: 6174 6528 7b73 656c 662e 7375 7266 6163  ate({self.surfac
+000147b0: 655f 6172 6561 5f6b 6579 203a 204e 6f6e  e_area_key : Non
+000147c0: 657d 290d 0a20 2020 2020 2020 2073 656c  e})..        sel
+000147d0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000147e0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+000147f0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00014800: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
+00014810: 6b5f 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  k_key : None})..
+00014820: 0d0a 2020 2020 2020 2020 6966 2073 6f75  ..        if sou
+00014830: 7263 655f 6964 2069 7320 6e6f 7420 4e6f  rce_id is not No
+00014840: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00014850: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014860: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014870: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014880: 6528 7b73 656c 662e 6265 666f 7265 6964  e({self.beforeid
+00014890: 5f6b 6579 203a 2069 6e74 2873 6f75 7263  _key : int(sourc
+000148a0: 655f 6964 297d 290d 0a20 2020 2020 2020  e_id)})..       
+000148b0: 2020 2020 2076 6563 5f31 203d 205b 666c       vec_1 = [fl
+000148c0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000148d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000148e0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+000148f0: 6c66 2e78 706f 7369 645f 6b65 795d 2920  lf.xposid_key]) 
+00014900: 2d20 666c 6f61 7428 7365 6c66 2e75 6e69  - float(self.uni
+00014910: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014920: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
+00014930: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00014940: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
+00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014960: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
+00014970: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014980: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014990: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
+000149a0: 5f6b 6579 5d29 202d 2066 6c6f 6174 2873  _key]) - float(s
+000149b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000149c0: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
+000149d0: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+000149e0: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
+000149f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a00: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+00014a10: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014a20: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014a30: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00014a40: 2e7a 706f 7369 645f 6b65 795d 2920 2d20  .zposid_key]) - 
+00014a50: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00014a60: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014a70: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+00014a80: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+00014a90: 6579 5d29 5d0d 0a20 2020 2020 2020 2020  ey])]..         
+00014aa0: 2020 2073 7065 6564 203d 206e 702e 7371     speed = np.sq
+00014ab0: 7274 286e 702e 646f 7428 7665 635f 312c  rt(np.dot(vec_1,
+00014ac0: 2076 6563 5f31 2929 2f73 656c 662e 7463   vec_1))/self.tc
+00014ad0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00014ae0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014af0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014b00: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014b10: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
+00014b20: 7065 6564 5f6b 6579 203a 2073 7065 6564  peed_key : speed
+00014b30: 7d29 0d0a 0d0a 2020 2020 2020 2020 2020  })....          
+00014b40: 2020 6d6f 7469 6f6e 5f61 6e67 6c65 203d    motion_angle =
+00014b50: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+00014b60: 7665 635f 6d61 736b 2c20 7665 635f 3129  vec_mask, vec_1)
+00014b70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00014b80: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014b90: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014ba0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00014bb0: 287b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ({self.motion_an
+00014bc0: 676c 655f 6b65 7920 3a20 6d6f 7469 6f6e  gle_key : motion
+00014bd0: 5f61 6e67 6c65 7d29 200d 0a0d 0a20 2020  _angle}) ....   
+00014be0: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
+00014bf0: 6365 5f69 6420 696e 2073 656c 662e 6564  ce_id in self.ed
+00014c00: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
+00014c10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014c20: 2020 2020 2020 2070 7265 5f73 6f75 7263         pre_sourc
+00014c30: 655f 6964 203d 2073 656c 662e 6564 6765  e_id = self.edge
+00014c40: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b73  _source_lookup[s
+00014c50: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
+00014c60: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00014c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c80: 2020 2020 2076 6563 5f32 203d 205b 666c       vec_2 = [fl
+00014c90: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014ca0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014cb0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014cc0: 6c66 2e78 706f 7369 645f 6b65 795d 2920  lf.xposid_key]) 
+00014cd0: 2d20 3220 2a20 666c 6f61 7428 7365 6c66  - 2 * float(self
+00014ce0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014cf0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+00014d00: 6365 5f69 6429 5d5b 7365 6c66 2e78 706f  ce_id)][self.xpo
+00014d10: 7369 645f 6b65 795d 2920 2b20 666c 6f61  sid_key]) + floa
+00014d20: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014d30: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014d40: 7428 7072 655f 736f 7572 6365 5f69 6429  t(pre_source_id)
+00014d50: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+00014d60: 795d 292c 200d 0a20 2020 2020 2020 2020  y]), ..         
+00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d80: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
+00014d90: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014da0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014db0: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
+00014dc0: 6579 5d29 202d 2032 202a 2066 6c6f 6174  ey]) - 2 * float
+00014dd0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014de0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014df0: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
+00014e00: 662e 7970 6f73 6964 5f6b 6579 5d29 202b  f.yposid_key]) +
+00014e10: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00014e20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014e30: 6573 5b69 6e74 2870 7265 5f73 6f75 7263  es[int(pre_sourc
+00014e40: 655f 6964 295d 5b73 656c 662e 7970 6f73  e_id)][self.ypos
+00014e50: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
+00014e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e70: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
+00014e80: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014e90: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014ea0: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
+00014eb0: 7369 645f 6b65 795d 2920 2d20 2032 202a  sid_key]) -  2 *
+00014ec0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00014ed0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014ee0: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+00014ef0: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+00014f00: 6579 5d29 202b 2066 6c6f 6174 2873 656c  ey]) + float(sel
+00014f10: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014f20: 6f70 6572 7469 6573 5b69 6e74 2870 7265  operties[int(pre
+00014f30: 5f73 6f75 7263 655f 6964 295d 5b73 656c  _source_id)][sel
+00014f40: 662e 7a70 6f73 6964 5f6b 6579 5d29 5d0d  f.zposid_key])].
+00014f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014f60: 2020 2020 2061 6363 203d 206e 702e 7371       acc = np.sq
+00014f70: 7274 286e 702e 646f 7428 7665 635f 322c  rt(np.dot(vec_2,
+00014f80: 2076 6563 5f32 2929 2f73 656c 662e 7463   vec_2))/self.tc
+00014f90: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00014fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014fc0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00014fd0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014fe0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00014ff0: 7570 6461 7465 287b 7365 6c66 2e61 6363  update({self.acc
+00015000: 656c 6572 6174 696f 6e5f 6b65 7920 3a20  eleration_key : 
+00015010: 6163 637d 290d 0a20 2020 2020 2020 2065  acc})..        e
+00015020: 6c69 6620 736f 7572 6365 5f69 6420 6973  lif source_id is
+00015030: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00015040: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015050: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015060: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015070: 6461 7465 287b 7365 6c66 2e62 6566 6f72  date({self.befor
+00015080: 6569 645f 6b65 7920 3a20 4e6f 6e65 7d29  eid_key : None})
+00015090: 200d 0a20 2020 2020 2020 2020 2020 200d   ..            .
+000150a0: 0a0d 0a20 2020 2020 2020 2069 6620 7461  ...        if ta
+000150b0: 7267 6574 5f69 6420 6973 206e 6f74 204e  rget_id is not N
+000150c0: 6f6e 653a 2020 2020 2020 200d 0a20 2020  one:       ..   
+000150d0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000150e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000150f0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015100: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015110: 6166 7465 7269 645f 6b65 7920 3a20 696e  afterid_key : in
+00015120: 7428 7461 7267 6574 5f69 6429 7d29 200d  t(target_id)}) .
+00015130: 0a20 2020 2020 2020 2065 6c69 6620 7461  .        elif ta
+00015140: 7267 6574 5f69 6420 6973 204e 6f6e 653a  rget_id is None:
+00015150: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00015160: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015170: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015180: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015190: 7365 6c66 2e61 6674 6572 6964 5f6b 6579  self.afterid_key
+000151a0: 203a 204e 6f6e 657d 290d 0a20 2020 2020   : None})..     
+000151b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000151c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015200: 2020 0d0a 2020 2020 6465 6620 5f74 656d    ..    def _tem
+00015210: 706f 7261 6c5f 706c 6f74 735f 7472 6163  poral_plots_trac
+00015220: 6b6d 6174 6528 7365 6c66 293a 0d0a 2020  kmate(self):..  
+00015230: 2020 0d0a 2020 2020 0d0a 2020 2020 0d0a    ..    ..    ..
+00015240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015250: 7365 6c66 2e41 7474 7220 3d20 7b7d 0d0a  self.Attr = {}..
+00015260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015270: 7374 6172 7474 696d 6520 3d20 696e 7428  starttime = int(
+00015280: 6d69 6e28 7365 6c66 2e41 6c6c 5661 6c75  min(self.AllValu
+00015290: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
+000152a0: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
+000152b0: 2020 2020 2020 2020 656e 6474 696d 6520          endtime 
+000152c0: 3d20 696e 7428 6d61 7828 7365 6c66 2e41  = int(max(self.A
+000152d0: 6c6c 5661 6c75 6573 5b73 656c 662e 6672  llValues[self.fr
+000152e0: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
+000152f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00015300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015310: 2073 656c 662e 7469 6d65 203d 205b 5d0d   self.time = [].
+00015320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015330: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00015340: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
+00015350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015360: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00015370: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
+00015380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015390: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+000153a0: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
+000153b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000153c0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+000153d0: 6469 7370 5f79 203d 205b 5d0d 0a0d 0a20  disp_y = [].... 
+000153e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000153f0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00015400: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+00015410: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015420: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+00015430: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
+00015440: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015450: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00015460: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00015470: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015480: 662e 6d69 746f 7469 635f 7661 725f 7261  f.mitotic_var_ra
+00015490: 6469 7573 203d 205b 5d0d 0a0d 0a20 2020  dius = []....   
+000154a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000154b0: 662e 6d69 746f 7469 635f 6d65 616e 5f73  f.mitotic_mean_s
+000154c0: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
+000154d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000154e0: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
+000154f0: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
+00015500: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015510: 6974 6f74 6963 5f6d 6561 6e5f 6163 6320  itotic_mean_acc 
+00015520: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015530: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015540: 6963 5f76 6172 5f61 6363 203d 205b 5d0d  ic_var_acc = [].
+00015550: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00015560: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00015570: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+00015580: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
+00015590: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000155a0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+000155b0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+000155c0: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
+000155d0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000155e0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
+000155f0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00015600: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00015610: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015620: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
+00015630: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
+00015640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015650: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00015660: 635f 6d65 616e 5f64 6973 705f 7a20 3d20  c_mean_disp_z = 
+00015670: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00015680: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00015690: 6f74 6963 5f76 6172 5f64 6973 705f 7a20  otic_var_disp_z 
+000156a0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+000156b0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000156c0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+000156d0: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
+000156e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000156f0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00015700: 6469 7370 5f79 203d 205b 5d0d 0a0d 0a20  disp_y = [].... 
+00015710: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015720: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00015730: 6d65 616e 5f64 6973 705f 7820 3d20 5b5d  mean_disp_x = []
+00015740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015750: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015760: 6963 5f76 6172 5f64 6973 705f 7820 3d20  ic_var_disp_x = 
+00015770: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015780: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00015790: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
+000157a0: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+000157b0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000157c0: 6e5f 6d69 746f 7469 635f 7661 725f 7261  n_mitotic_var_ra
+000157d0: 6469 7573 203d 205b 5d0d 0a0d 0a20 2020  dius = []....   
+000157e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000157f0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00015800: 616e 5f73 7065 6564 203d 205b 5d0d 0a20  an_speed = [].. 
+00015810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015820: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00015830: 7661 725f 7370 6565 6420 3d20 5b5d 0d0a  var_speed = []..
+00015840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015850: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015860: 6963 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ic_mean_acc = []
+00015870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015880: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015890: 6963 5f76 6172 5f61 6363 203d 205b 5d0d  ic_var_acc = [].
+000158a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000158b0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+000158c0: 7469 635f 6d65 616e 5f64 6972 6563 7469  tic_mean_directi
+000158d0: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+000158e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000158f0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015900: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
+00015910: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
+00015920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015930: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015940: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
+00015950: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00015960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015970: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00015980: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
+00015990: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
+000159a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000159b0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+000159c0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
+000159d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000159e0: 2e61 6c6c 5f76 6172 5f64 6973 705f 7a20  .all_var_disp_z 
+000159f0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015a00: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00015a10: 5f6d 6561 6e5f 6469 7370 5f79 203d 205b  _mean_disp_y = [
+00015a20: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015a30: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00015a40: 6469 7370 5f79 203d 205b 5d0d 0a0d 0a20  disp_y = [].... 
+00015a50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015a60: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00015a70: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00015a80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015a90: 6c6c 5f76 6172 5f64 6973 705f 7820 3d20  ll_var_disp_x = 
+00015aa0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015ab0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00015ac0: 6561 6e5f 7261 6469 7573 203d 205b 5d0d  ean_radius = [].
+00015ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015ae0: 2073 656c 662e 616c 6c5f 7661 725f 7261   self.all_var_ra
+00015af0: 6469 7573 203d 205b 5d0d 0a0d 0a20 2020  dius = []....   
+00015b00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015b10: 662e 616c 6c5f 6d65 616e 5f73 7065 6564  f.all_mean_speed
+00015b20: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015b30: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00015b40: 7661 725f 7370 6565 6420 3d20 5b5d 0d0a  var_speed = []..
+00015b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015b60: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00015b70: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
+00015b80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015b90: 6c6c 5f76 6172 5f61 6363 203d 205b 5d0d  ll_var_acc = [].
+00015ba0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00015bb0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00015bc0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00015bd0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+00015be0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015bf0: 6c6c 5f76 6172 5f64 6972 6563 7469 6f6e  ll_var_direction
+00015c00: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
+00015c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015c20: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00015c30: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00015c40: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
+00015c50: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00015c60: 6c5f 7661 725f 6469 7374 616e 6365 5f63  l_var_distance_c
+00015c70: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
+00015c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015c90: 2073 656c 662e 6d69 746f 7469 635f 636c   self.mitotic_cl
+00015ca0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
+00015cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015cc0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015cd0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+00015ce0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015cf0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00015d00: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
+00015d10: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015d20: 2020 2020 2020 616c 6c5f 7370 6f74 735f        all_spots_
+00015d30: 7472 6163 6b73 203d 207b 7d0d 0a20 2020  tracks = {}..   
+00015d40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00015d50: 2028 6b2c 7629 2069 6e20 7365 6c66 2e75   (k,v) in self.u
+00015d60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015d70: 7274 6965 732e 6974 656d 7328 293a 0d0a  rties.items():..
+00015d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00015da0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00015db0: 6c5f 7370 6f74 7320 3d20 7365 6c66 2e75  l_spots = self.u
+00015dc0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015dd0: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
+00015de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015df0: 6966 2073 656c 662e 7472 6163 6b69 645f  if self.trackid_
+00015e00: 6b65 7920 696e 2061 6c6c 5f73 706f 7473  key in all_spots
+00015e10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00015e20: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00015e30: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00015e40: 203d 2061 6c6c 5f73 706f 7473 0d0a 2020   = all_spots..  
+00015e50: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00015e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015e70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00015e80: 2020 2020 6675 7475 7265 7320 3d20 5b5d      futures = []
+00015e90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015ea0: 2020 7769 7468 2063 6f6e 6375 7272 656e    with concurren
+00015eb0: 742e 6675 7475 7265 732e 5468 7265 6164  t.futures.Thread
+00015ec0: 506f 6f6c 4578 6563 7574 6f72 286d 6178  PoolExecutor(max
+00015ed0: 5f77 6f72 6b65 7273 203d 206f 732e 6370  _workers = os.cp
+00015ee0: 755f 636f 756e 7428 2929 2061 7320 6578  u_count()) as ex
+00015ef0: 6563 7574 6f72 3a0d 0a20 2020 2020 2020  ecutor:..       
+00015f00: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00015f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015f20: 2020 2020 2066 6f72 2069 2069 6e20 7471       for i in tq
+00015f30: 646d 2872 616e 6765 2873 7461 7274 7469  dm(range(startti
+00015f40: 6d65 2c20 656e 6474 696d 6529 2c20 746f  me, endtime), to
+00015f50: 7461 6c3d 656e 6474 696d 6520 2d20 7374  tal=endtime - st
+00015f60: 6172 7474 696d 6529 3a0d 0a20 2020 2020  arttime):..     
+00015f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00015f90: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+00015fa0: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
+00015fb0: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
+00015fc0: 636f 6d70 7574 655f 7465 6d70 6f72 616c  compute_temporal
+00015fd0: 2c20 692c 2061 6c6c 5f73 706f 7473 5f74  , i, all_spots_t
+00015fe0: 7261 636b 7329 290d 0a20 0d0a 2020 2020  racks)).. ..    
+00015ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016000: 5b72 2e72 6573 756c 7428 2920 666f 7220  [r.result() for 
+00016010: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
+00016020: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
+00016030: 6574 6564 2866 7574 7572 6573 295d 0d0a  eted(futures)]..
+00016040: 0d0a 0d0a 2020 2020 6465 6620 5f63 6f6d  ....    def _com
+00016050: 7075 7465 5f74 656d 706f 7261 6c28 7365  pute_temporal(se
+00016060: 6c66 2c20 692c 2061 6c6c 5f73 706f 7473  lf, i, all_spots
+00016070: 5f74 7261 636b 7329 3a20 2020 2020 2020  _tracks):       
+00016080: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00016090: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000160a0: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
+000160b0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000160c0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+000160d0: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
+000160e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160f0: 206d 6974 6f74 6963 5f64 6973 705f 7820   mitotic_disp_x 
+00016100: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016110: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00016120: 635f 7261 6469 7573 203d 205b 5d0d 0a20  c_radius = [].. 
+00016130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016140: 2020 206d 6974 6f74 6963 5f73 7065 6564     mitotic_speed
+00016150: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016160: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016170: 6963 5f61 6363 203d 205b 5d0d 0a20 2020  ic_acc = []..   
+00016180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016190: 206d 6974 6f74 6963 5f64 6972 6563 7469   mitotic_directi
+000161a0: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+000161b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000161c0: 2020 2020 2020 6d69 746f 7469 635f 636c        mitotic_cl
+000161d0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
+000161e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000161f0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016200: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00016210: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016220: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00016230: 5f6d 6974 6f74 6963 5f64 6973 705f 7a20  _mitotic_disp_z 
+00016240: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016250: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016260: 746f 7469 635f 6469 7370 5f79 203d 205b  totic_disp_y = [
+00016270: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016280: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016290: 6963 5f64 6973 705f 7820 3d20 5b5d 0d0a  ic_disp_x = []..
+000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162b0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+000162c0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
 000162d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162e0: 6675 7475 7265 7320 3d20 5b5d 0d0a 2020  futures = []..  
-000162f0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00016300: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
-00016310: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
-00016320: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
-00016330: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
-00016340: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
-00016350: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00016360: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00016370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016380: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
-00016390: 616e 6765 2873 7461 7274 7469 6d65 2c20  ange(starttime, 
-000163a0: 656e 6474 696d 6529 2c20 746f 7461 6c3d  endtime), total=
-000163b0: 656e 6474 696d 6520 2d20 7374 6172 7474  endtime - startt
-000163c0: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
+000162e0: 206e 6f6e 5f6d 6974 6f74 6963 5f73 7065   non_mitotic_spe
+000162f0: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
+00016300: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00016310: 5f6d 6974 6f74 6963 5f61 6363 203d 205b  _mitotic_acc = [
+00016320: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016330: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016340: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+00016350: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
+00016360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016370: 6e6f 6e5f 6d69 746f 7469 635f 636c 7573  non_mitotic_clus
+00016380: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
+00016390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163a0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+000163b0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000163c0: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
 000163d0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 000163e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163f0: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
-00016400: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
-00016410: 7562 6d69 7428 7365 6c66 2e5f 636f 6d70  ubmit(self._comp
-00016420: 7574 655f 7465 6d70 6f72 616c 2c20 692c  ute_temporal, i,
-00016430: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00016440: 7329 290d 0a20 0d0a 2020 2020 2020 2020  s)).. ..        
-00016450: 2020 2020 2020 2020 2020 2020 5b72 2e72              [r.r
-00016460: 6573 756c 7428 2920 666f 7220 7220 696e  esult() for r in
-00016470: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-00016480: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
-00016490: 2866 7574 7572 6573 295d 0d0a 0d0a 0d0a  (futures)]......
-000164a0: 2020 2020 6465 6620 5f63 6f6d 7075 7465      def _compute
-000164b0: 5f74 656d 706f 7261 6c28 7365 6c66 2c20  _temporal(self, 
-000164c0: 692c 2061 6c6c 5f73 706f 7473 5f74 7261  i, all_spots_tra
-000164d0: 636b 7329 3a20 2020 2020 2020 2020 2020  cks):           
-000164e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000164f0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016500: 6963 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ic_disp_z = []..
-00016510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016520: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
-00016530: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00016540: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016550: 6f74 6963 5f64 6973 705f 7820 3d20 5b5d  otic_disp_x = []
-00016560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016570: 2020 2020 2020 6d69 746f 7469 635f 7261        mitotic_ra
-00016580: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-00016590: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000165a0: 6974 6f74 6963 5f73 7065 6564 203d 205b  itotic_speed = [
-000165b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000165c0: 2020 2020 2020 206d 6974 6f74 6963 5f61         mitotic_a
-000165d0: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-000165e0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-000165f0: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-00016600: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
-00016610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016620: 2020 6d69 746f 7469 635f 636c 7573 7465    mitotic_cluste
-00016630: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
-00016640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016650: 2020 6d69 746f 7469 635f 6469 7374 616e    mitotic_distan
-00016660: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00016670: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016680: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00016690: 6f74 6963 5f64 6973 705f 7a20 3d20 5b5d  otic_disp_z = []
-000166a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000166b0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-000166c0: 635f 6469 7370 5f79 203d 205b 5d0d 0a20  c_disp_y = [].. 
+000163f0: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
+00016400: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016410: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00016420: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00016430: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00016440: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+00016450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016460: 2020 616c 6c5f 7261 6469 7573 203d 205b    all_radius = [
+00016470: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016480: 2020 2020 2020 2061 6c6c 5f73 7065 6564         all_speed
+00016490: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000164a0: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
+000164b0: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
+000164c0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000164d0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000164e0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+000164f0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00016500: 6c5f 636c 7573 7465 725f 636c 6173 7320  l_cluster_class 
+00016510: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016520: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00016530: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00016540: 203d 205b 5d0d 0a0d 0a0d 0a0d 0a0d 0a20   = [].......... 
+00016550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016560: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+00016570: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016580: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00016590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000165b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165c0: 2020 2020 2063 7572 7265 6e74 5f74 696d       current_tim
+000165d0: 6520 3d20 616c 6c5f 7370 6f74 735f 7472  e = all_spots_tr
+000165e0: 6163 6b73 5b6b 5d5b 7365 6c66 2e66 7261  acks[k][self.fra
+000165f0: 6d65 6964 5f6b 6579 5d0d 0a20 2020 2020  meid_key]..     
+00016600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016610: 2020 2020 2020 206d 6974 6f74 6963 203d         mitotic =
+00016620: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00016630: 735b 6b5d 5b73 656c 662e 6469 7669 6469  s[k][self.dividi
+00016640: 6e67 5f6b 6579 5d0d 0a20 2020 2020 2020  ng_key]..       
+00016650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016660: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016680: 2020 6966 2069 203d 3d20 696e 7428 6375    if i == int(cu
+00016690: 7272 656e 745f 7469 6d65 293a 0d0a 2020  rrent_time):..  
+000166a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166c0: 6966 206d 6974 6f74 6963 3a0d 0a20 2020  if mitotic:..   
 000166d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166e0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-000166f0: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
-00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016710: 6e6f 6e5f 6d69 746f 7469 635f 7261 6469  non_mitotic_radi
-00016720: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-00016730: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00016740: 5f6d 6974 6f74 6963 5f73 7065 6564 203d  _mitotic_speed =
-00016750: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016760: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00016770: 6f74 6963 5f61 6363 203d 205b 5d0d 0a20  otic_acc = [].. 
-00016780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016790: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-000167a0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-000167b0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-000167c0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000167d0: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
-000167e0: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
-000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016800: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
-00016810: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00016820: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016830: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00016840: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00016850: 6c6c 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ll_disp_z = []..
-00016860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016870: 2020 2020 616c 6c5f 6469 7370 5f79 203d      all_disp_y =
-00016880: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016890: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-000168a0: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-000168b0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-000168c0: 6c5f 7261 6469 7573 203d 205b 5d0d 0a20  l_radius = [].. 
+000166e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166f0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+00016700: 705f 7a2e 6170 7065 6e64 2861 6c6c 5f73  p_z.append(all_s
+00016710: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00016720: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00016730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016750: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00016760: 635f 6469 7370 5f79 2e61 7070 656e 6428  c_disp_y.append(
+00016770: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016780: 5b6b 5d5b 7365 6c66 2e79 706f 7369 645f  [k][self.yposid_
+00016790: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000167a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000167c0: 6974 6f74 6963 5f64 6973 705f 782e 6170  itotic_disp_x.ap
+000167d0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000167e0: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
+000167f0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00016800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016820: 2020 2020 6d69 746f 7469 635f 7261 6469      mitotic_radi
+00016830: 7573 2e61 7070 656e 6428 616c 6c5f 7370  us.append(all_sp
+00016840: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00016850: 6c66 2e72 6164 6975 735f 6b65 795d 290d  lf.radius_key]).
+00016860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016880: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00016890: 5f73 7065 6564 2e61 7070 656e 6428 616c  _speed.append(al
+000168a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000168b0: 5d5b 7365 6c66 2e73 7065 6564 5f6b 6579  ][self.speed_key
+000168c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
 000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168e0: 2020 2061 6c6c 5f73 7065 6564 203d 205b     all_speed = [
-000168f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016900: 2020 2020 2020 2061 6c6c 5f61 6363 203d         all_acc =
-00016910: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016920: 2020 2020 2020 2020 2061 6c6c 5f64 6972           all_dir
-00016930: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00016940: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016950: 2020 2020 2020 2020 2020 616c 6c5f 636c            all_cl
-00016960: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
-00016970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016980: 2020 2020 2020 616c 6c5f 6469 7374 616e        all_distan
-00016990: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-000169a0: 5d0d 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020  ]..........     
-000169b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000169c0: 6f72 2028 6b2c 7629 2069 6e20 616c 6c5f  or (k,v) in all_
-000169d0: 7370 6f74 735f 7472 6163 6b73 2e69 7465  spots_tracks.ite
-000169e0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00016a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a20: 2063 7572 7265 6e74 5f74 696d 6520 3d20   current_time = 
-00016a30: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016a40: 5b6b 5d5b 7365 6c66 2e66 7261 6d65 6964  [k][self.frameid
-00016a50: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a70: 2020 206d 6974 6f74 6963 203d 2061 6c6c     mitotic = all
-00016a80: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00016a90: 5b73 656c 662e 6469 7669 6469 6e67 5f6b  [self.dividing_k
-00016aa0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-00016ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016ad0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016ae0: 2069 203d 3d20 696e 7428 6375 7272 656e   i == int(curren
-00016af0: 745f 7469 6d65 293a 0d0a 2020 2020 2020  t_time):..      
+000168e0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+000168f0: 7469 635f 6163 632e 6170 7065 6e64 2861  tic_acc.append(a
+00016900: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00016910: 6b5d 5b73 656c 662e 6163 6365 6c65 7261  k][self.accelera
+00016920: 7469 6f6e 5f6b 6579 5d29 0d0a 2020 2020  tion_key])..    
+00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016950: 2020 2020 6d69 746f 7469 635f 6469 7265      mitotic_dire
+00016960: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00016970: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00016980: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
+00016990: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
+000169a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000169b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169c0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+000169d0: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+000169e0: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
+000169f0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00016a00: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
+00016a10: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
+00016a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00016a50: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+00016a60: 2069 6e20 616c 6c5f 7370 6f74 735f 7472   in all_spots_tr
+00016a70: 6163 6b73 5b6b 5d2e 6b65 7973 2829 203a  acks[k].keys() :
+00016a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ab0: 206d 6974 6f74 6963 5f63 6c75 7374 6572   mitotic_cluster
+00016ac0: 5f63 6c61 7373 2e61 7070 656e 6428 616c  _class.append(al
+00016ad0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00016ae0: 5d5b 7365 6c66 2e63 6c75 7374 6572 636c  ][self.clustercl
+00016af0: 6173 735f 6b65 795d 290d 0a0d 0a0d 0a20  ass_key])...... 
 00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b10: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00016b20: 6974 6f74 6963 3a0d 0a20 2020 2020 2020  itotic:..       
-00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b20: 2069 6620 6e6f 7420 6d69 746f 7469 633a   if not mitotic:
+00016b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b50: 206d 6974 6f74 6963 5f64 6973 705f 7a2e   mitotic_disp_z.
-00016b60: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00016b70: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00016b80: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
-00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b50: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016b60: 746f 7469 635f 6469 7370 5f7a 2e61 7070  totic_disp_z.app
+00016b70: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00016b80: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
+00016b90: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
 00016ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bb0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00016bc0: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
-00016bd0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00016be0: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00016bf0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00016c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c10: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016c20: 6963 5f64 6973 705f 782e 6170 7065 6e64  ic_disp_x.append
-00016c30: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00016c40: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
-00016c50: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00016c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bc0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00016bd0: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
+00016be0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00016bf0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00016c00: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00016c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c20: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016c30: 6d69 746f 7469 635f 6469 7370 5f78 2e61  mitotic_disp_x.a
+00016c40: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00016c50: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e78  tracks[k][self.x
+00016c60: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
 00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c80: 6d69 746f 7469 635f 7261 6469 7573 2e61  mitotic_radius.a
-00016c90: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00016ca0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e72  tracks[k][self.r
-00016cb0: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
-00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ce0: 2020 2020 206d 6974 6f74 6963 5f73 7065       mitotic_spe
-00016cf0: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
-00016d00: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00016d10: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
-00016d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d40: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00016d50: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
-00016d60: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00016d70: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00016d80: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00016d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016db0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
-00016dc0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
-00016dd0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00016de0: 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74 696f  ks[k][self.motio
-00016df0: 6e5f 616e 676c 655f 6b65 795d 290d 0a20  n_angle_key]).. 
-00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e20: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00016e30: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00016e40: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
-00016e50: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00016e60: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
-00016e70: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
-00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2020 2020 6966 2073 656c 662e 636c 7573      if self.clus
-00016eb0: 7465 7263 6c61 7373 5f6b 6579 2069 6e20  terclass_key in 
-00016ec0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016ed0: 5b6b 5d2e 6b65 7973 2829 203a 0d0a 2020  [k].keys() :..  
-00016ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f00: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016f10: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
-00016f20: 7373 2e61 7070 656e 6428 616c 6c5f 7370  ss.append(all_sp
-00016f30: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00016f40: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
-00016f50: 6b65 795d 290d 0a0d 0a0d 0a20 2020 2020  key])......     
-00016f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00016f80: 6e6f 7420 6d69 746f 7469 633a 0d0a 2020  not mitotic:..  
+00016c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c90: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00016ca0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
+00016cb0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00016cc0: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
+00016cd0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00016ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016cf0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016d00: 6e5f 6d69 746f 7469 635f 7370 6565 642e  n_mitotic_speed.
+00016d10: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00016d20: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00016d30: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
+00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d60: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00016d70: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
+00016d80: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00016d90: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+00016da0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
+00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016dd0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
+00016de0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+00016df0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00016e00: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00016e10: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
+00016e20: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e40: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016e50: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00016e60: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+00016e70: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00016e80: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
+00016e90: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+00016ea0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00016eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ec0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016ed0: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
+00016ee0: 735f 6b65 7920 696e 2061 6c6c 5f73 706f  s_key in all_spo
+00016ef0: 7473 5f74 7261 636b 735b 6b5d 2e6b 6579  ts_tracks[k].key
+00016f00: 7328 2920 3a0d 0a20 2020 2020 2020 2020  s() :..         
+00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f30: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00016f40: 635f 636c 7573 7465 725f 636c 6173 732e  c_cluster_class.
+00016f50: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00016f60: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00016f70: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+00016f80: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
 00016f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fb0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00016fc0: 635f 6469 7370 5f7a 2e61 7070 656e 6428  c_disp_z.append(
-00016fd0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016fe0: 5b6b 5d5b 7365 6c66 2e7a 706f 7369 645f  [k][self.zposid_
-00016ff0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00017000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017010: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017020: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00017030: 792e 6170 7065 6e64 2861 6c6c 5f73 706f  y.append(all_spo
-00017040: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017050: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
-00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017080: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00017090: 7469 635f 6469 7370 5f78 2e61 7070 656e  tic_disp_x.appen
-000170a0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000170b0: 6b73 5b6b 5d5b 7365 6c66 2e78 706f 7369  ks[k][self.xposi
-000170c0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170f0: 206e 6f6e 5f6d 6974 6f74 6963 5f72 6164   non_mitotic_rad
-00017100: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
-00017110: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017120: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
-00017130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00017160: 746f 7469 635f 7370 6565 642e 6170 7065  totic_speed.appe
-00017170: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017180: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
-00017190: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-000171a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fa0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00016fb0: 5f7a 2e61 7070 656e 6428 616c 6c5f 7370  _z.append(all_sp
+00016fc0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00016fd0: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
+00016fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017000: 2020 2061 6c6c 5f64 6973 705f 792e 6170     all_disp_y.ap
+00017010: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017020: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
+00017030: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017050: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017060: 6c5f 6469 7370 5f78 2e61 7070 656e 6428  l_disp_x.append(
+00017070: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017080: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
+00017090: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170b0: 2020 2020 2020 2020 2061 6c6c 5f72 6164           all_rad
+000170c0: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
+000170d0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000170e0: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
+000170f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017110: 2020 2020 616c 6c5f 7370 6565 642e 6170      all_speed.ap
+00017120: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017130: 7261 636b 735b 6b5d 5b73 656c 662e 7370  racks[k][self.sp
+00017140: 6565 645f 6b65 795d 290d 0a20 2020 2020  eed_key])..     
+00017150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017160: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017170: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
+00017180: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017190: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+000171a0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
 000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171c0: 206e 6f6e 5f6d 6974 6f74 6963 5f61 6363   non_mitotic_acc
-000171d0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-000171e0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-000171f0: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-00017200: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017220: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017230: 5f6d 6974 6f74 6963 5f64 6972 6563 7469  _mitotic_directi
-00017240: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00017250: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017260: 636b 735b 6b5d 5b73 656c 662e 6d6f 7469  cks[k][self.moti
-00017270: 6f6e 5f61 6e67 6c65 5f6b 6579 5d29 0d0a  on_angle_key])..
-00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171c0: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+000171d0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+000171e0: 652e 6170 7065 6e64 2861 6c6c 5f73 706f  e.append(all_spo
+000171f0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017200: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
+00017210: 6579 5d29 2020 200d 0a20 2020 2020 2020  ey])   ..       
+00017220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017230: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00017240: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00017250: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
+00017260: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017270: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+00017280: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
 00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172a0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-000172b0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
-000172c0: 6c5f 6d61 736b 2e61 7070 656e 6428 616c  l_mask.append(al
-000172d0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000172e0: 5d5b 7365 6c66 2e64 6973 7461 6e63 655f  ][self.distance_
-000172f0: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
-00017300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017320: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00017330: 2e63 6c75 7374 6572 636c 6173 735f 6b65  .clusterclass_ke
-00017340: 7920 696e 2061 6c6c 5f73 706f 7473 5f74  y in all_spots_t
-00017350: 7261 636b 735b 6b5d 2e6b 6579 7328 2920  racks[k].keys() 
-00017360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000172a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000172b0: 2073 656c 662e 636c 7573 7465 7263 6c61   self.clustercla
+000172c0: 7373 5f6b 6579 2069 6e20 616c 6c5f 7370  ss_key in all_sp
+000172d0: 6f74 735f 7472 6163 6b73 5b6b 5d2e 6b65  ots_tracks[k].ke
+000172e0: 7973 2829 203a 0d0a 2020 2020 2020 2020  ys() :..        
+000172f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017310: 2020 2020 2020 2061 6c6c 5f63 6c75 7374         all_clust
+00017320: 6572 5f63 6c61 7373 2e61 7070 656e 6428  er_class.append(
+00017330: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017340: 5b6b 5d5b 7365 6c66 2e63 6c75 7374 6572  [k][self.cluster
+00017350: 636c 6173 735f 6b65 795d 2920 2020 200d  class_key])    .
+00017360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017390: 2020 6e6f 6e5f 6d69 746f 7469 635f 636c    non_mitotic_cl
-000173a0: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
-000173b0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000173c0: 636b 735b 6b5d 5b73 656c 662e 636c 7573  cks[k][self.clus
-000173d0: 7465 7263 6c61 7373 5f6b 6579 5d29 0d0a  terclass_key])..
-000173e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017400: 2020 2020 616c 6c5f 6469 7370 5f7a 2e61      all_disp_z.a
-00017410: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017420: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e7a  tracks[k][self.z
-00017430: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017450: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017460: 6c6c 5f64 6973 705f 792e 6170 7065 6e64  ll_disp_y.append
-00017470: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017480: 735b 6b5d 5b73 656c 662e 7970 6f73 6964  s[k][self.yposid
-00017490: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-000174c0: 7370 5f78 2e61 7070 656e 6428 616c 6c5f  sp_x.append(all_
-000174d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-000174e0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-000174f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017510: 2020 2020 2061 6c6c 5f72 6164 6975 732e       all_radius.
-00017520: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017530: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017540: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
-00017550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017570: 616c 6c5f 7370 6565 642e 6170 7065 6e64  all_speed.append
-00017580: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017590: 735b 6b5d 5b73 656c 662e 7370 6565 645f  s[k][self.speed_
-000175a0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 2020 2020 2020 2020 2061 6c6c 5f61 6363           all_acc
-000175d0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-000175e0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-000175f0: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-00017600: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017620: 2020 2020 2020 2061 6c6c 5f64 6972 6563         all_direc
-00017630: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-00017640: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017650: 7261 636b 735b 6b5d 5b73 656c 662e 6d6f  racks[k][self.mo
-00017660: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 5d29  tion_angle_key])
-00017670: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017690: 2020 2020 2020 2061 6c6c 5f64 6973 7461         all_dista
-000176a0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-000176b0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-000176c0: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-000176d0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000176e0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017700: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00017710: 662e 636c 7573 7465 7263 6c61 7373 5f6b  f.clusterclass_k
-00017720: 6579 2069 6e20 616c 6c5f 7370 6f74 735f  ey in all_spots_
-00017730: 7472 6163 6b73 5b6b 5d2e 6b65 7973 2829  tracks[k].keys()
-00017740: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017770: 2020 2061 6c6c 5f63 6c75 7374 6572 5f63     all_cluster_c
-00017780: 6c61 7373 2e61 7070 656e 6428 616c 6c5f  lass.append(all_
-00017790: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-000177a0: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
-000177b0: 735f 6b65 795d 2920 2020 200d 0a20 2020  s_key])    ..   
-000177c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177e0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-000177f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017800: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-00017810: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
-00017820: 6666 286d 6974 6f74 6963 5f64 6973 705f  ff(mitotic_disp_
-00017830: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
-00017840: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017850: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
-00017860: 286e 702e 6469 6666 286d 6974 6f74 6963  (np.diff(mitotic
-00017870: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
-00017880: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00017890: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-000178a0: 6e70 2e61 6273 286e 702e 6469 6666 286d  np.abs(np.diff(m
-000178b0: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
-000178c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000178d0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-000178e0: 6963 5f64 6973 705f 7a20 3d20 6e70 2e61  ic_disp_z = np.a
-000178f0: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
-00017900: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
-00017910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017920: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00017930: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
-00017940: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
-00017950: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
+00017380: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00017390: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000173a0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+000173b0: 6973 705f 7a20 3d20 6e70 2e61 6273 286e  isp_z = np.abs(n
+000173c0: 702e 6469 6666 286d 6974 6f74 6963 5f64  p.diff(mitotic_d
+000173d0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+000173e0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+000173f0: 6f74 6963 5f64 6973 705f 7920 3d20 6e70  otic_disp_y = np
+00017400: 2e61 6273 286e 702e 6469 6666 286d 6974  .abs(np.diff(mit
+00017410: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
+00017420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017430: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+00017440: 7820 3d20 6e70 2e61 6273 286e 702e 6469  x = np.abs(np.di
+00017450: 6666 286d 6974 6f74 6963 5f64 6973 705f  ff(mitotic_disp_
+00017460: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
+00017470: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00017480: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
+00017490: 6e70 2e61 6273 286e 702e 6469 6666 286e  np.abs(np.diff(n
+000174a0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+000174b0: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+000174c0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+000174d0: 6f74 6963 5f64 6973 705f 7920 3d20 6e70  otic_disp_y = np
+000174e0: 2e61 6273 286e 702e 6469 6666 286e 6f6e  .abs(np.diff(non
+000174f0: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
+00017500: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017510: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00017520: 6963 5f64 6973 705f 7820 3d20 6e70 2e61  ic_disp_x = np.a
+00017530: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
+00017540: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00017550: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017560: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+00017570: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
+00017580: 6666 2861 6c6c 5f64 6973 705f 7a29 290d  ff(all_disp_z)).
+00017590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000175a0: 2020 2020 2061 6c6c 5f64 6973 705f 7920       all_disp_y 
+000175b0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+000175c0: 2861 6c6c 5f64 6973 705f 7929 290d 0a20  (all_disp_y)).. 
+000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175e0: 2020 2061 6c6c 5f64 6973 705f 7820 3d20     all_disp_x = 
+000175f0: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
+00017600: 6c6c 5f64 6973 705f 7829 290d 0a0d 0a0d  ll_disp_x)).....
+00017610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017630: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00017640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017650: 656c 662e 7469 6d65 2e61 7070 656e 6428  elf.time.append(
+00017660: 6920 2a20 7365 6c66 2e74 6361 6c69 6272  i * self.tcalibr
+00017670: 6174 696f 6e29 0d0a 0d0a 2020 2020 2020  ation)....      
+00017680: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017690: 6c66 2e6d 6974 6f74 6963 5f63 6c75 7374  lf.mitotic_clust
+000176a0: 6572 5f63 6c61 7373 2e61 7070 656e 6428  er_class.append(
+000176b0: 6e70 2e61 7361 7272 6179 286d 6974 6f74  np.asarray(mitot
+000176c0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+000176d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000176e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000176f0: 5f6d 6974 6f74 6963 5f63 6c75 7374 6572  _mitotic_cluster
+00017700: 5f63 6c61 7373 2e61 7070 656e 6428 6e70  _class.append(np
+00017710: 2e61 7361 7272 6179 286e 6f6e 5f6d 6974  .asarray(non_mit
+00017720: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
+00017730: 7373 2929 0d0a 2020 2020 2020 2020 2020  ss))..          
+00017740: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00017750: 6c6c 5f63 6c75 7374 6572 5f63 6c61 7373  ll_cluster_class
+00017760: 2e61 7070 656e 6428 6e70 2e61 7361 7272  .append(np.asarr
+00017770: 6179 2861 6c6c 5f63 6c75 7374 6572 5f63  ay(all_cluster_c
+00017780: 6c61 7373 2929 0d0a 0d0a 2020 2020 2020  lass))....      
+00017790: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000177a0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+000177b0: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+000177c0: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+000177d0: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+000177e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000177f0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+00017800: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
+00017810: 6428 6d69 746f 7469 635f 6469 7370 5f7a  d(mitotic_disp_z
+00017820: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00017830: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017840: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00017850: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
+00017860: 6e28 6d69 746f 7469 635f 6469 7370 5f79  n(mitotic_disp_y
+00017870: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00017880: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00017890: 6f74 6963 5f76 6172 5f64 6973 705f 792e  otic_var_disp_y.
+000178a0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+000178b0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
+000178c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000178d0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000178e0: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
+000178f0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00017900: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017920: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00017930: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
+00017940: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00017950: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
 00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017970: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00017980: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
-00017990: 702e 6469 6666 286e 6f6e 5f6d 6974 6f74  p.diff(non_mitot
-000179a0: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
+00017970: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00017980: 6561 6e5f 7261 6469 7573 2e61 7070 656e  ean_radius.appen
+00017990: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+000179a0: 635f 7261 6469 7573 2929 0d0a 2020 2020  c_radius))..    
 000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179c0: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
-000179d0: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
-000179e0: 6c6c 5f64 6973 705f 7a29 290d 0a20 2020  ll_disp_z))..   
-000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a00: 2061 6c6c 5f64 6973 705f 7920 3d20 6e70   all_disp_y = np
-00017a10: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
-00017a20: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
-00017a30: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017a40: 6c6c 5f64 6973 705f 7820 3d20 6e70 2e61  ll_disp_x = np.a
-00017a50: 6273 286e 702e 6469 6666 2861 6c6c 5f64  bs(np.diff(all_d
-00017a60: 6973 705f 7829 290d 0a0d 0a0d 0a20 2020  isp_x))......   
-00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a90: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00017aa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017ab0: 7469 6d65 2e61 7070 656e 6428 6920 2a20  time.append(i * 
-00017ac0: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
-00017ad0: 6e29 0d0a 0d0a 2020 2020 2020 2020 2020  n)....          
-00017ae0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017af0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-00017b00: 6c61 7373 2e61 7070 656e 6428 6e70 2e61  lass.append(np.a
-00017b10: 7361 7272 6179 286d 6974 6f74 6963 5f63  sarray(mitotic_c
-00017b20: 6c75 7374 6572 5f63 6c61 7373 2929 0d0a  luster_class))..
-00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b40: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00017b50: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
-00017b60: 7373 2e61 7070 656e 6428 6e70 2e61 7361  ss.append(np.asa
-00017b70: 7272 6179 286e 6f6e 5f6d 6974 6f74 6963  rray(non_mitotic
-00017b80: 5f63 6c75 7374 6572 5f63 6c61 7373 2929  _cluster_class))
-00017b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017ba0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f63        self.all_c
-00017bb0: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
-00017bc0: 656e 6428 6e70 2e61 7361 7272 6179 2861  end(np.asarray(a
-00017bd0: 6c6c 5f63 6c75 7374 6572 5f63 6c61 7373  ll_cluster_class
-00017be0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00017bf0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017c00: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00017c10: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
-00017c20: 6e28 6d69 746f 7469 635f 6469 7370 5f7a  n(mitotic_disp_z
-00017c30: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00017c40: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00017c50: 6f74 6963 5f76 6172 5f64 6973 705f 7a2e  otic_var_disp_z.
-00017c60: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
-00017c70: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
-00017c80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017c90: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017ca0: 6963 5f6d 6561 6e5f 6469 7370 5f79 2e61  ic_mean_disp_y.a
-00017cb0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00017cc0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
-00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ce0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017cf0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
-00017d00: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-00017d10: 635f 6469 7370 5f79 2929 0d0a 0d0a 2020  c_disp_y))....  
-00017d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d30: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00017d40: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
-00017d50: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
-00017d60: 635f 6469 7370 5f78 2929 0d0a 2020 2020  c_disp_x))..    
-00017d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d80: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00017d90: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
-00017da0: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-00017db0: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
-00017dc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017dd0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00017de0: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-00017df0: 2e6d 6561 6e28 6d69 746f 7469 635f 7261  .mean(mitotic_ra
-00017e00: 6469 7573 2929 0d0a 2020 2020 2020 2020  dius))..        
-00017e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017e20: 2e6d 6974 6f74 6963 5f76 6172 5f72 6164  .mitotic_var_rad
-00017e30: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
-00017e40: 6428 6d69 746f 7469 635f 7261 6469 7573  d(mitotic_radius
-00017e50: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00017e60: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017e70: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
-00017e80: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
-00017e90: 286d 6974 6f74 6963 5f73 7065 6564 2929  (mitotic_speed))
-00017ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017eb0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017ec0: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
-00017ed0: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
-00017ee0: 6963 5f73 7065 6564 2929 0d0a 0d0a 2020  ic_speed))....  
-00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f00: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00017f10: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
-00017f20: 702e 6d65 616e 286d 6974 6f74 6963 5f61  p.mean(mitotic_a
-00017f30: 6363 2929 0d0a 2020 2020 2020 2020 2020  cc))..          
-00017f40: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017f50: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
-00017f60: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00017f70: 6f74 6963 5f61 6363 2929 0d0a 0d0a 2020  otic_acc))....  
-00017f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f90: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00017fa0: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
-00017fb0: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00017fc0: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
-00017fd0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00017fe0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00017ff0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018000: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
-00018010: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00018020: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-00018030: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
-00018040: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
-00018050: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018060: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00018070: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018080: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
-00018090: 6e28 6d69 746f 7469 635f 6469 7374 616e  n(mitotic_distan
-000180a0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180c0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000180d0: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
-000180e0: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
-000180f0: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-00018100: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018110: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018120: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018130: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00018140: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00018150: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018160: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
-00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018180: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018190: 5f76 6172 5f64 6973 705f 7a2e 6170 7065  _var_disp_z.appe
-000181a0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-000181b0: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
-000181c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000181d0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000181e0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-000181f0: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
-00018200: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00018210: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-00018220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018230: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018240: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
-00018250: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-00018260: 635f 6469 7370 5f79 2929 0d0a 0d0a 2020  c_disp_y))....  
+000179c0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+000179d0: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
+000179e0: 702e 7374 6428 6d69 746f 7469 635f 7261  p.std(mitotic_ra
+000179f0: 6469 7573 2929 0d0a 0d0a 2020 2020 2020  dius))....      
+00017a00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017a10: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00017a20: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
+00017a30: 6d65 616e 286d 6974 6f74 6963 5f73 7065  mean(mitotic_spe
+00017a40: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
+00017a50: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017a60: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
+00017a70: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+00017a80: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
+00017a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017aa0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00017ab0: 6963 5f6d 6561 6e5f 6163 632e 6170 7065  ic_mean_acc.appe
+00017ac0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+00017ad0: 6963 5f61 6363 2929 0d0a 2020 2020 2020  ic_acc))..      
+00017ae0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017af0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f61  lf.mitotic_var_a
+00017b00: 6363 2e61 7070 656e 6428 6e70 2e73 7464  cc.append(np.std
+00017b10: 286d 6974 6f74 6963 5f61 6363 2929 0d0a  (mitotic_acc))..
+00017b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017b30: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00017b40: 6963 5f6d 6561 6e5f 6469 7265 6374 696f  ic_mean_directio
+00017b50: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00017b60: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+00017b70: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00017b80: 616e 6765 2929 0d0a 2020 2020 2020 2020  ange))..        
+00017b90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017ba0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6972  .mitotic_var_dir
+00017bb0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+00017bc0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+00017bd0: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+00017be0: 6c5f 6368 616e 6765 2929 0d0a 0d0a 2020  l_change))....  
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c00: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00017c10: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
+00017c20: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00017c30: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+00017c40: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00017c50: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00017c60: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00017c70: 6f74 6963 5f76 6172 5f64 6973 7461 6e63  otic_var_distanc
+00017c80: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00017c90: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00017ca0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
+00017cb0: 6d61 736b 2929 0d0a 0d0a 2020 2020 2020  mask))....      
+00017cc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017cd0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00017ce0: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
+00017cf0: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
+00017d00: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+00017d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d20: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00017d30: 6f74 6963 5f76 6172 5f64 6973 705f 7a2e  otic_var_disp_z.
+00017d40: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00017d50: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
+00017d60: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00017d70: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00017d80: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00017d90: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+00017da0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00017db0: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
+00017dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017dd0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00017de0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
+00017df0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00017e00: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
+00017e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017e20: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00017e30: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00017e40: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
+00017e50: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+00017e60: 7370 5f78 2929 0d0a 2020 2020 2020 2020  sp_x))..        
+00017e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017e80: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00017e90: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+00017ea0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00017eb0: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
+00017ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ed0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00017ee0: 6963 5f6d 6561 6e5f 7261 6469 7573 2e61  ic_mean_radius.a
+00017ef0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00017f00: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
+00017f10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00017f20: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00017f30: 5f6d 6974 6f74 6963 5f76 6172 5f72 6164  _mitotic_var_rad
+00017f40: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
+00017f50: 6428 6e6f 6e5f 6d69 746f 7469 635f 7261  d(non_mitotic_ra
+00017f60: 6469 7573 2929 0d0a 0d0a 2020 2020 2020  dius))....      
+00017f70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017f80: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00017f90: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
+00017fa0: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
+00017fb0: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
+00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fd0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00017fe0: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
+00017ff0: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+00018000: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
+00018010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018020: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018030: 6974 6f74 6963 5f6d 6561 6e5f 6163 632e  itotic_mean_acc.
+00018040: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00018050: 6f6e 5f6d 6974 6f74 6963 5f61 6363 2929  on_mitotic_acc))
+00018060: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018070: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018080: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
+00018090: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
+000180a0: 5f6d 6974 6f74 6963 5f61 6363 2929 0d0a  _mitotic_acc))..
+000180b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000180c0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000180d0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
+000180e0: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+000180f0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00018100: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
+00018110: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00018120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018130: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018140: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+00018150: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+00018160: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00018170: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+00018180: 6c5f 6368 616e 6765 2929 200d 0a0d 0a20  l_change)) .... 
+00018190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181a0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+000181b0: 7469 635f 6d65 616e 5f64 6973 7461 6e63  tic_mean_distanc
+000181c0: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+000181d0: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+000181e0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+000181f0: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+00018200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018210: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00018220: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
+00018230: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+00018240: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00018250: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+00018260: 5f6d 6173 6b29 290d 0a0d 0a0d 0a20 2020  _mask))......   
 00018270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018280: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00018290: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
-000182a0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-000182b0: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
-000182c0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000182d0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000182e0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-000182f0: 705f 782e 6170 7065 6e64 286e 702e 7374  p_x.append(np.st
-00018300: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-00018310: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
-00018320: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018330: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018340: 6561 6e5f 7261 6469 7573 2e61 7070 656e  ean_radius.appen
-00018350: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-00018360: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-00018370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018380: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00018390: 6f74 6963 5f76 6172 5f72 6164 6975 732e  otic_var_radius.
-000183a0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-000183b0: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
-000183c0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000183d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000183e0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-000183f0: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
-00018400: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00018410: 5f73 7065 6564 2929 0d0a 2020 2020 2020  _speed))..      
-00018420: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018430: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00018440: 6172 5f73 7065 6564 2e61 7070 656e 6428  ar_speed.append(
-00018450: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
-00018460: 6963 5f73 7065 6564 2929 0d0a 0d0a 2020  ic_speed))....  
-00018470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018480: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00018490: 6963 5f6d 6561 6e5f 6163 632e 6170 7065  ic_mean_acc.appe
-000184a0: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
-000184b0: 6974 6f74 6963 5f61 6363 2929 0d0a 2020  itotic_acc))..  
-000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184d0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000184e0: 6963 5f76 6172 5f61 6363 2e61 7070 656e  ic_var_acc.appen
-000184f0: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-00018500: 6f74 6963 5f61 6363 2929 0d0a 0d0a 2020  otic_acc))....  
-00018510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018520: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00018530: 6963 5f6d 6561 6e5f 6469 7265 6374 696f  ic_mean_directio
-00018540: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
-00018550: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-00018560: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
-00018570: 6c5f 6368 616e 6765 2929 0d0a 2020 2020  l_change))..    
-00018580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018590: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-000185a0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-000185b0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
-000185c0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-000185d0: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
-000185e0: 616e 6765 2929 200d 0a0d 0a20 2020 2020  ange)) ....     
-000185f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018600: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00018610: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
-00018620: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
-00018630: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
-00018640: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
-00018650: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
-00018660: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018670: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00018680: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-00018690: 6d61 736b 2e61 7070 656e 6428 6e70 2e73  mask.append(np.s
-000186a0: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
-000186b0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000186c0: 6b29 290d 0a0d 0a0d 0a20 2020 2020 2020  k))......       
-000186d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000186e0: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
-000186f0: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
-00018700: 2861 6c6c 5f64 6973 705f 7a29 290d 0a20  (all_disp_z)).. 
-00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018720: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00018730: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00018740: 2e73 7464 2861 6c6c 5f64 6973 705f 7a29  .std(all_disp_z)
-00018750: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018760: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018770: 6c5f 6d65 616e 5f64 6973 705f 792e 6170  l_mean_disp_y.ap
-00018780: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-00018790: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
-000187a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000187b0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
-000187c0: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
-000187d0: 2861 6c6c 5f64 6973 705f 7929 290d 0a0d  (all_disp_y))...
-000187e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000187f0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018800: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
-00018810: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
-00018820: 705f 7829 290d 0a20 2020 2020 2020 2020  p_x))..         
-00018830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018840: 616c 6c5f 7661 725f 6469 7370 5f78 2e61  all_var_disp_x.a
-00018850: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00018860: 5f64 6973 705f 7829 290d 0a0d 0a20 2020  _disp_x))....   
-00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018880: 2073 656c 662e 616c 6c5f 6d65 616e 5f72   self.all_mean_r
-00018890: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-000188a0: 6d65 616e 2861 6c6c 5f72 6164 6975 7329  mean(all_radius)
-000188b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000188c0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-000188d0: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
-000188e0: 6428 6e70 2e73 7464 2861 6c6c 5f72 6164  d(np.std(all_rad
-000188f0: 6975 7329 290d 0a0d 0a20 2020 2020 2020  ius))....       
-00018900: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018910: 662e 616c 6c5f 6d65 616e 5f73 7065 6564  f.all_mean_speed
-00018920: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018930: 616c 6c5f 7370 6565 6429 290d 0a20 2020  all_speed))..   
-00018940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018950: 2073 656c 662e 616c 6c5f 7661 725f 7370   self.all_var_sp
-00018960: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
-00018970: 6428 616c 6c5f 7370 6565 6429 290d 0a0d  d(all_speed))...
-00018980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018990: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-000189a0: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
-000189b0: 2e6d 6561 6e28 616c 6c5f 6163 6329 290d  .mean(all_acc)).
-000189c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189d0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-000189e0: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
-000189f0: 7374 6428 616c 6c5f 6163 6329 290d 0a0d  std(all_acc))...
-00018a00: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00018a10: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018a20: 6c5f 6d65 616e 5f64 6972 6563 7469 6f6e  l_mean_direction
-00018a30: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-00018a40: 286e 702e 6d65 616e 2861 6c6c 5f64 6972  (np.mean(all_dir
-00018a50: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-00018a60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018a70: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018a80: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
-00018a90: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00018aa0: 2e73 7464 2861 6c6c 5f64 6972 6563 7469  .std(all_directi
-00018ab0: 6f6e 616c 5f63 6861 6e67 6529 290d 0a0d  onal_change))...
-00018ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ad0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018ae0: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
-00018af0: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
-00018b00: 6d65 616e 2861 6c6c 5f64 6973 7461 6e63  mean(all_distanc
-00018b10: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
-00018b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b30: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00018b40: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018b50: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
-00018b60: 2861 6c6c 5f64 6973 7461 6e63 655f 6365  (all_distance_ce
-00018b70: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00018ba0: 200d 0a64 6566 2062 6f75 6e64 6172 795f   ..def boundary_
-00018bb0: 706f 696e 7473 286d 6173 6b2c 2078 6361  points(mask, xca
-00018bc0: 6c69 6272 6174 696f 6e2c 2079 6361 6c69  libration, ycali
-00018bd0: 6272 6174 696f 6e2c 207a 6361 6c69 6272  bration, zcalibr
-00018be0: 6174 696f 6e29 3a0d 0a0d 0a20 2020 206e  ation):....    n
-00018bf0: 6469 6d20 3d20 6c65 6e28 6d61 736b 2e73  dim = len(mask.s
-00018c00: 6861 7065 290d 0a20 2020 2074 696d 6564  hape)..    timed
-00018c10: 5f6d 6173 6b20 3d20 7b7d 0d0a 2020 2020  _mask = {}..    
-00018c20: 6d61 736b 203d 206d 6173 6b20 3e20 300d  mask = mask > 0.
-00018c30: 0a20 2020 206d 6173 6b20 3d20 6d61 736b  .    mask = mask
-00018c40: 2e61 7374 7970 6528 2775 696e 7438 2729  .astype('uint8')
-00018c50: 0d0a 2020 2020 2320 5958 2073 6861 7065  ..    # YX shape
-00018c60: 6420 6f62 6a65 6374 0d0a 2020 2020 6966  d object..    if
-00018c70: 206e 6469 6d20 3d3d 2032 3a0d 0a20 2020   ndim == 2:..   
-00018c80: 2020 2020 200d 0a20 2020 2020 2020 2062       ..        b
-00018c90: 6f75 6e64 6172 7920 3d20 6669 6e64 5f62  oundary = find_b
-00018ca0: 6f75 6e64 6172 6965 7328 6d61 736b 290d  oundaries(mask).
-00018cb0: 0a20 2020 2020 2020 2072 6567 696f 6e63  .        regionc
-00018cc0: 656e 7472 6f69 6420 3d20 2830 2c29 202b  entroid = (0,) +
-00018cd0: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
-00018ce0: 6428 626f 756e 6461 7279 2920 0d0a 2020  d(boundary) ..  
-00018cf0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-00018d00: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
-00018d10: 7920 3e20 3029 0d0a 2020 2020 2020 2020  y > 0)..        
-00018d20: 7265 616c 5f69 6e64 6963 6573 203d 206e  real_indices = n
-00018d30: 702e 7472 616e 7370 6f73 6528 6e70 2e61  p.transpose(np.a
-00018d40: 7361 7272 6179 2869 6e64 6963 6573 2929  sarray(indices))
-00018d50: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
-00018d60: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-00018d70: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
-00018d80: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
-00018d90: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-00018da0: 6963 6573 5b6a 5d5b 305d 203d 2072 6561  ices[j][0] = rea
-00018db0: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
-00018dc0: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
-00018dd0: 2020 2020 2020 2020 2020 2020 7265 616c              real
-00018de0: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
-00018df0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00018e00: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
-00018e10: 6f6e 0d0a 0d0a 2020 2020 2020 2020 7472  on....        tr
-00018e20: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
-00018e30: 5472 6565 2872 6561 6c5f 696e 6469 6365  Tree(real_indice
-00018e40: 7329 0d0a 2020 2020 2020 2020 2320 5468  s)..        # Th
-00018e50: 6973 206f 626a 6563 7420 636f 6e74 6169  is object contai
-00018e60: 6e73 206c 6973 7420 6f66 2061 6c6c 2074  ns list of all t
-00018e70: 6865 2070 6f69 6e74 7320 666f 7220 616c  he points for al
-00018e80: 6c20 7468 6520 6c61 6265 6c73 2069 6e20  l the labels in 
-00018e90: 7468 6520 4d61 736b 2069 6d61 6765 2077  the Mask image w
-00018ea0: 6974 6820 7468 6520 6c61 6265 6c20 6964  ith the label id
-00018eb0: 2061 6e64 2076 6f6c 756d 6520 6f66 2065   and volume of e
-00018ec0: 6163 6820 6c61 6265 6c0d 0a20 2020 2020  ach label..     
-00018ed0: 2020 2074 696d 6564 5f6d 6173 6b5b 7374     timed_mask[st
-00018ee0: 7228 3029 5d20 3d20 5b74 7265 652c 2069  r(0)] = [tree, i
-00018ef0: 6e64 6963 6573 2c20 7265 6769 6f6e 6365  ndices, regionce
-00018f00: 6e74 726f 6964 5d0d 0a0d 0a20 2020 2023  ntroid]....    #
-00018f10: 2054 5958 2073 6861 7065 6420 6f62 6a65   TYX shaped obje
-00018f20: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
-00018f30: 3d3d 2033 3a0d 0a0d 0a0d 0a20 2020 2020  == 3:......     
-00018f40: 2020 2066 6f72 2069 2069 6e20 7471 646d     for i in tqdm
-00018f50: 2872 616e 6765 2830 2c20 6d61 736b 2e73  (range(0, mask.s
-00018f60: 6861 7065 5b30 5d29 293a 0d0a 2020 2020  hape[0])):..    
-00018f70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00018f80: 2020 2020 2020 2020 2020 2020 2020 626f                bo
-00018f90: 756e 6461 7279 203d 2066 696e 645f 626f  undary = find_bo
-00018fa0: 756e 6461 7269 6573 286d 6173 6b5b 692c  undaries(mask[i,
-00018fb0: 3a5d 290d 0a20 2020 2020 2020 2020 2020  :])..           
-00018fc0: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
-00018fd0: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
-00018fe0: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
-00018ff0: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
-00019000: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-00019010: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
-00019020: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
-00019030: 2020 2020 2020 2020 2020 2020 7265 616c              real
-00019040: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
-00019050: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
-00019060: 6179 2869 6e64 6963 6573 2929 2e63 6f70  ay(indices)).cop
-00019070: 7928 290d 0a0d 0a20 2020 2020 2020 2020  y()....         
-00019080: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-00019090: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
-000190a0: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
-000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190c0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-000190d0: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
-000190e0: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
-000190f0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019110: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00019120: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
-00019130: 735b 6a5d 5b31 5d20 2a20 7863 616c 6962  s[j][1] * xcalib
-00019140: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
-00019150: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
-00019160: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-00019170: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
-00019180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019190: 2020 7469 6d65 645f 6d61 736b 5b73 7472    timed_mask[str
-000191a0: 2869 295d 203d 205b 7472 6565 2c20 696e  (i)] = [tree, in
-000191b0: 6469 6365 732c 2072 6567 696f 6e63 656e  dices, regioncen
-000191c0: 7472 6f69 645d 0d0a 2020 2020 2020 2020  troid]..        
-000191d0: 2020 2020 0d0a 2020 2020 2320 545a 5958      ..    # TZYX
-000191e0: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
-000191f0: 2020 2020 6966 206e 6469 6d20 3d3d 2034      if ndim == 4
-00019200: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
-00019210: 2827 4d61 736b 7320 6d61 6465 2069 6e74  ('Masks made int
-00019220: 6f20 6120 3444 2063 796c 696e 6465 722c  o a 4D cylinder,
-00019230: 2075 7027 290d 0a20 2020 2020 2020 2062   up')..        b
-00019240: 6f75 6e64 6172 7920 3d20 6e70 2e7a 6572  oundary = np.zer
-00019250: 6f73 280d 0a20 2020 2020 2020 2020 2020  os(..           
-00019260: 205b 6d61 736b 2e73 6861 7065 5b30 5d2c   [mask.shape[0],
-00019270: 206d 6173 6b2e 7368 6170 655b 315d 2c20   mask.shape[1], 
-00019280: 6d61 736b 2e73 6861 7065 5b32 5d2c 206d  mask.shape[2], m
-00019290: 6173 6b2e 7368 6170 655b 335d 5d0d 0a20  ask.shape[3]].. 
-000192a0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000192b0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-000192c0: 2830 2c20 6d61 736b 2e73 6861 7065 5b30  (0, mask.shape[0
-000192d0: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
-000192e0: 200d 0a20 2020 2020 2020 2020 2020 2062   ..            b
-000192f0: 6f75 6e64 6172 795b 692c 3a5d 203d 2066  oundary[i,:] = f
-00019300: 696e 645f 626f 756e 6461 7269 6573 286d  ind_boundaries(m
-00019310: 6173 6b5b 692c 3a5d 290d 0a20 2020 2020  ask[i,:])..     
-00019320: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
-00019330: 7472 6f69 6420 3d20 636f 6d70 7574 655f  troid = compute_
-00019340: 6365 6e74 726f 6964 2862 6f75 6e64 6172  centroid(boundar
-00019350: 795b 692c 3a5d 2920 0d0a 2020 2020 2020  y[i,:]) ..      
-00019360: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-00019370: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
-00019380: 795b 692c 3a5d 203e 2030 290d 0a20 2020  y[i,:] > 0)..   
-00019390: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-000193a0: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
-000193b0: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
-000193c0: 696e 6469 6365 7329 292e 636f 7079 2829  indices)).copy()
-000193d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000193e0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
-000193f0: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
-00019400: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
-00019410: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00019420: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
-00019430: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-00019440: 5d5b 305d 202a 207a 6361 6c69 6272 6174  ][0] * zcalibrat
-00019450: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00019460: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-00019470: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
-00019480: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-00019490: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
-000194a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000194b0: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-000194c0: 735b 6a5d 5b32 5d20 3d20 7265 616c 5f69  s[j][2] = real_i
-000194d0: 6e64 6963 6573 5b6a 5d5b 325d 202a 2078  ndices[j][2] * x
-000194e0: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
-000194f0: 2020 2020 2020 2020 2020 2074 7265 6520             tree 
-00019500: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
-00019510: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
-00019520: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-00019530: 6564 5f6d 6173 6b5b 7374 7228 6929 5d20  ed_mask[str(i)] 
-00019540: 3d20 5b74 7265 652c 2069 6e64 6963 6573  = [tree, indices
-00019550: 2c20 7265 6769 6f6e 6365 6e74 726f 6964  , regioncentroid
-00019560: 5d0d 0a20 2020 2070 7269 6e74 2827 436f  ]..    print('Co
-00019570: 6d70 7574 6564 2074 6865 2062 6f75 6e64  mputed the bound
-00019580: 6172 7920 706f 696e 7473 2729 0d0a 0d0a  ary points')....
-00019590: 2020 2020 7265 7475 726e 2074 696d 6564      return timed
-000195a0: 5f6d 6173 6b2c 2062 6f75 6e64 6172 7920  _mask, boundary 
-000195b0: 2020 2020 2020 200d 0a0d 0a64 6566 2063         ....def c
-000195c0: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
-000195d0: 6269 6e61 7279 5f69 6d61 6765 293a 0d0a  binary_image):..
-000195e0: 2020 2020 2320 456e 7375 7265 2062 696e      # Ensure bin
-000195f0: 6172 7920 696d 6167 6520 6973 2061 204e  ary image is a N
-00019600: 756d 5079 2061 7272 6179 0d0a 2020 2020  umPy array..    
-00019610: 6269 6e61 7279 5f69 6d61 6765 203d 206e  binary_image = n
-00019620: 702e 6172 7261 7928 6269 6e61 7279 5f69  p.array(binary_i
-00019630: 6d61 6765 290d 0a0d 0a20 2020 2077 6869  mage)....    whi
-00019640: 7465 5f70 6978 656c 7320 3d20 6e70 2e77  te_pixels = np.w
-00019650: 6865 7265 2862 696e 6172 795f 696d 6167  here(binary_imag
-00019660: 6520 3d3d 2031 290d 0a20 2020 206e 756d  e == 1)..    num
-00019670: 5f70 6978 656c 7320 3d20 6c65 6e28 7768  _pixels = len(wh
-00019680: 6974 655f 7069 7865 6c73 5b30 5d29 0d0a  ite_pixels[0])..
-00019690: 0d0a 2020 2020 2320 436f 6d70 7574 6520  ..    # Compute 
-000196a0: 7468 6520 6365 6e74 726f 6964 206f 6620  the centroid of 
-000196b0: 7468 6520 7768 6974 6520 7069 7865 6c73  the white pixels
-000196c0: 2069 6e20 7468 6520 626f 756e 6461 7279   in the boundary
-000196d0: 2069 6d61 6765 0d0a 2020 2020 6365 6e74   image..    cent
-000196e0: 726f 6964 203d 206e 702e 7a65 726f 7328  roid = np.zeros(
-000196f0: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
-00019700: 6d29 0d0a 2020 2020 666f 7220 6469 6d20  m)..    for dim 
-00019710: 696e 2072 616e 6765 2862 696e 6172 795f  in range(binary_
-00019720: 696d 6167 652e 6e64 696d 293a 0d0a 2020  image.ndim):..  
-00019730: 2020 2020 2020 6365 6e74 726f 6964 5b64        centroid[d
-00019740: 696d 5d20 3d20 7768 6974 655f 7069 7865  im] = white_pixe
-00019750: 6c73 5b64 696d 5d2e 7375 6d28 2920 2f20  ls[dim].sum() / 
-00019760: 6e75 6d5f 7069 7865 6c73 0d0a 0d0a 2020  num_pixels....  
-00019770: 2020 7265 7475 726e 2063 656e 7472 6f69    return centroi
-00019780: 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465  d........ ....de
-00019790: 6620 6765 745f 6373 765f 6461 7461 2863  f get_csv_data(c
-000197a0: 7376 293a 0d0a 0d0a 2020 2020 2020 2020  sv):....        
-000197b0: 6461 7461 7365 7420 3d20 7064 2e72 6561  dataset = pd.rea
-000197c0: 645f 6373 7628 0d0a 2020 2020 2020 2020  d_csv(..        
-000197d0: 2020 2020 6373 762c 2064 656c 696d 6974      csv, delimit
-000197e0: 6572 3d22 2c22 2c20 656e 636f 6469 6e67  er=",", encoding
-000197f0: 3d22 756e 6963 6f64 655f 6573 6361 7065  ="unicode_escape
-00019800: 222c 206c 6f77 5f6d 656d 6f72 793d 4661  ", low_memory=Fa
-00019810: 6c73 650d 0a20 2020 2020 2020 2029 5b33  lse..        )[3
-00019820: 3a5d 0d0a 2020 2020 2020 2020 6461 7461  :]..        data
-00019830: 7365 745f 696e 6465 7820 3d20 6461 7461  set_index = data
-00019840: 7365 742e 696e 6465 780d 0a20 2020 2020  set.index..     
-00019850: 2020 2072 6574 7572 6e20 6461 7461 7365     return datase
-00019860: 742c 2064 6174 6173 6574 5f69 6e64 6578  t, dataset_index
-00019870: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
-00019880: 7370 6f74 5f64 6174 6173 6574 2873 706f  spot_dataset(spo
-00019890: 745f 6461 7461 7365 742c 2074 7261 636b  t_dataset, track
-000198a0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-000198b0: 6579 732c 2078 6361 6c69 6272 6174 696f  eys, xcalibratio
-000198c0: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
-000198d0: 207a 6361 6c69 6272 6174 696f 6e2c 2041   zcalibration, A
-000198e0: 7474 7269 6275 7465 426f 786e 616d 652c  ttributeBoxname,
-000198f0: 2064 6574 6563 7469 6f6e 6368 616e 6e65   detectionchanne
-00019900: 6c29 3a0d 0a20 2020 2020 2020 2041 6c6c  l):..        All
-00019910: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
-00019920: 2020 2020 2070 6f73 6978 203d 2074 7261       posix = tra
-00019930: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00019940: 5f6b 6579 735b 2270 6f73 6978 225d 0d0a  _keys["posix"]..
-00019950: 2020 2020 2020 2020 706f 7369 7920 3d20          posiy = 
-00019960: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-00019970: 706f 745f 6b65 7973 5b22 706f 7369 7922  pot_keys["posiy"
-00019980: 5d0d 0a20 2020 2020 2020 2070 6f73 697a  ]..        posiz
-00019990: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
-000199a0: 735f 7370 6f74 5f6b 6579 735b 2270 6f73  s_spot_keys["pos
-000199b0: 697a 225d 0d0a 2020 2020 2020 2020 6672  iz"]..        fr
-000199c0: 616d 6520 3d20 7472 6163 6b5f 616e 616c  ame = track_anal
-000199d0: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-000199e0: 6672 616d 6522 5d0d 0a20 2020 2020 2020  frame"]..       
-000199f0: 200d 0a20 2020 2020 2020 204c 6f63 6174   ..        Locat
-00019a00: 696f 6e58 203d 2028 0d0a 2020 2020 2020  ionX = (..      
-00019a10: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
-00019a20: 6574 5b70 6f73 6978 5d2e 6173 7479 7065  et[posix].astype
-00019a30: 2822 666c 6f61 7422 2920 2f20 7863 616c  ("float") / xcal
-00019a40: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00019a50: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
-00019a60: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
-00019a70: 696f 6e59 203d 2028 0d0a 2020 2020 2020  ionY = (..      
-00019a80: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
-00019a90: 6574 5b70 6f73 6979 5d2e 6173 7479 7065  et[posiy].astype
-00019aa0: 2822 666c 6f61 7422 2920 2f20 7963 616c  ("float") / ycal
-00019ab0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00019ac0: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
-00019ad0: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
-00019ae0: 696f 6e5a 203d 2028 0d0a 2020 2020 2020  ionZ = (..      
-00019af0: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
-00019b00: 6574 5b70 6f73 697a 5d2e 6173 7479 7065  et[posiz].astype
-00019b10: 2822 666c 6f61 7422 2920 2f20 7a63 616c  ("float") / zcal
-00019b20: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00019b30: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
-00019b40: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
-00019b50: 696f 6e54 203d 2028 7370 6f74 5f64 6174  ionT = (spot_dat
-00019b60: 6173 6574 5b66 7261 6d65 5d2e 6173 7479  aset[frame].asty
-00019b70: 7065 2822 666c 6f61 7422 2929 2e61 7374  pe("float")).ast
-00019b80: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
-00019b90: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-00019ba0: 6967 6e6f 7265 5f76 616c 7565 7320 3d20  ignore_values = 
-00019bb0: 5b74 7261 636b 5f61 6e61 6c79 7369 735f  [track_analysis_
-00019bc0: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
-00019bd0: 696e 7465 6e73 6974 7922 5d2c 7472 6163  intensity"],trac
-00019be0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00019bf0: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
-00019c00: 6e73 6974 7922 5d5d 200d 0a20 2020 2020  nsity"]] ..     
-00019c10: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
-00019c20: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-00019c30: 706f 745f 6b65 7973 2e69 7465 6d73 2829  pot_keys.items()
-00019c40: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00019c50: 2020 2020 2069 6620 6465 7465 6374 696f       if detectio
-00019c60: 6e63 6861 6e6e 656c 203d 3d20 313a 0d0a  nchannel == 1:..
-00019c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c80: 2020 2020 2069 6620 6b20 3d3d 2022 6d65       if k == "me
-00019c90: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
-00019ca0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-00019cb0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00019cc0: 616c 7565 203d 2074 7261 636b 5f61 6e61  alue = track_ana
-00019cd0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-00019ce0: 226d 6561 6e5f 696e 7465 6e73 6974 7922  "mean_intensity"
-00019cf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00019d00: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-00019d10: 6c56 616c 7565 735b 7661 6c75 655d 203d  lValues[value] =
-00019d20: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
-00019d30: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-00019d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019d50: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
-00019d60: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-00019d70: 6368 3222 3a0d 0a20 2020 2020 2020 2020  ch2":..         
-00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d90: 2020 7661 6c75 6520 3d20 7472 6163 6b5f    value = track_
-00019da0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-00019db0: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
-00019dc0: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
-00019dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019de0: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
-00019df0: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
-00019e00: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
-00019e10: 6174 2229 2020 2020 2020 200d 0a0d 0a20  at")       .... 
-00019e20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00019e30: 6620 7620 6e6f 7420 696e 2069 676e 6f72  f v not in ignor
-00019e40: 655f 7661 6c75 6573 3a0d 0a20 2020 2020  e_values:..     
-00019e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e60: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00019e70: 2020 2020 2020 2020 2020 2041 6c6c 5661             AllVa
-00019e80: 6c75 6573 5b76 5d20 3d20 7370 6f74 5f64  lues[v] = spot_d
-00019e90: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
-00019ea0: 2822 666c 6f61 7422 290d 0a0d 0a20 2020  ("float")....   
-00019eb0: 2020 2020 2041 6c6c 5661 6c75 6573 5b70       AllValues[p
-00019ec0: 6f73 6978 5d20 3d20 726f 756e 6428 4c6f  osix] = round(Lo
-00019ed0: 6361 7469 6f6e 582c 3329 0d0a 2020 2020  cationX,3)..    
-00019ee0: 2020 2020 416c 6c56 616c 7565 735b 706f      AllValues[po
-00019ef0: 7369 795d 203d 2072 6f75 6e64 284c 6f63  siy] = round(Loc
-00019f00: 6174 696f 6e59 2c33 290d 0a20 2020 2020  ationY,3)..     
-00019f10: 2020 2041 6c6c 5661 6c75 6573 5b70 6f73     AllValues[pos
-00019f20: 697a 5d20 3d20 726f 756e 6428 4c6f 6361  iz] = round(Loca
-00019f30: 7469 6f6e 5a2c 3329 0d0a 2020 2020 2020  tionZ,3)..      
-00019f40: 2020 416c 6c56 616c 7565 735b 6672 616d    AllValues[fram
-00019f50: 655d 203d 2072 6f75 6e64 284c 6f63 6174  e] = round(Locat
-00019f60: 696f 6e54 2c33 290d 0a20 2020 2020 2020  ionT,3)..       
-00019f70: 2041 7474 7269 6275 7465 6964 7320 3d20   Attributeids = 
-00019f80: 5b5d 0d0a 2020 2020 2020 2020 4174 7472  []..        Attr
-00019f90: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
-00019fa0: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
-00019fb0: 290d 0a20 2020 2020 2020 2066 6f72 2061  )..        for a
-00019fc0: 7474 7269 6275 7465 6e61 6d65 2069 6e20  ttributename in 
-00019fd0: 416c 6c56 616c 7565 732e 6b65 7973 2829  AllValues.keys()
-00019fe0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019ff0: 2041 7474 7269 6275 7465 6964 732e 6170   Attributeids.ap
-0001a000: 7065 6e64 2861 7474 7269 6275 7465 6e61  pend(attributena
-0001a010: 6d65 2920 2020 200d 0a20 2020 2020 2020  me)    ..       
-0001a020: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-0001a030: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a040: 4174 7472 6962 7574 6569 6473 2c20 416c  Attributeids, Al
-0001a050: 6c56 616c 7565 7320 2020 2020 0d0a 2020  lValues     ..  
-0001a060: 2020 0d0a 6465 6620 6765 745f 7472 6163    ..def get_trac
-0001a070: 6b5f 6461 7461 7365 7428 7472 6163 6b5f  k_dataset(track_
-0001a080: 6461 7461 7365 742c 2074 7261 636b 5f61  dataset, track_a
-0001a090: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001a0a0: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
-0001a0b0: 735f 7472 6163 6b5f 6b65 7973 2c20 5472  s_track_keys, Tr
-0001a0c0: 6163 6b41 7474 7269 6275 7465 426f 786e  ackAttributeBoxn
-0001a0d0: 616d 6529 3a0d 0a0d 0a20 2020 2020 2020  ame):....       
-0001a0e0: 2041 6c6c 5472 6163 6b56 616c 7565 7320   AllTrackValues 
-0001a0f0: 3d20 7b7d 0d0a 2020 2020 2020 2020 7472  = {}..        tr
-0001a100: 6163 6b5f 6964 203d 2074 7261 636b 5f61  ack_id = track_a
-0001a110: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001a120: 735b 2274 7261 636b 5f69 6422 5d0d 0a20  s["track_id"].. 
-0001a130: 2020 2020 2020 2054 6964 203d 2074 7261         Tid = tra
-0001a140: 636b 5f64 6174 6173 6574 5b74 7261 636b  ck_dataset[track
-0001a150: 5f69 645d 2e61 7374 7970 6528 2266 6c6f  _id].astype("flo
-0001a160: 6174 2229 0d0a 2020 2020 2020 200d 0a20  at")..       .. 
-0001a170: 2020 2020 2020 2041 6c6c 5472 6163 6b56         AllTrackV
-0001a180: 616c 7565 735b 7472 6163 6b5f 6964 5d20  alues[track_id] 
-0001a190: 3d20 5469 640d 0a20 2020 2020 200d 0a20  = Tid..      .. 
-0001a1a0: 2020 2020 2020 2066 6f72 2028 6b2c 2076         for (k, v
-0001a1b0: 2920 696e 2074 7261 636b 5f61 6e61 6c79  ) in track_analy
-0001a1c0: 7369 735f 7472 6163 6b5f 6b65 7973 2e69  sis_track_keys.i
-0001a1d0: 7465 6d73 2829 3a0d 0a0d 0a20 2020 2020  tems():....     
-0001a1e0: 2020 2020 2020 2020 2020 2078 203d 2074             x = t
-0001a1f0: 7261 636b 5f64 6174 6173 6574 5b76 5d2e  rack_dataset[v].
-0001a200: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-0001a210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a220: 206d 696e 7661 6c20 3d20 6d69 6e28 7829   minval = min(x)
-0001a230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a240: 2020 6d61 7876 616c 203d 206d 6178 2878    maxval = max(x
-0001a250: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0001a260: 2020 2020 2069 6620 6d69 6e76 616c 203e       if minval >
-0001a270: 2030 2061 6e64 206d 6178 7661 6c20 3c3d   0 and maxval <=
-0001a280: 2031 3a0d 0a0d 0a20 2020 2020 2020 2020   1:....         
-0001a290: 2020 2020 2020 2020 2020 2078 203d 2078             x = x
-0001a2a0: 202b 2031 0d0a 0d0a 2020 2020 2020 2020   + 1....        
-0001a2b0: 2020 2020 2020 2020 416c 6c54 7261 636b          AllTrack
-0001a2c0: 5661 6c75 6573 5b6b 5d20 3d20 726f 756e  Values[k] = roun
-0001a2d0: 6428 782c 2033 290d 0a0d 0a20 2020 2020  d(x, 3)....     
-0001a2e0: 2020 2054 7261 636b 4174 7472 6962 7574     TrackAttribut
-0001a2f0: 6569 6473 203d 205b 5d0d 0a20 2020 2020  eids = []..     
-0001a300: 2020 2054 7261 636b 4174 7472 6962 7574     TrackAttribut
-0001a310: 6569 6473 2e61 7070 656e 6428 5472 6163  eids.append(Trac
-0001a320: 6b41 7474 7269 6275 7465 426f 786e 616d  kAttributeBoxnam
-0001a330: 6529 0d0a 2020 2020 2020 2020 666f 7220  e)..        for 
-0001a340: 6174 7472 6962 7574 656e 616d 6520 696e  attributename in
-0001a350: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a360: 7472 6163 6b5f 6b65 7973 2e6b 6579 7328  track_keys.keys(
-0001a370: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001a380: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
-0001a390: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
-0001a3a0: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
-0001a3b0: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
-0001a3c0: 6e20 5472 6163 6b41 7474 7269 6275 7465  n TrackAttribute
-0001a3d0: 6964 732c 2041 6c6c 5472 6163 6b56 616c  ids, AllTrackVal
-0001a3e0: 7565 730d 0a20 2020 200d 0a64 6566 2067  ues..    ..def g
-0001a3f0: 6574 5f65 6467 6573 5f64 6174 6173 6574  et_edges_dataset
-0001a400: 2865 6467 6573 5f64 6174 6173 6574 2c20  (edges_dataset, 
-0001a410: 6564 6765 735f 6461 7461 7365 745f 696e  edges_dataset_in
-0001a420: 6465 782c 2074 7261 636b 5f61 6e61 6c79  dex, track_analy
-0001a430: 7369 735f 7370 6f74 5f6b 6579 732c 2074  sis_spot_keys, t
-0001a440: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
-0001a450: 6765 735f 6b65 7973 293a 0d0a 0d0a 2020  ges_keys):....  
-0001a460: 2020 2020 2020 416c 6c45 6467 6573 5661        AllEdgesVa
-0001a470: 6c75 6573 203d 207b 7d0d 0a20 2020 2020  lues = {}..     
-0001a480: 2020 2074 7261 636b 5f69 6420 3d20 7472     track_id = tr
-0001a490: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001a4a0: 745f 6b65 7973 5b22 7472 6163 6b5f 6964  t_keys["track_id
-0001a4b0: 225d 0d0a 2020 2020 2020 2020 5469 6420  "]..        Tid 
-0001a4c0: 3d20 6564 6765 735f 6461 7461 7365 745b  = edges_dataset[
-0001a4d0: 7472 6163 6b5f 6964 5d2e 6173 7479 7065  track_id].astype
-0001a4e0: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
-0001a4f0: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
-0001a500: 7768 6572 6528 5469 6420 3d3d 2030 290d  where(Tid == 0).
-0001a510: 0a20 2020 2020 2020 206d 6178 7472 6163  .        maxtrac
-0001a520: 6b5f 6964 203d 206d 6178 2854 6964 290d  k_id = max(Tid).
-0001a530: 0a20 2020 2020 2020 2063 6f6e 6469 7469  .        conditi
-0001a540: 6f6e 5f69 6e64 6963 6573 203d 2065 6467  on_indices = edg
-0001a550: 6573 5f64 6174 6173 6574 5f69 6e64 6578  es_dataset_index
-0001a560: 5b69 6e64 6963 6573 5d0d 0a20 2020 2020  [indices]..     
-0001a570: 2020 2054 6964 5b63 6f6e 6469 7469 6f6e     Tid[condition
-0001a580: 5f69 6e64 6963 6573 5d20 3d20 6d61 7874  _indices] = maxt
-0001a590: 7261 636b 5f69 6420 2b20 310d 0a20 2020  rack_id + 1..   
-0001a5a0: 2020 2020 2041 6c6c 4564 6765 7356 616c       AllEdgesVal
-0001a5b0: 7565 735b 7472 6163 6b5f 6964 5d20 3d20  ues[track_id] = 
-0001a5c0: 5469 640d 0a0d 0a20 2020 2020 2020 2066  Tid....        f
-0001a5d0: 6f72 206b 2069 6e20 7472 6163 6b5f 616e  or k in track_an
-0001a5e0: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
-0001a5f0: 732e 7661 6c75 6573 2829 3a0d 0a0d 0a20  s.values():.... 
-0001a600: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
-0001a610: 213d 2074 7261 636b 5f69 643a 0d0a 2020  != track_id:..  
-0001a620: 2020 2020 2020 2020 2020 2020 2020 7820                x 
-0001a630: 3d20 6564 6765 735f 6461 7461 7365 745b  = edges_dataset[
-0001a640: 6b5d 2e61 7374 7970 6528 2266 6c6f 6174  k].astype("float
-0001a650: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
-0001a660: 2020 2020 2020 416c 6c45 6467 6573 5661        AllEdgesVa
-0001a670: 6c75 6573 5b6b 5d20 3d20 7820 2020 0d0a  lues[k] = x   ..
-0001a680: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001a690: 2020 2072 6574 7572 6e20 416c 6c45 6467     return AllEdg
-0001a6a0: 6573 5661 6c75 6573 2020 200d 0a20 2020  esValues   ..   
-0001a6b0: 200d 0a20 2020 2020 2020 0d0a 2020 2020   ..       ..    
-0001a6c0: 0d0a 6465 6620 7363 616c 655f 7661 6c75  ..def scale_valu
-0001a6d0: 6528 782c 2073 6361 6c65 203d 2032 3535  e(x, scale = 255
-0001a6e0: 202a 2032 3535 293a 0d0a 0d0a 0d0a 2020   * 255):......  
-0001a6f0: 2020 2072 6574 7572 6e20 7820 2a20 7363     return x * sc
-0001a700: 616c 6520 2020 0d0a 2020 2020 0d0a 0d0a  ale   ..    ....
-0001a710: 0d0a 6465 6620 7072 6f62 5f73 6967 6d6f  ..def prob_sigmo
-0001a720: 6964 2878 293a 0d0a 2020 2020 7265 7475  id(x):..    retu
-0001a730: 726e 2031 202d 206d 6174 682e 6578 7028  rn 1 - math.exp(
-0001a740: 2d78 290d 0a0d 0a0d 0a64 6566 2061 6e67  -x)......def ang
-0001a750: 756c 6172 5f63 6861 6e67 6528 7665 635f  ular_change(vec_
-0001a760: 302c 2076 6563 5f31 293a 0d0a 2020 2020  0, vec_1):..    
-0001a770: 2020 2020 0d0a 2020 2020 2020 2020 7665      ..        ve
-0001a780: 635f 3020 3d20 7665 635f 3020 2f20 6e70  c_0 = vec_0 / np
-0001a790: 2e6c 696e 616c 672e 6e6f 726d 2876 6563  .linalg.norm(vec
-0001a7a0: 5f30 290d 0a20 2020 2020 2020 2076 6563  _0)..        vec
-0001a7b0: 5f31 203d 2076 6563 5f31 202f 206e 702e  _1 = vec_1 / np.
-0001a7c0: 6c69 6e61 6c67 2e6e 6f72 6d28 7665 635f  linalg.norm(vec_
-0001a7d0: 3129 0d0a 2020 2020 2020 2020 616e 676c  1)..        angl
-0001a7e0: 6520 3d20 6e70 2e61 7263 636f 7328 6e70  e = np.arccos(np
-0001a7f0: 2e63 6c69 7028 6e70 2e64 6f74 2876 6563  .clip(np.dot(vec
-0001a800: 5f30 2c20 7665 635f 3129 2c20 2d31 2e30  _0, vec_1), -1.0
-0001a810: 2c20 312e 3029 290d 0a20 2020 2020 2020  , 1.0))..       
-0001a820: 2061 6e67 6c65 203d 2061 6e67 6c65 202a   angle = angle *
-0001a830: 2031 3830 202f 206e 702e 7069 0d0a 2020   180 / np.pi..  
-0001a840: 2020 2020 2020 7265 7475 726e 2061 6e67        return ang
-0001a850: 6c65 0d0a 2020 2020 200d 0a0d 0a64 6566  le..     ....def
-0001a860: 2065 7661 6c5f 626f 6f6c 2876 616c 7565   eval_bool(value
-0001a870: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001a880: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001a890: 6966 2076 616c 7565 2020 3d3d 2027 5472  if value  == 'Tr
-0001a8a0: 7565 273a 200d 0a20 2020 2020 2020 2020  ue': ..         
-0001a8b0: 2020 2020 2020 2064 6976 5f6b 6579 203d         div_key =
-0001a8c0: 2054 7275 650d 0a20 2020 2020 2020 2065   True..        e
-0001a8d0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0001a8e0: 2020 2020 2020 6469 765f 6b65 7920 3d20        div_key = 
-0001a8f0: 4661 6c73 6520 0d0a 0d0a 2020 2020 2020  False ....      
-0001a900: 2020 7265 7475 726e 2064 6976 5f6b 6579    return div_key
-0001a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a920: 0d0a 0d0a 6465 6620 6368 6563 6b5f 616e  ....def check_an
-0001a930: 645f 7570 6461 7465 5f6d 6173 6b28 6d61  d_update_mask(ma
-0001a940: 736b 2c69 6d61 6765 293a 0d0a 2020 2020  sk,image):..    
-0001a950: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-0001a960: 6c65 6e28 6d61 736b 2e73 6861 7065 2920  len(mask.shape) 
-0001a970: 3c20 6c65 6e28 696d 6167 652e 7368 6170  < len(image.shap
-0001a980: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-0001a990: 2075 7064 6174 655f 6d61 736b 203d 206e   update_mask = n
-0001a9a0: 702e 7a65 726f 7328 0d0a 2020 2020 2020  p.zeros(..      
-0001a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a9c0: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
-0001a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a9e0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
-0001a9f0: 6861 7065 5b30 5d2c 0d0a 2020 2020 2020  hape[0],..      
-0001aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa10: 2020 2020 2020 2020 2020 696d 6167 652e            image.
-0001aa20: 7368 6170 655b 315d 2c0d 0a20 2020 2020  shape[1],..     
-0001aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa40: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-0001aa50: 2e73 6861 7065 5b32 5d2c 0d0a 2020 2020  .shape[2],..    
-0001aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa70: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-0001aa80: 652e 7368 6170 655b 335d 2c0d 0a20 2020  e.shape[3],..   
-0001aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aaa0: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aac0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0001aad0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0001aae0: 6528 302c 2075 7064 6174 655f 6d61 736b  e(0, update_mask
-0001aaf0: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
-0001ab00: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0001ab10: 206a 2069 6e20 7261 6e67 6528 302c 2075   j in range(0, u
-0001ab20: 7064 6174 655f 6d61 736b 2e73 6861 7065  pdate_mask.shape
-0001ab30: 5b31 5d29 3a0d 0a0d 0a20 2020 2020 2020  [1]):....       
-0001ab40: 2020 2020 2020 2020 2020 2020 2075 7064               upd
-0001ab50: 6174 655f 6d61 736b 5b69 2c20 6a2c 203a  ate_mask[i, j, :
-0001ab60: 2c20 3a5d 203d 206d 6173 6b5b 692c 203a  , :] = mask[i, :
-0001ab70: 2c20 3a5d 0d0a 2020 2020 2020 2020 656c  , :]..        el
-0001ab80: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0001ab90: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
-0001aba0: 203d 206d 6173 6b0d 0a0d 0a20 2020 2020   = mask....     
-0001abb0: 2020 2072 6574 7572 6e20 7570 6461 7465     return update
-0001abc0: 5f6d 6173 6b20 2020 2020 2020 200d 0a20  _mask        .. 
-0001abd0: 2020 2020 2020 0d0a                            ..
+00018280: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+00018290: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+000182a0: 6d65 616e 2861 6c6c 5f64 6973 705f 7a29  mean(all_disp_z)
+000182b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000182c0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+000182d0: 7661 725f 6469 7370 5f7a 2e61 7070 656e  var_disp_z.appen
+000182e0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
+000182f0: 705f 7a29 290d 0a0d 0a20 2020 2020 2020  p_z))....       
+00018300: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018310: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+00018320: 792e 6170 7065 6e64 286e 702e 6d65 616e  y.append(np.mean
+00018330: 2861 6c6c 5f64 6973 705f 7929 290d 0a20  (all_disp_y)).. 
+00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018350: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00018360: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+00018370: 2e73 7464 2861 6c6c 5f64 6973 705f 7929  .std(all_disp_y)
+00018380: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018390: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000183a0: 6c5f 6d65 616e 5f64 6973 705f 782e 6170  l_mean_disp_x.ap
+000183b0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+000183c0: 5f64 6973 705f 7829 290d 0a20 2020 2020  _disp_x))..     
+000183d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000183e0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+000183f0: 5f78 2e61 7070 656e 6428 6e70 2e73 7464  _x.append(np.std
+00018400: 2861 6c6c 5f64 6973 705f 7829 290d 0a0d  (all_disp_x))...
+00018410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018420: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00018430: 616e 5f72 6164 6975 732e 6170 7065 6e64  an_radius.append
+00018440: 286e 702e 6d65 616e 2861 6c6c 5f72 6164  (np.mean(all_rad
+00018450: 6975 7329 290d 0a20 2020 2020 2020 2020  ius))..         
+00018460: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018470: 616c 6c5f 7661 725f 7261 6469 7573 2e61  all_var_radius.a
+00018480: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00018490: 5f72 6164 6975 7329 290d 0a0d 0a20 2020  _radius))....   
+000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184b0: 2073 656c 662e 616c 6c5f 6d65 616e 5f73   self.all_mean_s
+000184c0: 7065 6564 2e61 7070 656e 6428 6e70 2e6d  peed.append(np.m
+000184d0: 6561 6e28 616c 6c5f 7370 6565 6429 290d  ean(all_speed)).
+000184e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000184f0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00018500: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
+00018510: 702e 7374 6428 616c 6c5f 7370 6565 6429  p.std(all_speed)
+00018520: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018530: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018540: 6c5f 6d65 616e 5f61 6363 2e61 7070 656e  l_mean_acc.appen
+00018550: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6163  d(np.mean(all_ac
+00018560: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
+00018570: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018580: 6c5f 7661 725f 6163 632e 6170 7065 6e64  l_var_acc.append
+00018590: 286e 702e 7374 6428 616c 6c5f 6163 6329  (np.std(all_acc)
+000185a0: 290d 0a0d 0a0d 0a0d 0a20 2020 2020 2020  )........       
+000185b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000185c0: 662e 616c 6c5f 6d65 616e 5f64 6972 6563  f.all_mean_direc
+000185d0: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
+000185e0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+000185f0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018600: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
+00018610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018620: 616c 6c5f 7661 725f 6469 7265 6374 696f  all_var_directio
+00018630: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00018640: 6428 6e70 2e73 7464 2861 6c6c 5f64 6972  d(np.std(all_dir
+00018650: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00018660: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018670: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018680: 6c5f 6d65 616e 5f64 6973 7461 6e63 655f  l_mean_distance_
+00018690: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+000186a0: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
+000186b0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+000186c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000186d0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+000186e0: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
+000186f0: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00018700: 2e73 7464 2861 6c6c 5f64 6973 7461 6e63  .std(all_distanc
+00018710: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
+00018720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018730: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00018740: 2020 2020 200d 0a64 6566 2062 6f75 6e64       ..def bound
+00018750: 6172 795f 706f 696e 7473 286d 6173 6b2c  ary_points(mask,
+00018760: 2078 6361 6c69 6272 6174 696f 6e2c 2079   xcalibration, y
+00018770: 6361 6c69 6272 6174 696f 6e2c 207a 6361  calibration, zca
+00018780: 6c69 6272 6174 696f 6e29 3a0d 0a0d 0a20  libration):.... 
+00018790: 2020 206e 6469 6d20 3d20 6c65 6e28 6d61     ndim = len(ma
+000187a0: 736b 2e73 6861 7065 290d 0a20 2020 2074  sk.shape)..    t
+000187b0: 696d 6564 5f6d 6173 6b20 3d20 7b7d 0d0a  imed_mask = {}..
+000187c0: 2020 2020 6d61 736b 203d 206d 6173 6b20      mask = mask 
+000187d0: 3e20 300d 0a20 2020 206d 6173 6b20 3d20  > 0..    mask = 
+000187e0: 6d61 736b 2e61 7374 7970 6528 2775 696e  mask.astype('uin
+000187f0: 7438 2729 0d0a 2020 2020 2320 5958 2073  t8')..    # YX s
+00018800: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
+00018810: 2020 6966 206e 6469 6d20 3d3d 2032 3a0d    if ndim == 2:.
+00018820: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00018830: 2020 2062 6f75 6e64 6172 7920 3d20 6669     boundary = fi
+00018840: 6e64 5f62 6f75 6e64 6172 6965 7328 6d61  nd_boundaries(ma
+00018850: 736b 290d 0a20 2020 2020 2020 2072 6567  sk)..        reg
+00018860: 696f 6e63 656e 7472 6f69 6420 3d20 2830  ioncentroid = (0
+00018870: 2c29 202b 2063 6f6d 7075 7465 5f63 656e  ,) + compute_cen
+00018880: 7472 6f69 6428 626f 756e 6461 7279 2920  troid(boundary) 
+00018890: 0d0a 2020 2020 2020 2020 696e 6469 6365  ..        indice
+000188a0: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+000188b0: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
+000188c0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+000188d0: 203d 206e 702e 7472 616e 7370 6f73 6528   = np.transpose(
+000188e0: 6e70 2e61 7361 7272 6179 2869 6e64 6963  np.asarray(indic
+000188f0: 6573 2929 2e63 6f70 7928 290d 0a0d 0a20  es)).copy().... 
+00018900: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00018910: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
+00018920: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
+00018930: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00018940: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
+00018950: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00018960: 5b30 5d20 2a20 7963 616c 6962 7261 7469  [0] * ycalibrati
+00018970: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00018980: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+00018990: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
+000189a0: 735b 6a5d 5b31 5d20 2a20 7863 616c 6962  s[j][1] * xcalib
+000189b0: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
+000189c0: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
+000189d0: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
+000189e0: 6469 6365 7329 0d0a 2020 2020 2020 2020  dices)..        
+000189f0: 2320 5468 6973 206f 626a 6563 7420 636f  # This object co
+00018a00: 6e74 6169 6e73 206c 6973 7420 6f66 2061  ntains list of a
+00018a10: 6c6c 2074 6865 2070 6f69 6e74 7320 666f  ll the points fo
+00018a20: 7220 616c 6c20 7468 6520 6c61 6265 6c73  r all the labels
+00018a30: 2069 6e20 7468 6520 4d61 736b 2069 6d61   in the Mask ima
+00018a40: 6765 2077 6974 6820 7468 6520 6c61 6265  ge with the labe
+00018a50: 6c20 6964 2061 6e64 2076 6f6c 756d 6520  l id and volume 
+00018a60: 6f66 2065 6163 6820 6c61 6265 6c0d 0a20  of each label.. 
+00018a70: 2020 2020 2020 2074 696d 6564 5f6d 6173         timed_mas
+00018a80: 6b5b 7374 7228 3029 5d20 3d20 5b74 7265  k[str(0)] = [tre
+00018a90: 652c 2069 6e64 6963 6573 2c20 7265 6769  e, indices, regi
+00018aa0: 6f6e 6365 6e74 726f 6964 5d0d 0a0d 0a20  oncentroid].... 
+00018ab0: 2020 2023 2054 5958 2073 6861 7065 6420     # TYX shaped 
+00018ac0: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
+00018ad0: 6469 6d20 3d3d 2033 3a0d 0a0d 0a0d 0a20  dim == 3:...... 
+00018ae0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00018af0: 7471 646d 2872 616e 6765 2830 2c20 6d61  tqdm(range(0, ma
+00018b00: 736b 2e73 6861 7065 5b30 5d29 293a 0d0a  sk.shape[0])):..
+00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018b30: 2020 626f 756e 6461 7279 203d 2066 696e    boundary = fin
+00018b40: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
+00018b50: 6b5b 692c 3a5d 290d 0a20 2020 2020 2020  k[i,:])..       
+00018b60: 2020 2020 2020 2020 2072 6567 696f 6e63           regionc
+00018b70: 656e 7472 6f69 6420 3d20 2830 2c29 202b  entroid = (0,) +
+00018b80: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
+00018b90: 6428 626f 756e 6461 7279 2920 0d0a 2020  d(boundary) ..  
+00018ba0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00018bb0: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
+00018bc0: 2862 6f75 6e64 6172 7920 3e20 3029 0d0a  (boundary > 0)..
+00018bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018be0: 7265 616c 5f69 6e64 6963 6573 203d 206e  real_indices = n
+00018bf0: 702e 7472 616e 7370 6f73 6528 6e70 2e61  p.transpose(np.a
+00018c00: 7361 7272 6179 2869 6e64 6963 6573 2929  sarray(indices))
+00018c10: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
+00018c20: 2020 2020 2020 2020 2020 2066 6f72 206a             for j
+00018c30: 2069 6e20 7261 6e67 6528 302c 206c 656e   in range(0, len
+00018c40: 2872 6561 6c5f 696e 6469 6365 7329 293a  (real_indices)):
+00018c50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018c60: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+00018c70: 6963 6573 5b6a 5d5b 305d 203d 2072 6561  ices[j][0] = rea
+00018c80: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+00018c90: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
+00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cb0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+00018cc0: 5b6a 5d5b 315d 203d 2072 6561 6c5f 696e  [j][1] = real_in
+00018cd0: 6469 6365 735b 6a5d 5b31 5d20 2a20 7863  dices[j][1] * xc
+00018ce0: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
+00018cf0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00018d00: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
+00018d10: 5472 6565 2872 6561 6c5f 696e 6469 6365  Tree(real_indice
+00018d20: 7329 0d0a 0d0a 2020 2020 2020 2020 2020  s)....          
+00018d30: 2020 2020 2020 7469 6d65 645f 6d61 736b        timed_mask
+00018d40: 5b73 7472 2869 295d 203d 205b 7472 6565  [str(i)] = [tree
+00018d50: 2c20 696e 6469 6365 732c 2072 6567 696f  , indices, regio
+00018d60: 6e63 656e 7472 6f69 645d 0d0a 2020 2020  ncentroid]..    
+00018d70: 2020 2020 2020 2020 0d0a 2020 2020 2320          ..    # 
+00018d80: 545a 5958 2073 6861 7065 6420 6f62 6a65  TZYX shaped obje
+00018d90: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
+00018da0: 3d3d 2034 3a0d 0a20 2020 2020 2020 2070  == 4:..        p
+00018db0: 7269 6e74 2827 4d61 736b 7320 6d61 6465  rint('Masks made
+00018dc0: 2069 6e74 6f20 6120 3444 2063 796c 696e   into a 4D cylin
+00018dd0: 6465 722c 2075 7027 290d 0a20 2020 2020  der, up')..     
+00018de0: 2020 2062 6f75 6e64 6172 7920 3d20 6e70     boundary = np
+00018df0: 2e7a 6572 6f73 280d 0a20 2020 2020 2020  .zeros(..       
+00018e00: 2020 2020 205b 6d61 736b 2e73 6861 7065       [mask.shape
+00018e10: 5b30 5d2c 206d 6173 6b2e 7368 6170 655b  [0], mask.shape[
+00018e20: 315d 2c20 6d61 736b 2e73 6861 7065 5b32  1], mask.shape[2
+00018e30: 5d2c 206d 6173 6b2e 7368 6170 655b 335d  ], mask.shape[3]
+00018e40: 5d0d 0a20 2020 2020 2020 2029 0d0a 2020  ]..        )..  
+00018e50: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00018e60: 616e 6765 2830 2c20 6d61 736b 2e73 6861  ange(0, mask.sha
+00018e70: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
+00018e80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00018e90: 2020 2062 6f75 6e64 6172 795b 692c 3a5d     boundary[i,:]
+00018ea0: 203d 2066 696e 645f 626f 756e 6461 7269   = find_boundari
+00018eb0: 6573 286d 6173 6b5b 692c 3a5d 290d 0a20  es(mask[i,:]).. 
+00018ec0: 2020 2020 2020 2020 2020 2072 6567 696f             regio
+00018ed0: 6e63 656e 7472 6f69 6420 3d20 636f 6d70  ncentroid = comp
+00018ee0: 7574 655f 6365 6e74 726f 6964 2862 6f75  ute_centroid(bou
+00018ef0: 6e64 6172 795b 692c 3a5d 2920 0d0a 2020  ndary[i,:]) ..  
+00018f00: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+00018f10: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+00018f20: 6e64 6172 795b 692c 3a5d 203e 2030 290d  ndary[i,:] > 0).
+00018f30: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+00018f40: 6c5f 696e 6469 6365 7320 3d20 6e70 2e74  l_indices = np.t
+00018f50: 7261 6e73 706f 7365 286e 702e 6173 6172  ranspose(np.asar
+00018f60: 7261 7928 696e 6469 6365 7329 292e 636f  ray(indices)).co
+00018f70: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
+00018f80: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+00018f90: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
+00018fa0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
+00018fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fc0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00018fd0: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
+00018fe0: 6573 5b6a 5d5b 305d 202a 207a 6361 6c69  es[j][0] * zcali
+00018ff0: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00019000: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00019010: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+00019020: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00019030: 5d5b 315d 202a 2079 6361 6c69 6272 6174  ][1] * ycalibrat
+00019040: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00019050: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00019060: 6469 6365 735b 6a5d 5b32 5d20 3d20 7265  dices[j][2] = re
+00019070: 616c 5f69 6e64 6963 6573 5b6a 5d5b 325d  al_indices[j][2]
+00019080: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
+00019090: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+000190a0: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+000190b0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
+000190c0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+000190d0: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
+000190e0: 6929 5d20 3d20 5b74 7265 652c 2069 6e64  i)] = [tree, ind
+000190f0: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
+00019100: 726f 6964 5d0d 0a20 2020 2070 7269 6e74  roid]..    print
+00019110: 2827 436f 6d70 7574 6564 2074 6865 2062  ('Computed the b
+00019120: 6f75 6e64 6172 7920 706f 696e 7473 2729  oundary points')
+00019130: 0d0a 0d0a 2020 2020 7265 7475 726e 2074  ....    return t
+00019140: 696d 6564 5f6d 6173 6b2c 2062 6f75 6e64  imed_mask, bound
+00019150: 6172 7920 2020 2020 2020 200d 0a0d 0a64  ary        ....d
+00019160: 6566 2063 6f6d 7075 7465 5f63 656e 7472  ef compute_centr
+00019170: 6f69 6428 6269 6e61 7279 5f69 6d61 6765  oid(binary_image
+00019180: 293a 0d0a 2020 2020 2320 456e 7375 7265  ):..    # Ensure
+00019190: 2062 696e 6172 7920 696d 6167 6520 6973   binary image is
+000191a0: 2061 204e 756d 5079 2061 7272 6179 0d0a   a NumPy array..
+000191b0: 2020 2020 6269 6e61 7279 5f69 6d61 6765      binary_image
+000191c0: 203d 206e 702e 6172 7261 7928 6269 6e61   = np.array(bina
+000191d0: 7279 5f69 6d61 6765 290d 0a0d 0a20 2020  ry_image)....   
+000191e0: 2077 6869 7465 5f70 6978 656c 7320 3d20   white_pixels = 
+000191f0: 6e70 2e77 6865 7265 2862 696e 6172 795f  np.where(binary_
+00019200: 696d 6167 6520 3d3d 2031 290d 0a20 2020  image == 1)..   
+00019210: 206e 756d 5f70 6978 656c 7320 3d20 6c65   num_pixels = le
+00019220: 6e28 7768 6974 655f 7069 7865 6c73 5b30  n(white_pixels[0
+00019230: 5d29 0d0a 0d0a 2020 2020 2320 436f 6d70  ])....    # Comp
+00019240: 7574 6520 7468 6520 6365 6e74 726f 6964  ute the centroid
+00019250: 206f 6620 7468 6520 7768 6974 6520 7069   of the white pi
+00019260: 7865 6c73 2069 6e20 7468 6520 626f 756e  xels in the boun
+00019270: 6461 7279 2069 6d61 6765 0d0a 2020 2020  dary image..    
+00019280: 6365 6e74 726f 6964 203d 206e 702e 7a65  centroid = np.ze
+00019290: 726f 7328 6269 6e61 7279 5f69 6d61 6765  ros(binary_image
+000192a0: 2e6e 6469 6d29 0d0a 2020 2020 666f 7220  .ndim)..    for 
+000192b0: 6469 6d20 696e 2072 616e 6765 2862 696e  dim in range(bin
+000192c0: 6172 795f 696d 6167 652e 6e64 696d 293a  ary_image.ndim):
+000192d0: 0d0a 2020 2020 2020 2020 6365 6e74 726f  ..        centro
+000192e0: 6964 5b64 696d 5d20 3d20 7768 6974 655f  id[dim] = white_
+000192f0: 7069 7865 6c73 5b64 696d 5d2e 7375 6d28  pixels[dim].sum(
+00019300: 2920 2f20 6e75 6d5f 7069 7865 6c73 0d0a  ) / num_pixels..
+00019310: 0d0a 2020 2020 7265 7475 726e 2063 656e  ..    return cen
+00019320: 7472 6f69 640d 0a0d 0a0d 0a0d 0a20 0d0a  troid........ ..
+00019330: 0d0a 6465 6620 6765 745f 6373 765f 6461  ..def get_csv_da
+00019340: 7461 2863 7376 293a 0d0a 0d0a 2020 2020  ta(csv):....    
+00019350: 2020 2020 6461 7461 7365 7420 3d20 7064      dataset = pd
+00019360: 2e72 6561 645f 6373 7628 0d0a 2020 2020  .read_csv(..    
+00019370: 2020 2020 2020 2020 6373 762c 2064 656c          csv, del
+00019380: 696d 6974 6572 3d22 2c22 2c20 656e 636f  imiter=",", enco
+00019390: 6469 6e67 3d22 756e 6963 6f64 655f 6573  ding="unicode_es
+000193a0: 6361 7065 222c 206c 6f77 5f6d 656d 6f72  cape", low_memor
+000193b0: 793d 4661 6c73 650d 0a20 2020 2020 2020  y=False..       
+000193c0: 2029 5b33 3a5d 0d0a 2020 2020 2020 2020   )[3:]..        
+000193d0: 6461 7461 7365 745f 696e 6465 7820 3d20  dataset_index = 
+000193e0: 6461 7461 7365 742e 696e 6465 780d 0a20  dataset.index.. 
+000193f0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
+00019400: 7461 7365 742c 2064 6174 6173 6574 5f69  taset, dataset_i
+00019410: 6e64 6578 0d0a 2020 2020 0d0a 6465 6620  ndex..    ..def 
+00019420: 6765 745f 7370 6f74 5f64 6174 6173 6574  get_spot_dataset
+00019430: 2873 706f 745f 6461 7461 7365 742c 2074  (spot_dataset, t
+00019440: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00019450: 6f74 5f6b 6579 732c 2078 6361 6c69 6272  ot_keys, xcalibr
+00019460: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
+00019470: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
+00019480: 6e2c 2041 7474 7269 6275 7465 426f 786e  n, AttributeBoxn
+00019490: 616d 652c 2064 6574 6563 7469 6f6e 6368  ame, detectionch
+000194a0: 616e 6e65 6c29 3a0d 0a20 2020 2020 2020  annel):..       
+000194b0: 2041 6c6c 5661 6c75 6573 203d 207b 7d0d   AllValues = {}.
+000194c0: 0a20 2020 2020 2020 2070 6f73 6978 203d  .        posix =
+000194d0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+000194e0: 7370 6f74 5f6b 6579 735b 2270 6f73 6978  spot_keys["posix
+000194f0: 225d 0d0a 2020 2020 2020 2020 706f 7369  "]..        posi
+00019500: 7920 3d20 7472 6163 6b5f 616e 616c 7973  y = track_analys
+00019510: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
+00019520: 7369 7922 5d0d 0a20 2020 2020 2020 2070  siy"]..        p
+00019530: 6f73 697a 203d 2074 7261 636b 5f61 6e61  osiz = track_ana
+00019540: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+00019550: 2270 6f73 697a 225d 0d0a 2020 2020 2020  "posiz"]..      
+00019560: 2020 6672 616d 6520 3d20 7472 6163 6b5f    frame = track_
+00019570: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00019580: 7973 5b22 6672 616d 6522 5d0d 0a20 2020  ys["frame"]..   
+00019590: 2020 2020 200d 0a20 2020 2020 2020 204c       ..        L
+000195a0: 6f63 6174 696f 6e58 203d 2028 0d0a 2020  ocationX = (..  
+000195b0: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+000195c0: 6174 6173 6574 5b70 6f73 6978 5d2e 6173  ataset[posix].as
+000195d0: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+000195e0: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
+000195f0: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+00019600: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+00019610: 6f63 6174 696f 6e59 203d 2028 0d0a 2020  ocationY = (..  
+00019620: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+00019630: 6174 6173 6574 5b70 6f73 6979 5d2e 6173  ataset[posiy].as
+00019640: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+00019650: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+00019660: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+00019670: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+00019680: 6f63 6174 696f 6e5a 203d 2028 0d0a 2020  ocationZ = (..  
+00019690: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+000196a0: 6174 6173 6574 5b70 6f73 697a 5d2e 6173  ataset[posiz].as
+000196b0: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+000196c0: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
+000196d0: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+000196e0: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+000196f0: 6f63 6174 696f 6e54 203d 2028 7370 6f74  ocationT = (spot
+00019700: 5f64 6174 6173 6574 5b66 7261 6d65 5d2e  _dataset[frame].
+00019710: 6173 7479 7065 2822 666c 6f61 7422 2929  astype("float"))
+00019720: 2e61 7374 7970 6528 2269 6e74 2229 0d0a  .astype("int")..
+00019730: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00019740: 2020 2020 6967 6e6f 7265 5f76 616c 7565      ignore_value
+00019750: 7320 3d20 5b74 7261 636b 5f61 6e61 6c79  s = [track_analy
+00019760: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
+00019770: 6561 6e5f 696e 7465 6e73 6974 7922 5d2c  ean_intensity"],
+00019780: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00019790: 706f 745f 6b65 7973 5b22 746f 7461 6c5f  pot_keys["total_
+000197a0: 696e 7465 6e73 6974 7922 5d5d 200d 0a20  intensity"]] .. 
+000197b0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
+000197c0: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
+000197d0: 6973 5f73 706f 745f 6b65 7973 2e69 7465  is_spot_keys.ite
+000197e0: 6d73 2829 3a0d 0a0d 0a20 2020 2020 2020  ms():....       
+000197f0: 2020 2020 2020 2020 2069 6620 6465 7465           if dete
+00019800: 6374 696f 6e63 6861 6e6e 656c 203d 3d20  ctionchannel == 
+00019810: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+00019820: 2020 2020 2020 2020 2069 6620 6b20 3d3d           if k ==
+00019830: 2022 6d65 616e 5f69 6e74 656e 7369 7479   "mean_intensity
+00019840: 5f63 6832 223a 0d0a 2020 2020 2020 2020  _ch2":..        
+00019850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019860: 2020 2076 616c 7565 203d 2074 7261 636b     value = track
+00019870: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00019880: 6579 735b 226d 6561 6e5f 696e 7465 6e73  eys["mean_intens
+00019890: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
+000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198b0: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
+000198c0: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
+000198d0: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
+000198e0: 6174 2229 0d0a 2020 2020 2020 2020 2020  at")..          
+000198f0: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+00019900: 3d3d 2022 746f 7461 6c5f 696e 7465 6e73  == "total_intens
+00019910: 6974 795f 6368 3222 3a0d 0a20 2020 2020  ity_ch2":..     
+00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019930: 2020 2020 2020 7661 6c75 6520 3d20 7472        value = tr
+00019940: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+00019950: 745f 6b65 7973 5b22 746f 7461 6c5f 696e  t_keys["total_in
+00019960: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
+00019970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019980: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+00019990: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
+000199a0: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+000199b0: 2266 6c6f 6174 2229 2020 2020 2020 200d  "float")       .
+000199c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000199d0: 2020 2069 6620 7620 6e6f 7420 696e 2069     if v not in i
+000199e0: 676e 6f72 655f 7661 6c75 6573 3a0d 0a20  gnore_values:.. 
+000199f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00019a10: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00019a20: 6c6c 5661 6c75 6573 5b76 5d20 3d20 7370  llValues[v] = sp
+00019a30: 6f74 5f64 6174 6173 6574 5b76 5d2e 6173  ot_dataset[v].as
+00019a40: 7479 7065 2822 666c 6f61 7422 290d 0a0d  type("float")...
+00019a50: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
+00019a60: 6573 5b70 6f73 6978 5d20 3d20 726f 756e  es[posix] = roun
+00019a70: 6428 4c6f 6361 7469 6f6e 582c 3329 0d0a  d(LocationX,3)..
+00019a80: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+00019a90: 735b 706f 7369 795d 203d 2072 6f75 6e64  s[posiy] = round
+00019aa0: 284c 6f63 6174 696f 6e59 2c33 290d 0a20  (LocationY,3).. 
+00019ab0: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+00019ac0: 5b70 6f73 697a 5d20 3d20 726f 756e 6428  [posiz] = round(
+00019ad0: 4c6f 6361 7469 6f6e 5a2c 3329 0d0a 2020  LocationZ,3)..  
+00019ae0: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+00019af0: 6672 616d 655d 203d 2072 6f75 6e64 284c  frame] = round(L
+00019b00: 6f63 6174 696f 6e54 2c33 290d 0a20 2020  ocationT,3)..   
+00019b10: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+00019b20: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00019b30: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+00019b40: 656e 6428 4174 7472 6962 7574 6542 6f78  end(AttributeBox
+00019b50: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
+00019b60: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
+00019b70: 2069 6e20 416c 6c56 616c 7565 732e 6b65   in AllValues.ke
+00019b80: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+00019b90: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+00019ba0: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
+00019bb0: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
+00019bc0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00019bd0: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+00019be0: 7572 6e20 4174 7472 6962 7574 6569 6473  urn Attributeids
+00019bf0: 2c20 416c 6c56 616c 7565 7320 2020 2020  , AllValues     
+00019c00: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+00019c10: 7472 6163 6b5f 6461 7461 7365 7428 7472  track_dataset(tr
+00019c20: 6163 6b5f 6461 7461 7365 742c 2074 7261  ack_dataset, tra
+00019c30: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00019c40: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
+00019c50: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
+00019c60: 2c20 5472 6163 6b41 7474 7269 6275 7465  , TrackAttribute
+00019c70: 426f 786e 616d 6529 3a0d 0a0d 0a20 2020  Boxname):....   
+00019c80: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
+00019c90: 7565 7320 3d20 7b7d 0d0a 2020 2020 2020  ues = {}..      
+00019ca0: 2020 7472 6163 6b5f 6964 203d 2074 7261    track_id = tra
+00019cb0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00019cc0: 5f6b 6579 735b 2274 7261 636b 5f69 6422  _keys["track_id"
+00019cd0: 5d0d 0a20 2020 2020 2020 2054 6964 203d  ]..        Tid =
+00019ce0: 2074 7261 636b 5f64 6174 6173 6574 5b74   track_dataset[t
+00019cf0: 7261 636b 5f69 645d 2e61 7374 7970 6528  rack_id].astype(
+00019d00: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+00019d10: 200d 0a20 2020 2020 2020 2041 6c6c 5472   ..        AllTr
+00019d20: 6163 6b56 616c 7565 735b 7472 6163 6b5f  ackValues[track_
+00019d30: 6964 5d20 3d20 5469 640d 0a20 2020 2020  id] = Tid..     
+00019d40: 200d 0a20 2020 2020 2020 2066 6f72 2028   ..        for (
+00019d50: 6b2c 2076 2920 696e 2074 7261 636b 5f61  k, v) in track_a
+00019d60: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+00019d70: 7973 2e69 7465 6d73 2829 3a0d 0a0d 0a20  ys.items():.... 
+00019d80: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00019d90: 203d 2074 7261 636b 5f64 6174 6173 6574   = track_dataset
+00019da0: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+00019db0: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+00019dc0: 2020 2020 206d 696e 7661 6c20 3d20 6d69       minval = mi
+00019dd0: 6e28 7829 0d0a 2020 2020 2020 2020 2020  n(x)..          
+00019de0: 2020 2020 2020 6d61 7876 616c 203d 206d        maxval = m
+00019df0: 6178 2878 290d 0a0d 0a20 2020 2020 2020  ax(x)....       
+00019e00: 2020 2020 2020 2020 2069 6620 6d69 6e76           if minv
+00019e10: 616c 203e 2030 2061 6e64 206d 6178 7661  al > 0 and maxva
+00019e20: 6c20 3c3d 2031 3a0d 0a0d 0a20 2020 2020  l <= 1:....     
+00019e30: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00019e40: 203d 2078 202b 2031 0d0a 0d0a 2020 2020   = x + 1....    
+00019e50: 2020 2020 2020 2020 2020 2020 416c 6c54              AllT
+00019e60: 7261 636b 5661 6c75 6573 5b6b 5d20 3d20  rackValues[k] = 
+00019e70: 726f 756e 6428 782c 2033 290d 0a0d 0a20  round(x, 3).... 
+00019e80: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
+00019e90: 6962 7574 6569 6473 203d 205b 5d0d 0a20  ibuteids = [].. 
+00019ea0: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
+00019eb0: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
+00019ec0: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
+00019ed0: 786e 616d 6529 0d0a 2020 2020 2020 2020  xname)..        
+00019ee0: 666f 7220 6174 7472 6962 7574 656e 616d  for attributenam
+00019ef0: 6520 696e 2074 7261 636b 5f61 6e61 6c79  e in track_analy
+00019f00: 7369 735f 7472 6163 6b5f 6b65 7973 2e6b  sis_track_keys.k
+00019f10: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+00019f20: 2020 2020 5472 6163 6b41 7474 7269 6275      TrackAttribu
+00019f30: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
+00019f40: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
+00019f50: 0a20 2020 200d 0a20 2020 2020 2020 2072  .    ..        r
+00019f60: 6574 7572 6e20 5472 6163 6b41 7474 7269  eturn TrackAttri
+00019f70: 6275 7465 6964 732c 2041 6c6c 5472 6163  buteids, AllTrac
+00019f80: 6b56 616c 7565 730d 0a20 2020 200d 0a64  kValues..    ..d
+00019f90: 6566 2067 6574 5f65 6467 6573 5f64 6174  ef get_edges_dat
+00019fa0: 6173 6574 2865 6467 6573 5f64 6174 6173  aset(edges_datas
+00019fb0: 6574 2c20 6564 6765 735f 6461 7461 7365  et, edges_datase
+00019fc0: 745f 696e 6465 782c 2074 7261 636b 5f61  t_index, track_a
+00019fd0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+00019fe0: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
+00019ff0: 735f 6564 6765 735f 6b65 7973 293a 0d0a  s_edges_keys):..
+0001a000: 0d0a 2020 2020 2020 2020 416c 6c45 6467  ..        AllEdg
+0001a010: 6573 5661 6c75 6573 203d 207b 7d0d 0a20  esValues = {}.. 
+0001a020: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+0001a030: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+0001a040: 5f73 706f 745f 6b65 7973 5b22 7472 6163  _spot_keys["trac
+0001a050: 6b5f 6964 225d 0d0a 2020 2020 2020 2020  k_id"]..        
+0001a060: 5469 6420 3d20 6564 6765 735f 6461 7461  Tid = edges_data
+0001a070: 7365 745b 7472 6163 6b5f 6964 5d2e 6173  set[track_id].as
+0001a080: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+0001a090: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+0001a0a0: 206e 702e 7768 6572 6528 5469 6420 3d3d   np.where(Tid ==
+0001a0b0: 2030 290d 0a20 2020 2020 2020 206d 6178   0)..        max
+0001a0c0: 7472 6163 6b5f 6964 203d 206d 6178 2854  track_id = max(T
+0001a0d0: 6964 290d 0a20 2020 2020 2020 2063 6f6e  id)..        con
+0001a0e0: 6469 7469 6f6e 5f69 6e64 6963 6573 203d  dition_indices =
+0001a0f0: 2065 6467 6573 5f64 6174 6173 6574 5f69   edges_dataset_i
+0001a100: 6e64 6578 5b69 6e64 6963 6573 5d0d 0a20  ndex[indices].. 
+0001a110: 2020 2020 2020 2054 6964 5b63 6f6e 6469         Tid[condi
+0001a120: 7469 6f6e 5f69 6e64 6963 6573 5d20 3d20  tion_indices] = 
+0001a130: 6d61 7874 7261 636b 5f69 6420 2b20 310d  maxtrack_id + 1.
+0001a140: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
+0001a150: 7356 616c 7565 735b 7472 6163 6b5f 6964  sValues[track_id
+0001a160: 5d20 3d20 5469 640d 0a0d 0a20 2020 2020  ] = Tid....     
+0001a170: 2020 2066 6f72 206b 2069 6e20 7472 6163     for k in trac
+0001a180: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+0001a190: 5f6b 6579 732e 7661 6c75 6573 2829 3a0d  _keys.values():.
+0001a1a0: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0001a1b0: 6620 6b20 213d 2074 7261 636b 5f69 643a  f k != track_id:
+0001a1c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a1d0: 2020 7820 3d20 6564 6765 735f 6461 7461    x = edges_data
+0001a1e0: 7365 745b 6b5d 2e61 7374 7970 6528 2266  set[k].astype("f
+0001a1f0: 6c6f 6174 2229 0d0a 0d0a 2020 2020 2020  loat")....      
+0001a200: 2020 2020 2020 2020 2020 416c 6c45 6467            AllEdg
+0001a210: 6573 5661 6c75 6573 5b6b 5d20 3d20 7820  esValues[k] = x 
+0001a220: 2020 0d0a 2020 2020 2020 2020 200d 0a20    ..         .. 
+0001a230: 2020 2020 2020 2072 6574 7572 6e20 416c         return Al
+0001a240: 6c45 6467 6573 5661 6c75 6573 2020 200d  lEdgesValues   .
+0001a250: 0a20 2020 200d 0a20 2020 2020 2020 0d0a  .    ..       ..
+0001a260: 2020 2020 0d0a 6465 6620 7363 616c 655f      ..def scale_
+0001a270: 7661 6c75 6528 782c 2073 6361 6c65 203d  value(x, scale =
+0001a280: 2032 3535 202a 2032 3535 293a 0d0a 0d0a   255 * 255):....
+0001a290: 0d0a 2020 2020 2072 6574 7572 6e20 7820  ..     return x 
+0001a2a0: 2a20 7363 616c 6520 2020 0d0a 2020 2020  * scale   ..    
+0001a2b0: 0d0a 0d0a 0d0a 6465 6620 7072 6f62 5f73  ......def prob_s
+0001a2c0: 6967 6d6f 6964 2878 293a 0d0a 2020 2020  igmoid(x):..    
+0001a2d0: 7265 7475 726e 2031 202d 206d 6174 682e  return 1 - math.
+0001a2e0: 6578 7028 2d78 290d 0a0d 0a0d 0a64 6566  exp(-x)......def
+0001a2f0: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+0001a300: 7665 635f 302c 2076 6563 5f31 293a 0d0a  vec_0, vec_1):..
+0001a310: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001a320: 2020 7665 635f 3020 3d20 7665 635f 3020    vec_0 = vec_0 
+0001a330: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
+0001a340: 2876 6563 5f30 290d 0a20 2020 2020 2020  (vec_0)..       
+0001a350: 2076 6563 5f31 203d 2076 6563 5f31 202f   vec_1 = vec_1 /
+0001a360: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
+0001a370: 7665 635f 3129 0d0a 2020 2020 2020 2020  vec_1)..        
+0001a380: 616e 676c 6520 3d20 6e70 2e61 7263 636f  angle = np.arcco
+0001a390: 7328 6e70 2e63 6c69 7028 6e70 2e64 6f74  s(np.clip(np.dot
+0001a3a0: 2876 6563 5f30 2c20 7665 635f 3129 2c20  (vec_0, vec_1), 
+0001a3b0: 2d31 2e30 2c20 312e 3029 290d 0a20 2020  -1.0, 1.0))..   
+0001a3c0: 2020 2020 2061 6e67 6c65 203d 2061 6e67       angle = ang
+0001a3d0: 6c65 202a 2031 3830 202f 206e 702e 7069  le * 180 / np.pi
+0001a3e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001a3f0: 2061 6e67 6c65 0d0a 2020 2020 200d 0a0d   angle..     ...
+0001a400: 0a64 6566 2065 7661 6c5f 626f 6f6c 2876  .def eval_bool(v
+0001a410: 616c 7565 293a 0d0a 2020 2020 2020 2020  alue):..        
+0001a420: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001a430: 2020 2020 6966 2076 616c 7565 2020 3d3d      if value  ==
+0001a440: 2027 5472 7565 273a 200d 0a20 2020 2020   'True': ..     
+0001a450: 2020 2020 2020 2020 2020 2064 6976 5f6b             div_k
+0001a460: 6579 203d 2054 7275 650d 0a20 2020 2020  ey = True..     
+0001a470: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0001a480: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
+0001a490: 7920 3d20 4661 6c73 6520 0d0a 0d0a 2020  y = False ....  
+0001a4a0: 2020 2020 2020 7265 7475 726e 2064 6976        return div
+0001a4b0: 5f6b 6579 2020 2020 2020 2020 2020 2020  _key            
+0001a4c0: 2020 2020 0d0a 0d0a 6465 6620 6368 6563      ....def chec
+0001a4d0: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
+0001a4e0: 6b28 6d61 736b 2c69 6d61 6765 293a 0d0a  k(mask,image):..
+0001a4f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001a500: 2069 6620 6c65 6e28 6d61 736b 2e73 6861   if len(mask.sha
+0001a510: 7065 2920 3c20 6c65 6e28 696d 6167 652e  pe) < len(image.
+0001a520: 7368 6170 6529 3a0d 0a20 2020 2020 2020  shape):..       
+0001a530: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
+0001a540: 203d 206e 702e 7a65 726f 7328 0d0a 2020   = np.zeros(..  
+0001a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a560: 2020 2020 2020 2020 2020 5b0d 0a20 2020            [..   
+0001a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a580: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001a590: 6765 2e73 6861 7065 5b30 5d2c 0d0a 2020  ge.shape[0],..  
+0001a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5b0: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0001a5c0: 6167 652e 7368 6170 655b 315d 2c0d 0a20  age.shape[1],.. 
+0001a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a5f0: 6d61 6765 2e73 6861 7065 5b32 5d2c 0d0a  mage.shape[2],..
+0001a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a620: 696d 6167 652e 7368 6170 655b 335d 2c0d  image.shape[3],.
+0001a630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a640: 2020 2020 2020 2020 2020 2020 205d 0d0a               ]..
+0001a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a660: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001a670: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0001a680: 7261 6e67 6528 302c 2075 7064 6174 655f  range(0, update_
+0001a690: 6d61 736b 2e73 6861 7065 5b30 5d29 3a0d  mask.shape[0]):.
+0001a6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a6b0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+0001a6c0: 302c 2075 7064 6174 655f 6d61 736b 2e73  0, update_mask.s
+0001a6d0: 6861 7065 5b31 5d29 3a0d 0a0d 0a20 2020  hape[1]):....   
+0001a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6f0: 2075 7064 6174 655f 6d61 736b 5b69 2c20   update_mask[i, 
+0001a700: 6a2c 203a 2c20 3a5d 203d 206d 6173 6b5b  j, :, :] = mask[
+0001a710: 692c 203a 2c20 3a5d 0d0a 2020 2020 2020  i, :, :]..      
+0001a720: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001a730: 2020 2020 2020 2020 2075 7064 6174 655f           update_
+0001a740: 6d61 736b 203d 206d 6173 6b0d 0a0d 0a20  mask = mask.... 
+0001a750: 2020 2020 2020 2072 6574 7572 6e20 7570         return up
+0001a760: 6461 7465 5f6d 6173 6b20 2020 2020 2020  date_mask       
+0001a770: 200d 0a20 2020 2020 2020 0d0a             ..       ..
```

### Comparing `napatrackmater-3.3.9/napatrackmater/Trackvector.py` & `napatrackmater-3.4.0/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater/__init__.py` & `napatrackmater-3.4.0/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater/clustering.py` & `napatrackmater-3.4.0/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.4.0/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater/fate_mapping.py` & `napatrackmater-3.4.0/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater/pretrained.py` & `napatrackmater-3.4.0/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.4.0/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.3.9
+Version: 3.4.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.3.9/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.4.0/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.9/setup.py` & `napatrackmater-3.4.0/setup.py`

 * *Files identical despite different names*

