# Comparing `tmp/napatrackmater-3.3.8.tar.gz` & `tmp/napatrackmater-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-e4hf_wq3/napatrackmater-3.3.8.tar", last modified: Sat Apr 29 21:48:51 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-ttt3b2mp/napatrackmater-3.3.9.tar", last modified: Sun Apr 30 11:21:44 2023, max compression
```

## Comparing `napatrackmater-3.3.8.tar` & `napatrackmater-3.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-29 21:48:51.554608 napatrackmater-3.3.8/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.3.8/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-04-29 21:48:51.549184 napatrackmater-3.3.8/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.3.8/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-29 21:48:51.201084 napatrackmater-3.3.8/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.3.8/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.3.8/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   109716 2023-04-29 21:47:25.000000 napatrackmater-3.3.8/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.3.8/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.3.8/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.3.8/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.3.8/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.3.8/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.3.8/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-29 21:47:36.000000 napatrackmater-3.3.8/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-29 21:48:51.504470 napatrackmater-3.3.8/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-04-29 21:48:50.000000 napatrackmater-3.3.8/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-04-29 21:48:50.000000 napatrackmater-3.3.8/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-29 21:48:50.000000 napatrackmater-3.3.8/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-04-29 21:48:50.000000 napatrackmater-3.3.8/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-04-29 21:48:50.000000 napatrackmater-3.3.8/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-04-29 21:48:50.000000 napatrackmater-3.3.8/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-04-29 21:48:51.559958 napatrackmater-3.3.8/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.3.8/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 11:21:44.106428 napatrackmater-3.3.9/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.3.9/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-04-30 11:21:44.097821 napatrackmater-3.3.9/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.3.9/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 11:21:43.735334 napatrackmater-3.3.9/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.3.9/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.3.9/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   109528 2023-04-30 11:03:51.000000 napatrackmater-3.3.9/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.3.9/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.3.9/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.3.9/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.3.9/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.3.9/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.3.9/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-04-30 11:20:54.000000 napatrackmater-3.3.9/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-04-30 11:21:44.038261 napatrackmater-3.3.9/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-04-30 11:21:43.000000 napatrackmater-3.3.9/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-04-30 11:21:42.000000 napatrackmater-3.3.9/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-04-30 11:21:44.108713 napatrackmater-3.3.9/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.3.9/setup.py
```

### Comparing `napatrackmater-3.3.8/LICENSE` & `napatrackmater-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/PKG-INFO` & `napatrackmater-3.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.3.8
+Version: 3.3.9
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.3.8/README.md` & `napatrackmater-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.3.9/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.3.9/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater/Trackmate.py` & `napatrackmater-3.3.9/napatrackmater/Trackmate.py`

 * *Files 1% similar despite different names*

```diff
@@ -3170,3689 +3170,3677 @@
 0000c610: 6578 202a 2073 697a 6579 202a 2073 697a  ex * sizey * siz
 0000c620: 657a 0d0a 2020 2020 2020 2020 2020 2020  ez..            
 0000c630: 7665 746f 5f72 6164 6975 7320 3d20 6d61  veto_radius = ma
 0000c640: 7468 2e70 6f77 2833 202a 2076 6574 6f5f  th.pow(3 * veto_
 0000c650: 766f 6c75 6d65 202f 2028 3420 2a20 6d61  volume / (4 * ma
 0000c660: 7468 2e70 6929 2c20 312e 3020 2f20 332e  th.pi), 1.0 / 3.
 0000c670: 3029 0d0a 0d0a 2020 2020 2020 2020 2020  0)....          
-0000c680: 2020 6966 2064 6973 7420 3c20 7665 746f    if dist < veto
-0000c690: 5f72 6164 6975 733a 0d0a 2020 2020 2020  _radius:..      
-0000c6a0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000c6b0: 6361 7469 6f6e 203d 2028 696e 7428 6365  cation = (int(ce
-0000c6c0: 6e74 726f 6964 735b 696e 6465 785d 5b30  ntroids[index][0
-0000c6d0: 5d29 2c20 696e 7428 6365 6e74 726f 6964  ]), int(centroid
-0000c6e0: 735b 696e 6465 785d 5b31 5d29 2c20 696e  s[index][1]), in
-0000c6f0: 7428 6365 6e74 726f 6964 735b 696e 6465  t(centroids[inde
-0000c700: 785d 5b32 5d29 290d 0a20 2020 2020 2020  x][2]))..       
-0000c710: 2020 2020 2020 2020 2020 2020 2051 5541               QUA
-0000c720: 4c49 5459 203d 2076 6f6c 756d 655b 696e  LITY = volume[in
-0000c730: 6465 785d 0d0a 2020 2020 2020 2020 2020  dex]..          
-0000c740: 2020 2020 2020 2020 2020 5241 4449 5553            RADIUS
-0000c750: 203d 206d 6174 682e 706f 7728 5155 414c   = math.pow(QUAL
-0000c760: 4954 592c 2031 2e30 2f33 2e30 2920 2a20  ITY, 1.0/3.0) * 
-0000c770: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-0000c780: 6e20 2a20 7365 6c66 2e79 6361 6c69 6272  n * self.ycalibr
-0000c790: 6174 696f 6e20 2a20 7365 6c66 2e7a 6361  ation * self.zca
-0000c7a0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000c7c0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-0000c7d0: 6b2c 206d 6173 6b63 656e 7472 6f69 6420  k, maskcentroid 
-0000c7e0: 3d20 7365 6c66 2e5f 6765 745f 626f 756e  = self._get_boun
-0000c7f0: 6461 7279 5f64 6973 7428 6672 616d 652c  dary_dist(frame,
-0000c800: 206c 6f63 6174 696f 6e2c 2052 4144 4955   location, RADIU
-0000c810: 5329 0d0a 2020 2020 2020 2020 2020 2020  S)..            
-0000c820: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-0000c830: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000c840: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-0000c850: 5f69 645d 203d 207b 0d0a 2020 2020 2020  _id] = {..      
-0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c870: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
-0000c880: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
-0000c890: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
-0000c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8b0: 2020 2073 656c 662e 6672 616d 6569 645f     self.frameid_
-0000c8c0: 6b65 7920 3a20 696e 7428 666c 6f61 7428  key : int(float(
-0000c8d0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000c8e0: 656c 662e 6672 616d 6569 645f 6b65 7929  elf.frameid_key)
-0000c8f0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c910: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
-0000c920: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
-0000c930: 6473 5b69 6e64 6578 5d5b 305d 292c 0d0a  ds[index][0]),..
-0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c950: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c960: 2e79 706f 7369 645f 6b65 7920 3a20 666c  .yposid_key : fl
-0000c970: 6f61 7428 6365 6e74 726f 6964 735b 696e  oat(centroids[in
-0000c980: 6465 785d 5b31 5d29 2c0d 0a20 2020 2020  dex][1]),..     
-0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9a0: 2020 2020 2020 2073 656c 662e 7870 6f73         self.xpos
-0000c9b0: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
-0000c9c0: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-0000c9d0: 325d 292c 0d0a 0d0a 2020 2020 2020 2020  2]),....        
-0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9f0: 2020 2020 7365 6c66 2e74 6f74 616c 5f69      self.total_i
-0000ca00: 6e74 656e 7369 7479 5f6b 6579 203a 2028  ntensity_key : (
-0000ca10: 666c 6f61 7428 696e 7465 6e73 6974 795f  float(intensity_
-0000ca20: 746f 7461 6c5b 696e 6465 785d 2929 2c0d  total[index])),.
-0000ca30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ca40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ca50: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
-0000ca60: 5f6b 6579 203a 2028 666c 6f61 7428 696e  _key : (float(in
-0000ca70: 7465 6e73 6974 795f 6d65 616e 5b69 6e64  tensity_mean[ind
-0000ca80: 6578 5d29 292c 0d0a 0d0a 2020 2020 2020  ex])),....      
-0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caa0: 2020 2020 2020 7365 6c66 2e72 6164 6975        self.radiu
-0000cab0: 735f 6b65 7920 3a20 2866 6c6f 6174 2852  s_key : (float(R
-0000cac0: 4144 4955 5329 292c 0d0a 2020 2020 2020  ADIUS)),..      
-0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cae0: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
-0000caf0: 7479 5f6b 6579 203a 2028 666c 6f61 7428  ty_key : (float(
-0000cb00: 5155 414c 4954 5929 292c 0d0a 2020 2020  QUALITY)),..    
-0000cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb20: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-0000cb30: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-0000cb40: 6b65 793a 2066 6c6f 6174 2864 6973 7461  key: float(dista
-0000cb50: 6e63 655f 6365 6c6c 5f6d 6173 6b29 2c0d  nce_cell_mask),.
-0000cb60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cb70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000cb80: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
-0000cb90: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
-0000cba0: 6365 6e74 726f 6964 5b30 5d29 2c0d 0a20  centroid[0]),.. 
+0000c680: 2020 6c6f 6361 7469 6f6e 203d 2028 696e    location = (in
+0000c690: 7428 6365 6e74 726f 6964 735b 696e 6465  t(centroids[inde
+0000c6a0: 785d 5b30 5d29 2c20 696e 7428 6365 6e74  x][0]), int(cent
+0000c6b0: 726f 6964 735b 696e 6465 785d 5b31 5d29  roids[index][1])
+0000c6c0: 2c20 696e 7428 6365 6e74 726f 6964 735b  , int(centroids[
+0000c6d0: 696e 6465 785d 5b32 5d29 290d 0a20 2020  index][2]))..   
+0000c6e0: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
+0000c6f0: 203d 2076 6f6c 756d 655b 696e 6465 785d   = volume[index]
+0000c700: 0d0a 2020 2020 2020 2020 2020 2020 5241  ..            RA
+0000c710: 4449 5553 203d 206d 6174 682e 706f 7728  DIUS = math.pow(
+0000c720: 5155 414c 4954 592c 2031 2e30 2f33 2e30  QUALITY, 1.0/3.0
+0000c730: 2920 2a20 7365 6c66 2e78 6361 6c69 6272  ) * self.xcalibr
+0000c740: 6174 696f 6e20 2a20 7365 6c66 2e79 6361  ation * self.yca
+0000c750: 6c69 6272 6174 696f 6e20 2a20 7365 6c66  libration * self
+0000c760: 2e7a 6361 6c69 6272 6174 696f 6e0d 0a20  .zcalibration.. 
+0000c770: 2020 2020 2020 2020 2020 2064 6973 7461             dista
+0000c780: 6e63 655f 6365 6c6c 5f6d 6173 6b2c 206d  nce_cell_mask, m
+0000c790: 6173 6b63 656e 7472 6f69 6420 3d20 7365  askcentroid = se
+0000c7a0: 6c66 2e5f 6765 745f 626f 756e 6461 7279  lf._get_boundary
+0000c7b0: 5f64 6973 7428 6672 616d 652c 206c 6f63  _dist(frame, loc
+0000c7c0: 6174 696f 6e2c 2052 4144 4955 5329 0d0a  ation, RADIUS)..
+0000c7d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c7e0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000c7f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000c800: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
+0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c820: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
+0000c830: 793a 2069 6e74 2863 656c 6c5f 6964 292c  y: int(cell_id),
+0000c840: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000c850: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+0000c860: 6569 645f 6b65 7920 3a20 696e 7428 666c  eid_key : int(fl
+0000c870: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000c880: 6574 2873 656c 662e 6672 616d 6569 645f  et(self.frameid_
+0000c890: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
+0000c8a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c8b0: 662e 7a70 6f73 6964 5f6b 6579 203a 2066  f.zposid_key : f
+0000c8c0: 6c6f 6174 2863 656e 7472 6f69 6473 5b69  loat(centroids[i
+0000c8d0: 6e64 6578 5d5b 305d 292c 0d0a 2020 2020  ndex][0]),..    
+0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8f0: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
+0000c900: 3a20 666c 6f61 7428 6365 6e74 726f 6964  : float(centroid
+0000c910: 735b 696e 6465 785d 5b31 5d29 2c0d 0a20  s[index][1]),.. 
+0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c930: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+0000c940: 6579 203a 2066 6c6f 6174 2863 656e 7472  ey : float(centr
+0000c950: 6f69 6473 5b69 6e64 6578 5d5b 325d 292c  oids[index][2]),
+0000c960: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000c970: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+0000c980: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
+0000c990: 203a 2028 666c 6f61 7428 696e 7465 6e73   : (float(intens
+0000c9a0: 6974 795f 746f 7461 6c5b 696e 6465 785d  ity_total[index]
+0000c9b0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000c9c0: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
+0000c9d0: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
+0000c9e0: 203a 2028 666c 6f61 7428 696e 7465 6e73   : (float(intens
+0000c9f0: 6974 795f 6d65 616e 5b69 6e64 6578 5d29  ity_mean[index])
+0000ca00: 292c 0d0a 0d0a 2020 2020 2020 2020 2020  ),....          
+0000ca10: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000ca20: 6164 6975 735f 6b65 7920 3a20 2866 6c6f  adius_key : (flo
+0000ca30: 6174 2852 4144 4955 5329 292c 0d0a 2020  at(RADIUS)),..  
+0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca50: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
+0000ca60: 6579 203a 2028 666c 6f61 7428 5155 414c  ey : (float(QUAL
+0000ca70: 4954 5929 292c 0d0a 2020 2020 2020 2020  ITY)),..        
+0000ca80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ca90: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
+0000caa0: 6173 6b5f 6b65 793a 2066 6c6f 6174 2864  ask_key: float(d
+0000cab0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0000cac0: 6b29 2c0d 0a20 2020 2020 2020 2020 2020  k),..           
+0000cad0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000cae0: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
+0000caf0: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+0000cb00: 726f 6964 5b30 5d29 2c0d 0a20 2020 2020  roid[0]),..     
+0000cb10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000cb20: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+0000cb30: 5f79 5f6b 6579 3a20 666c 6f61 7428 6d61  _y_key: float(ma
+0000cb40: 736b 6365 6e74 726f 6964 5b31 5d29 2c0d  skcentroid[1]),.
+0000cb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cb60: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
+0000cb70: 6e74 726f 6964 5f78 5f6b 6579 3a20 666c  ntroid_x_key: fl
+0000cb80: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
+0000cb90: 5b32 5d29 200d 0a0d 0a20 2020 2020 2020  [2]) ....       
+0000cba0: 2020 2020 207d 200d 0a20 2020 2020 2020       } ..       
 0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cbd0: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
-0000cbe0: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
-0000cbf0: 6e74 726f 6964 5b31 5d29 2c0d 0a20 2020  ntroid[1]),..   
-0000cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc10: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000cc20: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-0000cc30: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
-0000cc40: 726f 6964 5b32 5d29 200d 0a0d 0a20 2020  roid[2]) ....   
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc60: 207d 200d 0a20 2020 2020 2020 2020 2020   } ..           
-0000cc70: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-0000cc80: 0a20 2020 2064 6566 205f 6765 745f 6d61  .    def _get_ma
-0000cc90: 7374 6572 5f78 6d6c 5f64 6174 6128 7365  ster_xml_data(se
-0000cca0: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
-0000ccb0: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
-0000ccc0: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
-0000ccd0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000cbc0: 200d 0a0d 0a20 2020 2064 6566 205f 6765   ....    def _ge
+0000cbd0: 745f 6d61 7374 6572 5f78 6d6c 5f64 6174  t_master_xml_dat
+0000cbe0: 6128 7365 6c66 293a 0d0a 2020 2020 2020  a(self):..      
+0000cbf0: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
+0000cc00: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
+0000cc10: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc30: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+0000cc40: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
+0000cc50: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
+0000cc60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc70: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
+0000cc80: 7472 6565 203d 2065 742e 7061 7273 6528  tree = et.parse(
+0000cc90: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
+0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccb0: 2020 2020 2020 7365 6c66 2e78 6d6c 5f72        self.xml_r
+0000ccc0: 6f6f 7420 3d20 7365 6c66 2e78 6d6c 5f74  oot = self.xml_t
+0000ccd0: 7265 652e 6765 7472 6f6f 7428 290d 0a20  ree.getroot().. 
 0000cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccf0: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000cd00: 5f63 6f6e 7465 6e74 203d 2073 656c 662e  _content = self.
-0000cd10: 786d 6c5f 636f 6e74 656e 740d 0a20 2020  xml_content..   
-0000cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd30: 2020 2073 656c 662e 786d 6c5f 7472 6565     self.xml_tree
-0000cd40: 203d 2065 742e 7061 7273 6528 7365 6c66   = et.parse(self
-0000cd50: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
+0000ccf0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+0000cd00: 6c5f 786d 6c5f 6e61 6d65 203d 2027 7365  l_xml_name = 'se
+0000cd10: 636f 6e64 5f63 6861 6e6e 656c 5f27 202b  cond_channel_' +
+0000cd20: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+0000cd30: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
+0000cd40: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
+0000cd50: 2929 5b30 5d20 2b20 272e 786d 6c27 0d0a  ))[0] + '.xml'..
 0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2020 7365 6c66 2e78 6d6c 5f72 6f6f 7420    self.xml_root 
-0000cd80: 3d20 7365 6c66 2e78 6d6c 5f74 7265 652e  = self.xml_tree.
-0000cd90: 6765 7472 6f6f 7428 290d 0a20 2020 2020  getroot()..     
-0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdb0: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
-0000cdc0: 6c5f 6e61 6d65 203d 2027 7365 636f 6e64  l_name = 'second
-0000cdd0: 5f63 6861 6e6e 656c 5f27 202b 206f 732e  _channel_' + os.
-0000cde0: 7061 7468 2e73 706c 6974 6578 7428 6f73  path.splitext(os
-0000cdf0: 2e70 6174 682e 6261 7365 6e61 6d65 2873  .path.basename(s
-0000ce00: 656c 662e 786d 6c5f 7061 7468 2929 5b30  elf.xml_path))[0
-0000ce10: 5d20 2b20 272e 786d 6c27 0d0a 2020 2020  ] + '.xml'..    
-0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce30: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
-0000ce40: 6d6c 5f70 6174 6820 3d20 6f73 2e70 6174  ml_path = os.pat
-0000ce50: 682e 6469 726e 616d 6528 7365 6c66 2e78  h.dirname(self.x
-0000ce60: 6d6c 5f70 6174 6829 0d0a 2020 2020 2020  ml_path)..      
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce80: 7365 6c66 2e5f 6372 6561 7465 5f63 6861  self._create_cha
-0000ce90: 6e6e 656c 5f74 7265 6528 290d 0a0d 0a20  nnel_tree().... 
-0000cea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ceb0: 756e 6971 7565 5f6f 626a 6563 7473 203d  unique_objects =
-0000cec0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-0000ced0: 2073 656c 662e 756e 6971 7565 5f70 726f   self.unique_pro
-0000cee0: 7065 7274 6965 7320 3d20 7b7d 0d0a 2020  perties = {}..  
-0000cef0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-0000cf00: 6c6c 5472 6163 6b49 6473 203d 205b 5d0d  llTrackIds = [].
-0000cf10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000cf20: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
-0000cf30: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0000cf40: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
-0000cf50: 5472 6163 6b49 6473 203d 205b 5d0d 0a20  TrackIds = [].. 
-0000cf60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cf70: 616c 6c5f 7472 6163 6b5f 7072 6f70 6572  all_track_proper
-0000cf80: 7469 6573 203d 205b 5d0d 0a20 2020 2020  ties = []..     
-0000cf90: 2020 2020 2020 2073 656c 662e 7370 6c69         self.spli
-0000cfa0: 745f 706f 696e 7473 5f74 696d 6573 203d  t_points_times =
-0000cfb0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-0000cfc0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000cfd0: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-0000cfe0: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-0000cff0: 6170 7065 6e64 284e 6f6e 6529 0d0a 2020  append(None)..  
-0000d000: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
-0000d010: 6976 6964 696e 6754 7261 636b 4964 732e  ividingTrackIds.
-0000d020: 6170 7065 6e64 284e 6f6e 6529 0d0a 2020  append(None)..  
-0000d030: 2020 2020 2020 2020 2020 7365 6c66 2e4e            self.N
-0000d040: 6f72 6d61 6c54 7261 636b 4964 732e 6170  ormalTrackIds.ap
-0000d050: 7065 6e64 284e 6f6e 6529 0d0a 2020 2020  pend(None)..    
-0000d060: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000d070: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
-0000d080: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
-0000d090: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
-0000d0a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d0b0: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
-0000d0c0: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
-0000d0d0: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
-0000d0e0: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
-0000d0f0: 616c 5472 6163 6b49 6473 2e61 7070 656e  alTrackIds.appen
-0000d100: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
-0000d110: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0000d120: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000d130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d140: 2e53 706f 746f 626a 6563 7473 203d 2073  .Spotobjects = s
-0000d150: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
-0000d160: 6669 6e64 2827 4d6f 6465 6c27 292e 6669  find('Model').fi
-0000d170: 6e64 2827 416c 6c53 706f 7473 2729 0d0a  nd('AllSpots')..
-0000d180: 2020 2020 2020 2020 2020 2020 2320 4578              # Ex
-0000d190: 7472 6163 7420 7468 6520 7472 6163 6b73  tract the tracks
-0000d1a0: 2066 726f 6d20 786d 6c0d 0a20 2020 2020   from xml..     
-0000d1b0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-0000d1c0: 6b73 203d 2073 656c 662e 786d 6c5f 636f  ks = self.xml_co
-0000d1d0: 6e74 656e 742e 6669 6e64 2822 4d6f 6465  ntent.find("Mode
-0000d1e0: 6c22 292e 6669 6e64 2822 416c 6c54 7261  l").find("AllTra
-0000d1f0: 636b 7322 290d 0a20 2020 2020 2020 2020  cks")..         
-0000d200: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000d210: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000d220: 656e 742e 6669 6e64 2822 5365 7474 696e  ent.find("Settin
-0000d230: 6773 2229 2e66 696e 6428 2249 6d61 6765  gs").find("Image
-0000d240: 4461 7461 2229 0d0a 2020 2020 2020 2020  Data")..        
-0000d250: 2020 2020 7365 6c66 2e78 6361 6c69 6272      self.xcalibr
-0000d260: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
-0000d270: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000d280: 2270 6978 656c 7769 6474 6822 2929 0d0a  "pixelwidth"))..
-0000d290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d2a0: 2e79 6361 6c69 6272 6174 696f 6e20 3d20  .ycalibration = 
-0000d2b0: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
-0000d2c0: 6e67 732e 6765 7428 2270 6978 656c 6865  ngs.get("pixelhe
-0000d2d0: 6967 6874 2229 290d 0a20 2020 2020 2020  ight"))..       
-0000d2e0: 2020 2020 2073 656c 662e 7a63 616c 6962       self.zcalib
-0000d2f0: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
-0000d300: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000d310: 2822 766f 7865 6c64 6570 7468 2229 290d  ("voxeldepth")).
-0000d320: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d330: 662e 7463 616c 6962 7261 7469 6f6e 203d  f.tcalibration =
-0000d340: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
-0000d350: 7365 7474 696e 6773 2e67 6574 2822 7469  settings.get("ti
-0000d360: 6d65 696e 7465 7276 616c 2229 2929 0d0a  meinterval")))..
-0000d370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d380: 2e64 6574 6563 746f 7273 6574 7469 6e67  .detectorsetting
-0000d390: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000d3a0: 7465 6e74 2e66 696e 6428 2253 6574 7469  tent.find("Setti
-0000d3b0: 6e67 7322 292e 6669 6e64 2822 4465 7465  ngs").find("Dete
-0000d3c0: 6374 6f72 5365 7474 696e 6773 2229 0d0a  ctorSettings")..
-0000d3d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d3e0: 2e62 6173 6963 7365 7474 696e 6773 203d  .basicsettings =
-0000d3f0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000d400: 742e 6669 6e64 2822 5365 7474 696e 6773  t.find("Settings
-0000d410: 2229 2e66 696e 6428 2242 6173 6963 5365  ").find("BasicSe
-0000d420: 7474 696e 6773 2229 0d0a 2020 2020 2020  ttings")..      
-0000d430: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
-0000d440: 746f 7263 6861 6e6e 656c 203d 2069 6e74  torchannel = int
-0000d450: 2866 6c6f 6174 2873 656c 662e 6465 7465  (float(self.dete
-0000d460: 6374 6f72 7365 7474 696e 6773 2e67 6574  ctorsettings.get
-0000d470: 2822 5441 5247 4554 5f43 4841 4e4e 454c  ("TARGET_CHANNEL
-0000d480: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
-0000d490: 2020 7365 6c66 2e74 7374 6172 7420 3d20    self.tstart = 
-0000d4a0: 696e 7428 666c 6f61 7428 7365 6c66 2e62  int(float(self.b
-0000d4b0: 6173 6963 7365 7474 696e 6773 2e67 6574  asicsettings.get
-0000d4c0: 2822 7473 7461 7274 2229 2929 0d0a 2020  ("tstart")))..  
-0000d4d0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000d4e0: 656e 6420 3d20 696e 7428 666c 6f61 7428  end = int(float(
-0000d4f0: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
-0000d500: 6773 2e67 6574 2822 7465 6e64 2229 2929  gs.get("tend")))
-0000d510: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-0000d520: 2020 2020 2020 7072 696e 7428 2749 7465        print('Ite
-0000d530: 7261 7469 6e67 206f 7665 7220 7370 6f74  rating over spot
-0000d540: 7320 696e 2066 7261 6d65 2729 0d0a 2020  s in frame')..  
-0000d550: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000d560: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
-0000d570: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
-0000d580: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-0000d590: 2020 7769 7468 2063 6f6e 6375 7272 656e    with concurren
-0000d5a0: 742e 6675 7475 7265 732e 5468 7265 6164  t.futures.Thread
-0000d5b0: 506f 6f6c 4578 6563 7574 6f72 286d 6178  PoolExecutor(max
-0000d5c0: 5f77 6f72 6b65 7273 203d 206f 732e 6370  _workers = os.cp
-0000d5d0: 755f 636f 756e 7428 2929 2061 7320 6578  u_count()) as ex
-0000d5e0: 6563 7574 6f72 3a0d 0a20 2020 2020 2020  ecutor:..       
-0000d5f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000d600: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
-0000d610: 7261 6d65 2069 6e20 7365 6c66 2e53 706f  rame in self.Spo
-0000d620: 746f 626a 6563 7473 2e66 696e 6461 6c6c  tobjects.findall
-0000d630: 2827 5370 6f74 7349 6e46 7261 6d65 2729  ('SpotsInFrame')
-0000d640: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d650: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000d660: 7574 7572 6573 2e61 7070 656e 6428 6578  utures.append(ex
-0000d670: 6563 7574 6f72 2e73 7562 6d69 7428 7365  ecutor.submit(se
-0000d680: 6c66 2e5f 6d61 7374 6572 5f73 706f 745f  lf._master_spot_
-0000d690: 636f 6d70 7574 6572 2c20 6672 616d 6529  computer, frame)
-0000d6a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d6b0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-0000d6c0: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-0000d6d0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000cd70: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
+0000cd80: 656c 5f78 6d6c 5f70 6174 6820 3d20 6f73  el_xml_path = os
+0000cd90: 2e70 6174 682e 6469 726e 616d 6528 7365  .path.dirname(se
+0000cda0: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
+0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdc0: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
+0000cdd0: 5f63 6861 6e6e 656c 5f74 7265 6528 290d  _channel_tree().
+0000cde0: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
+0000cdf0: 656c 662e 756e 6971 7565 5f6f 626a 6563  elf.unique_objec
+0000ce00: 7473 203d 207b 7d0d 0a20 2020 2020 2020  ts = {}..       
+0000ce10: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+0000ce20: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+0000ce30: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000ce40: 6c66 2e41 6c6c 5472 6163 6b49 6473 203d  lf.AllTrackIds =
+0000ce50: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000ce60: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
+0000ce70: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
+0000ce80: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
+0000ce90: 726d 616c 5472 6163 6b49 6473 203d 205b  rmalTrackIds = [
+0000cea0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+0000ceb0: 656c 662e 616c 6c5f 7472 6163 6b5f 7072  elf.all_track_pr
+0000cec0: 6f70 6572 7469 6573 203d 205b 5d0d 0a20  operties = [].. 
+0000ced0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cee0: 7370 6c69 745f 706f 696e 7473 5f74 696d  split_points_tim
+0000cef0: 6573 203d 205b 5d0d 0a0d 0a20 2020 2020  es = []....     
+0000cf00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000cf10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000cf20: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+0000cf30: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
+0000cf40: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000cf50: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
+0000cf60: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
+0000cf70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000cf80: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+0000cf90: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
+0000cfa0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000cfb0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+0000cfc0: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
+0000cfd0: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
+0000cfe0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000cff0: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
+0000d000: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
+0000d010: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
+0000d020: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d030: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
+0000d040: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
+0000d050: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
+0000d060: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d070: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d080: 7365 6c66 2e53 706f 746f 626a 6563 7473  self.Spotobjects
+0000d090: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
+0000d0a0: 656e 742e 6669 6e64 2827 4d6f 6465 6c27  ent.find('Model'
+0000d0b0: 292e 6669 6e64 2827 416c 6c53 706f 7473  ).find('AllSpots
+0000d0c0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+0000d0d0: 2320 4578 7472 6163 7420 7468 6520 7472  # Extract the tr
+0000d0e0: 6163 6b73 2066 726f 6d20 786d 6c0d 0a20  acks from xml.. 
+0000d0f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d100: 7472 6163 6b73 203d 2073 656c 662e 786d  tracks = self.xm
+0000d110: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
+0000d120: 4d6f 6465 6c22 292e 6669 6e64 2822 416c  Model").find("Al
+0000d130: 6c54 7261 636b 7322 290d 0a20 2020 2020  lTracks")..     
+0000d140: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000d150: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
+0000d160: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
+0000d170: 7474 696e 6773 2229 2e66 696e 6428 2249  ttings").find("I
+0000d180: 6d61 6765 4461 7461 2229 0d0a 2020 2020  mageData")..    
+0000d190: 2020 2020 2020 2020 7365 6c66 2e78 6361          self.xca
+0000d1a0: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
+0000d1b0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000d1c0: 6765 7428 2270 6978 656c 7769 6474 6822  get("pixelwidth"
+0000d1d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000d1e0: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+0000d1f0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000d200: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
+0000d210: 656c 6865 6967 6874 2229 290d 0a20 2020  elheight"))..   
+0000d220: 2020 2020 2020 2020 2073 656c 662e 7a63           self.zc
+0000d230: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
+0000d240: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000d250: 2e67 6574 2822 766f 7865 6c64 6570 7468  .get("voxeldepth
+0000d260: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+0000d270: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
+0000d280: 6f6e 203d 2069 6e74 2866 6c6f 6174 2873  on = int(float(s
+0000d290: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000d2a0: 2822 7469 6d65 696e 7465 7276 616c 2229  ("timeinterval")
+0000d2b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000d2c0: 7365 6c66 2e64 6574 6563 746f 7273 6574  self.detectorset
+0000d2d0: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
+0000d2e0: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
+0000d2f0: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
+0000d300: 4465 7465 6374 6f72 5365 7474 696e 6773  DetectorSettings
+0000d310: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000d320: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
+0000d330: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
+0000d340: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
+0000d350: 696e 6773 2229 2e66 696e 6428 2242 6173  ings").find("Bas
+0000d360: 6963 5365 7474 696e 6773 2229 0d0a 2020  icSettings")..  
+0000d370: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000d380: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
+0000d390: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
+0000d3a0: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
+0000d3b0: 2e67 6574 2822 5441 5247 4554 5f43 4841  .get("TARGET_CHA
+0000d3c0: 4e4e 454c 2229 2929 0d0a 2020 2020 2020  NNEL")))..      
+0000d3d0: 2020 2020 2020 7365 6c66 2e74 7374 6172        self.tstar
+0000d3e0: 7420 3d20 696e 7428 666c 6f61 7428 7365  t = int(float(se
+0000d3f0: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
+0000d400: 2e67 6574 2822 7473 7461 7274 2229 2929  .get("tstart")))
+0000d410: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d420: 6c66 2e74 656e 6420 3d20 696e 7428 666c  lf.tend = int(fl
+0000d430: 6f61 7428 7365 6c66 2e62 6173 6963 7365  oat(self.basicse
+0000d440: 7474 696e 6773 2e67 6574 2822 7465 6e64  ttings.get("tend
+0000d450: 2229 2929 2020 2020 2020 0d0a 0d0a 2020  ")))      ....  
+0000d460: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000d470: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
+0000d480: 7370 6f74 7320 696e 2066 7261 6d65 2729  spots in frame')
+0000d490: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d4a0: 6c66 2e63 6f75 6e74 203d 2030 0d0a 2020  lf.count = 0..  
+0000d4b0: 2020 2020 2020 2020 2020 6675 7475 7265            future
+0000d4c0: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+0000d4d0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
+0000d4e0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
+0000d4f0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
+0000d500: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
+0000d510: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
+0000d520: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
+0000d530: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000d540: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d550: 6f72 2066 7261 6d65 2069 6e20 7365 6c66  or frame in self
+0000d560: 2e53 706f 746f 626a 6563 7473 2e66 696e  .Spotobjects.fin
+0000d570: 6461 6c6c 2827 5370 6f74 7349 6e46 7261  dall('SpotsInFra
+0000d580: 6d65 2729 3a0d 0a20 2020 2020 2020 2020  me'):..         
+0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5a0: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
+0000d5b0: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
+0000d5c0: 7428 7365 6c66 2e5f 6d61 7374 6572 5f73  t(self._master_s
+0000d5d0: 706f 745f 636f 6d70 7574 6572 2c20 6672  pot_computer, fr
+0000d5e0: 616d 6529 290d 0a20 2020 2020 2020 2020  ame))..         
+0000d5f0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+0000d600: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+0000d610: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d630: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d660: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+0000d670: 6265 6c20 3d20 2243 6f6c 6c65 6374 696e  bel = "Collectin
+0000d680: 6720 5370 6f74 7322 0d0a 2020 2020 2020  g Spots"..      
+0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6a0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000d6b0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+0000d6c0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6e0: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
+0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d710: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000d720: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
-0000d730: 3d20 2243 6f6c 6c65 6374 696e 6720 5370  = "Collecting Sp
-0000d740: 6f74 7322 0d0a 2020 2020 2020 2020 2020  ots"..          
+0000d710: 2020 206c 656e 2866 7574 7572 6573 292c     len(futures),
+0000d720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
 0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000d770: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
-0000d780: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7a0: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
-0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000d7d0: 656e 2866 7574 7572 6573 292c 0d0a 2020  en(futures),..  
-0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7f0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-0000d800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d760: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000d770: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
+0000d780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d790: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
+0000d7a0: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
+0000d7b0: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
+0000d7c0: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000d7f0: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+0000d800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000d830: 6172 2e73 686f 7728 290d 0a0d 0a20 2020  ar.show()....   
-0000d840: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000d850: 2072 2069 6e20 636f 6e63 7572 7265 6e74   r in concurrent
-0000d860: 2e66 7574 7572 6573 2e61 735f 636f 6d70  .futures.as_comp
-0000d870: 6c65 7465 6428 6675 7475 7265 7329 3a0d  leted(futures):.
-0000d880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d820: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000d830: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000d840: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d860: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000d870: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+0000d880: 203d 2020 7365 6c66 2e63 6f75 6e74 0d0a   =  self.count..
 0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8a0: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
-0000d8b0: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
-0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000d8e0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000d8f0: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
-0000d900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d920: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000d930: 7373 5f62 6172 2e76 616c 7565 203d 2020  ss_bar.value =  
-0000d940: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
-0000d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d960: 2020 2020 2020 2020 2020 2020 722e 7265              r.re
-0000d970: 7375 6c74 2829 2020 2020 0d0a 0d0a 2020  sult()    ....  
-0000d980: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d990: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-0000d9a0: 4974 6572 6174 696e 6720 6f76 6572 2074  Iterating over t
-0000d9b0: 7261 636b 7320 7b6c 656e 2873 656c 662e  racks {len(self.
-0000d9c0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000d9d0: 6473 297d 2729 2020 0d0a 2020 2020 2020  ds)}')  ..      
-0000d9e0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000d9f0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
-0000da00: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
-0000da10: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000da20: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-0000da30: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
-0000da40: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
-0000da50: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
-0000da60: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
-0000da70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000da80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000da90: 2020 2020 2066 6f72 2074 7261 636b 2069       for track i
-0000daa0: 6e20 7365 6c66 2e74 7261 636b 732e 6669  n self.tracks.fi
-0000dab0: 6e64 616c 6c28 2754 7261 636b 2729 3a0d  ndall('Track'):.
-0000dac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dad0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daf0: 2020 2074 7261 636b 5f69 6420 3d20 696e     track_id = in
-0000db00: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
-0000db10: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
-0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db30: 2020 2020 2020 2020 6966 2074 7261 636b          if track
-0000db40: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
-0000db50: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
-0000db60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8b0: 722e 7265 7375 6c74 2829 2020 2020 0d0a  r.result()    ..
+0000d8c0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000d8d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000d8e0: 7428 6627 4974 6572 6174 696e 6720 6f76  t(f'Iterating ov
+0000d8f0: 6572 2074 7261 636b 7320 7b6c 656e 2873  er tracks {len(s
+0000d900: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000d910: 636b 5f69 6473 297d 2729 2020 0d0a 2020  ck_ids)}')  ..  
+0000d920: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000d930: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+0000d940: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
+0000d950: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+0000d960: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
+0000d970: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
+0000d980: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
+0000d990: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
+0000d9a0: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
+0000d9b0: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
+0000d9c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000d9d0: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
+0000d9e0: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
+0000d9f0: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
+0000da00: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+0000da10: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+0000da40: 3d20 696e 7428 7472 6163 6b2e 6765 7428  = int(track.get(
+0000da50: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+0000da60: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000da70: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+0000da80: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
+0000da90: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+0000daa0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dac0: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
+0000dad0: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
+0000dae0: 6d69 7428 7365 6c66 2e5f 6d61 7374 6572  mit(self._master
+0000daf0: 5f74 7261 636b 5f63 6f6d 7075 7465 722c  _track_computer,
+0000db00: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
+0000db10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000db20: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+0000db30: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+0000db40: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+0000db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 2066 7574 7572 6573 2e61 7070 656e 6428   futures.append(
-0000db90: 6578 6563 7574 6f72 2e73 7562 6d69 7428  executor.submit(
-0000dba0: 7365 6c66 2e5f 6d61 7374 6572 5f74 7261  self._master_tra
-0000dbb0: 636b 5f63 6f6d 7075 7465 722c 2074 7261  ck_computer, tra
-0000dbc0: 636b 2c20 7472 6163 6b5f 6964 2929 0d0a  ck, track_id))..
-0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbe0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-0000dbf0: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-0000dc00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000db80: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000db90: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+0000dba0: 203d 2022 436f 6c6c 6563 7469 6e67 2054   = "Collecting T
+0000dbb0: 7261 636b 7322 0d0a 2020 2020 2020 2020  racks"..        
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbd0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000dbe0: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
+0000dbf0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc10: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
+0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc40: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000dc50: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
-0000dc60: 436f 6c6c 6563 7469 6e67 2054 7261 636b  Collecting Track
-0000dc70: 7322 0d0a 2020 2020 2020 2020 2020 2020  s"..            
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000dca0: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
-0000dcb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
-0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcf0: 2020 2020 2020 2020 2020 2020 206c 656e               len
-0000dd00: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
-0000dd10: 7261 636b 5f69 6473 292c 0d0a 2020 2020  rack_ids),..    
-0000dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd30: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000dd60: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000dd70: 2e73 686f 7728 290d 0a0d 0a0d 0a20 2020  .show()......   
-0000dd80: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000dd90: 2072 2069 6e20 636f 6e63 7572 7265 6e74   r in concurrent
-0000dda0: 2e66 7574 7572 6573 2e61 735f 636f 6d70  .futures.as_comp
-0000ddb0: 6c65 7465 6428 6675 7475 7265 7329 3a0d  leted(futures):.
-0000ddc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc40: 206c 656e 2873 656c 662e 6669 6c74 6572   len(self.filter
+0000dc50: 6564 5f74 7261 636b 5f69 6473 292c 0d0a  ed_track_ids),..
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000dcb0: 5f62 6172 2e73 686f 7728 290d 0a0d 0a0d  _bar.show().....
+0000dcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dcd0: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
+0000dce0: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
+0000dcf0: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
+0000dd00: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd20: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000dd30: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+0000dd40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd60: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000dd70: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000dd80: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dda0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000ddb0: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+0000ddc0: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
 0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dde0: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
-0000ddf0: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000de20: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000de30: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
-0000de40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de60: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000de70: 7373 5f62 6172 2e76 616c 7565 203d 2073  ss_bar.value = s
-0000de80: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
-0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dea0: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
-0000deb0: 756c 7428 290d 0a20 2020 2020 2020 2020  ult()..         
-0000dec0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000ded0: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
-0000dee0: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
-0000def0: 7420 4e6f 6e65 3a20 200d 0a20 2020 2020  t None:  ..     
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df10: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000df20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000df30: 5f63 7265 6174 655f 7365 636f 6e64 5f63  _create_second_c
-0000df40: 6861 6e6e 656c 5f78 6d6c 2829 0d0a 2020  hannel_xml()..  
-0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df60: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-0000df70: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
-0000df80: 2920 696e 2073 656c 662e 6772 6170 685f  ) in self.graph_
-0000df90: 7370 6c69 742e 6974 656d 7328 293a 0d0a  split.items():..
-0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfb0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfd0: 2020 2020 2020 2020 2064 6175 6768 7465           daughte
-0000dfe0: 725f 7472 6163 6b5f 6964 203d 2020 696e  r_track_id =  in
-0000dff0: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
-0000e000: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-0000e010: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
-0000e020: 7428 6b29 295d 5b73 656c 662e 756e 6971  t(k))][self.uniq
-0000e030: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
-0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e050: 2020 2020 2020 2020 2020 7061 7265 6e74            parent
-0000e060: 5f74 7261 636b 5f69 6420 3d20 696e 7428  _track_id = int(
-0000e070: 666c 6f61 7428 7374 7228 7365 6c66 2e75  float(str(self.u
-0000e080: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000e090: 7274 6965 735b 696e 7428 666c 6f61 7428  rties[int(float(
-0000e0a0: 7629 295d 5b73 656c 662e 756e 6971 7565  v))][self.unique
-0000e0b0: 6964 5f6b 6579 5d29 2929 0d0a 2020 2020  id_key])))..    
-0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0d0: 2020 2020 2020 2020 7365 6c66 2e67 7261          self.gra
-0000e0e0: 7068 5f74 7261 636b 735b 6461 7567 6874  ph_tracks[daught
-0000e0f0: 6572 5f74 7261 636b 5f69 645d 203d 2070  er_track_id] = p
-0000e100: 6172 656e 745f 7472 6163 6b5f 6964 0d0a  arent_track_id..
-0000e110: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-0000e120: 696e 7428 2767 6574 7469 6e67 2061 7474  int('getting att
-0000e130: 7269 6275 7465 7327 2920 2020 2020 2020  ributes')       
-0000e140: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000e150: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
-0000e160: 5f61 7474 7269 6275 7465 7328 290d 0a20  _attributes().. 
-0000e170: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000e180: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000e190: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
-0000e1a0: 2020 2020 666f 7220 7472 6163 6b5f 6964      for track_id
-0000e1b0: 2069 6e20 7365 6c66 2e66 696c 7465 7265   in self.filtere
-0000e1c0: 645f 7472 6163 6b5f 6964 733a 0d0a 2020  d_track_ids:..  
-0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-0000e200: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-0000e210: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e230: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e240: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
-0000e250: 6162 656c 203d 2022 4a75 7374 206f 6e65  abel = "Just one
-0000e260: 206d 6f72 6520 7468 696e 6722 0d0a 2020   more thing"..  
-0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dde0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000ddf0: 2e72 6573 756c 7428 290d 0a20 2020 2020  .result()..     
+0000de00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000de10: 2020 2020 2069 6620 7365 6c66 2e63 6861       if self.cha
+0000de20: 6e6e 656c 5f73 6567 5f69 6d61 6765 2069  nnel_seg_image i
+0000de30: 7320 6e6f 7420 4e6f 6e65 3a20 200d 0a20  s not None:  .. 
+0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000de60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000de70: 656c 662e 5f63 7265 6174 655f 7365 636f  elf._create_seco
+0000de80: 6e64 5f63 6861 6e6e 656c 5f78 6d6c 2829  nd_channel_xml()
+0000de90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dea0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+0000deb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000dec0: 286b 2c76 2920 696e 2073 656c 662e 6772  (k,v) in self.gr
+0000ded0: 6170 685f 7370 6c69 742e 6974 656d 7328  aph_split.items(
+0000dee0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000def0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000df00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df10: 2020 2020 2020 2020 2020 2020 2064 6175               dau
+0000df20: 6768 7465 725f 7472 6163 6b5f 6964 203d  ghter_track_id =
+0000df30: 2020 696e 7428 666c 6f61 7428 7374 7228    int(float(str(
+0000df40: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+0000df50: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+0000df60: 666c 6f61 7428 6b29 295d 5b73 656c 662e  float(k))][self.
+0000df70: 756e 6971 7565 6964 5f6b 6579 5d29 2929  uniqueid_key])))
+0000df80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000df90: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000dfa0: 7265 6e74 5f74 7261 636b 5f69 6420 3d20  rent_track_id = 
+0000dfb0: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
+0000dfc0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+0000dfd0: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
+0000dfe0: 6f61 7428 7629 295d 5b73 656c 662e 756e  oat(v))][self.un
+0000dff0: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
+0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e020: 2e67 7261 7068 5f74 7261 636b 735b 6461  .graph_tracks[da
+0000e030: 7567 6874 6572 5f74 7261 636b 5f69 645d  ughter_track_id]
+0000e040: 203d 2070 6172 656e 745f 7472 6163 6b5f   = parent_track_
+0000e050: 6964 0d0a 0d0a 2020 2020 2020 2020 2020  id....          
+0000e060: 2020 7072 696e 7428 2767 6574 7469 6e67    print('getting
+0000e070: 2061 7474 7269 6275 7465 7327 2920 2020   attributes')   
+0000e080: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000e090: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e0a0: 5f67 6574 5f61 7474 7269 6275 7465 7328  _get_attributes(
+0000e0b0: 290d 0a20 2020 2020 2020 2020 2020 0d0a  )..           ..
+0000e0c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e0d0: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
+0000e0e0: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
+0000e0f0: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
+0000e100: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
+0000e110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e130: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000e140: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+0000e150: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e180: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000e190: 6172 2e6c 6162 656c 203d 2022 4a75 7374  ar.label = "Just
+0000e1a0: 206f 6e65 206d 6f72 6520 7468 696e 6722   one more thing"
+0000e1b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000e1e0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+0000e1f0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e220: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
+0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e250: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
+0000e260: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000e270: 636b 5f69 6473 292c 0d0a 2020 2020 2020  ck_ids),..      
 0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e290: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000e2a0: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
-0000e2b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2a0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2e0: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+0000e2d0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000e2e0: 6172 2e73 686f 7728 290d 0a20 2020 2020  ar.show()..     
 0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e310: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
-0000e320: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000e330: 6473 292c 0d0a 2020 2020 2020 2020 2020  ds),..          
+0000e310: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+0000e320: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e360: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e380: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e390: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
-0000e3a0: 686f 7728 290d 0a20 2020 2020 2020 2020  how()..         
-0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e3d0: 656c 662e 636f 756e 7420 3d20 7365 6c66  elf.count = self
-0000e3e0: 2e63 6f75 6e74 202b 2031 0d0a 2020 2020  .count + 1..    
-0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e410: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000e420: 735f 6261 722e 7661 6c75 6520 3d20 7365  s_bar.value = se
-0000e430: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
+0000e350: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000e360: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
+0000e370: 3d20 7365 6c66 2e63 6f75 6e74 0d0a 2020  = self.count..  
+0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3a0: 2020 7365 6c66 2e5f 6669 6e61 6c5f 7472    self._final_tr
+0000e3b0: 6163 6b73 2874 7261 636b 5f69 6429 200d  acks(track_id) .
+0000e3c0: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0000e3d0: 6620 7365 6c66 2e66 6f75 7269 6572 3a0d  f self.fourier:.
+0000e3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e3f0: 2020 2020 7072 696e 7428 2763 6f6d 7075      print('compu
+0000e400: 7469 6e67 2046 6f75 7269 6572 2729 0d0a  ting Fourier')..
+0000e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e420: 2020 2073 656c 662e 5f63 6f6d 7075 7465     self._compute
+0000e430: 5f70 6865 6e6f 7479 7065 7328 2920 2020  _phenotypes()   
 0000e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e450: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e460: 6c66 2e5f 6669 6e61 6c5f 7472 6163 6b73  lf._final_tracks
-0000e470: 2874 7261 636b 5f69 6429 200d 0a0d 0a20  (track_id) .... 
-0000e480: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000e490: 6c66 2e66 6f75 7269 6572 3a0d 0a20 2020  lf.fourier:..   
-0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4b0: 7072 696e 7428 2763 6f6d 7075 7469 6e67  print('computing
-0000e4c0: 2046 6f75 7269 6572 2729 0d0a 2020 2020   Fourier')..    
-0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e4e0: 656c 662e 5f63 6f6d 7075 7465 5f70 6865  elf._compute_phe
-0000e4f0: 6e6f 7479 7065 7328 2920 2020 2020 2020  notypes()       
+0000e450: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e460: 2020 2073 656c 662e 5f74 656d 706f 7261     self._tempora
+0000e470: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
+0000e480: 6528 2920 2020 2020 2020 200d 0a0d 0a0d  e()        .....
+0000e490: 0a20 2020 2064 6566 205f 6372 6561 7465  .    def _create
+0000e4a0: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
+0000e4b0: 786d 6c28 7365 6c66 293a 0d0a 2020 2020  xml(self):..    
+0000e4c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000e4d0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+0000e4e0: 6e6e 656c 5f66 696c 7465 7265 645f 7472  nnel_filtered_tr
+0000e4f0: 6163 6b73 203d 205b 5d20 2020 200d 0a20  acks = []    .. 
 0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e510: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-0000e520: 656c 662e 5f74 656d 706f 7261 6c5f 706c  elf._temporal_pl
-0000e530: 6f74 735f 7472 6163 6b6d 6174 6528 2920  ots_trackmate() 
-0000e540: 2020 2020 2020 200d 0a0d 0a0d 0a20 2020         ......   
-0000e550: 2064 6566 205f 6372 6561 7465 5f73 6563   def _create_sec
-0000e560: 6f6e 645f 6368 616e 6e65 6c5f 786d 6c28  ond_channel_xml(
-0000e570: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-0000e580: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000e590: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
-0000e5a0: 5f66 696c 7465 7265 645f 7472 6163 6b73  _filtered_tracks
-0000e5b0: 203d 205b 5d20 2020 200d 0a20 2020 2020   = []    ..     
-0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000e5d0: 7269 6e74 2827 5472 616e 7366 6572 7269  rint('Transferri
-0000e5e0: 6e67 2058 4d4c 2729 2020 2020 2020 2020  ng XML')        
-0000e5f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000e600: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000e610: 2053 706f 746f 626a 6563 7420 696e 2073   Spotobject in s
-0000e620: 656c 662e 786d 6c5f 726f 6f74 2e69 7465  elf.xml_root.ite
-0000e630: 7228 2753 706f 7427 293a 0d0a 2020 2020  r('Spot'):..    
-0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 2020 2020 2020 2020 6365 6c6c 5f69 6420          cell_id 
-0000e660: 3d20 696e 7428 5370 6f74 6f62 6a65 6374  = int(Spotobject
-0000e670: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
-0000e680: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6a0: 2020 2020 6966 2063 656c 6c5f 6964 2069      if cell_id i
-0000e6b0: 6e20 7365 6c66 2e63 6861 6e6e 656c 5f75  n self.channel_u
-0000e6c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000e6d0: 7274 6965 732e 6b65 7973 2829 3a20 2020  rties.keys():   
-0000e6e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e700: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e720: 2020 2020 2020 2020 206e 6577 5f70 6f73           new_pos
-0000e730: 6974 696f 6e78 203d 2020 7365 6c66 2e63  itionx =  self.c
-0000e740: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-0000e750: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-0000e760: 6c6c 5f69 645d 5b73 656c 662e 7870 6f73  ll_id][self.xpos
-0000e770: 6964 5f6b 6579 5d0d 0a20 2020 2020 2020  id_key]..       
-0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e790: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000e7a0: 5f70 6f73 6974 696f 6e79 203d 2020 7365  _positiony =  se
-0000e7b0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-0000e7c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000e7d0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
-0000e7e0: 7970 6f73 6964 5f6b 6579 5d0d 0a20 2020  yposid_key]..   
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e810: 206e 6577 5f70 6f73 6974 696f 6e7a 203d   new_positionz =
-0000e820: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
-0000e830: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000e840: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
-0000e850: 656c 662e 7a70 6f73 6964 5f6b 6579 5d0d  elf.zposid_key].
-0000e860: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e880: 2020 2020 2020 206e 6577 5f74 6f74 616c         new_total
-0000e890: 5f69 6e74 656e 7369 7479 203d 2073 656c  _intensity = sel
-0000e8a0: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000e8b0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000e8c0: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e74  [cell_id][self.t
-0000e8d0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
-0000e8e0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e900: 2020 2020 2020 2020 206e 6577 5f6d 6561           new_mea
-0000e910: 6e5f 696e 7465 6e73 6974 7920 3d20 7365  n_intensity = se
-0000e920: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-0000e930: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000e940: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
-0000e950: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
-0000e960: 6579 5d0d 0a0d 0a20 2020 2020 2020 2020  ey]....         
-0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e980: 2020 2020 2020 2020 2020 206e 6577 5f72             new_r
-0000e990: 6164 6975 7320 3d20 7365 6c66 2e63 6861  adius = self.cha
-0000e9a0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000e9b0: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-0000e9c0: 5f69 645d 5b73 656c 662e 7261 6469 7573  _id][self.radius
-0000e9d0: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2020 2020 2020 2020 2020 206e 6577 5f71             new_q
-0000ea00: 7561 6c69 7479 203d 2073 656c 662e 6368  uality = self.ch
-0000ea10: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000ea20: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000ea30: 6c5f 6964 5d5b 7365 6c66 2e71 7561 6c69  l_id][self.quali
-0000ea40: 7479 5f6b 6579 5d0d 0a20 2020 2020 2020  ty_key]..       
-0000ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea60: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000ea70: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-0000ea80: 6173 6b20 3d20 7365 6c66 2e63 6861 6e6e  ask = self.chann
-0000ea90: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-0000eaa0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-0000eab0: 645d 5b73 656c 662e 6469 7374 616e 6365  d][self.distance
-0000eac0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 5d0d  _cell_mask_key].
-0000ead0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000e510: 2020 2070 7269 6e74 2827 5472 616e 7366     print('Transf
+0000e520: 6572 7269 6e67 2058 4d4c 2729 2020 2020  erring XML')    
+0000e530: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e550: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
+0000e560: 696e 2073 656c 662e 786d 6c5f 726f 6f74  in self.xml_root
+0000e570: 2e69 7465 7228 2753 706f 7427 293a 0d0a  .iter('Spot'):..
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+0000e5a0: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
+0000e5b0: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
+0000e5c0: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2020 2020 2020 2020 6966 2063 656c 6c5f          if cell_
+0000e5f0: 6964 2069 6e20 7365 6c66 2e63 6861 6e6e  id in self.chann
+0000e600: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000e610: 726f 7065 7274 6965 732e 6b65 7973 2829  roperties.keys()
+0000e620: 3a20 2020 2020 2020 200d 0a20 2020 2020  :        ..     
+0000e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e640: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000e670: 5f70 6f73 6974 696f 6e78 203d 2020 7365  _positionx =  se
+0000e680: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000e690: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000e6a0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000e6b0: 7870 6f73 6964 5f6b 6579 5d0d 0a20 2020  xposid_key]..   
+0000e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6e0: 206e 6577 5f70 6f73 6974 696f 6e79 203d   new_positiony =
+0000e6f0: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+0000e700: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000e710: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
+0000e720: 656c 662e 7970 6f73 6964 5f6b 6579 5d0d  elf.yposid_key].
+0000e730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e750: 2020 2020 206e 6577 5f70 6f73 6974 696f       new_positio
+0000e760: 6e7a 203d 2020 7365 6c66 2e63 6861 6e6e  nz =  self.chann
+0000e770: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000e780: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+0000e790: 645d 5b73 656c 662e 7a70 6f73 6964 5f6b  d][self.zposid_k
+0000e7a0: 6579 5d0d 0a0d 0a20 2020 2020 2020 2020  ey]....         
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7c0: 2020 2020 2020 2020 2020 206e 6577 5f74             new_t
+0000e7d0: 6f74 616c 5f69 6e74 656e 7369 7479 203d  otal_intensity =
+0000e7e0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+0000e7f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000e800: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
+0000e810: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000e820: 7479 5f6b 6579 5d0d 0a20 2020 2020 2020  ty_key]..       
+0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e840: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000e850: 5f6d 6561 6e5f 696e 7465 6e73 6974 7920  _mean_intensity 
+0000e860: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f75  = self.channel_u
+0000e870: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000e880: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
+0000e890: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000e8a0: 7479 5f6b 6579 5d0d 0a0d 0a20 2020 2020  ty_key]....     
+0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e8d0: 6577 5f72 6164 6975 7320 3d20 7365 6c66  ew_radius = self
+0000e8e0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000e8f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000e900: 6365 6c6c 5f69 645d 5b73 656c 662e 7261  cell_id][self.ra
+0000e910: 6469 7573 5f6b 6579 5d0d 0a20 2020 2020  dius_key]..     
+0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e930: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e940: 6577 5f71 7561 6c69 7479 203d 2073 656c  ew_quality = sel
+0000e950: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000e960: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000e970: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e71  [cell_id][self.q
+0000e980: 7561 6c69 7479 5f6b 6579 5d0d 0a20 2020  uality_key]..   
+0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 206e 6577 5f64 6973 7461 6e63 655f 6365   new_distance_ce
+0000e9c0: 6c6c 5f6d 6173 6b20 3d20 7365 6c66 2e63  ll_mask = self.c
+0000e9d0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+0000e9e0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000e9f0: 6c6c 5f69 645d 5b73 656c 662e 6469 7374  ll_id][self.dist
+0000ea00: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+0000ea10: 6579 5d0d 0a0d 0a20 2020 2020 2020 2020  ey]....         
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea30: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000ea40: 626a 6563 742e 7365 7428 7365 6c66 2e78  bject.set(self.x
+0000ea50: 706f 7369 645f 6b65 792c 2073 7472 286e  posid_key, str(n
+0000ea60: 6577 5f70 6f73 6974 696f 6e78 2929 2020  ew_positionx))  
+0000ea70: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea90: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
+0000eaa0: 6563 742e 7365 7428 7365 6c66 2e79 706f  ect.set(self.ypo
+0000eab0: 7369 645f 6b65 792c 2073 7472 286e 6577  sid_key, str(new
+0000eac0: 5f70 6f73 6974 696f 6e79 2929 0d0a 2020  _positiony))..  
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
-0000eb00: 742e 7365 7428 7365 6c66 2e78 706f 7369  t.set(self.xposi
-0000eb10: 645f 6b65 792c 2073 7472 286e 6577 5f70  d_key, str(new_p
-0000eb20: 6f73 6974 696f 6e78 2929 2020 2020 200d  ositionx))     .
-0000eb30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb50: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-0000eb60: 7365 7428 7365 6c66 2e79 706f 7369 645f  set(self.yposid_
-0000eb70: 6b65 792c 2073 7472 286e 6577 5f70 6f73  key, str(new_pos
-0000eb80: 6974 696f 6e79 2929 0d0a 2020 2020 2020  itiony))..      
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eba0: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-0000ebb0: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
-0000ebc0: 662e 7a70 6f73 6964 5f6b 6579 2c20 7374  f.zposid_key, st
-0000ebd0: 7228 6e65 775f 706f 7369 7469 6f6e 7a29  r(new_positionz)
-0000ebe0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0000ebf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec00: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
-0000ec10: 6563 742e 7365 7428 7365 6c66 2e74 6f74  ect.set(self.tot
-0000ec20: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-0000ec30: 2c20 7374 7228 6e65 775f 746f 7461 6c5f  , str(new_total_
-0000ec40: 696e 7465 6e73 6974 7929 2920 2020 2020  intensity))     
-0000ec50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000eaf0: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+0000eb00: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
+0000eb10: 2c20 7374 7228 6e65 775f 706f 7369 7469  , str(new_positi
+0000eb20: 6f6e 7a29 290d 0a0d 0a20 2020 2020 2020  onz))....       
+0000eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb40: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000eb50: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000eb60: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000eb70: 5f6b 6579 2c20 7374 7228 6e65 775f 746f  _key, str(new_to
+0000eb80: 7461 6c5f 696e 7465 6e73 6974 7929 2920  tal_intensity)) 
+0000eb90: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000eba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebb0: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
+0000ebc0: 6a65 6374 2e73 6574 2873 656c 662e 6d65  ject.set(self.me
+0000ebd0: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
+0000ebe0: 2c20 7374 7228 6e65 775f 6d65 616e 5f69  , str(new_mean_i
+0000ebf0: 6e74 656e 7369 7479 2929 0d0a 0d0a 2020  ntensity))....  
+0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec20: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+0000ec30: 2873 656c 662e 7261 6469 7573 5f6b 6579  (self.radius_key
+0000ec40: 2c20 7374 7228 6e65 775f 7261 6469 7573  , str(new_radius
+0000ec50: 2929 2020 2020 200d 0a20 2020 2020 2020  ))     ..       
 0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec70: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
-0000ec80: 2e73 6574 2873 656c 662e 6d65 616e 5f69  .set(self.mean_i
-0000ec90: 6e74 656e 7369 7479 5f6b 6579 2c20 7374  ntensity_key, st
-0000eca0: 7228 6e65 775f 6d65 616e 5f69 6e74 656e  r(new_mean_inten
-0000ecb0: 7369 7479 2929 0d0a 0d0a 2020 2020 2020  sity))....      
+0000ec70: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000ec80: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000ec90: 2e71 7561 6c69 7479 5f6b 6579 2c20 7374  .quality_key, st
+0000eca0: 7228 6e65 775f 7175 616c 6974 7929 290d  r(new_quality)).
+0000ecb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-0000ece0: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
-0000ecf0: 662e 7261 6469 7573 5f6b 6579 2c20 7374  f.radius_key, st
-0000ed00: 7228 6e65 775f 7261 6469 7573 2929 2020  r(new_radius))  
-0000ed10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ecd0: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
+0000ece0: 7365 7428 7365 6c66 2e64 6973 7461 6e63  set(self.distanc
+0000ecf0: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 792c  e_cell_mask_key,
+0000ed00: 2073 7472 286e 6577 5f64 6973 7461 6e63   str(new_distanc
+0000ed10: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
 0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed30: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
-0000ed40: 6563 742e 7365 7428 7365 6c66 2e71 7561  ect.set(self.qua
-0000ed50: 6c69 7479 5f6b 6579 2c20 7374 7228 6e65  lity_key, str(ne
-0000ed60: 775f 7175 616c 6974 7929 290d 0a20 2020  w_quality))..   
-0000ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed90: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
-0000eda0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-0000edb0: 6c6c 5f6d 6173 6b5f 6b65 792c 2073 7472  ll_mask_key, str
-0000edc0: 286e 6577 5f64 6973 7461 6e63 655f 6365  (new_distance_ce
-0000edd0: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000ee00: 6620 7365 6c66 2e74 7261 636b 6964 5f6b  f self.trackid_k
-0000ee10: 6579 2069 6e20 7365 6c66 2e75 6e69 7175  ey in self.uniqu
-0000ee20: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000ee30: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-0000ee40: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
-0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee90: 2020 2020 2020 2020 2020 2074 7261 636b             track
-0000eea0: 5f69 6420 3d20 7365 6c66 2e75 6e69 7175  _id = self.uniqu
-0000eeb0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000eec0: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-0000eed0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-0000eee0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef00: 2020 2020 2020 2020 2020 2063 6861 6e6e             chann
-0000ef10: 656c 5f66 696c 7465 7265 645f 7472 6163  el_filtered_trac
-0000ef20: 6b73 2e61 7070 656e 6428 7472 6163 6b5f  ks.append(track_
-0000ef30: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
-0000ef40: 2020 2020 2020 2020 2066 6f72 2070 6172           for par
-0000ef50: 656e 7420 696e 2073 656c 662e 786d 6c5f  ent in self.xml_
-0000ef60: 726f 6f74 2e66 696e 6461 6c6c 2827 4d6f  root.findall('Mo
-0000ef70: 6465 6c27 293a 0d0a 2020 2020 2020 2020  del'):..        
-0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef90: 666f 7220 6669 7273 7463 6869 6c64 2069  for firstchild i
-0000efa0: 6e20 7061 7265 6e74 2e66 696e 6461 6c6c  n parent.findall
-0000efb0: 2827 416c 6c54 7261 636b 7327 293a 0d0a  ('AllTracks'):..
-0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000efe0: 7365 636f 6e64 6368 696c 6420 696e 2066  secondchild in f
-0000eff0: 6972 7374 6368 696c 642e 6669 6e64 616c  irstchild.findal
-0000f000: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
-0000f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f020: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-0000f030: 636b 5f69 6420 3d20 696e 7428 7365 636f  ck_id = int(seco
-0000f040: 6e64 6368 696c 642e 6765 7428 7365 6c66  ndchild.get(self
-0000f050: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
-0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f080: 6966 2074 7261 636b 5f69 6420 6e6f 7420  if track_id not 
-0000f090: 696e 2063 6861 6e6e 656c 5f66 696c 7465  in channel_filte
-0000f0a0: 7265 645f 7472 6163 6b73 3a20 2020 200d  red_tracks:    .
-0000f0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0d0: 2020 2020 2066 6972 7374 6368 696c 642e       firstchild.
-0000f0e0: 7265 6d6f 7665 2873 6563 6f6e 6463 6869  remove(secondchi
-0000f0f0: 6c64 290d 0a20 2020 2020 2020 2020 2020  ld)..           
+0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed40: 2020 2069 6620 7365 6c66 2e74 7261 636b     if self.track
+0000ed50: 6964 5f6b 6579 2069 6e20 7365 6c66 2e75  id_key in self.u
+0000ed60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000ed70: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+0000ed80: 6429 5d2e 6b65 7973 2829 3a0d 0a20 2020  d)].keys():..   
+0000ed90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edb0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000ede0: 7261 636b 5f69 6420 3d20 7365 6c66 2e75  rack_id = self.u
+0000edf0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000ee00: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+0000ee10: 6429 5d5b 7365 6c66 2e74 7261 636b 6964  d)][self.trackid
+0000ee20: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
+0000ee30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000ee50: 6861 6e6e 656c 5f66 696c 7465 7265 645f  hannel_filtered_
+0000ee60: 7472 6163 6b73 2e61 7070 656e 6428 7472  tracks.append(tr
+0000ee70: 6163 6b5f 6964 290d 0a20 2020 2020 2020  ack_id)..       
+0000ee80: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000ee90: 2070 6172 656e 7420 696e 2073 656c 662e   parent in self.
+0000eea0: 786d 6c5f 726f 6f74 2e66 696e 6461 6c6c  xml_root.findall
+0000eeb0: 2827 4d6f 6465 6c27 293a 0d0a 2020 2020  ('Model'):..    
+0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eed0: 2020 2020 666f 7220 6669 7273 7463 6869      for firstchi
+0000eee0: 6c64 2069 6e20 7061 7265 6e74 2e66 696e  ld in parent.fin
+0000eef0: 6461 6c6c 2827 416c 6c54 7261 636b 7327  dall('AllTracks'
+0000ef00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef20: 666f 7220 7365 636f 6e64 6368 696c 6420  for secondchild 
+0000ef30: 696e 2066 6972 7374 6368 696c 642e 6669  in firstchild.fi
+0000ef40: 6e64 616c 6c28 2754 7261 636b 2729 3a0d  ndall('Track'):.
+0000ef50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef70: 2074 7261 636b 5f69 6420 3d20 696e 7428   track_id = int(
+0000ef80: 7365 636f 6e64 6368 696c 642e 6765 7428  secondchild.get(
+0000ef90: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+0000efa0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efc0: 2020 2020 6966 2074 7261 636b 5f69 6420      if track_id 
+0000efd0: 6e6f 7420 696e 2063 6861 6e6e 656c 5f66  not in channel_f
+0000efe0: 696c 7465 7265 645f 7472 6163 6b73 3a20  iltered_tracks: 
+0000eff0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f010: 2020 2020 2020 2020 2066 6972 7374 6368           firstch
+0000f020: 696c 642e 7265 6d6f 7665 2873 6563 6f6e  ild.remove(secon
+0000f030: 6463 6869 6c64 290d 0a20 2020 2020 2020  dchild)..       
+0000f040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f050: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000f060: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000f070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f080: 2020 2020 2066 6f72 2070 6172 656e 7420       for parent 
+0000f090: 696e 2073 656c 662e 786d 6c5f 726f 6f74  in self.xml_root
+0000f0a0: 2e66 696e 6461 6c6c 2827 4d6f 6465 6c27  .findall('Model'
+0000f0b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000f0c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000f0d0: 6669 7273 7463 6869 6c64 2069 6e20 7061  firstchild in pa
+0000f0e0: 7265 6e74 2e66 696e 6461 6c6c 2827 416c  rent.findall('Al
+0000f0f0: 6c54 7261 636b 7327 293a 0d0a 2020 2020  lTracks'):..    
 0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f110: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000f120: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000f130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f140: 2066 6f72 2070 6172 656e 7420 696e 2073   for parent in s
-0000f150: 656c 662e 786d 6c5f 726f 6f74 2e66 696e  elf.xml_root.fin
-0000f160: 6461 6c6c 2827 4d6f 6465 6c27 293a 0d0a  dall('Model'):..
-0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f180: 2020 2020 2020 2020 666f 7220 6669 7273          for firs
-0000f190: 7463 6869 6c64 2069 6e20 7061 7265 6e74  tchild in parent
-0000f1a0: 2e66 696e 6461 6c6c 2827 416c 6c54 7261  .findall('AllTra
-0000f1b0: 636b 7327 293a 0d0a 2020 2020 2020 2020  cks'):..        
-0000f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1d0: 2020 2020 666f 7220 7365 636f 6e64 6368      for secondch
-0000f1e0: 696c 6420 696e 2066 6972 7374 6368 696c  ild in firstchil
-0000f1f0: 642e 6669 6e64 616c 6c28 2754 7261 636b  d.findall('Track
-0000f200: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+0000f110: 2020 2020 2020 2020 666f 7220 7365 636f          for seco
+0000f120: 6e64 6368 696c 6420 696e 2066 6972 7374  ndchild in first
+0000f130: 6368 696c 642e 6669 6e64 616c 6c28 2754  child.findall('T
+0000f140: 7261 636b 2729 3a0d 0a20 2020 2020 2020  rack'):..       
+0000f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f160: 2020 2020 2020 2020 2066 6f72 2045 6467           for Edg
+0000f170: 656f 626a 6563 7420 696e 2073 6563 6f6e  eobject in secon
+0000f180: 6463 6869 6c64 2e66 696e 6461 6c6c 2827  dchild.findall('
+0000f190: 4564 6765 2729 3a0d 0a20 2020 2020 2020  Edge'):..       
+0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1c0: 2073 706f 745f 736f 7572 6365 5f69 6420   spot_source_id 
+0000f1d0: 3d20 696e 7428 666c 6f61 7428 4564 6765  = int(float(Edge
+0000f1e0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000f1f0: 7370 6f74 5f73 6f75 7263 655f 6964 5f6b  spot_source_id_k
+0000f200: 6579 2929 2920 200d 0a20 2020 2020 2020  ey)))  ..       
 0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 2020 2020 2066 6f72 2045 6467 656f 626a       for Edgeobj
-0000f230: 6563 7420 696e 2073 6563 6f6e 6463 6869  ect in secondchi
-0000f240: 6c64 2e66 696e 6461 6c6c 2827 4564 6765  ld.findall('Edge
-0000f250: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f270: 2020 2020 2020 2020 2020 2020 2073 706f               spo
-0000f280: 745f 736f 7572 6365 5f69 6420 3d20 696e  t_source_id = in
-0000f290: 7428 666c 6f61 7428 4564 6765 6f62 6a65  t(float(Edgeobje
-0000f2a0: 6374 2e67 6574 2873 656c 662e 7370 6f74  ct.get(self.spot
-0000f2b0: 5f73 6f75 7263 655f 6964 5f6b 6579 2929  _source_id_key))
-0000f2c0: 2920 200d 0a20 2020 2020 2020 2020 2020  )  ..           
-0000f2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2e0: 2020 2020 2020 2020 2020 2020 2073 706f               spo
-0000f2f0: 745f 7461 7267 6574 5f69 6420 3d20 696e  t_target_id = in
-0000f300: 7428 666c 6f61 7428 4564 6765 6f62 6a65  t(float(Edgeobje
-0000f310: 6374 2e67 6574 2873 656c 662e 7370 6f74  ct.get(self.spot
-0000f320: 5f74 6172 6765 745f 6964 5f6b 6579 2929  _target_id_key))
-0000f330: 2920 2020 2020 200d 0a20 2020 2020 2020  )      ..       
+0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f230: 2073 706f 745f 7461 7267 6574 5f69 6420   spot_target_id 
+0000f240: 3d20 696e 7428 666c 6f61 7428 4564 6765  = int(float(Edge
+0000f250: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000f260: 7370 6f74 5f74 6172 6765 745f 6964 5f6b  spot_target_id_k
+0000f270: 6579 2929 2920 2020 2020 200d 0a20 2020  ey)))      ..   
+0000f280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2a0: 2020 2020 2069 6620 7370 6f74 5f73 6f75       if spot_sou
+0000f2b0: 7263 655f 6964 206e 6f74 2069 6e20 7365  rce_id not in se
+0000f2c0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000f2d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000f2e0: 732e 6b65 7973 2829 2061 6e64 2073 706f  s.keys() and spo
+0000f2f0: 745f 7461 7267 6574 5f69 6420 6e6f 7420  t_target_id not 
+0000f300: 696e 2073 656c 662e 6368 616e 6e65 6c5f  in self.channel_
+0000f310: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000f320: 6572 7469 6573 2e6b 6579 7328 293a 2020  erties.keys():  
+0000f330: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f360: 2069 6620 7370 6f74 5f73 6f75 7263 655f   if spot_source_
-0000f370: 6964 206e 6f74 2069 6e20 7365 6c66 2e63  id not in self.c
-0000f380: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-0000f390: 6f74 5f70 726f 7065 7274 6965 732e 6b65  ot_properties.ke
-0000f3a0: 7973 2829 2061 6e64 2073 706f 745f 7461  ys() and spot_ta
-0000f3b0: 7267 6574 5f69 6420 6e6f 7420 696e 2073  rget_id not in s
-0000f3c0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-0000f3d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000f3e0: 6573 2e6b 6579 7328 293a 2020 2020 200d  es.keys():     .
-0000f3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f420: 2020 2020 2020 2020 2020 2020 2073 6563               sec
-0000f430: 6f6e 6463 6869 6c64 2e72 656d 6f76 6528  ondchild.remove(
-0000f440: 4564 6765 6f62 6a65 6374 2920 200d 0a0d  Edgeobject)  ...
-0000f450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f460: 2020 2020 2066 6f72 2070 6172 656e 7420       for parent 
-0000f470: 696e 2073 656c 662e 786d 6c5f 726f 6f74  in self.xml_root
-0000f480: 2e66 696e 6461 6c6c 2827 4d6f 6465 6c27  .findall('Model'
-0000f490: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000f4a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000f4b0: 6669 7273 7463 6869 6c64 2069 6e20 7061  firstchild in pa
-0000f4c0: 7265 6e74 2e66 696e 6461 6c6c 2827 4669  rent.findall('Fi
-0000f4d0: 6c74 6572 6564 5472 6163 6b73 2729 3a0d  lteredTracks'):.
-0000f4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f4f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f500: 2073 6563 6f6e 6463 6869 6c64 2069 6e20   secondchild in 
-0000f510: 6669 7273 7463 6869 6c64 2e66 696e 6461  firstchild.finda
-0000f520: 6c6c 2827 5472 6163 6b49 4427 293a 200d  ll('TrackID'): .
-0000f530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f370: 2073 6563 6f6e 6463 6869 6c64 2e72 656d   secondchild.rem
+0000f380: 6f76 6528 4564 6765 6f62 6a65 6374 2920  ove(Edgeobject) 
+0000f390: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+0000f3a0: 2020 2020 2020 2020 2066 6f72 2070 6172           for par
+0000f3b0: 656e 7420 696e 2073 656c 662e 786d 6c5f  ent in self.xml_
+0000f3c0: 726f 6f74 2e66 696e 6461 6c6c 2827 4d6f  root.findall('Mo
+0000f3d0: 6465 6c27 293a 0d0a 2020 2020 2020 2020  del'):..        
+0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3f0: 666f 7220 6669 7273 7463 6869 6c64 2069  for firstchild i
+0000f400: 6e20 7061 7265 6e74 2e66 696e 6461 6c6c  n parent.findall
+0000f410: 2827 4669 6c74 6572 6564 5472 6163 6b73  ('FilteredTracks
+0000f420: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f440: 2066 6f72 2073 6563 6f6e 6463 6869 6c64   for secondchild
+0000f450: 2069 6e20 6669 7273 7463 6869 6c64 2e66   in firstchild.f
+0000f460: 696e 6461 6c6c 2827 5472 6163 6b49 4427  indall('TrackID'
+0000f470: 293a 200d 0a20 2020 2020 2020 2020 2020  ): ..           
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f490: 2020 2020 2020 2020 2066 696c 7465 725f           filter_
+0000f4a0: 7472 6163 6b5f 6964 203d 2069 6e74 2873  track_id = int(s
+0000f4b0: 6563 6f6e 6463 6869 6c64 2e67 6574 2873  econdchild.get(s
+0000f4c0: 656c 662e 7472 6163 6b69 645f 6b65 7929  elf.trackid_key)
+0000f4d0: 2920 200d 0a20 2020 2020 2020 2020 2020  )  ..           
+0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4f0: 2020 2020 2020 2020 2069 6620 6669 6c74           if filt
+0000f500: 6572 5f74 7261 636b 5f69 6420 6e6f 7420  er_track_id not 
+0000f510: 696e 2063 6861 6e6e 656c 5f66 696c 7465  in channel_filte
+0000f520: 7265 645f 7472 6163 6b73 3a0d 0a20 2020  red_tracks:..   
+0000f530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f550: 2020 2020 2066 696c 7465 725f 7472 6163       filter_trac
-0000f560: 6b5f 6964 203d 2069 6e74 2873 6563 6f6e  k_id = int(secon
-0000f570: 6463 6869 6c64 2e67 6574 2873 656c 662e  dchild.get(self.
-0000f580: 7472 6163 6b69 645f 6b65 7929 2920 200d  trackid_key))  .
-0000f590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5b0: 2020 2020 2069 6620 6669 6c74 6572 5f74       if filter_t
-0000f5c0: 7261 636b 5f69 6420 6e6f 7420 696e 2063  rack_id not in c
-0000f5d0: 6861 6e6e 656c 5f66 696c 7465 7265 645f  hannel_filtered_
-0000f5e0: 7472 6163 6b73 3a0d 0a20 2020 2020 2020  tracks:..       
-0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f610: 2020 2020 2066 6972 7374 6368 696c 642e       firstchild.
-0000f620: 7265 6d6f 7665 2873 6563 6f6e 6463 6869  remove(secondchi
-0000f630: 6c64 2920 2020 2020 2020 2020 2020 2020  ld)             
-0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f650: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000f660: 2020 2020 2020 2020 7365 6c66 2e78 6d6c          self.xml
-0000f670: 5f74 7265 652e 7772 6974 6528 6f73 2e70  _tree.write(os.p
-0000f680: 6174 682e 6a6f 696e 2873 656c 662e 6368  ath.join(self.ch
-0000f690: 616e 6e65 6c5f 786d 6c5f 7061 7468 2c20  annel_xml_path, 
-0000f6a0: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000f6b0: 5f6e 616d 6529 2920 0d0a 0d0a 2020 2020  _name)) ....    
-0000f6c0: 6465 6620 5f67 6574 5f78 6d6c 5f64 6174  def _get_xml_dat
-0000f6d0: 6128 7365 6c66 293a 0d0a 0d0a 2020 2020  a(self):....    
-0000f6e0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+0000f550: 2020 2020 2020 2020 2066 6972 7374 6368           firstch
+0000f560: 696c 642e 7265 6d6f 7665 2873 6563 6f6e  ild.remove(secon
+0000f570: 6463 6869 6c64 2920 2020 2020 2020 2020  dchild)         
+0000f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f590: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0000f5a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f5b0: 2e78 6d6c 5f74 7265 652e 7772 6974 6528  .xml_tree.write(
+0000f5c0: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
+0000f5d0: 662e 6368 616e 6e65 6c5f 786d 6c5f 7061  f.channel_xml_pa
+0000f5e0: 7468 2c20 7365 6c66 2e63 6861 6e6e 656c  th, self.channel
+0000f5f0: 5f78 6d6c 5f6e 616d 6529 2920 0d0a 0d0a  _xml_name)) ....
+0000f600: 2020 2020 6465 6620 5f67 6574 5f78 6d6c      def _get_xml
+0000f610: 5f64 6174 6128 7365 6c66 293a 0d0a 0d0a  _data(self):....
+0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f630: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000f640: 2020 2020 6966 2073 656c 662e 6368 616e      if self.chan
+0000f650: 6e65 6c5f 7365 675f 696d 6167 6520 6973  nel_seg_image is
+0000f660: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f680: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
+0000f690: 6d6c 5f63 6f6e 7465 6e74 203d 2073 656c  ml_content = sel
+0000f6a0: 662e 786d 6c5f 636f 6e74 656e 740d 0a20  f.xml_content.. 
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 2020 2020 2073 656c 662e 786d 6c5f 7472       self.xml_tr
+0000f6d0: 6565 203d 2065 742e 7061 7273 6528 7365  ee = et.parse(se
+0000f6e0: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
 0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
-0000f710: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-0000f720: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000f730: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f740: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f63  lf.channel_xml_c
-0000f750: 6f6e 7465 6e74 203d 2073 656c 662e 786d  ontent = self.xm
-0000f760: 6c5f 636f 6e74 656e 740d 0a20 2020 2020  l_content..     
-0000f770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f780: 2073 656c 662e 786d 6c5f 7472 6565 203d   self.xml_tree =
-0000f790: 2065 742e 7061 7273 6528 7365 6c66 2e78   et.parse(self.x
-0000f7a0: 6d6c 5f70 6174 6829 0d0a 2020 2020 2020  ml_path)..      
+0000f700: 2020 2020 7365 6c66 2e78 6d6c 5f72 6f6f      self.xml_roo
+0000f710: 7420 3d20 7365 6c66 2e78 6d6c 5f74 7265  t = self.xml_tre
+0000f720: 652e 6765 7472 6f6f 7428 290d 0a20 2020  e.getroot()..   
+0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f740: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+0000f750: 786d 6c5f 6e61 6d65 203d 2027 7365 636f  xml_name = 'seco
+0000f760: 6e64 5f63 6861 6e6e 656c 5f27 202b 206f  nd_channel_' + o
+0000f770: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
+0000f780: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
+0000f790: 2873 656c 662e 786d 6c5f 7061 7468 2929  (self.xml_path))
+0000f7a0: 5b30 5d20 2b20 272e 786d 6c27 0d0a 2020  [0] + '.xml'..  
 0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7c0: 7365 6c66 2e78 6d6c 5f72 6f6f 7420 3d20  self.xml_root = 
-0000f7d0: 7365 6c66 2e78 6d6c 5f74 7265 652e 6765  self.xml_tree.ge
-0000f7e0: 7472 6f6f 7428 290d 0a20 2020 2020 2020  troot()..       
-0000f7f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f800: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000f810: 6e61 6d65 203d 2027 7365 636f 6e64 5f63  name = 'second_c
-0000f820: 6861 6e6e 656c 5f27 202b 206f 732e 7061  hannel_' + os.pa
-0000f830: 7468 2e73 706c 6974 6578 7428 6f73 2e70  th.splitext(os.p
-0000f840: 6174 682e 6261 7365 6e61 6d65 2873 656c  ath.basename(sel
-0000f850: 662e 786d 6c5f 7061 7468 2929 5b30 5d20  f.xml_path))[0] 
-0000f860: 2b20 272e 786d 6c27 0d0a 2020 2020 2020  + '.xml'..      
-0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f880: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000f890: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0000f8a0: 6469 726e 616d 6528 7365 6c66 2e78 6d6c  dirname(self.xml
-0000f8b0: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
-0000f8c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f8d0: 6c66 2e5f 6372 6561 7465 5f63 6861 6e6e  lf._create_chann
-0000f8e0: 656c 5f74 7265 6528 290d 0a20 2020 2020  el_tree()..     
-0000f8f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000f900: 6c66 2e63 6c75 7374 6572 5f6d 6f64 656c  lf.cluster_model
-0000f910: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000f920: 2073 656c 662e 7365 675f 696d 6167 6520   self.seg_image 
-0000f930: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f950: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
-0000f960: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
-0000f970: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
-0000f980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f990: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-0000f9a0: 7465 725f 786d 6c5f 7472 6565 203d 2065  ter_xml_tree = e
-0000f9b0: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
-0000f9c0: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
-0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f9e0: 656c 662e 6d61 7374 6572 5f78 6d6c 5f72  elf.master_xml_r
-0000f9f0: 6f6f 7420 3d20 7365 6c66 2e6d 6173 7465  oot = self.maste
-0000fa00: 725f 786d 6c5f 7472 6565 2e67 6574 726f  r_xml_tree.getro
-0000fa10: 6f74 2829 0d0a 2020 2020 2020 2020 2020  ot()..          
-0000fa20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fa30: 662e 6d61 7374 6572 5f78 6d6c 5f6e 616d  f.master_xml_nam
-0000fa40: 6520 3d20 276d 6173 7465 725f 2720 2b20  e = 'master_' + 
-0000fa50: 7365 6c66 2e6d 6173 7465 725f 6578 7472  self.master_extr
-0000fa60: 615f 6e61 6d65 2020 2b20 6f73 2e70 6174  a_name  + os.pat
-0000fa70: 682e 7370 6c69 7465 7874 286f 732e 7061  h.splitext(os.pa
-0000fa80: 7468 2e62 6173 656e 616d 6528 7365 6c66  th.basename(self
-0000fa90: 2e78 6d6c 5f70 6174 6829 295b 305d 202b  .xml_path))[0] +
-0000faa0: 2027 2e78 6d6c 270d 0a20 2020 2020 2020   '.xml'..       
-0000fab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fac0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-0000fad0: 7061 7468 203d 206f 732e 7061 7468 2e64  path = os.path.d
-0000fae0: 6972 6e61 6d65 2873 656c 662e 786d 6c5f  irname(self.xml_
-0000faf0: 7061 7468 2920 2020 2020 200d 0a20 2020  path)      ..   
-0000fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000fb20: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-0000fb30: 655f 6f62 6a65 6374 7320 3d20 7b7d 0d0a  e_objects = {}..
-0000fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb50: 7365 6c66 2e75 6e69 7175 655f 7072 6f70  self.unique_prop
-0000fb60: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
-0000fb70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fb80: 662e 416c 6c54 7261 636b 4964 7320 3d20  f.AllTrackIds = 
-0000fb90: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000fba0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
-0000fbb0: 6754 7261 636b 4964 7320 3d20 5b5d 0d0a  gTrackIds = []..
-0000fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbd0: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-0000fbe0: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
-0000fbf0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000fc00: 6c6c 5f74 7261 636b 5f70 726f 7065 7274  ll_track_propert
-0000fc10: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
-0000fc20: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000fc30: 706c 6974 5f70 6f69 6e74 735f 7469 6d65  plit_points_time
-0000fc40: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-0000fc50: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000fc60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fc80: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
-0000fc90: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000fca0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fcb0: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
-0000fcc0: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
-0000fcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fce0: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
-0000fcf0: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
-0000fd00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fd10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000fd20: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
-0000fd30: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
-0000fd40: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
-0000fd50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fd60: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
-0000fd70: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
-0000fd80: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fda0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000fdb0: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
-0000fdc0: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
-0000fdd0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000fde0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000fdf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fe00: 656c 662e 5370 6f74 6f62 6a65 6374 7320  elf.Spotobjects 
-0000fe10: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000fe20: 6e74 2e66 696e 6428 274d 6f64 656c 2729  nt.find('Model')
-0000fe30: 2e66 696e 6428 2741 6c6c 5370 6f74 7327  .find('AllSpots'
-0000fe40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fe50: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
-0000fe60: 2074 7261 636b 7320 6672 6f6d 2078 6d6c   tracks from xml
-0000fe70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fe80: 2020 7365 6c66 2e74 7261 636b 7320 3d20    self.tracks = 
-0000fe90: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-0000fea0: 2e66 696e 6428 224d 6f64 656c 2229 2e66  .find("Model").f
-0000feb0: 696e 6428 2241 6c6c 5472 6163 6b73 2229  ind("AllTracks")
-0000fec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fed0: 2020 7365 6c66 2e73 6574 7469 6e67 7320    self.settings 
-0000fee0: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000fef0: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
-0000ff00: 7322 292e 6669 6e64 2822 496d 6167 6544  s").find("ImageD
-0000ff10: 6174 6122 290d 0a20 2020 2020 2020 2020  ata")..         
-0000ff20: 2020 2020 2020 2073 656c 662e 7863 616c         self.xcal
-0000ff30: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
-0000ff40: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
-0000ff50: 6574 2822 7069 7865 6c77 6964 7468 2229  et("pixelwidth")
-0000ff60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ff70: 2020 2073 656c 662e 7963 616c 6962 7261     self.ycalibra
-0000ff80: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
-0000ff90: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000ffa0: 7069 7865 6c68 6569 6768 7422 2929 0d0a  pixelheight"))..
-0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffc0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-0000ffd0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
-0000ffe0: 6574 7469 6e67 732e 6765 7428 2276 6f78  ettings.get("vox
-0000fff0: 656c 6465 7074 6822 2929 0d0a 2020 2020  eldepth"))..    
-00010000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010010: 2e74 6361 6c69 6272 6174 696f 6e20 3d20  .tcalibration = 
-00010020: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
-00010030: 6574 7469 6e67 732e 6765 7428 2274 696d  ettings.get("tim
-00010040: 6569 6e74 6572 7661 6c22 2929 290d 0a20  einterval"))).. 
-00010050: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010060: 656c 662e 6465 7465 6374 6f72 7365 7474  elf.detectorsett
-00010070: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
-00010080: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
-00010090: 7474 696e 6773 2229 2e66 696e 6428 2244  ttings").find("D
-000100a0: 6574 6563 746f 7253 6574 7469 6e67 7322  etectorSettings"
-000100b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000100c0: 2020 2073 656c 662e 6261 7369 6373 6574     self.basicset
-000100d0: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
-000100e0: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
-000100f0: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
-00010100: 4261 7369 6353 6574 7469 6e67 7322 290d  BasicSettings").
-00010110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010120: 2073 656c 662e 6465 7465 6374 6f72 6368   self.detectorch
-00010130: 616e 6e65 6c20 3d20 696e 7428 666c 6f61  annel = int(floa
-00010140: 7428 7365 6c66 2e64 6574 6563 746f 7273  t(self.detectors
-00010150: 6574 7469 6e67 732e 6765 7428 2254 4152  ettings.get("TAR
-00010160: 4745 545f 4348 414e 4e45 4c22 2929 290d  GET_CHANNEL"))).
-00010170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010180: 2073 656c 662e 7473 7461 7274 203d 2069   self.tstart = i
-00010190: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
-000101a0: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
-000101b0: 2274 7374 6172 7422 2929 290d 0a20 2020  "tstart")))..   
-000101c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000101d0: 662e 7465 6e64 203d 2069 6e74 2866 6c6f  f.tend = int(flo
-000101e0: 6174 2873 656c 662e 6261 7369 6373 6574  at(self.basicset
-000101f0: 7469 6e67 732e 6765 7428 2274 656e 6422  tings.get("tend"
-00010200: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-00010210: 2020 2020 2073 656c 662e 5f67 6574 5f62       self._get_b
-00010220: 6f75 6e64 6172 795f 706f 696e 7473 2829  oundary_points()
-00010230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010240: 2020 7072 696e 7428 2749 7465 7261 7469    print('Iterati
-00010250: 6e67 206f 7665 7220 7370 6f74 7320 696e  ng over spots in
-00010260: 2066 7261 6d65 2729 0d0a 2020 2020 2020   frame')..      
-00010270: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00010280: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
-00010290: 2020 2020 2020 2020 2020 6675 7475 7265            future
-000102a0: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-000102b0: 2020 2020 2020 2020 2020 7769 7468 2063            with c
-000102c0: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-000102d0: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
-000102e0: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
-000102f0: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
-00010300: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
+0000f7c0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+0000f7d0: 5f78 6d6c 5f70 6174 6820 3d20 6f73 2e70  _xml_path = os.p
+0000f7e0: 6174 682e 6469 726e 616d 6528 7365 6c66  ath.dirname(self
+0000f7f0: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
+0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f810: 2020 7365 6c66 2e5f 6372 6561 7465 5f63    self._create_c
+0000f820: 6861 6e6e 656c 5f74 7265 6528 290d 0a20  hannel_tree().. 
+0000f830: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f840: 6620 7365 6c66 2e63 6c75 7374 6572 5f6d  f self.cluster_m
+0000f850: 6f64 656c 2069 7320 6e6f 7420 4e6f 6e65  odel is not None
+0000f860: 2061 6e64 2073 656c 662e 7365 675f 696d   and self.seg_im
+0000f870: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
+0000f880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f890: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000f8a0: 7374 6572 5f78 6d6c 5f63 6f6e 7465 6e74  ster_xml_content
+0000f8b0: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
+0000f8c0: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
+0000f8d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f8e0: 2e6d 6173 7465 725f 786d 6c5f 7472 6565  .master_xml_tree
+0000f8f0: 203d 2065 742e 7061 7273 6528 7365 6c66   = et.parse(self
+0000f900: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
+0000f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f920: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
+0000f930: 6d6c 5f72 6f6f 7420 3d20 7365 6c66 2e6d  ml_root = self.m
+0000f940: 6173 7465 725f 786d 6c5f 7472 6565 2e67  aster_xml_tree.g
+0000f950: 6574 726f 6f74 2829 0d0a 2020 2020 2020  etroot()..      
+0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f970: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
+0000f980: 5f6e 616d 6520 3d20 276d 6173 7465 725f  _name = 'master_
+0000f990: 2720 2b20 7365 6c66 2e6d 6173 7465 725f  ' + self.master_
+0000f9a0: 6578 7472 615f 6e61 6d65 2020 2b20 6f73  extra_name  + os
+0000f9b0: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
+0000f9c0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+0000f9d0: 7365 6c66 2e78 6d6c 5f70 6174 6829 295b  self.xml_path))[
+0000f9e0: 305d 202b 2027 2e78 6d6c 270d 0a20 2020  0] + '.xml'..   
+0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa00: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
+0000fa10: 786d 6c5f 7061 7468 203d 206f 732e 7061  xml_path = os.pa
+0000fa20: 7468 2e64 6972 6e61 6d65 2873 656c 662e  th.dirname(self.
+0000fa30: 786d 6c5f 7061 7468 2920 2020 2020 200d  xml_path)      .
+0000fa40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fa50: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000fa60: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000fa70: 6e69 7175 655f 6f62 6a65 6374 7320 3d20  nique_objects = 
+0000fa80: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+0000fa90: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000faa0: 7072 6f70 6572 7469 6573 203d 207b 7d0d  properties = {}.
+0000fab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fac0: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
+0000fad0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000fae0: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
+0000faf0: 6964 696e 6754 7261 636b 4964 7320 3d20  idingTrackIds = 
+0000fb00: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+0000fb10: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
+0000fb20: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
+0000fb30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fb40: 6c66 2e61 6c6c 5f74 7261 636b 5f70 726f  lf.all_track_pro
+0000fb50: 7065 7274 6965 7320 3d20 5b5d 0d0a 2020  perties = []..  
+0000fb60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fb70: 6c66 2e73 706c 6974 5f70 6f69 6e74 735f  lf.split_points_
+0000fb80: 7469 6d65 7320 3d20 5b5d 0d0a 0d0a 2020  times = []....  
+0000fb90: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fbc0: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+0000fbd0: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
+0000fbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fbf0: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
+0000fc00: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
+0000fc10: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
+0000fc20: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
+0000fc30: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+0000fc40: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
+0000fc50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000fc60: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
+0000fc70: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000fc80: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
+0000fc90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fca0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
+0000fcb0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+0000fcc0: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
+0000fcd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fce0: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
+0000fcf0: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
+0000fd00: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
+0000fd10: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000fd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fd30: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000fd40: 2020 2073 656c 662e 5370 6f74 6f62 6a65     self.Spotobje
+0000fd50: 6374 7320 3d20 7365 6c66 2e78 6d6c 5f63  cts = self.xml_c
+0000fd60: 6f6e 7465 6e74 2e66 696e 6428 274d 6f64  ontent.find('Mod
+0000fd70: 656c 2729 2e66 696e 6428 2741 6c6c 5370  el').find('AllSp
+0000fd80: 6f74 7327 290d 0a20 2020 2020 2020 2020  ots')..         
+0000fd90: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
+0000fda0: 2074 6865 2074 7261 636b 7320 6672 6f6d   the tracks from
+0000fdb0: 2078 6d6c 0d0a 2020 2020 2020 2020 2020   xml..          
+0000fdc0: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+0000fdd0: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
+0000fde0: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
+0000fdf0: 2229 2e66 696e 6428 2241 6c6c 5472 6163  ").find("AllTrac
+0000fe00: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
+0000fe10: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000fe20: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
+0000fe30: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
+0000fe40: 7469 6e67 7322 292e 6669 6e64 2822 496d  tings").find("Im
+0000fe50: 6167 6544 6174 6122 290d 0a20 2020 2020  ageData")..     
+0000fe60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fe70: 7863 616c 6962 7261 7469 6f6e 203d 2066  xcalibration = f
+0000fe80: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+0000fe90: 6773 2e67 6574 2822 7069 7865 6c77 6964  gs.get("pixelwid
+0000fea0: 7468 2229 290d 0a20 2020 2020 2020 2020  th"))..         
+0000feb0: 2020 2020 2020 2073 656c 662e 7963 616c         self.ycal
+0000fec0: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
+0000fed0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000fee0: 6574 2822 7069 7865 6c68 6569 6768 7422  et("pixelheight"
+0000fef0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000ff00: 2020 2020 7365 6c66 2e7a 6361 6c69 6272      self.zcalibr
+0000ff10: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
+0000ff20: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
+0000ff30: 2276 6f78 656c 6465 7074 6822 2929 0d0a  "voxeldepth"))..
+0000ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff50: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+0000ff60: 6e20 3d20 696e 7428 666c 6f61 7428 7365  n = int(float(se
+0000ff70: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
+0000ff80: 2274 696d 6569 6e74 6572 7661 6c22 2929  "timeinterval"))
+0000ff90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ffa0: 2020 2073 656c 662e 6465 7465 6374 6f72     self.detector
+0000ffb0: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
+0000ffc0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000ffd0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
+0000ffe0: 6428 2244 6574 6563 746f 7253 6574 7469  d("DetectorSetti
+0000fff0: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
+00010000: 2020 2020 2020 2073 656c 662e 6261 7369         self.basi
+00010010: 6373 6574 7469 6e67 7320 3d20 7365 6c66  csettings = self
+00010020: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
+00010030: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
+00010040: 6e64 2822 4261 7369 6353 6574 7469 6e67  nd("BasicSetting
+00010050: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
+00010060: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
+00010070: 6f72 6368 616e 6e65 6c20 3d20 696e 7428  orchannel = int(
+00010080: 666c 6f61 7428 7365 6c66 2e64 6574 6563  float(self.detec
+00010090: 746f 7273 6574 7469 6e67 732e 6765 7428  torsettings.get(
+000100a0: 2254 4152 4745 545f 4348 414e 4e45 4c22  "TARGET_CHANNEL"
+000100b0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+000100c0: 2020 2020 2073 656c 662e 7473 7461 7274       self.tstart
+000100d0: 203d 2069 6e74 2866 6c6f 6174 2873 656c   = int(float(sel
+000100e0: 662e 6261 7369 6373 6574 7469 6e67 732e  f.basicsettings.
+000100f0: 6765 7428 2274 7374 6172 7422 2929 290d  get("tstart"))).
+00010100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010110: 2073 656c 662e 7465 6e64 203d 2069 6e74   self.tend = int
+00010120: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
+00010130: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
+00010140: 656e 6422 2929 290d 0a20 2020 2020 2020  end")))..       
+00010150: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
+00010160: 6574 5f62 6f75 6e64 6172 795f 706f 696e  et_boundary_poin
+00010170: 7473 2829 0d0a 2020 2020 2020 2020 2020  ts()..          
+00010180: 2020 2020 2020 7072 696e 7428 2749 7465        print('Ite
+00010190: 7261 7469 6e67 206f 7665 7220 7370 6f74  rating over spot
+000101a0: 7320 696e 2066 7261 6d65 2729 0d0a 2020  s in frame')..  
+000101b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000101c0: 6c66 2e63 6f75 6e74 203d 2030 0d0a 2020  lf.count = 0..  
+000101d0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+000101e0: 7475 7265 7320 3d20 5b5d 0d0a 0d0a 2020  tures = []....  
+000101f0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00010200: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
+00010210: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
+00010220: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
+00010230: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
+00010240: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
+00010250: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+00010260: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00010270: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010280: 6f72 2066 7261 6d65 2069 6e20 7365 6c66  or frame in self
+00010290: 2e53 706f 746f 626a 6563 7473 2e66 696e  .Spotobjects.fin
+000102a0: 6461 6c6c 2827 5370 6f74 7349 6e46 7261  dall('SpotsInFra
+000102b0: 6d65 2729 3a0d 0a20 2020 2020 2020 2020  me'):..         
+000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102d0: 2020 2020 6675 7475 7265 732e 6170 7065      futures.appe
+000102e0: 6e64 2865 7865 6375 746f 722e 7375 626d  nd(executor.subm
+000102f0: 6974 2873 656c 662e 5f73 706f 745f 636f  it(self._spot_co
+00010300: 6d70 7574 6572 2c20 6672 616d 6529 290d  mputer, frame)).
 00010310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010320: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00010330: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
-00010340: 7261 6d65 2069 6e20 7365 6c66 2e53 706f  rame in self.Spo
-00010350: 746f 626a 6563 7473 2e66 696e 6461 6c6c  tobjects.findall
-00010360: 2827 5370 6f74 7349 6e46 7261 6d65 2729  ('SpotsInFrame')
-00010370: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
-000103a0: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
-000103b0: 656c 662e 5f73 706f 745f 636f 6d70 7574  elf._spot_comput
-000103c0: 6572 2c20 6672 616d 6529 290d 0a20 2020  er, frame))..   
+00010320: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
+00010330: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+00010340: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010380: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010390: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+000103a0: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
+000103b0: 7469 6e67 2053 706f 7473 220d 0a20 2020  ting Spots"..   
+000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-000103f0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-00010400: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000103e0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+000103f0: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
+00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010420: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00010420: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
 00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010440: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010450: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
-00010460: 656c 203d 2022 436f 6c6c 6563 7469 6e67  el = "Collecting
-00010470: 2053 706f 7473 220d 0a20 2020 2020 2020   Spots"..       
-00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010490: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000104a0: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-000104b0: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104e0: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010500: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00010510: 6e28 6675 7475 7265 7329 2c0d 0a20 2020  n(futures),..   
+00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010450: 2020 6c65 6e28 6675 7475 7265 7329 2c0d    len(futures),.
+00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010480: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000104b0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
+000104c0: 6f77 2829 0d0a 0d0a 2020 2020 2020 2020  ow()....        
+000104d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000104e0: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
+000104f0: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
+00010500: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
+00010510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010540: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00010570: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
-00010580: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00010590: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
-000105a0: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-000105b0: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
-000105c0: 2866 7574 7572 6573 293a 0d0a 2020 2020  (futures):..    
-000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105f0: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
-00010600: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
-00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010630: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-00010640: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-00010650: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010680: 726f 6772 6573 735f 6261 722e 7661 6c75  rogress_bar.valu
-00010690: 6520 3d20 2073 656c 662e 636f 756e 740d  e =  self.count.
-000106a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 2020 2020 2072 2e72 6573 756c 7428 290d       r.result().
-000106d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000106e0: 2020 2070 7269 6e74 2866 2749 7465 7261     print(f'Itera
-000106f0: 7469 6e67 206f 7665 7220 7472 6163 6b73  ting over tracks
-00010700: 207b 6c65 6e28 7365 6c66 2e66 696c 7465   {len(self.filte
-00010710: 7265 645f 7472 6163 6b5f 6964 7329 7d27  red_track_ids)}'
-00010720: 2920 200d 0a20 2020 2020 2020 2020 2020  )  ..           
-00010730: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-00010740: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
-00010750: 2020 2020 2066 7574 7572 6573 203d 205b       futures = [
-00010760: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00010770: 2020 2077 6974 6820 636f 6e63 7572 7265     with concurre
-00010780: 6e74 2e66 7574 7572 6573 2e54 6872 6561  nt.futures.Threa
-00010790: 6450 6f6f 6c45 7865 6375 746f 7228 6d61  dPoolExecutor(ma
-000107a0: 785f 776f 726b 6572 7320 3d20 6f73 2e63  x_workers = os.c
-000107b0: 7075 5f63 6f75 6e74 2829 2920 6173 2065  pu_count()) as e
-000107c0: 7865 6375 746f 723a 0d0a 2020 2020 2020  xecutor:..      
-000107d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107f0: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
-00010800: 2073 656c 662e 7472 6163 6b73 2e66 696e   self.tracks.fin
-00010810: 6461 6c6c 2827 5472 6163 6b27 293a 0d0a  dall('Track'):..
+00010530: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+00010540: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
+00010550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010570: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
+00010580: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+00010590: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000105c0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+000105d0: 7661 6c75 6520 3d20 2073 656c 662e 636f  value =  self.co
+000105e0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010600: 2020 2020 2020 2020 2072 2e72 6573 756c           r.resul
+00010610: 7428 290d 0a0d 0a20 2020 2020 2020 2020  t()....         
+00010620: 2020 2020 2020 2070 7269 6e74 2866 2749         print(f'I
+00010630: 7465 7261 7469 6e67 206f 7665 7220 7472  terating over tr
+00010640: 6163 6b73 207b 6c65 6e28 7365 6c66 2e66  acks {len(self.f
+00010650: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+00010660: 7329 7d27 2920 200d 0a20 2020 2020 2020  s)}')  ..       
+00010670: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00010680: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
+00010690: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+000106a0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000106b0: 2020 2020 2020 2077 6974 6820 636f 6e63         with conc
+000106c0: 7572 7265 6e74 2e66 7574 7572 6573 2e54  urrent.futures.T
+000106d0: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+000106e0: 7228 6d61 785f 776f 726b 6572 7320 3d20  r(max_workers = 
+000106f0: 6f73 2e63 7075 5f63 6f75 6e74 2829 2920  os.cpu_count()) 
+00010700: 6173 2065 7865 6375 746f 723a 0d0a 2020  as executor:..  
+00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010720: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00010730: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
+00010740: 6b20 696e 2073 656c 662e 7472 6163 6b73  k in self.tracks
+00010750: 2e66 696e 6461 6c6c 2827 5472 6163 6b27  .findall('Track'
+00010760: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00010770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010790: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000107a0: 6163 6b5f 6964 203d 2069 6e74 2874 7261  ack_id = int(tra
+000107b0: 636b 2e67 6574 2873 656c 662e 7472 6163  ck.get(self.trac
+000107c0: 6b69 645f 6b65 7929 290d 0a20 2020 2020  kid_key))..     
+000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107e0: 2020 2020 2020 2069 6620 7472 6163 6b5f         if track_
+000107f0: 6964 2069 6e20 7365 6c66 2e66 696c 7465  id in self.filte
+00010800: 7265 645f 7472 6163 6b5f 6964 733a 0d0a  red_track_ids:..
+00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010830: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010850: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
-00010860: 6964 203d 2069 6e74 2874 7261 636b 2e67  id = int(track.g
-00010870: 6574 2873 656c 662e 7472 6163 6b69 645f  et(self.trackid_
-00010880: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108a0: 2020 2069 6620 7472 6163 6b5f 6964 2069     if track_id i
-000108b0: 6e20 7365 6c66 2e66 696c 7465 7265 645f  n self.filtered_
-000108c0: 7472 6163 6b5f 6964 733a 0d0a 2020 2020  track_ids:..    
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-000108f0: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
-00010900: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
-00010910: 662e 5f74 7261 636b 5f63 6f6d 7075 7465  f._track_compute
-00010920: 722c 2074 7261 636b 2c20 7472 6163 6b5f  r, track, track_
-00010930: 6964 2929 0d0a 2020 2020 2020 2020 2020  id))..          
-00010940: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00010950: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
-00010960: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00010830: 2020 6675 7475 7265 732e 6170 7065 6e64    futures.append
+00010840: 2865 7865 6375 746f 722e 7375 626d 6974  (executor.submit
+00010850: 2873 656c 662e 5f74 7261 636b 5f63 6f6d  (self._track_com
+00010860: 7075 7465 722c 2074 7261 636b 2c20 7472  puter, track, tr
+00010870: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
+00010880: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010890: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+000108a0: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+000108b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108f0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00010900: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
+00010910: 3d20 2243 6f6c 6c65 6374 696e 6720 5472  = "Collecting Tr
+00010920: 6163 6b73 220d 0a20 2020 2020 2020 2020  acks"..         
+00010930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010950: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
+00010960: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
 00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010980: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
 000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109b0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-000109c0: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
-000109d0: 6f6c 6c65 6374 696e 6720 5472 6163 6b73  ollecting Tracks
-000109e0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a00: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00010a10: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
-00010a20: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a40: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
-00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a70: 2020 2020 2020 2020 6c65 6e28 7365 6c66          len(self
-00010a80: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
-00010a90: 6964 7329 2c0d 0a20 2020 2020 2020 2020  ids),..         
+000109b0: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+000109c0: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+000109d0: 6163 6b5f 6964 7329 2c0d 0a20 2020 2020  ack_ids),..     
+000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+00010a30: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
+00010a40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00010a50: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
+00010a60: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+00010a70: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
+00010a80: 2866 7574 7572 6573 293a 0d0a 2020 2020  (futures):..    
+00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ab0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00010ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ab0: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
+00010ac0: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
 00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ae0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00010af0: 6261 722e 7368 6f77 2829 0d0a 0d0a 0d0a  bar.show()......
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b10: 2020 2020 666f 7220 7220 696e 2063 6f6e      for r in con
-00010b20: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-00010b30: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-00010b40: 7572 6573 293a 0d0a 2020 2020 2020 2020  ures):..        
-00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010b70: 2e63 6f75 6e74 203d 2073 656c 662e 636f  .count = self.co
-00010b80: 756e 7420 2b20 310d 0a20 2020 2020 2020  unt + 1..       
-00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ba0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010bb0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010bc0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010af0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+00010b00: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+00010b10: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010b40: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
+00010b50: 7565 203d 2073 656c 662e 636f 756e 740d  ue = self.count.
+00010b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b80: 2020 2020 2072 2e72 6573 756c 7428 290d       r.result().
+00010b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ba0: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
+00010bb0: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
+00010bc0: 7420 4e6f 6e65 3a20 200d 0a20 2020 2020  t None:  ..     
 00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bf0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00010c00: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-00010c10: 2073 656c 662e 636f 756e 740d 0a20 2020   self.count..   
-00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c40: 2072 2e72 6573 756c 7428 290d 0a20 2020   r.result()..   
-00010c50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010c60: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
-00010c70: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
-00010c80: 6e65 3a20 200d 0a20 2020 2020 2020 2020  ne:  ..         
-00010c90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010ca0: 6c66 2e5f 6372 6561 7465 5f73 6563 6f6e  lf._create_secon
-00010cb0: 645f 6368 616e 6e65 6c5f 786d 6c28 290d  d_channel_xml().
-00010cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010cd0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00010ce0: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-00010cf0: 6e20 7365 6c66 2e67 7261 7068 5f73 706c  n self.graph_spl
-00010d00: 6974 2e69 7465 6d73 2829 3a0d 0a20 2020  it.items():..   
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d40: 2020 2020 2020 6461 7567 6874 6572 5f74        daughter_t
-00010d50: 7261 636b 5f69 6420 3d20 2069 6e74 2866  rack_id =  int(f
-00010d60: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
-00010d70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00010d80: 7469 6573 5b69 6e74 2866 6c6f 6174 286b  ties[int(float(k
-00010d90: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
-00010da0: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
-00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dc0: 2020 2020 2020 2070 6172 656e 745f 7472         parent_tr
-00010dd0: 6163 6b5f 6964 203d 2069 6e74 2866 6c6f  ack_id = int(flo
-00010de0: 6174 2873 7472 2873 656c 662e 756e 6971  at(str(self.uniq
-00010df0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00010e00: 6573 5b69 6e74 2866 6c6f 6174 2876 2929  es[int(float(v))
-00010e10: 5d5b 7365 6c66 2e75 6e69 7175 6569 645f  ][self.uniqueid_
-00010e20: 6b65 795d 2929 290d 0a20 2020 2020 2020  key])))..       
+00010be0: 2020 7365 6c66 2e5f 6372 6561 7465 5f73    self._create_s
+00010bf0: 6563 6f6e 645f 6368 616e 6e65 6c5f 786d  econd_channel_xm
+00010c00: 6c28 290d 0a20 2020 2020 2020 2020 2020  l()..           
+00010c10: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00010c20: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
+00010c30: 7629 2069 6e20 7365 6c66 2e67 7261 7068  v) in self.graph
+00010c40: 5f73 706c 6974 2e69 7465 6d73 2829 3a0d  _split.items():.
+00010c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c80: 2020 2020 2020 2020 2020 6461 7567 6874            daught
+00010c90: 6572 5f74 7261 636b 5f69 6420 3d20 2069  er_track_id =  i
+00010ca0: 6e74 2866 6c6f 6174 2873 7472 2873 656c  nt(float(str(sel
+00010cb0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00010cc0: 6f70 6572 7469 6573 5b69 6e74 2866 6c6f  operties[int(flo
+00010cd0: 6174 286b 2929 5d5b 7365 6c66 2e75 6e69  at(k))][self.uni
+00010ce0: 7175 6569 645f 6b65 795d 2929 290d 0a20  queid_key]))).. 
+00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d00: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+00010d10: 745f 7472 6163 6b5f 6964 203d 2069 6e74  t_track_id = int
+00010d20: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
+00010d30: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00010d40: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
+00010d50: 2876 2929 5d5b 7365 6c66 2e75 6e69 7175  (v))][self.uniqu
+00010d60: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
+00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d80: 2020 2020 2020 2020 2073 656c 662e 6772           self.gr
+00010d90: 6170 685f 7472 6163 6b73 5b64 6175 6768  aph_tracks[daugh
+00010da0: 7465 725f 7472 6163 6b5f 6964 5d20 3d20  ter_track_id] = 
+00010db0: 7061 7265 6e74 5f74 7261 636b 5f69 640d  parent_track_id.
+00010dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010dd0: 2073 656c 662e 5f67 6574 5f61 7474 7269   self._get_attri
+00010de0: 6275 7465 7328 290d 0a20 2020 2020 2020  butes()..       
+00010df0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00010e00: 2e63 6c75 7374 6572 5f6d 6f64 656c 2061  .cluster_model a
+00010e10: 6e64 2073 656c 662e 7365 675f 696d 6167  nd self.seg_imag
+00010e20: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
 00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e40: 2020 2020 2073 656c 662e 6772 6170 685f       self.graph_
-00010e50: 7472 6163 6b73 5b64 6175 6768 7465 725f  tracks[daughter_
-00010e60: 7472 6163 6b5f 6964 5d20 3d20 7061 7265  track_id] = pare
-00010e70: 6e74 5f74 7261 636b 5f69 640d 0a20 2020  nt_track_id..   
-00010e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010e90: 662e 5f67 6574 5f61 7474 7269 6275 7465  f._get_attribute
-00010ea0: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
-00010eb0: 2020 2020 2069 6620 7365 6c66 2e63 6c75       if self.clu
-00010ec0: 7374 6572 5f6d 6f64 656c 2061 6e64 2073  ster_model and s
-00010ed0: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
-00010ee0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f00: 2020 2073 656c 662e 5f61 7373 6967 6e5f     self._assign_
-00010f10: 636c 7573 7465 725f 636c 6173 7328 290d  cluster_class().
-00010f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010f30: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
-00010f40: 6561 7465 5f6d 6173 7465 725f 786d 6c28  eate_master_xml(
-00010f50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010f60: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-00010f70: 3020 0d0a 2020 2020 2020 2020 2020 2020  0 ..            
-00010f80: 2020 2020 666f 7220 7472 6163 6b5f 6964      for track_id
-00010f90: 2069 6e20 7365 6c66 2e66 696c 7465 7265   in self.filtere
-00010fa0: 645f 7472 6163 6b5f 6964 733a 0d0a 2020  d_track_ids:..  
-00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fd0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-00010fe0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-00010ff0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00011000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011010: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011020: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
-00011030: 6162 656c 203d 2022 4a75 7374 206f 6e65  abel = "Just one
-00011040: 206d 6f72 6520 7468 696e 6722 0d0a 2020   more thing"..  
-00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 2020 2020 2020 2073 656c 662e 5f61 7373         self._ass
+00010e50: 6967 6e5f 636c 7573 7465 725f 636c 6173  ign_cluster_clas
+00010e60: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
+00010e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010e80: 2e5f 6372 6561 7465 5f6d 6173 7465 725f  ._create_master_
+00010e90: 786d 6c28 290d 0a20 2020 2020 2020 2020  xml()..         
+00010ea0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+00010eb0: 7420 3d20 3020 0d0a 2020 2020 2020 2020  t = 0 ..        
+00010ec0: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
+00010ed0: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
+00010ee0: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
+00010ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f10: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+00010f20: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+00010f30: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f60: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00010f70: 6172 2e6c 6162 656c 203d 2022 4a75 7374  ar.label = "Just
+00010f80: 206f 6e65 206d 6f72 6520 7468 696e 6722   one more thing"
+00010f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fb0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00010fc0: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+00010fd0: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011000: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011030: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
+00011040: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+00011050: 636b 5f69 6473 292c 0d0a 2020 2020 2020  ck_ids),..      
 00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011070: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-00011080: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
-00011090: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011080: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110c0: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+000110b0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+000110c0: 6172 2e73 686f 7728 290d 0a20 2020 2020  ar.show()..     
 000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
-00011100: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-00011110: 6473 292c 0d0a 2020 2020 2020 2020 2020  ds),..          
+000110f0: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+00011100: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011140: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011170: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
-00011180: 686f 7728 290d 0a20 2020 2020 2020 2020  how()..         
-00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000111b0: 656c 662e 636f 756e 7420 3d20 7365 6c66  elf.count = self
-000111c0: 2e63 6f75 6e74 202b 2031 0d0a 2020 2020  .count + 1..    
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111f0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-00011200: 735f 6261 722e 7661 6c75 6520 3d20 7365  s_bar.value = se
-00011210: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
-00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011240: 6c66 2e5f 6669 6e61 6c5f 7472 6163 6b73  lf._final_tracks
-00011250: 2874 7261 636b 5f69 6429 200d 0a0d 0a20  (track_id) .... 
-00011260: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011270: 6620 7365 6c66 2e66 6f75 7269 6572 3a0d  f self.fourier:.
-00011280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011290: 2020 2020 7072 696e 7428 2763 6f6d 7075      print('compu
-000112a0: 7469 6e67 2046 6f75 7269 6572 2729 0d0a  ting Fourier')..
-000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112c0: 2020 2073 656c 662e 5f63 6f6d 7075 7465     self._compute
-000112d0: 5f70 6865 6e6f 7479 7065 7328 2920 2020  _phenotypes()   
-000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00011300: 2020 2020 2020 2073 656c 662e 5f74 656d         self._tem
-00011310: 706f 7261 6c5f 706c 6f74 735f 7472 6163  poral_plots_trac
-00011320: 6b6d 6174 6528 290d 0a20 2020 2020 2020  kmate()..       
-00011330: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00011340: 2064 6566 205f 6372 6561 7465 5f6d 6173   def _create_mas
-00011350: 7465 725f 786d 6c28 7365 6c66 293a 0d0a  ter_xml(self):..
-00011360: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00011370: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00011380: 2020 666f 7220 5370 6f74 6f62 6a65 6374    for Spotobject
-00011390: 2069 6e20 7365 6c66 2e6d 6173 7465 725f   in self.master_
-000113a0: 786d 6c5f 726f 6f74 2e69 7465 7228 2753  xml_root.iter('S
-000113b0: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
-000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113d0: 2020 2020 2020 2020 6365 6c6c 5f69 6420          cell_id 
-000113e0: 3d20 696e 7428 5370 6f74 6f62 6a65 6374  = int(Spotobject
-000113f0: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
-00011400: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011420: 2020 2020 2020 2020 6966 2063 656c 6c5f          if cell_
-00011430: 6964 2069 6e20 7365 6c66 2e75 6e69 7175  id in self.uniqu
-00011440: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00011450: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
-00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011480: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114a0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-000114b0: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
-000114c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000114d0: 6365 6c6c 5f69 645d 2e6b 6579 7328 293a  cell_id].keys():
-000114e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00011510: 706f 746f 626a 6563 742e 7365 7428 6b2c  potobject.set(k,
-00011520: 2073 7472 2873 656c 662e 756e 6971 7565   str(self.unique
-00011530: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011540: 5b63 656c 6c5f 6964 5d5b 6b5d 2929 2020  [cell_id][k]))  
-00011550: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00011130: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00011140: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
+00011150: 3d20 7365 6c66 2e63 6f75 6e74 0d0a 2020  = self.count..  
+00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011180: 2020 7365 6c66 2e5f 6669 6e61 6c5f 7472    self._final_tr
+00011190: 6163 6b73 2874 7261 636b 5f69 6429 200d  acks(track_id) .
+000111a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000111b0: 2020 2069 6620 7365 6c66 2e66 6f75 7269     if self.fouri
+000111c0: 6572 3a0d 0a20 2020 2020 2020 2020 2020  er:..           
+000111d0: 2020 2020 2020 2020 7072 696e 7428 2763          print('c
+000111e0: 6f6d 7075 7469 6e67 2046 6f75 7269 6572  omputing Fourier
+000111f0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00011200: 2020 2020 2020 2073 656c 662e 5f63 6f6d         self._com
+00011210: 7075 7465 5f70 6865 6e6f 7479 7065 7328  pute_phenotypes(
+00011220: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+00011230: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00011240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011250: 5f74 656d 706f 7261 6c5f 706c 6f74 735f  _temporal_plots_
+00011260: 7472 6163 6b6d 6174 6528 290d 0a20 2020  trackmate()..   
+00011270: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+00011280: 0a20 2020 2064 6566 205f 6372 6561 7465  .    def _create
+00011290: 5f6d 6173 7465 725f 786d 6c28 7365 6c66  _master_xml(self
+000112a0: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
+000112b0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+000112c0: 2020 2020 2020 666f 7220 5370 6f74 6f62        for Spotob
+000112d0: 6a65 6374 2069 6e20 7365 6c66 2e6d 6173  ject in self.mas
+000112e0: 7465 725f 786d 6c5f 726f 6f74 2e69 7465  ter_xml_root.ite
+000112f0: 7228 2753 706f 7427 293a 0d0a 2020 2020  r('Spot'):..    
+00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011310: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+00011320: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
+00011330: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
+00011340: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
+00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011360: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00011370: 656c 6c5f 6964 2069 6e20 7365 6c66 2e75  ell_id in self.u
+00011380: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00011390: 7274 6965 732e 6b65 7973 2829 3a0d 0a20  rties.keys():.. 
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000113f0: 6f72 206b 2069 6e20 7365 6c66 2e75 6e69  or k in self.uni
+00011400: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011410: 6965 735b 6365 6c6c 5f69 645d 2e6b 6579  ies[cell_id].key
+00011420: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011450: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
+00011460: 7428 6b2c 2073 7472 2873 656c 662e 756e  t(k, str(self.un
+00011470: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00011480: 7469 6573 5b63 656c 6c5f 6964 5d5b 6b5d  ties[cell_id][k]
+00011490: 2929 2020 200d 0a0d 0a20 2020 2020 2020  ))   ....       
+000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000114c0: 0a0d 0a20 2020 2020 2020 2020 2020 7365  ...           se
+000114d0: 6c66 2e6d 6173 7465 725f 786d 6c5f 7472  lf.master_xml_tr
+000114e0: 6565 2e77 7269 7465 286f 732e 7061 7468  ee.write(os.path
+000114f0: 2e6a 6f69 6e28 7365 6c66 2e6d 6173 7465  .join(self.maste
+00011500: 725f 786d 6c5f 7061 7468 2c20 7365 6c66  r_xml_path, self
+00011510: 2e6d 6173 7465 725f 786d 6c5f 6e61 6d65  .master_xml_name
+00011520: 2929 0d0a 2020 2020 2020 2020 2020 200d  ))..           .
+00011530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011550: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011570: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-00011580: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00011590: 6173 7465 725f 786d 6c5f 7472 6565 2e77  aster_xml_tree.w
-000115a0: 7269 7465 286f 732e 7061 7468 2e6a 6f69  rite(os.path.joi
-000115b0: 6e28 7365 6c66 2e6d 6173 7465 725f 786d  n(self.master_xm
-000115c0: 6c5f 7061 7468 2c20 7365 6c66 2e6d 6173  l_path, self.mas
-000115d0: 7465 725f 786d 6c5f 6e61 6d65 2929 0d0a  ter_xml_name))..
-000115e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011610: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011630: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00011640: 0a20 2020 2064 6566 205f 6173 7369 676e  .    def _assign
-00011650: 5f63 6c75 7374 6572 5f63 6c61 7373 2873  _cluster_class(s
-00011660: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-00011670: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00011680: 2020 2020 2020 2020 7365 6c66 2e61 7865          self.axe
-00011690: 7320 3d20 7365 6c66 2e61 7865 732e 7265  s = self.axes.re
-000116a0: 706c 6163 6528 2254 222c 2022 2229 0d0a  place("T", "")..
-000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000116d0: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-000116e0: 756e 742c 2074 696d 655f 6b65 7920 696e  unt, time_key in
-000116f0: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
-00011700: 5f74 696d 6564 5f63 656e 7472 6f69 642e  _timed_centroid.
-00011710: 6b65 7973 2829 293a 0d0a 2020 2020 2020  keys()):..      
-00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011730: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011750: 2020 7472 6565 2c20 7370 6f74 5f63 656e    tree, spot_cen
-00011760: 7472 6f69 6473 203d 2073 656c 662e 5f74  troids = self._t
-00011770: 696d 6564 5f63 656e 7472 6f69 645b 7469  imed_centroid[ti
-00011780: 6d65 5f6b 6579 5d0d 0a20 2020 2020 2020  me_key]..       
-00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117a0: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-000117b0: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-000117c0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011580: 200d 0a0d 0a20 2020 2064 6566 205f 6173   ....    def _as
+00011590: 7369 676e 5f63 6c75 7374 6572 5f63 6c61  sign_cluster_cla
+000115a0: 7373 2873 656c 6629 3a0d 0a20 2020 2020  ss(self):..     
+000115b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000115c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000115d0: 2e61 7865 7320 3d20 7365 6c66 2e61 7865  .axes = self.axe
+000115e0: 732e 7265 706c 6163 6528 2254 222c 2022  s.replace("T", "
+000115f0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00011600: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00011610: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00011620: 7220 636f 756e 742c 2074 696d 655f 6b65  r count, time_ke
+00011630: 7920 696e 2065 6e75 6d65 7261 7465 2873  y in enumerate(s
+00011640: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
+00011650: 6f69 642e 6b65 7973 2829 293a 0d0a 2020  oid.keys()):..  
+00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011670: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011690: 2020 2020 2020 7472 6565 2c20 7370 6f74        tree, spot
+000116a0: 5f63 656e 7472 6f69 6473 203d 2073 656c  _centroids = sel
+000116b0: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
+000116c0: 645b 7469 6d65 5f6b 6579 5d0d 0a20 2020  d[time_key]..   
+000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000116f0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+00011700: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011720: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011730: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
+00011740: 656c 203d 2022 436f 6d70 7574 696e 6720  el = "Computing 
+00011750: 636c 7573 7465 7269 6e67 2063 6c61 7373  clustering class
+00011760: 6573 220d 0a20 2020 2020 2020 2020 2020  es"..           
+00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011780: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00011790: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+000117a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000117d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117e0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-000117f0: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
-00011800: 2022 436f 6d70 7574 696e 6720 636c 7573   "Computing clus
-00011810: 7465 7269 6e67 2063 6c61 7373 6573 220d  tering classes".
-00011820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011840: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00011850: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
+000117e0: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
+000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011820: 2020 2020 2020 6c65 6e28 7365 6c66 2e5f        len(self._
+00011830: 7469 6d65 645f 6365 6e74 726f 6964 2e6b  timed_centroid.k
+00011840: 6579 7328 2929 202b 2031 2c0d 0a20 2020  eys()) + 1,..   
+00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011860: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011890: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-000118a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000118b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011880: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000118b0: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
+000118c0: 6c75 6520 3d20 2063 6f75 6e74 200d 0a20  lue =  count .. 
 000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118e0: 2020 6c65 6e28 7365 6c66 2e5f 7469 6d65    len(self._time
-000118f0: 645f 6365 6e74 726f 6964 2e6b 6579 7328  d_centroid.keys(
-00011900: 2929 202b 2031 2c0d 0a20 2020 2020 2020  )) + 1,..       
+000118e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000118f0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00011900: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
 00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011940: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011960: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00011970: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
-00011980: 3d20 2063 6f75 6e74 200d 0a20 2020 2020  =  count ..     
-00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000119b0: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
-000119c0: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
-000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119e0: 2020 636c 7573 7465 725f 6576 616c 203d    cluster_eval =
-000119f0: 2043 6c75 7374 6572 696e 6728 7365 6c66   Clustering(self
-00011a00: 2e73 6567 5f69 6d61 6765 5b69 6e74 2874  .seg_image[int(t
-00011a10: 696d 655f 6b65 7929 2c3a 5d2c 2020 7365  ime_key),:],  se
-00011a20: 6c66 2e61 7865 732c 2073 656c 662e 6e75  lf.axes, self.nu
-00011a30: 6d5f 706f 696e 7473 2c20 7365 6c66 2e63  m_points, self.c
-00011a40: 6c75 7374 6572 5f6d 6f64 656c 2c20 6b65  luster_model, ke
-00011a50: 7920 3d20 7469 6d65 5f6b 6579 2c20 7072  y = time_key, pr
-00011a60: 6f67 7265 7373 5f62 6172 3d73 656c 662e  ogress_bar=self.
-00011a70: 7072 6f67 7265 7373 5f62 6172 2c20 6261  progress_bar, ba
-00011a80: 7463 685f 7369 7a65 203d 2073 656c 662e  tch_size = self.
-00011a90: 6261 7463 685f 7369 7a65 2920 2020 2020  batch_size)     
-00011aa0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00011ab0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011ac0: 6c75 7374 6572 5f65 7661 6c2e 5f63 7265  luster_eval._cre
-00011ad0: 6174 655f 636c 7573 7465 725f 6c61 6265  ate_cluster_labe
-00011ae0: 6c73 2829 0d0a 2020 2020 2020 2020 2020  ls()..          
-00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b00: 2074 696d 6564 5f63 6c75 7374 6572 5f6c   timed_cluster_l
-00011b10: 6162 656c 203d 2063 6c75 7374 6572 5f65  abel = cluster_e
-00011b20: 7661 6c2e 7469 6d65 645f 636c 7573 7465  val.timed_cluste
-00011b30: 725f 6c61 6265 6c20 0d0a 2020 2020 2020  r_label ..      
-00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b50: 2020 2020 206f 7574 7075 745f 6c61 6265       output_labe
-00011b60: 6c73 2c20 6f75 7470 7574 5f63 6c75 7374  ls, output_clust
-00011b70: 6572 5f73 636f 7265 2c20 6f75 7470 7574  er_score, output
-00011b80: 5f63 6c75 7374 6572 5f63 6c61 7373 2c20  _cluster_class, 
-00011b90: 6f75 7470 7574 5f63 6c75 7374 6572 5f63  output_cluster_c
-00011ba0: 656e 7472 6f69 642c 206f 7574 7075 745f  entroid, output_
-00011bb0: 636c 6f75 645f 6563 6365 6e74 7269 6369  cloud_eccentrici
-00011bc0: 7479 2c20 6f75 7470 7574 5f6c 6172 6765  ty, output_large
-00011bd0: 7374 5f65 6967 656e 7665 6374 6f72 2c20  st_eigenvector, 
-00011be0: 6f75 7470 7574 5f63 6c6f 7564 5f73 7572  output_cloud_sur
-00011bf0: 6661 6365 5f61 7265 6120 3d20 7469 6d65  face_area = time
-00011c00: 645f 636c 7573 7465 725f 6c61 6265 6c5b  d_cluster_label[
-00011c10: 7469 6d65 5f6b 6579 5d0d 0a20 2020 2020  time_key]..     
+00011920: 2020 2020 2020 636c 7573 7465 725f 6576        cluster_ev
+00011930: 616c 203d 2043 6c75 7374 6572 696e 6728  al = Clustering(
+00011940: 7365 6c66 2e73 6567 5f69 6d61 6765 5b69  self.seg_image[i
+00011950: 6e74 2874 696d 655f 6b65 7929 2c3a 5d2c  nt(time_key),:],
+00011960: 2020 7365 6c66 2e61 7865 732c 2073 656c    self.axes, sel
+00011970: 662e 6e75 6d5f 706f 696e 7473 2c20 7365  f.num_points, se
+00011980: 6c66 2e63 6c75 7374 6572 5f6d 6f64 656c  lf.cluster_model
+00011990: 2c20 6b65 7920 3d20 7469 6d65 5f6b 6579  , key = time_key
+000119a0: 2c20 7072 6f67 7265 7373 5f62 6172 3d73  , progress_bar=s
+000119b0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+000119c0: 2c20 6261 7463 685f 7369 7a65 203d 2073  , batch_size = s
+000119d0: 656c 662e 6261 7463 685f 7369 7a65 2920  elf.batch_size) 
+000119e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a00: 2020 2063 6c75 7374 6572 5f65 7661 6c2e     cluster_eval.
+00011a10: 5f63 7265 6174 655f 636c 7573 7465 725f  _create_cluster_
+00011a20: 6c61 6265 6c73 2829 0d0a 2020 2020 2020  labels()..      
+00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a40: 2020 2020 2074 696d 6564 5f63 6c75 7374       timed_clust
+00011a50: 6572 5f6c 6162 656c 203d 2063 6c75 7374  er_label = clust
+00011a60: 6572 5f65 7661 6c2e 7469 6d65 645f 636c  er_eval.timed_cl
+00011a70: 7573 7465 725f 6c61 6265 6c20 0d0a 2020  uster_label ..  
+00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a90: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+00011aa0: 6c61 6265 6c73 2c20 6f75 7470 7574 5f63  labels, output_c
+00011ab0: 6c75 7374 6572 5f73 636f 7265 2c20 6f75  luster_score, ou
+00011ac0: 7470 7574 5f63 6c75 7374 6572 5f63 6c61  tput_cluster_cla
+00011ad0: 7373 2c20 6f75 7470 7574 5f63 6c75 7374  ss, output_clust
+00011ae0: 6572 5f63 656e 7472 6f69 642c 206f 7574  er_centroid, out
+00011af0: 7075 745f 636c 6f75 645f 6563 6365 6e74  put_cloud_eccent
+00011b00: 7269 6369 7479 2c20 6f75 7470 7574 5f6c  ricity, output_l
+00011b10: 6172 6765 7374 5f65 6967 656e 7665 6374  argest_eigenvect
+00011b20: 6f72 2c20 6f75 7470 7574 5f63 6c6f 7564  or, output_cloud
+00011b30: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
+00011b40: 7469 6d65 645f 636c 7573 7465 725f 6c61  timed_cluster_la
+00011b50: 6265 6c5b 7469 6d65 5f6b 6579 5d0d 0a20  bel[time_key].. 
+00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b70: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b90: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00011ba0: 7261 6e67 6528 6c65 6e28 6f75 7470 7574  range(len(output
+00011bb0: 5f63 6c75 7374 6572 5f63 656e 7472 6f69  _cluster_centroi
+00011bc0: 6429 293a 0d0a 2020 2020 2020 2020 2020  d)):..          
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 2020 2020 2020 2020 2020 6365 6e74 726f            centro
+00011bf0: 6964 203d 206f 7574 7075 745f 636c 7573  id = output_clus
+00011c00: 7465 725f 6365 6e74 726f 6964 5b69 5d0d  ter_centroid[i].
+00011c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c50: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00011c60: 6528 6c65 6e28 6f75 7470 7574 5f63 6c75  e(len(output_clu
-00011c70: 7374 6572 5f63 656e 7472 6f69 6429 293a  ster_centroid)):
-00011c80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ca0: 2020 2020 2020 6365 6e74 726f 6964 203d        centroid =
-00011cb0: 206f 7574 7075 745f 636c 7573 7465 725f   output_cluster_
-00011cc0: 6365 6e74 726f 6964 5b69 5d0d 0a20 2020  centroid[i]..   
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cf0: 2063 6c75 7374 6572 5f63 6c61 7373 203d   cluster_class =
-00011d00: 206f 7574 7075 745f 636c 7573 7465 725f   output_cluster_
-00011d10: 636c 6173 735b 695d 0d0a 2020 2020 2020  class[i]..      
-00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d30: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00011d40: 7573 7465 725f 7363 6f72 6520 3d20 6f75  uster_score = ou
-00011d50: 7470 7574 5f63 6c75 7374 6572 5f73 636f  tput_cluster_sco
-00011d60: 7265 5b69 5d0d 0a20 2020 2020 2020 2020  re[i]..         
-00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d80: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
-00011d90: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00011da0: 7374 797a 203d 206f 7574 7075 745f 636c  styz = output_cl
-00011db0: 6f75 645f 6563 6365 6e74 7269 6369 7479  oud_eccentricity
-00011dc0: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011de0: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
-00011df0: 6973 203d 206f 7574 7075 745f 6c61 7267  is = output_larg
-00011e00: 6573 745f 6569 6765 6e76 6563 746f 725b  est_eigenvector[
-00011e10: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
-00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e30: 2020 2020 2020 2020 7375 7266 6163 655f          surface_
-00011e40: 6172 6561 203d 206f 7574 7075 745f 636c  area = output_cl
-00011e50: 6f75 645f 7375 7266 6163 655f 6172 6561  oud_surface_area
-00011e60: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e80: 2020 2020 2020 2020 2064 6973 742c 2069           dist, i
-00011e90: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
-00011ea0: 7928 6365 6e74 726f 6964 290d 0a20 2020  y(centroid)..   
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ed0: 2063 6c6f 7365 7374 5f63 656e 7472 6f69   closest_centroi
-00011ee0: 6420 3d20 7370 6f74 5f63 656e 7472 6f69  d = spot_centroi
-00011ef0: 6473 5b69 6e64 6578 5d0d 0a20 2020 2020  ds[index]..     
-00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011f20: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
-00011f30: 6964 203d 2028 696e 7428 7469 6d65 5f6b  id = (int(time_k
-00011f40: 6579 292c 636c 6f73 6573 745f 6365 6e74  ey),closest_cent
-00011f50: 726f 6964 5b30 5d2c 2063 6c6f 7365 7374  roid[0], closest
-00011f60: 5f63 656e 7472 6f69 645b 315d 2c20 636c  _centroid[1], cl
-00011f70: 6f73 6573 745f 6365 6e74 726f 6964 5b32  osest_centroid[2
-00011f80: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fa0: 2020 2020 2020 2020 636c 6f73 6573 745f          closest_
-00011fb0: 6365 6c6c 5f69 6420 3d20 7365 6c66 2e75  cell_id = self.u
-00011fc0: 6e69 7175 655f 7370 6f74 5f63 656e 7472  nique_spot_centr
-00011fd0: 6f69 645b 6672 616d 655f 7370 6f74 5f63  oid[frame_spot_c
-00011fe0: 656e 7472 6f69 645d 0d0a 2020 2020 2020  entroid]..      
-00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012000: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00012010: 736b 5f76 6563 746f 7220 3d20 5b20 666c  sk_vector = [ fl
-00012020: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00012030: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00012040: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00012050: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
-00012060: 656e 7472 6f69 645f 785f 6b65 795d 292c  entroid_x_key]),
-00012070: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00012080: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012090: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-000120a0: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-000120b0: 736b 6365 6e74 726f 6964 5f79 5f6b 6579  skcentroid_y_key
-000120c0: 5d29 2c20 666c 6f61 7428 7365 6c66 2e75  ]), float(self.u
-000120d0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000120e0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-000120f0: 745f 6365 6c6c 5f69 6429 5d5b 7365 6c66  t_cell_id)][self
-00012100: 2e6d 6173 6b63 656e 7472 6f69 645f 7a5f  .maskcentroid_z_
-00012110: 6b65 795d 2920 5d0d 0a20 2020 2020 2020  key]) ]..       
-00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012130: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00012140: 6c5f 6178 6973 5f6d 6173 6b20 3d20 616e  l_axis_mask = an
-00012150: 6775 6c61 725f 6368 616e 6765 2863 656c  gular_change(cel
-00012160: 6c5f 6178 6973 2c20 6d61 736b 5f76 6563  l_axis, mask_vec
-00012170: 746f 7229 0d0a 2020 2020 2020 2020 2020  tor)..          
-00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012190: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121c0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000121d0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000121e0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-000121f0: 5d2e 7570 6461 7465 287b 7365 6c66 2e63  ].update({self.c
-00012200: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
-00012210: 203a 2063 656c 6c5f 6178 6973 5f6d 6173   : cell_axis_mas
-00012220: 6b7d 290d 0a20 2020 2020 2020 2020 2020  k})..           
-00012230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012240: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00012250: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00012260: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00012270: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
-00012280: 6528 7b73 656c 662e 636c 7573 7465 7263  e({self.clusterc
-00012290: 6c61 7373 5f6b 6579 203a 2063 6c75 7374  lass_key : clust
-000122a0: 6572 5f63 6c61 7373 7d29 0d0a 2020 2020  er_class})..    
-000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122d0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000122e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000122f0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00012300: 5d2e 7570 6461 7465 287b 7365 6c66 2e63  ].update({self.c
-00012310: 6c75 7374 6572 7363 6f72 655f 6b65 7920  lusterscore_key 
-00012320: 3a20 636c 7573 7465 725f 7363 6f72 657d  : cluster_score}
-00012330: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012360: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012370: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00012380: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00012390: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
-000123a0: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
-000123b0: 203a 2065 6363 656e 7472 6963 6974 795f   : eccentricity_
-000123c0: 636f 6d70 5f66 6972 7374 797a 5b30 5d7d  comp_firstyz[0]}
-000123d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000123e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123f0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012400: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012410: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00012420: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00012430: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
-00012440: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
-00012450: 7920 3a20 6563 6365 6e74 7269 6369 7479  y : eccentricity
-00012460: 5f63 6f6d 705f 6669 7273 7479 7a5b 315d  _comp_firstyz[1]
-00012470: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00012480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012490: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000124a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000124b0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-000124c0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-000124d0: 287b 7365 6c66 2e73 7572 6661 6365 5f61  ({self.surface_a
-000124e0: 7265 615f 6b65 7920 3a20 7375 7266 6163  rea_key : surfac
-000124f0: 655f 6172 6561 7d29 0d0a 0d0a 2020 2020  e_area})....    
-00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012530: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00012540: 2028 6b2c 7629 2069 6e20 7365 6c66 2e72   (k,v) in self.r
-00012550: 6f6f 745f 7370 6f74 732e 6974 656d 7328  oot_spots.items(
-00012560: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012580: 2020 2020 2020 7365 6c66 2e72 6f6f 745f        self.root_
-00012590: 7370 6f74 735b 6b5d 203d 2073 656c 662e  spots[k] = self.
-000125a0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000125b0: 6572 7469 6573 5b6b 5d20 2020 2020 2020  erties[k]       
-000125c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000125d0: 2020 2020 0d0a 2020 2020 6465 6620 5f63      ..    def _c
-000125e0: 6f6d 7075 7465 5f70 6865 6e6f 7479 7065  ompute_phenotype
-000125f0: 7328 7365 6c66 293a 0d0a 0d0a 2020 2020  s(self):....    
-00012600: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
-00012610: 696e 2073 656c 662e 756e 6971 7565 5f74  in self.unique_t
-00012620: 7261 636b 732e 6974 656d 7328 293a 0d0a  racks.items():..
-00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012650: 2020 7472 6163 6b5f 6964 203d 206b 0d0a    track_id = k..
-00012660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012670: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00012680: 6965 7320 3d20 7365 6c66 2e75 6e69 7175  ies = self.uniqu
-00012690: 655f 7472 6163 6b5f 7072 6f70 6572 7469  e_track_properti
-000126a0: 6573 5b6b 5d0d 0a20 2020 2020 2020 2020  es[k]..         
-000126b0: 2020 2020 2020 2074 7261 636b 7320 3d20         tracks = 
-000126c0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-000126d0: 6b73 5b6b 5d0d 0a20 2020 2020 2020 2020  ks[k]..         
-000126e0: 2020 2020 2020 205a 203d 2074 7261 636b         Z = track
-000126f0: 735b 3a2c 325d 0d0a 2020 2020 2020 2020  s[:,2]..        
-00012700: 2020 2020 2020 2020 5920 3d20 7472 6163          Y = trac
-00012710: 6b73 5b3a 2c33 5d0d 0a20 2020 2020 2020  ks[:,3]..       
-00012720: 2020 2020 2020 2020 2058 203d 2074 7261           X = tra
-00012730: 636b 735b 3a2c 345d 0d0a 2020 2020 2020  cks[:,4]..      
-00012740: 2020 2020 2020 2020 2020 7469 6d65 203d            time =
-00012750: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00012760: 7469 6573 5b3a 2c30 5d0d 0a20 2020 2020  ties[:,0]..     
-00012770: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00012780: 655f 6964 7320 3d20 7472 6163 6b6c 6574  e_ids = tracklet
-00012790: 5f70 726f 7065 7274 6965 735b 3a2c 315d  _properties[:,1]
-000127a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000127b0: 2020 756e 6971 7565 5f69 6473 5f73 6574    unique_ids_set
-000127c0: 203d 2073 6574 2875 6e69 7175 655f 6964   = set(unique_id
-000127d0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-000127e0: 2020 2020 6765 6e65 7261 7469 6f6e 5f69      generation_i
-000127f0: 6473 203d 2074 7261 636b 6c65 745f 7072  ds = tracklet_pr
-00012800: 6f70 6572 7469 6573 5b3a 2c32 5d0d 0a20  operties[:,2].. 
-00012810: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012820: 6164 6975 7320 3d20 7472 6163 6b6c 6574  adius = tracklet
-00012830: 5f70 726f 7065 7274 6965 735b 3a2c 335d  _properties[:,3]
+00011c30: 2020 2020 2063 6c75 7374 6572 5f63 6c61       cluster_cla
+00011c40: 7373 203d 206f 7574 7075 745f 636c 7573  ss = output_clus
+00011c50: 7465 725f 636c 6173 735b 695d 0d0a 2020  ter_class[i]..  
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c80: 2020 636c 7573 7465 725f 7363 6f72 6520    cluster_score 
+00011c90: 3d20 6f75 7470 7574 5f63 6c75 7374 6572  = output_cluster
+00011ca0: 5f73 636f 7265 5b69 5d0d 0a20 2020 2020  _score[i]..     
+00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cc0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011cd0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00011ce0: 5f66 6972 7374 797a 203d 206f 7574 7075  _firstyz = outpu
+00011cf0: 745f 636c 6f75 645f 6563 6365 6e74 7269  t_cloud_eccentri
+00011d00: 6369 7479 5b69 5d0d 0a20 2020 2020 2020  city[i]..       
+00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d20: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+00011d30: 6c5f 6178 6973 203d 206f 7574 7075 745f  l_axis = output_
+00011d40: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
+00011d50: 746f 725b 695d 0d0a 2020 2020 2020 2020  tor[i]..        
+00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d70: 2020 2020 2020 2020 2020 2020 7375 7266              surf
+00011d80: 6163 655f 6172 6561 203d 206f 7574 7075  ace_area = outpu
+00011d90: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
+00011da0: 6172 6561 5b69 5d0d 0a20 2020 2020 2020  area[i]..       
+00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dc0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00011dd0: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
+00011de0: 7175 6572 7928 6365 6e74 726f 6964 290d  query(centroid).
+00011df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e10: 2020 2020 2063 6c6f 7365 7374 5f63 656e       closest_cen
+00011e20: 7472 6f69 6420 3d20 7370 6f74 5f63 656e  troid = spot_cen
+00011e30: 7472 6f69 6473 5b69 6e64 6578 5d0d 0a20  troids[index].. 
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e60: 2020 2066 7261 6d65 5f73 706f 745f 6365     frame_spot_ce
+00011e70: 6e74 726f 6964 203d 2028 696e 7428 7469  ntroid = (int(ti
+00011e80: 6d65 5f6b 6579 292c 636c 6f73 6573 745f  me_key),closest_
+00011e90: 6365 6e74 726f 6964 5b30 5d2c 2063 6c6f  centroid[0], clo
+00011ea0: 7365 7374 5f63 656e 7472 6f69 645b 315d  sest_centroid[1]
+00011eb0: 2c20 636c 6f73 6573 745f 6365 6e74 726f  , closest_centro
+00011ec0: 6964 5b32 5d29 0d0a 2020 2020 2020 2020  id[2])..        
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ee0: 2020 2020 2020 2020 2020 2020 636c 6f73              clos
+00011ef0: 6573 745f 6365 6c6c 5f69 6420 3d20 7365  est_cell_id = se
+00011f00: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
+00011f10: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
+00011f20: 6f74 5f63 656e 7472 6f69 645d 0d0a 2020  ot_centroid]..  
+00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f50: 2020 6d61 736b 5f76 6563 746f 7220 3d20    mask_vector = 
+00011f60: 5b20 666c 6f61 7428 7365 6c66 2e75 6e69  [ float(self.uni
+00011f70: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011f80: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00011f90: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00011fa0: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
+00011fb0: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
+00011fc0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00011fd0: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+00011fe0: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
+00011ff0: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
+00012000: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
+00012010: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00012020: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00012030: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
+00012040: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00012050: 645f 7a5f 6b65 795d 2920 5d0d 0a20 2020  d_z_key]) ]..   
+00012060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012080: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
+00012090: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
+000120a0: 2863 656c 6c5f 6178 6973 2c20 6d61 736b  (cell_axis, mask
+000120b0: 5f76 6563 746f 7229 0d0a 2020 2020 2020  _vector)..      
+000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012100: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00012110: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00012120: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
+00012130: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00012140: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
+00012150: 5f6b 6579 203a 2063 656c 6c5f 6178 6973  _key : cell_axis
+00012160: 5f6d 6173 6b7d 290d 0a20 2020 2020 2020  _mask})..       
+00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012180: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012190: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000121a0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+000121b0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+000121c0: 7064 6174 6528 7b73 656c 662e 636c 7573  pdate({self.clus
+000121d0: 7465 7263 6c61 7373 5f6b 6579 203a 2063  terclass_key : c
+000121e0: 6c75 7374 6572 5f63 6c61 7373 7d29 0d0a  luster_class})..
+000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012210: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00012220: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00012230: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
+00012240: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00012250: 6c66 2e63 6c75 7374 6572 7363 6f72 655f  lf.clusterscore_
+00012260: 6b65 7920 3a20 636c 7573 7465 725f 7363  key : cluster_sc
+00012270: 6f72 657d 290d 0a20 2020 2020 2020 2020  ore})..         
+00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000122a0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000122b0: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+000122c0: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
+000122d0: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
+000122e0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+000122f0: 746b 6579 203a 2065 6363 656e 7472 6963  tkey : eccentric
+00012300: 6974 795f 636f 6d70 5f66 6972 7374 797a  ity_comp_firstyz
+00012310: 5b30 5d7d 290d 0a20 2020 2020 2020 2020  [0]})..         
+00012320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012340: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00012350: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+00012360: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
+00012370: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
+00012380: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00012390: 6e64 6b65 7920 3a20 6563 6365 6e74 7269  ndkey : eccentri
+000123a0: 6369 7479 5f63 6f6d 705f 6669 7273 7479  city_comp_firsty
+000123b0: 7a5b 315d 7d29 0d0a 2020 2020 2020 2020  z[1]})..        
+000123c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000123e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000123f0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00012400: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00012410: 6461 7465 287b 7365 6c66 2e73 7572 6661  date({self.surfa
+00012420: 6365 5f61 7265 615f 6b65 7920 3a20 7375  ce_area_key : su
+00012430: 7266 6163 655f 6172 6561 7d29 0d0a 0d0a  rface_area})....
+00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012460: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012480: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+00012490: 6c66 2e72 6f6f 745f 7370 6f74 732e 6974  lf.root_spots.it
+000124a0: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
+000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000124d0: 6f6f 745f 7370 6f74 735b 6b5d 203d 2073  oot_spots[k] = s
+000124e0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000124f0: 7072 6f70 6572 7469 6573 5b6b 5d20 2020  properties[k]   
+00012500: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00012510: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00012520: 6620 5f63 6f6d 7075 7465 5f70 6865 6e6f  f _compute_pheno
+00012530: 7479 7065 7328 7365 6c66 293a 0d0a 0d0a  types(self):....
+00012540: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+00012550: 2c76 2920 696e 2073 656c 662e 756e 6971  ,v) in self.uniq
+00012560: 7565 5f74 7261 636b 732e 6974 656d 7328  ue_tracks.items(
+00012570: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00012580: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012590: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
+000125a0: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
+000125b0: 2020 2020 7472 6163 6b6c 6574 5f70 726f      tracklet_pro
+000125c0: 7065 7274 6965 7320 3d20 7365 6c66 2e75  perties = self.u
+000125d0: 6e69 7175 655f 7472 6163 6b5f 7072 6f70  nique_track_prop
+000125e0: 6572 7469 6573 5b6b 5d0d 0a20 2020 2020  erties[k]..     
+000125f0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00012600: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
+00012610: 7472 6163 6b73 5b6b 5d0d 0a20 2020 2020  tracks[k]..     
+00012620: 2020 2020 2020 2020 2020 205a 203d 2074             Z = t
+00012630: 7261 636b 735b 3a2c 325d 0d0a 2020 2020  racks[:,2]..    
+00012640: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
+00012650: 7472 6163 6b73 5b3a 2c33 5d0d 0a20 2020  tracks[:,3]..   
+00012660: 2020 2020 2020 2020 2020 2020 2058 203d               X =
+00012670: 2074 7261 636b 735b 3a2c 345d 0d0a 2020   tracks[:,4]..  
+00012680: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00012690: 6d65 203d 2074 7261 636b 6c65 745f 7072  me = tracklet_pr
+000126a0: 6f70 6572 7469 6573 5b3a 2c30 5d0d 0a20  operties[:,0].. 
+000126b0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+000126c0: 6e69 7175 655f 6964 7320 3d20 7472 6163  nique_ids = trac
+000126d0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+000126e0: 3a2c 315d 0d0a 2020 2020 2020 2020 2020  :,1]..          
+000126f0: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
+00012700: 5f73 6574 203d 2073 6574 2875 6e69 7175  _set = set(uniqu
+00012710: 655f 6964 7329 0d0a 2020 2020 2020 2020  e_ids)..        
+00012720: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
+00012730: 6f6e 5f69 6473 203d 2074 7261 636b 6c65  on_ids = trackle
+00012740: 745f 7072 6f70 6572 7469 6573 5b3a 2c32  t_properties[:,2
+00012750: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012760: 2020 2072 6164 6975 7320 3d20 7472 6163     radius = trac
+00012770: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012780: 3a2c 335d 0d0a 2020 2020 2020 2020 2020  :,3]..          
+00012790: 2020 2020 2020 766f 6c75 6d65 203d 2074        volume = t
+000127a0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+000127b0: 6573 5b3a 2c34 5d0d 0a20 2020 2020 2020  es[:,4]..       
+000127c0: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
+000127d0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+000127e0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+000127f0: 6572 7469 6573 5b3a 2c35 5d0d 0a20 2020  erties[:,5]..   
+00012800: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+00012810: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00012820: 6563 6f6e 6420 3d20 7472 6163 6b6c 6574  econd = tracklet
+00012830: 5f70 726f 7065 7274 6965 735b 3a2c 365d  _properties[:,6]
 00012840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012850: 2020 766f 6c75 6d65 203d 2074 7261 636b    volume = track
-00012860: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00012870: 2c34 5d0d 0a20 2020 2020 2020 2020 2020  ,4]..           
-00012880: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
-00012890: 795f 636f 6d70 5f66 6972 7374 203d 2074  y_comp_first = t
-000128a0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-000128b0: 6573 5b3a 2c35 5d0d 0a20 2020 2020 2020  es[:,5]..       
-000128c0: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-000128d0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-000128e0: 6420 3d20 7472 6163 6b6c 6574 5f70 726f  d = tracklet_pro
-000128f0: 7065 7274 6965 735b 3a2c 365d 0d0a 2020  perties[:,6]..  
-00012900: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00012910: 7266 6163 655f 6172 6561 203d 2074 7261  rface_area = tra
-00012920: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00012930: 5b3a 2c37 5d0d 0a20 2020 2020 2020 2020  [:,7]..         
-00012940: 2020 2020 2020 2063 6c75 7374 6572 5f63         cluster_c
-00012950: 6c61 7373 203d 2074 7261 636b 6c65 745f  lass = tracklet_
-00012960: 7072 6f70 6572 7469 6573 5b3a 2c38 5d0d  properties[:,8].
-00012970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012980: 2063 6c75 7374 6572 5f63 6c61 7373 5f73   cluster_class_s
-00012990: 636f 7265 203d 2074 7261 636b 6c65 745f  core = tracklet_
-000129a0: 7072 6f70 6572 7469 6573 5b3a 2c39 5d0d  properties[:,9].
-000129b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000129c0: 2069 6e74 656e 7369 7479 203d 2074 7261   intensity = tra
-000129d0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000129e0: 5b3a 2c31 305d 0d0a 2020 2020 2020 2020  [:,10]..        
-000129f0: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
-00012a00: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00012a10: 6965 735b 3a2c 3131 5d0d 0a20 2020 2020  ies[:,11]..     
-00012a20: 2020 2020 2020 2020 2020 206d 6f74 696f             motio
-00012a30: 6e5f 616e 676c 6520 3d20 7472 6163 6b6c  n_angle = trackl
-00012a40: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00012a50: 3132 5d0d 0a20 2020 2020 2020 2020 2020  12]..           
-00012a60: 2020 2020 2061 6363 656c 6572 6174 696f       acceleratio
-00012a70: 6e20 3d20 7472 6163 6b6c 6574 5f70 726f  n = tracklet_pro
-00012a80: 7065 7274 6965 735b 3a2c 3133 5d0d 0a20  perties[:,13].. 
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00012aa0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00012ab0: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
-00012ac0: 7065 7274 6965 735b 3a2c 3134 5d0d 0a20  perties[:,14].. 
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012ae0: 6164 6961 6c5f 616e 676c 6520 3d20 7472  adial_angle = tr
-00012af0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00012b00: 735b 3a2c 3135 5d0d 0a20 2020 2020 2020  s[:,15]..       
-00012b10: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
-00012b20: 6973 5f6d 6173 6b20 3d20 7472 6163 6b6c  is_mask = trackl
-00012b30: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00012b40: 3136 5d0d 0a0d 0a0d 0a20 2020 2020 2020  16]......       
-00012b50: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012b60: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00012b70: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
-00012b80: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
-00012b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ba0: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
-00012bb0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00012bc0: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
-00012bd0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00012be0: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
-00012bf0: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
-00012c00: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00012c10: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00012c20: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
-00012c30: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
-00012c40: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
-00012c50: 2020 2020 2075 6e69 7175 655f 7368 6170       unique_shap
-00012c60: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
-00012c70: 636b 6c65 7420 3d20 7b7d 0d0a 2020 2020  cklet = {}..    
-00012c80: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-00012c90: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
-00012ca0: 7274 6965 735f 7472 6163 6b6c 6574 203d  rties_tracklet =
-00012cb0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00012cc0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00012cd0: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
-00012ce0: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
-00012cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012d00: 2020 7365 6c66 2e75 6e69 7175 655f 6479    self.unique_dy
-00012d10: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
-00012d20: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
-00012d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d40: 2065 7870 616e 6465 645f 7469 6d65 203d   expanded_time =
-00012d50: 206e 702e 7a65 726f 7328 7365 6c66 2e74   np.zeros(self.t
-00012d60: 656e 6420 2d20 7365 6c66 2e74 7374 6172  end - self.tstar
-00012d70: 7420 2b20 3129 0d0a 2020 2020 2020 2020  t + 1)..        
-00012d80: 2020 2020 2020 2020 706f 696e 745f 7361          point_sa
-00012d90: 6d70 6c65 203d 2065 7870 616e 6465 645f  mple = expanded_
-00012da0: 7469 6d65 2e73 6861 7065 5b30 5d0d 0a20  time.shape[0].. 
-00012db0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012dc0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00012dd0: 6e28 6578 7061 6e64 6564 5f74 696d 6529  n(expanded_time)
-00012de0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00012df0: 2020 2020 2020 2020 2020 2065 7870 616e             expan
-00012e00: 6465 645f 7469 6d65 5b69 5d20 3d20 6920  ded_time[i] = i 
-00012e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012e20: 2020 666f 7220 6375 7272 656e 745f 756e    for current_un
-00012e30: 6971 7565 5f69 6420 696e 2075 6e69 7175  ique_id in uniqu
-00012e40: 655f 6964 735f 7365 743a 0d0a 2020 2020  e_ids_set:..    
-00012e50: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00012e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e70: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
-00012e80: 656e 7369 7479 203d 206e 702e 7a65 726f  ensity = np.zero
-00012e90: 7328 7365 6c66 2e74 656e 6420 2d20 7365  s(self.tend - se
-00012ea0: 6c66 2e74 7374 6172 7420 2b20 3129 0d0a  lf.tstart + 1)..
+00012850: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
+00012860: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00012870: 7469 6573 5b3a 2c37 5d0d 0a20 2020 2020  ties[:,7]..     
+00012880: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
+00012890: 6572 5f63 6c61 7373 203d 2074 7261 636b  er_class = track
+000128a0: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+000128b0: 2c38 5d0d 0a20 2020 2020 2020 2020 2020  ,8]..           
+000128c0: 2020 2020 2063 6c75 7374 6572 5f63 6c61       cluster_cla
+000128d0: 7373 5f73 636f 7265 203d 2074 7261 636b  ss_score = track
+000128e0: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+000128f0: 2c39 5d0d 0a20 2020 2020 2020 2020 2020  ,9]..           
+00012900: 2020 2020 2069 6e74 656e 7369 7479 203d       intensity =
+00012910: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00012920: 7469 6573 5b3a 2c31 305d 0d0a 2020 2020  ties[:,10]..    
+00012930: 2020 2020 2020 2020 2020 2020 7370 6565              spee
+00012940: 6420 3d20 7472 6163 6b6c 6574 5f70 726f  d = tracklet_pro
+00012950: 7065 7274 6965 735b 3a2c 3131 5d0d 0a20  perties[:,11].. 
+00012960: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00012970: 6f74 696f 6e5f 616e 676c 6520 3d20 7472  otion_angle = tr
+00012980: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00012990: 735b 3a2c 3132 5d0d 0a20 2020 2020 2020  s[:,12]..       
+000129a0: 2020 2020 2020 2020 2061 6363 656c 6572           acceler
+000129b0: 6174 696f 6e20 3d20 7472 6163 6b6c 6574  ation = tracklet
+000129c0: 5f70 726f 7065 7274 6965 735b 3a2c 3133  _properties[:,13
+000129d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000129e0: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
+000129f0: 5f6d 6173 6b20 3d20 7472 6163 6b6c 6574  _mask = tracklet
+00012a00: 5f70 726f 7065 7274 6965 735b 3a2c 3134  _properties[:,14
+00012a10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012a20: 2020 2072 6164 6961 6c5f 616e 676c 6520     radial_angle 
+00012a30: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00012a40: 7274 6965 735b 3a2c 3135 5d0d 0a20 2020  rties[:,15]..   
+00012a50: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+00012a60: 6c5f 6178 6973 5f6d 6173 6b20 3d20 7472  l_axis_mask = tr
+00012a70: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00012a80: 735b 3a2c 3136 5d0d 0a0d 0a0d 0a20 2020  s[:,16]......   
+00012a90: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00012aa0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00012ab0: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
+00012ac0: 7469 6573 5f74 7261 636b 6c65 7420 3d20  ties_tracklet = 
+00012ad0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+00012ae0: 2020 2020 756e 6971 7565 5f63 6c75 7374      unique_clust
+00012af0: 6572 5f70 726f 7065 7274 6965 735f 7472  er_properties_tr
+00012b00: 6163 6b6c 6574 203d 207b 7d0d 0a20 2020  acklet = {}..   
+00012b10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012b20: 662e 756e 6971 7565 5f66 6674 5f70 726f  f.unique_fft_pro
+00012b30: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00012b40: 5d20 3d20 7b7d 0d0a 2020 2020 2020 2020  ] = {}..        
+00012b50: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00012b60: 7175 655f 636c 7573 7465 725f 7072 6f70  que_cluster_prop
+00012b70: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
+00012b80: 203d 207b 7d0d 0a0d 0a20 2020 2020 2020   = {}....       
+00012b90: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
+00012ba0: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
+00012bb0: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
+00012be0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00012bf0: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
+00012c00: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00012c10: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
+00012c20: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
+00012c30: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00012c40: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00012c50: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
+00012c60: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
+00012c70: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00012c80: 2020 2020 2065 7870 616e 6465 645f 7469       expanded_ti
+00012c90: 6d65 203d 206e 702e 7a65 726f 7328 7365  me = np.zeros(se
+00012ca0: 6c66 2e74 656e 6420 2d20 7365 6c66 2e74  lf.tend - self.t
+00012cb0: 7374 6172 7420 2b20 3129 0d0a 2020 2020  start + 1)..    
+00012cc0: 2020 2020 2020 2020 2020 2020 706f 696e              poin
+00012cd0: 745f 7361 6d70 6c65 203d 2065 7870 616e  t_sample = expan
+00012ce0: 6465 645f 7469 6d65 2e73 6861 7065 5b30  ded_time.shape[0
+00012cf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012d00: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00012d10: 6528 6c65 6e28 6578 7061 6e64 6564 5f74  e(len(expanded_t
+00012d20: 696d 6529 293a 0d0a 2020 2020 2020 2020  ime)):..        
+00012d30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00012d40: 7870 616e 6465 645f 7469 6d65 5b69 5d20  xpanded_time[i] 
+00012d50: 3d20 6920 0d0a 2020 2020 2020 2020 2020  = i ..          
+00012d60: 2020 2020 2020 666f 7220 6375 7272 656e        for curren
+00012d70: 745f 756e 6971 7565 5f69 6420 696e 2075  t_unique_id in u
+00012d80: 6e69 7175 655f 6964 735f 7365 743a 0d0a  nique_ids_set:..
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00012db0: 2020 2020 2020 2020 6578 7061 6e64 6564          expanded
+00012dc0: 5f69 6e74 656e 7369 7479 203d 206e 702e  _intensity = np.
+00012dd0: 7a65 726f 7328 7365 6c66 2e74 656e 6420  zeros(self.tend 
+00012de0: 2d20 7365 6c66 2e74 7374 6172 7420 2b20  - self.tstart + 
+00012df0: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+00012e00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00012e10: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e30: 2063 7572 7265 6e74 5f74 696d 6520 3d20   current_time = 
+00012e40: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012e50: 2020 2020 2020 2063 7572 7265 6e74 5f7a         current_z
+00012e60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00012e70: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012e80: 745f 7920 3d20 5b5d 0d0a 2020 2020 2020  t_y = []..      
+00012e90: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012ea0: 7265 6e74 5f78 203d 205b 5d0d 0a20 2020  rent_x = []..   
 00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00012ed0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00012ee0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012ef0: 7265 6e74 5f74 696d 6520 3d20 5b5d 0d0a  rent_time = []..
-00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f10: 2020 2063 7572 7265 6e74 5f7a 203d 205b     current_z = [
-00012f20: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012f30: 2020 2020 2020 6375 7272 656e 745f 7920        current_y 
-00012f40: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00012f50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012f60: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
-00012f70: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012f80: 656e 745f 696e 7465 6e73 6974 7920 3d20  ent_intensity = 
-00012f90: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012fa0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00012fb0: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
-00012fc0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012fd0: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
-00012fe0: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
-00012ff0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-00013000: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013010: 6e74 5f72 6164 6975 7320 3d20 5b5d 0d0a  nt_radius = []..
-00013020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013030: 2020 2063 7572 7265 6e74 5f76 6f6c 756d     current_volum
-00013040: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-00013050: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013060: 6e74 5f73 7065 6564 203d 205b 5d0d 0a20  nt_speed = [].. 
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 6375 7272 656e 745f 6d6f 7469 6f6e    current_motion
-00013090: 5f61 6e67 6c65 203d 205b 5d0d 0a20 2020  _angle = []..   
-000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130b0: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
-000130c0: 7469 6f6e 203d 205b 5d0d 0a20 2020 2020  tion = []..     
-000130d0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000130e0: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
-000130f0: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
-00013100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013110: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
-00013120: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00013130: 7420 3d20 5b5d 0d0a 2020 2020 2020 2020  t = []..        
-00013140: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013150: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
-00013160: 636f 6d70 5f73 6563 6f6e 6420 3d20 5b5d  comp_second = []
-00013170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013180: 2020 2020 2063 7572 7265 6e74 5f73 7572       current_sur
-00013190: 6661 6365 5f61 7265 6120 3d20 5b5d 0d0a  face_area = []..
-000131a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000131b0: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
-000131c0: 6961 6c5f 616e 676c 6520 3d20 5b5d 0d0a  ial_angle = []..
+00012ec0: 6375 7272 656e 745f 696e 7465 6e73 6974  current_intensit
+00012ed0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00012ee0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012ef0: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
+00012f00: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00012f10: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012f20: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
+00012f30: 7363 6f72 6520 3d20 5b5d 0d0a 2020 2020  score = []..    
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012f50: 7572 7265 6e74 5f72 6164 6975 7320 3d20  urrent_radius = 
+00012f60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012f70: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
+00012f80: 6f6c 756d 6520 3d20 5b5d 0d0a 2020 2020  olume = []..    
+00012f90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012fa0: 7572 7265 6e74 5f73 7065 6564 203d 205b  urrent_speed = [
+00012fb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012fc0: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
+00012fd0: 7469 6f6e 5f61 6e67 6c65 203d 205b 5d0d  tion_angle = [].
+00012fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ff0: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
+00013000: 6c65 7261 7469 6f6e 203d 205b 5d0d 0a20  leration = [].. 
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
+00013030: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+00013040: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013050: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
+00013060: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00013070: 6669 7273 7420 3d20 5b5d 0d0a 2020 2020  first = []..    
+00013080: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013090: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+000130a0: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
+000130b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000130c0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000130d0: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
+000130e0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+000130f0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013100: 5f72 6164 6961 6c5f 616e 676c 6520 3d20  _radial_angle = 
+00013110: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00013120: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+00013130: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
+00013140: 5b5d 200d 0a20 2020 2020 2020 2020 2020  [] ..           
+00013150: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00013160: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00013170: 206a 2069 6e20 7261 6e67 6528 7469 6d65   j in range(time
+00013180: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
+00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131a0: 2020 2020 2020 2069 6620 6375 7272 656e         if curren
+000131b0: 745f 756e 6971 7565 5f69 6420 3d3d 2075  t_unique_id == u
+000131c0: 6e69 7175 655f 6964 735b 6a5d 3a0d 0a20  nique_ids[j]:.. 
 000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-000131f0: 6178 6973 5f6d 6173 6b20 3d20 5b5d 200d  axis_mask = [] .
-00013200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013210: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00013220: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00013230: 6e20 7261 6e67 6528 7469 6d65 2e73 6861  n range(time.sha
-00013240: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
+000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131f0: 6375 7272 656e 745f 7469 6d65 2e61 7070  current_time.app
+00013200: 656e 6428 7469 6d65 5b6a 5d29 0d0a 2020  end(time[j])..  
+00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013220: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013230: 7572 7265 6e74 5f7a 2e61 7070 656e 6428  urrent_z.append(
+00013240: 5a5b 6a5d 290d 0a20 2020 2020 2020 2020  Z[j])..         
 00013250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013260: 2020 2069 6620 6375 7272 656e 745f 756e     if current_un
-00013270: 6971 7565 5f69 6420 3d3d 2075 6e69 7175  ique_id == uniqu
-00013280: 655f 6964 735b 6a5d 3a0d 0a20 2020 2020  e_ids[j]:..     
+00013260: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013270: 792e 6170 7065 6e64 2859 5b6a 5d29 0d0a  y.append(Y[j])..
+00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132a0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000132b0: 656e 745f 7469 6d65 2e61 7070 656e 6428  ent_time.append(
-000132c0: 7469 6d65 5b6a 5d29 0d0a 2020 2020 2020  time[j])..      
-000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132e0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000132f0: 6e74 5f7a 2e61 7070 656e 6428 5a5b 6a5d  nt_z.append(Z[j]
-00013300: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000132a0: 2063 7572 7265 6e74 5f78 2e61 7070 656e   current_x.appen
+000132b0: 6428 585b 6a5d 290d 0a20 2020 2020 2020  d(X[j])..       
+000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132d0: 2020 2020 2020 2020 2020 6578 7061 6e64            expand
+000132e0: 6564 5f69 6e74 656e 7369 7479 5b69 6e74  ed_intensity[int
+000132f0: 2874 696d 655b 6a5d 295d 203d 2069 6e74  (time[j])] = int
+00013300: 656e 7369 7479 5b6a 5d0d 0a20 2020 2020  ensity[j]..     
 00013310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013320: 2020 2020 6375 7272 656e 745f 792e 6170      current_y.ap
-00013330: 7065 6e64 2859 5b6a 5d29 0d0a 2020 2020  pend(Y[j])..    
-00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013350: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013360: 7265 6e74 5f78 2e61 7070 656e 6428 585b  rent_x.append(X[
-00013370: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00013380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013390: 2020 2020 2020 6578 7061 6e64 6564 5f69        expanded_i
-000133a0: 6e74 656e 7369 7479 5b69 6e74 2874 696d  ntensity[int(tim
-000133b0: 655b 6a5d 295d 203d 2069 6e74 656e 7369  e[j])] = intensi
-000133c0: 7479 5b6a 5d0d 0a20 2020 2020 2020 2020  ty[j]..         
-000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000133f0: 696e 7465 6e73 6974 792e 6170 7065 6e64  intensity.append
-00013400: 2869 6e74 656e 7369 7479 5b6a 5d29 0d0a  (intensity[j])..
+00013320: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013330: 656e 745f 696e 7465 6e73 6974 792e 6170  ent_intensity.ap
+00013340: 7065 6e64 2869 6e74 656e 7369 7479 5b6a  pend(intensity[j
+00013350: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013370: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
+00013380: 7374 6572 5f63 6c61 7373 2e61 7070 656e  ster_class.appen
+00013390: 6428 636c 7573 7465 725f 636c 6173 735b  d(cluster_class[
+000133a0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133c0: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
+000133d0: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
+000133e0: 652e 6170 7065 6e64 2863 6c75 7374 6572  e.append(cluster
+000133f0: 5f63 6c61 7373 5f73 636f 7265 5b6a 5d29  _class_score[j])
+00013400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013430: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
-00013440: 5f63 6c61 7373 2e61 7070 656e 6428 636c  _class.append(cl
-00013450: 7573 7465 725f 636c 6173 735b 6a5d 290d  uster_class[j]).
-00013460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013480: 2020 6375 7272 656e 745f 636c 7573 7465    current_cluste
-00013490: 725f 636c 6173 735f 7363 6f72 652e 6170  r_class_score.ap
-000134a0: 7065 6e64 2863 6c75 7374 6572 5f63 6c61  pend(cluster_cla
-000134b0: 7373 5f73 636f 7265 5b6a 5d29 0d0a 2020  ss_score[j])..  
-000134c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000134e0: 7572 7265 6e74 5f72 6164 6975 732e 6170  urrent_radius.ap
-000134f0: 7065 6e64 2872 6164 6975 735b 6a5d 290d  pend(radius[j]).
-00013500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013520: 2020 6375 7272 656e 745f 766f 6c75 6d65    current_volume
-00013530: 2e61 7070 656e 6428 766f 6c75 6d65 5b6a  .append(volume[j
-00013540: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00013550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013560: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
-00013570: 6564 2e61 7070 656e 6428 7370 6565 645b  ed.append(speed[
-00013580: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135a0: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
-000135b0: 7469 6f6e 5f61 6e67 6c65 2e61 7070 656e  tion_angle.appen
-000135c0: 6428 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a  d(motion_angle[j
-000135d0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135f0: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
-00013600: 656c 6572 6174 696f 6e2e 6170 7065 6e64  eleration.append
-00013610: 2861 6363 656c 6572 6174 696f 6e5b 6a5d  (acceleration[j]
-00013620: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013420: 2020 2063 7572 7265 6e74 5f72 6164 6975     current_radiu
+00013430: 732e 6170 7065 6e64 2872 6164 6975 735b  s.append(radius[
+00013440: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013460: 2020 2020 2020 6375 7272 656e 745f 766f        current_vo
+00013470: 6c75 6d65 2e61 7070 656e 6428 766f 6c75  lume.append(volu
+00013480: 6d65 5b6a 5d29 0d0a 2020 2020 2020 2020  me[j])..        
+00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134a0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000134b0: 5f73 7065 6564 2e61 7070 656e 6428 7370  _speed.append(sp
+000134c0: 6565 645b 6a5d 290d 0a20 2020 2020 2020  eed[j])..       
+000134d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134e0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000134f0: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 2e61  t_motion_angle.a
+00013500: 7070 656e 6428 6d6f 7469 6f6e 5f61 6e67  ppend(motion_ang
+00013510: 6c65 5b6a 5d29 0d0a 2020 2020 2020 2020  le[j])..        
+00013520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013530: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013540: 5f61 6363 656c 6572 6174 696f 6e2e 6170  _acceleration.ap
+00013550: 7065 6e64 2861 6363 656c 6572 6174 696f  pend(acceleratio
+00013560: 6e5b 6a5d 290d 0a20 2020 2020 2020 2020  n[j])..         
+00013570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013580: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013590: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000135a0: 736b 2e61 7070 656e 6428 6469 7374 616e  sk.append(distan
+000135b0: 6365 5f63 656c 6c5f 6d61 736b 5b6a 5d29  ce_cell_mask[j])
+000135c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135e0: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
+000135f0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00013600: 7374 2e61 7070 656e 6428 6563 6365 6e74  st.append(eccent
+00013610: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00013620: 745b 6a5d 290d 0a20 2020 2020 2020 2020  t[j])..         
 00013630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013640: 2020 2020 6375 7272 656e 745f 6469 7374      current_dist
-00013650: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00013660: 7070 656e 6428 6469 7374 616e 6365 5f63  ppend(distance_c
-00013670: 656c 6c5f 6d61 736b 5b6a 5d29 0d0a 2020  ell_mask[j])..  
-00013680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013690: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000136a0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-000136b0: 6974 795f 636f 6d70 5f66 6972 7374 2e61  ity_comp_first.a
-000136c0: 7070 656e 6428 6563 6365 6e74 7269 6369  ppend(eccentrici
-000136d0: 7479 5f63 6f6d 705f 6669 7273 745b 6a5d  ty_comp_first[j]
-000136e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000136f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013700: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
-00013710: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00013720: 636f 6e64 2e61 7070 656e 6428 6563 6365  cond.append(ecce
-00013730: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00013740: 636f 6e64 5b6a 5d29 0d0a 2020 2020 2020  cond[j])..      
-00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013760: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013770: 6e74 5f73 7572 6661 6365 5f61 7265 612e  nt_surface_area.
-00013780: 6170 7065 6e64 2873 7572 6661 6365 5f61  append(surface_a
-00013790: 7265 615b 6a5d 290d 0a20 2020 2020 2020  rea[j])..       
-000137a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137b0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000137c0: 745f 7261 6469 616c 5f61 6e67 6c65 2e61  t_radial_angle.a
-000137d0: 7070 656e 6428 7261 6469 616c 5f61 6e67  ppend(radial_ang
-000137e0: 6c65 5b6a 5d29 0d0a 2020 2020 2020 2020  le[j])..        
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013810: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b2e  _cell_axis_mask.
-00013820: 6170 7065 6e64 2863 656c 6c5f 6178 6973  append(cell_axis
-00013830: 5f6d 6173 6b5b 6a5d 290d 0a20 2020 2020  _mask[j])..     
-00013840: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013850: 7272 656e 745f 7469 6d65 203d 206e 702e  rrent_time = np.
-00013860: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00013870: 7469 6d65 290d 0a20 2020 2020 2020 2020  time)..         
-00013880: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013890: 745f 696e 7465 6e73 6974 7920 3d20 6e70  t_intensity = np
-000138a0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-000138b0: 5f69 6e74 656e 7369 7479 290d 0a0d 0a0d  _intensity).....
-000138c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000138d0: 2020 2020 6375 7272 656e 745f 636c 7573      current_clus
-000138e0: 7465 725f 636c 6173 7320 3d20 6e70 2e61  ter_class = np.a
-000138f0: 7361 7272 6179 2863 7572 7265 6e74 5f63  sarray(current_c
-00013900: 6c75 7374 6572 5f63 6c61 7373 290d 0a20  luster_class).. 
-00013910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013920: 2020 6375 7272 656e 745f 636c 7573 7465    current_cluste
-00013930: 725f 636c 6173 735f 7363 6f72 6520 3d20  r_class_score = 
-00013940: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
-00013950: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00013960: 5f73 636f 7265 2920 2020 0d0a 0d0a 2020  _score)   ....  
-00013970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013980: 2063 7572 7265 6e74 5f72 6164 6975 7320   current_radius 
-00013990: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-000139a0: 7265 6e74 5f72 6164 6975 7329 0d0a 2020  rent_radius)..  
-000139b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139c0: 2063 7572 7265 6e74 5f76 6f6c 756d 6520   current_volume 
-000139d0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-000139e0: 7265 6e74 5f76 6f6c 756d 6529 0d0a 2020  rent_volume)..  
-000139f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a00: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
-00013a10: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00013a20: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00013a30: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-00013a40: 7479 5f63 6f6d 705f 6669 7273 7429 0d0a  ty_comp_first)..
-00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a60: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
-00013a70: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00013a80: 6f6e 6420 3d20 6e70 2e61 7361 7272 6179  ond = np.asarray
-00013a90: 2863 7572 7265 6e74 5f65 6363 656e 7472  (current_eccentr
-00013aa0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-00013ab0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00013ac0: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-00013ad0: 7572 6661 6365 5f61 7265 6120 3d20 6e70  urface_area = np
-00013ae0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013af0: 5f73 7572 6661 6365 5f61 7265 6129 0d0a  _surface_area)..
-00013b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013b10: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
-00013b20: 6564 203d 206e 702e 6173 6172 7261 7928  ed = np.asarray(
-00013b30: 6375 7272 656e 745f 7370 6565 6429 0d0a  current_speed)..
-00013b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b50: 2020 2063 7572 7265 6e74 5f6d 6f74 696f     current_motio
-00013b60: 6e5f 616e 676c 6520 3d20 6e70 2e61 7361  n_angle = np.asa
-00013b70: 7272 6179 2863 7572 7265 6e74 5f6d 6f74  rray(current_mot
-00013b80: 696f 6e5f 616e 676c 6529 0d0a 2020 2020  ion_angle)..    
-00013b90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013ba0: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
-00013bb0: 696f 6e20 3d20 6e70 2e61 7361 7272 6179  ion = np.asarray
-00013bc0: 2863 7572 7265 6e74 5f61 6363 656c 6572  (current_acceler
-00013bd0: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
-00013be0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013bf0: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
-00013c00: 5f6d 6173 6b20 3d20 6e70 2e61 7361 7272  _mask = np.asarr
-00013c10: 6179 2863 7572 7265 6e74 5f64 6973 7461  ay(current_dista
-00013c20: 6e63 655f 6365 6c6c 5f6d 6173 6b29 0d0a  nce_cell_mask)..
-00013c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c40: 2020 2063 7572 7265 6e74 5f72 6164 6961     current_radia
-00013c50: 6c5f 616e 676c 6520 3d20 6e70 2e61 7361  l_angle = np.asa
-00013c60: 7272 6179 2863 7572 7265 6e74 5f72 6164  rray(current_rad
-00013c70: 6961 6c5f 616e 676c 6529 0d0a 2020 2020  ial_angle)..    
-00013c80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013c90: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
-00013ca0: 5f6d 6173 6b20 3d20 6e70 2e61 7361 7272  _mask = np.asarr
-00013cb0: 6179 2863 7572 7265 6e74 5f63 656c 6c5f  ay(current_cell_
-00013cc0: 6178 6973 5f6d 6173 6b29 0d0a 0d0a 0d0a  axis_mask)......
-00013cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ce0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00013cf0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00013d00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00013d10: 706f 696e 745f 7361 6d70 6c65 203e 2030  point_sample > 0
-00013d20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d40: 2020 2078 665f 7361 6d70 6c65 203d 2066     xf_sample = f
-00013d50: 6674 6672 6571 2870 6f69 6e74 5f73 616d  ftfreq(point_sam
-00013d60: 706c 652c 2073 656c 662e 7463 616c 6962  ple, self.tcalib
-00013d70: 7261 7469 6f6e 290d 0a20 2020 2020 2020  ration)..       
-00013d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d90: 2020 2020 2020 2020 2066 6674 7374 7269           fftstri
-00013da0: 705f 7361 6d70 6c65 203d 2066 6674 2865  p_sample = fft(e
-00013db0: 7870 616e 6465 645f 696e 7465 6e73 6974  xpanded_intensit
-00013dc0: 7929 0d0a 2020 2020 2020 2020 2020 2020  y)..            
-00013dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013de0: 2020 2020 6666 7474 6f74 616c 5f73 616d      ffttotal_sam
-00013df0: 706c 6520 3d20 6e70 2e61 6273 2866 6674  ple = np.abs(fft
-00013e00: 7374 7269 705f 7361 6d70 6c65 290d 0a20  strip_sample).. 
-00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e20: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00013e30: 665f 7361 6d70 6c65 203d 2078 665f 7361  f_sample = xf_sa
-00013e40: 6d70 6c65 5b30 203a 206c 656e 2878 665f  mple[0 : len(xf_
-00013e50: 7361 6d70 6c65 2920 2f2f 2032 5d0d 0a20  sample) // 2].. 
-00013e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013e80: 6674 746f 7461 6c5f 7361 6d70 6c65 203d  fttotal_sample =
-00013e90: 2066 6674 746f 7461 6c5f 7361 6d70 6c65   ffttotal_sample
-00013ea0: 5b30 203a 206c 656e 2866 6674 746f 7461  [0 : len(ffttota
-00013eb0: 6c5f 7361 6d70 6c65 2920 2f2f 2032 5d0d  l_sample) // 2].
-00013ec0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00013ed0: 2020 2020 2020 756e 6971 7565 5f66 6674        unique_fft
-00013ee0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013ef0: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00013f00: 7175 655f 6964 5d20 3d20 6578 7061 6e64  que_id] = expand
-00013f10: 6564 5f74 696d 652c 2065 7870 616e 6465  ed_time, expande
-00013f20: 645f 696e 7465 6e73 6974 792c 2078 665f  d_intensity, xf_
-00013f30: 7361 6d70 6c65 2c20 6666 7474 6f74 616c  sample, ffttotal
-00013f40: 5f73 616d 706c 650d 0a20 2020 2020 2020  _sample..       
-00013f50: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-00013f60: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
-00013f70: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-00013f80: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00013f90: 5d20 3d20 2063 7572 7265 6e74 5f74 696d  ] =  current_tim
-00013fa0: 652c 2063 7572 7265 6e74 5f63 6c75 7374  e, current_clust
-00013fb0: 6572 5f63 6c61 7373 2c20 6375 7272 656e  er_class, curren
-00013fc0: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
-00013fd0: 7363 6f72 650d 0a20 2020 2020 2020 2020  score..         
-00013fe0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00013ff0: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
-00014000: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
-00014010: 6e74 5f75 6e69 7175 655f 6964 5d20 3d20  nt_unique_id] = 
-00014020: 6375 7272 656e 745f 7469 6d65 2c20 6375  current_time, cu
-00014030: 7272 656e 745f 7a2c 2063 7572 7265 6e74  rrent_z, current
-00014040: 5f79 2c20 6375 7272 656e 745f 782c 2063  _y, current_x, c
-00014050: 7572 7265 6e74 5f72 6164 6975 732c 2063  urrent_radius, c
-00014060: 7572 7265 6e74 5f76 6f6c 756d 652c 2063  urrent_volume, c
-00014070: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00014080: 6974 795f 636f 6d70 5f66 6972 7374 2c20  ity_comp_first, 
-00014090: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-000140a0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-000140b0: 2c20 6375 7272 656e 745f 7375 7266 6163  , current_surfac
-000140c0: 655f 6172 6561 2c20 6375 7272 656e 745f  e_area, current_
-000140d0: 636c 7573 7465 725f 636c 6173 732c 2063  cluster_class, c
-000140e0: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
-000140f0: 6c61 7373 5f73 636f 7265 0d0a 2020 2020  lass_score..    
-00014100: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00014110: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
-00014120: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00014130: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
-00014140: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
-00014150: 696d 652c 2063 7572 7265 6e74 5f73 7065  ime, current_spe
-00014160: 6564 2c20 6375 7272 656e 745f 6d6f 7469  ed, current_moti
-00014170: 6f6e 5f61 6e67 6c65 2c20 6375 7272 656e  on_angle, curren
-00014180: 745f 6163 6365 6c65 7261 7469 6f6e 2c20  t_acceleration, 
-00014190: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
-000141a0: 5f63 656c 6c5f 6d61 736b 2c20 6375 7272  _cell_mask, curr
-000141b0: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
-000141c0: 2c20 6375 7272 656e 745f 6365 6c6c 5f61  , current_cell_a
-000141d0: 7869 735f 6d61 736b 0d0a 2020 2020 2020  xis_mask..      
-000141e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000141f0: 662e 756e 6971 7565 5f66 6674 5f70 726f  f.unique_fft_pro
-00014200: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
-00014210: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
-00014220: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
-00014230: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
-00014240: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
-00014250: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
-00014260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014270: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00014280: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
-00014290: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
-000142a0: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
-000142b0: 7175 655f 6964 3a75 6e69 7175 655f 636c  que_id:unique_cl
-000142c0: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
-000142d0: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-000142e0: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
-000142f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014300: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00014310: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
-00014320: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
-00014330: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
-00014340: 7565 5f69 643a 756e 6971 7565 5f73 6861  ue_id:unique_sha
-00014350: 7065 5f70 726f 7065 7274 6965 735f 7472  pe_properties_tr
-00014360: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
-00014370: 6e69 7175 655f 6964 5d7d 290d 0a20 2020  nique_id]})..   
-00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014390: 7365 6c66 2e75 6e69 7175 655f 6479 6e61  self.unique_dyna
-000143a0: 6d69 635f 7072 6f70 6572 7469 6573 5b74  mic_properties[t
-000143b0: 7261 636b 5f69 645d 2e75 7064 6174 6528  rack_id].update(
-000143c0: 7b63 7572 7265 6e74 5f75 6e69 7175 655f  {current_unique_
-000143d0: 6964 3a75 6e69 7175 655f 6479 6e61 6d69  id:unique_dynami
-000143e0: 635f 7072 6f70 6572 7469 6573 5f74 7261  c_properties_tra
-000143f0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
-00014400: 6971 7565 5f69 645d 7d29 0d0a 0d0a 0d0a  ique_id]})......
-00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014430: 200d 0a20 2020 2064 6566 205f 6469 6374   ..    def _dict
-00014440: 5f75 7064 6174 6528 7365 6c66 2c20 756e  _update(self, un
-00014450: 6971 7565 5f74 7261 636b 6c65 745f 6964  ique_tracklet_id
-00014460: 733a 204c 6973 742c 2020 6365 6c6c 5f69  s: List,  cell_i
-00014470: 643a 2069 6e74 2c20 7472 6163 6b5f 6964  d: int, track_id
-00014480: 3a20 696e 742c 2073 6f75 7263 655f 6964  : int, source_id
-00014490: 3a20 696e 742c 2074 6172 6765 745f 6964  : int, target_id
-000144a0: 3a20 696e 7429 3a0d 0a0d 0a20 0d0a 2020  : int):.... ..  
-000144b0: 2020 2020 2020 6765 6e65 7261 7469 6f6e        generation
-000144c0: 5f69 6420 3d20 7365 6c66 2e67 656e 6572  _id = self.gener
-000144d0: 6174 696f 6e5f 6469 6374 5b63 656c 6c5f  ation_dict[cell_
-000144e0: 6964 5d0d 0a20 2020 2020 2020 2074 7261  id]..        tra
-000144f0: 636b 6c65 745f 6964 203d 2073 656c 662e  cklet_id = self.
-00014500: 7472 6163 6b6c 6574 5f64 6963 745b 6365  tracklet_dict[ce
-00014510: 6c6c 5f69 645d 0d0a 0d0a 2020 2020 2020  ll_id]....      
-00014520: 2020 756e 6971 7565 5f69 6420 3d20 7374    unique_id = st
-00014530: 7228 7472 6163 6b5f 6964 2920 2b20 7374  r(track_id) + st
-00014540: 7228 7365 6c66 2e6d 6178 5f74 7261 636b  r(self.max_track
-00014550: 5f69 6429 202b 2073 7472 2867 656e 6572  _id) + str(gener
-00014560: 6174 696f 6e5f 6964 2920 2b20 7374 7228  ation_id) + str(
-00014570: 7472 6163 6b6c 6574 5f69 6429 0d0a 2020  tracklet_id)..  
-00014580: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00014590: 7665 635f 6d61 736b 203d 205b 666c 6f61  vec_mask = [floa
-000145a0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-000145b0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000145c0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-000145d0: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
-000145e0: 6b65 795d 292c 2066 6c6f 6174 2873 656c  key]), float(sel
-000145f0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014600: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014610: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
-00014620: 6365 6e74 726f 6964 5f79 5f6b 6579 5d29  centroid_y_key])
-00014630: 2c20 666c 6f61 7428 7365 6c66 2e75 6e69  , float(self.uni
-00014640: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014650: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014660: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
-00014670: 6f69 645f 7a5f 6b65 795d 2920 5d0d 0a0d  oid_z_key]) ]...
-00014680: 0a20 2020 2020 2020 2076 6563 5f63 656c  .        vec_cel
-00014690: 6c20 3d20 5b66 6c6f 6174 2873 656c 662e  l = [float(self.
-000146a0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000146b0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000146c0: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
-000146d0: 5f6b 6579 5d29 202c 200d 0a20 2020 2020  _key]) , ..     
-000146e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146f0: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
-00014700: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014710: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014720: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
-00014730: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
-00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014750: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-00014760: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014770: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014780: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
-00014790: 7369 645f 6b65 795d 295d 0d0a 0d0a 2020  sid_key])]....  
-000147a0: 2020 2020 2020 616e 676c 6520 3d20 616e        angle = an
-000147b0: 6775 6c61 725f 6368 616e 6765 2876 6563  gular_change(vec
-000147c0: 5f6d 6173 6b2c 2076 6563 5f63 656c 6c29  _mask, vec_cell)
-000147d0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-000147e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000147f0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014800: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00014810: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
-00014820: 6b65 7920 3a20 616e 676c 657d 2920 2020  key : angle})   
-00014830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014840: 200d 0a0d 0a20 2020 2020 2020 2075 6e69   ....        uni
-00014850: 7175 655f 7472 6163 6b6c 6574 5f69 6473  que_tracklet_ids
-00014860: 2e61 7070 656e 6428 7374 7228 756e 6971  .append(str(uniq
-00014870: 7565 5f69 6429 290d 0a20 2020 2020 2020  ue_id))..       
-00014880: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014890: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000148a0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-000148b0: 6528 7b73 656c 662e 636c 7573 7465 7263  e({self.clusterc
-000148c0: 6c61 7373 5f6b 6579 203a 204e 6f6e 657d  lass_key : None}
-000148d0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000148e0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000148f0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014900: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00014910: 662e 636c 7573 7465 7273 636f 7265 5f6b  f.clusterscore_k
-00014920: 6579 203a 2030 7d29 0d0a 2020 2020 2020  ey : 0})..      
-00014930: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014940: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014950: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014960: 7465 287b 7365 6c66 2e75 6e69 7175 6569  te({self.uniquei
-00014970: 645f 6b65 7920 3a20 7374 7228 756e 6971  d_key : str(uniq
-00014980: 7565 5f69 6429 7d29 0d0a 2020 2020 2020  ue_id)})..      
-00014990: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-000149a0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000149b0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-000149c0: 7465 287b 7365 6c66 2e74 7261 636b 6c65  te({self.trackle
-000149d0: 7469 645f 6b65 7920 3a20 7374 7228 7472  tid_key : str(tr
-000149e0: 6163 6b6c 6574 5f69 6429 7d29 200d 0a20  acklet_id)}) .. 
-000149f0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00014a00: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014a10: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014a20: 2e75 7064 6174 6528 7b73 656c 662e 6765  .update({self.ge
-00014a30: 6e65 7261 7469 6f6e 6964 5f6b 6579 203a  nerationid_key :
-00014a40: 2073 7472 2867 656e 6572 6174 696f 6e5f   str(generation_
-00014a50: 6964 297d 2920 0d0a 2020 2020 2020 2020  id)}) ..        
-00014a60: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014a70: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014a80: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00014a90: 287b 7365 6c66 2e74 7261 636b 6964 5f6b  ({self.trackid_k
-00014aa0: 6579 203a 2073 7472 2874 7261 636b 5f69  ey : str(track_i
-00014ab0: 6429 7d29 0d0a 2020 2020 2020 2020 7365  d)})..        se
-00014ac0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014ad0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014ae0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00014af0: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
-00014b00: 655f 6b65 7920 3a20 302e 307d 290d 0a20  e_key : 0.0}).. 
-00014b10: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00014b20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014b30: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014b40: 2e75 7064 6174 6528 7b73 656c 662e 7370  .update({self.sp
-00014b50: 6565 645f 6b65 7920 3a20 302e 307d 290d  eed_key : 0.0}).
-00014b60: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00014b70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014b80: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014b90: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014ba0: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-00014bb0: 203a 2030 2e30 7d29 0d0a 2020 2020 2020   : 0.0})..      
-00014bc0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014bd0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014be0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014bf0: 7465 287b 7365 6c66 2e65 6363 656e 7472  te({self.eccentr
-00014c00: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00014c10: 6b65 7920 3a20 4e6f 6e65 7d29 0d0a 2020  key : None})..  
-00014c20: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014c30: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00014c40: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00014c50: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-00014c60: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00014c70: 6563 6f6e 646b 6579 203a 204e 6f6e 657d  econdkey : None}
-00014c80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00014c90: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014ca0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014cb0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00014cc0: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
-00014cd0: 6579 203a 204e 6f6e 657d 290d 0a20 2020  ey : None})..   
-00014ce0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00014cf0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014d00: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00014d10: 7064 6174 6528 7b73 656c 662e 6365 6c6c  pdate({self.cell
-00014d20: 6178 6973 5f6d 6173 6b5f 6b65 7920 3a20  axis_mask_key : 
-00014d30: 4e6f 6e65 7d29 0d0a 0d0a 2020 2020 2020  None})....      
-00014d40: 2020 6966 2073 6f75 7263 655f 6964 2069    if source_id i
-00014d50: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00014d60: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00014d70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014d80: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014d90: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014da0: 6265 666f 7265 6964 5f6b 6579 203a 2069  beforeid_key : i
-00014db0: 6e74 2873 6f75 7263 655f 6964 297d 290d  nt(source_id)}).
-00014dc0: 0a20 2020 2020 2020 2020 2020 2076 6563  .            vec
-00014dd0: 5f31 203d 205b 666c 6f61 7428 7365 6c66  _1 = [float(self
-00014de0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014df0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014e00: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
-00014e10: 645f 6b65 795d 2920 2d20 666c 6f61 7428  d_key]) - float(
-00014e20: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014e30: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014e40: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00014e50: 2e78 706f 7369 645f 6b65 795d 292c 200d  .xposid_key]), .
-00014e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014e70: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00014e80: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014e90: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014ea0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00014eb0: 662e 7970 6f73 6964 5f6b 6579 5d29 202d  f.yposid_key]) -
-00014ec0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00014ed0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014ee0: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
-00014ef0: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
-00014f00: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
-00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f20: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-00014f30: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014f40: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014f50: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
-00014f60: 6b65 795d 2920 2d20 2066 6c6f 6174 2873  key]) -  float(s
-00014f70: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014f80: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
-00014f90: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
-00014fa0: 7a70 6f73 6964 5f6b 6579 5d29 5d0d 0a20  zposid_key])].. 
-00014fb0: 2020 2020 2020 2020 2020 2073 7065 6564             speed
-00014fc0: 203d 206e 702e 7371 7274 286e 702e 646f   = np.sqrt(np.do
-00014fd0: 7428 7665 635f 312c 2076 6563 5f31 2929  t(vec_1, vec_1))
-00014fe0: 2f73 656c 662e 7463 616c 6962 7261 7469  /self.tcalibrati
-00014ff0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-00015000: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015010: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015020: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00015030: 287b 7365 6c66 2e73 7065 6564 5f6b 6579  ({self.speed_key
-00015040: 203a 2073 7065 6564 7d29 0d0a 0d0a 2020   : speed})....  
-00015050: 2020 2020 2020 2020 2020 6d6f 7469 6f6e            motion
-00015060: 5f61 6e67 6c65 203d 2061 6e67 756c 6172  _angle = angular
-00015070: 5f63 6861 6e67 6528 7665 635f 6d61 736b  _change(vec_mask
-00015080: 2c20 7665 635f 3129 0d0a 0d0a 2020 2020  , vec_1)....    
-00015090: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000150a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000150b0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000150c0: 5d2e 7570 6461 7465 287b 7365 6c66 2e6d  ].update({self.m
-000150d0: 6f74 696f 6e5f 616e 676c 655f 6b65 7920  otion_angle_key 
-000150e0: 3a20 6d6f 7469 6f6e 5f61 6e67 6c65 7d29  : motion_angle})
-000150f0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00015100: 2069 6620 736f 7572 6365 5f69 6420 696e   if source_id in
-00015110: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
-00015120: 655f 6c6f 6f6b 7570 3a0d 0a20 2020 2020  e_lookup:..     
-00015130: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00015140: 7265 5f73 6f75 7263 655f 6964 203d 2073  re_source_id = s
-00015150: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
-00015160: 6c6f 6f6b 7570 5b73 6f75 7263 655f 6964  lookup[source_id
-00015170: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015180: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00015190: 2020 2020 2020 2020 2020 2020 2076 6563               vec
-000151a0: 5f32 203d 205b 666c 6f61 7428 7365 6c66  _2 = [float(self
-000151b0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000151c0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000151d0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
-000151e0: 645f 6b65 795d 2920 2d20 3220 2a20 666c  d_key]) - 2 * fl
-000151f0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00015200: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015210: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
-00015220: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-00015230: 2920 2b20 666c 6f61 7428 7365 6c66 2e75  ) + float(self.u
-00015240: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015250: 7274 6965 735b 696e 7428 7072 655f 736f  rties[int(pre_so
-00015260: 7572 6365 5f69 6429 5d5b 7365 6c66 2e78  urce_id)][self.x
-00015270: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
-00015280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015290: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-000152a0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-000152b0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000152c0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-000152d0: 7970 6f73 6964 5f6b 6579 5d29 202d 2032  yposid_key]) - 2
-000152e0: 202a 2066 6c6f 6174 2873 656c 662e 756e   * float(self.un
-000152f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015300: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
-00015310: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
-00015320: 5f6b 6579 5d29 202b 2066 6c6f 6174 2873  _key]) + float(s
-00015330: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015340: 7072 6f70 6572 7469 6573 5b69 6e74 2870  properties[int(p
-00015350: 7265 5f73 6f75 7263 655f 6964 295d 5b73  re_source_id)][s
-00015360: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00015370: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-00015380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015390: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000153a0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000153b0: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-000153c0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-000153d0: 2920 2d20 2032 202a 2066 6c6f 6174 2873  ) -  2 * float(s
-000153e0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000153f0: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
-00015400: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
-00015410: 7a70 6f73 6964 5f6b 6579 5d29 202b 2066  zposid_key]) + f
-00015420: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00015430: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015440: 5b69 6e74 2870 7265 5f73 6f75 7263 655f  [int(pre_source_
-00015450: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-00015460: 5f6b 6579 5d29 5d0d 0a20 2020 2020 2020  _key])]..       
-00015470: 2020 2020 2020 2020 2020 2020 2061 6363               acc
-00015480: 203d 206e 702e 7371 7274 286e 702e 646f   = np.sqrt(np.do
-00015490: 7428 7665 635f 322c 2076 6563 5f32 2929  t(vec_2, vec_2))
-000154a0: 2f73 656c 662e 7463 616c 6962 7261 7469  /self.tcalibrati
-000154b0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-000154c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000154d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000154e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000154f0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015500: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00015510: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-00015520: 6e5f 6b65 7920 3a20 6163 637d 290d 0a20  n_key : acc}).. 
-00015530: 2020 2020 2020 2065 6c69 6620 736f 7572         elif sour
-00015540: 6365 5f69 6420 6973 204e 6f6e 653a 0d0a  ce_id is None:..
-00015550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015560: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015570: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015580: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015590: 6c66 2e62 6566 6f72 6569 645f 6b65 7920  lf.beforeid_key 
-000155a0: 3a20 4e6f 6e65 7d29 200d 0a20 2020 2020  : None}) ..     
-000155b0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-000155c0: 2020 2069 6620 7461 7267 6574 5f69 6420     if target_id 
-000155d0: 6973 206e 6f74 204e 6f6e 653a 2020 2020  is not None:    
-000155e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000155f0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00015600: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015610: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00015620: 6528 7b73 656c 662e 6166 7465 7269 645f  e({self.afterid_
-00015630: 6b65 7920 3a20 696e 7428 7461 7267 6574  key : int(target
-00015640: 5f69 6429 7d29 200d 0a20 2020 2020 2020  _id)}) ..       
-00015650: 2065 6c69 6620 7461 7267 6574 5f69 6420   elif target_id 
-00015660: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00015670: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00015680: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015690: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-000156a0: 7570 6461 7465 287b 7365 6c66 2e61 6674  update({self.aft
-000156b0: 6572 6964 5f6b 6579 203a 204e 6f6e 657d  erid_key : None}
-000156c0: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-000156d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000156e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000156f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015700: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00015710: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00015720: 6465 6620 5f74 656d 706f 7261 6c5f 706c  def _temporal_pl
-00015730: 6f74 735f 7472 6163 6b6d 6174 6528 7365  ots_trackmate(se
-00015740: 6c66 293a 0d0a 2020 2020 0d0a 2020 2020  lf):..    ..    
-00015750: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-00015760: 2020 2020 2020 2020 7365 6c66 2e41 7474          self.Att
-00015770: 7220 3d20 7b7d 0d0a 2020 2020 2020 2020  r = {}..        
-00015780: 2020 2020 2020 2020 7374 6172 7474 696d          starttim
-00015790: 6520 3d20 696e 7428 6d69 6e28 7365 6c66  e = int(min(self
-000157a0: 2e41 6c6c 5661 6c75 6573 5b73 656c 662e  .AllValues[self.
-000157b0: 6672 616d 6569 645f 6b65 795d 2929 0d0a  frameid_key]))..
-000157c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157d0: 656e 6474 696d 6520 3d20 696e 7428 6d61  endtime = int(ma
-000157e0: 7828 7365 6c66 2e41 6c6c 5661 6c75 6573  x(self.AllValues
-000157f0: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
-00015800: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
-00015810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00015820: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
-00015830: 6d65 203d 205b 5d0d 0a20 2020 2020 2020  me = []..       
-00015840: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015850: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00015860: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00015870: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015880: 6f74 6963 5f76 6172 5f64 6973 705f 7a20  otic_var_disp_z 
-00015890: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-000158a0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000158b0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
-000158c0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000158d0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-000158e0: 7469 635f 7661 725f 6469 7370 5f79 203d  tic_var_disp_y =
-000158f0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015900: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015910: 7469 635f 6d65 616e 5f64 6973 705f 7820  tic_mean_disp_x 
-00015920: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015930: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00015940: 6963 5f76 6172 5f64 6973 705f 7820 3d20  ic_var_disp_x = 
+00013640: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013650: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00013660: 705f 7365 636f 6e64 2e61 7070 656e 6428  p_second.append(
+00013670: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00013680: 705f 7365 636f 6e64 5b6a 5d29 0d0a 2020  p_second[j])..  
+00013690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000136b0: 7572 7265 6e74 5f73 7572 6661 6365 5f61  urrent_surface_a
+000136c0: 7265 612e 6170 7065 6e64 2873 7572 6661  rea.append(surfa
+000136d0: 6365 5f61 7265 615b 6a5d 290d 0a20 2020  ce_area[j])..   
+000136e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136f0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013700: 7272 656e 745f 7261 6469 616c 5f61 6e67  rrent_radial_ang
+00013710: 6c65 2e61 7070 656e 6428 7261 6469 616c  le.append(radial
+00013720: 5f61 6e67 6c65 5b6a 5d29 0d0a 2020 2020  _angle[j])..    
+00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013740: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013750: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
+00013760: 6173 6b2e 6170 7065 6e64 2863 656c 6c5f  ask.append(cell_
+00013770: 6178 6973 5f6d 6173 6b5b 6a5d 290d 0a20  axis_mask[j]).. 
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 2020 6375 7272 656e 745f 7469 6d65 203d    current_time =
+000137a0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+000137b0: 656e 745f 7469 6d65 290d 0a20 2020 2020  ent_time)..     
+000137c0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000137d0: 7272 656e 745f 696e 7465 6e73 6974 7920  rrent_intensity 
+000137e0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+000137f0: 7265 6e74 5f69 6e74 656e 7369 7479 290d  rent_intensity).
+00013800: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00013810: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013820: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
+00013830: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00013840: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
+00013850: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013860: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
+00013870: 7573 7465 725f 636c 6173 735f 7363 6f72  uster_class_scor
+00013880: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
+00013890: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
+000138a0: 6c61 7373 5f73 636f 7265 2920 2020 0d0a  lass_score)   ..
+000138b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000138c0: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
+000138d0: 6975 7320 3d20 6e70 2e61 7361 7272 6179  ius = np.asarray
+000138e0: 2863 7572 7265 6e74 5f72 6164 6975 7329  (current_radius)
+000138f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013900: 2020 2020 2063 7572 7265 6e74 5f76 6f6c       current_vol
+00013910: 756d 6520 3d20 6e70 2e61 7361 7272 6179  ume = np.asarray
+00013920: 2863 7572 7265 6e74 5f76 6f6c 756d 6529  (current_volume)
+00013930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013940: 2020 2020 2063 7572 7265 6e74 5f65 6363       current_ecc
+00013950: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00013960: 6972 7374 203d 206e 702e 6173 6172 7261  irst = np.asarra
+00013970: 7928 6375 7272 656e 745f 6563 6365 6e74  y(current_eccent
+00013980: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00013990: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000139a0: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
+000139b0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+000139c0: 5f73 6563 6f6e 6420 3d20 6e70 2e61 7361  _second = np.asa
+000139d0: 7272 6179 2863 7572 7265 6e74 5f65 6363  rray(current_ecc
+000139e0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+000139f0: 6563 6f6e 6429 0d0a 2020 2020 2020 2020  econd)..        
+00013a00: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013a10: 6e74 5f73 7572 6661 6365 5f61 7265 6120  nt_surface_area 
+00013a20: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+00013a30: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
+00013a40: 6129 0d0a 0d0a 2020 2020 2020 2020 2020  a)....          
+00013a50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013a60: 5f73 7065 6564 203d 206e 702e 6173 6172  _speed = np.asar
+00013a70: 7261 7928 6375 7272 656e 745f 7370 6565  ray(current_spee
+00013a80: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00013a90: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
+00013aa0: 6f74 696f 6e5f 616e 676c 6520 3d20 6e70  otion_angle = np
+00013ab0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013ac0: 5f6d 6f74 696f 6e5f 616e 676c 6529 0d0a  _motion_angle)..
+00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ae0: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
+00013af0: 6572 6174 696f 6e20 3d20 6e70 2e61 7361  eration = np.asa
+00013b00: 7272 6179 2863 7572 7265 6e74 5f61 6363  rray(current_acc
+00013b10: 656c 6572 6174 696f 6e29 0d0a 2020 2020  eleration)..    
+00013b20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013b30: 7572 7265 6e74 5f64 6973 7461 6e63 655f  urrent_distance_
+00013b40: 6365 6c6c 5f6d 6173 6b20 3d20 6e70 2e61  cell_mask = np.a
+00013b50: 7361 7272 6179 2863 7572 7265 6e74 5f64  sarray(current_d
+00013b60: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00013b70: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
+00013b80: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
+00013b90: 6164 6961 6c5f 616e 676c 6520 3d20 6e70  adial_angle = np
+00013ba0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013bb0: 5f72 6164 6961 6c5f 616e 676c 6529 0d0a  _radial_angle)..
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+00013be0: 6178 6973 5f6d 6173 6b20 3d20 6e70 2e61  axis_mask = np.a
+00013bf0: 7361 7272 6179 2863 7572 7265 6e74 5f63  sarray(current_c
+00013c00: 656c 6c5f 6178 6973 5f6d 6173 6b29 0d0a  ell_axis_mask)..
+00013c10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00013c20: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00013c30: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c50: 2069 6620 706f 696e 745f 7361 6d70 6c65   if point_sample
+00013c60: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c80: 2020 2020 2020 2078 665f 7361 6d70 6c65         xf_sample
+00013c90: 203d 2066 6674 6672 6571 2870 6f69 6e74   = fftfreq(point
+00013ca0: 5f73 616d 706c 652c 2073 656c 662e 7463  _sample, self.tc
+00013cb0: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
+00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cd0: 2020 2020 2020 2020 2020 2020 2066 6674               fft
+00013ce0: 7374 7269 705f 7361 6d70 6c65 203d 2066  strip_sample = f
+00013cf0: 6674 2865 7870 616e 6465 645f 696e 7465  ft(expanded_inte
+00013d00: 6e73 6974 7929 0d0a 2020 2020 2020 2020  nsity)..        
+00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d20: 2020 2020 2020 2020 6666 7474 6f74 616c          ffttotal
+00013d30: 5f73 616d 706c 6520 3d20 6e70 2e61 6273  _sample = np.abs
+00013d40: 2866 6674 7374 7269 705f 7361 6d70 6c65  (fftstrip_sample
+00013d50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d70: 2020 2078 665f 7361 6d70 6c65 203d 2078     xf_sample = x
+00013d80: 665f 7361 6d70 6c65 5b30 203a 206c 656e  f_sample[0 : len
+00013d90: 2878 665f 7361 6d70 6c65 2920 2f2f 2032  (xf_sample) // 2
+00013da0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013dc0: 2020 2066 6674 746f 7461 6c5f 7361 6d70     ffttotal_samp
+00013dd0: 6c65 203d 2066 6674 746f 7461 6c5f 7361  le = ffttotal_sa
+00013de0: 6d70 6c65 5b30 203a 206c 656e 2866 6674  mple[0 : len(fft
+00013df0: 746f 7461 6c5f 7361 6d70 6c65 2920 2f2f  total_sample) //
+00013e00: 2032 5d0d 0a0d 0a20 2020 2020 2020 2020   2]....         
+00013e10: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00013e20: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
+00013e30: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
+00013e40: 5f75 6e69 7175 655f 6964 5d20 3d20 6578  _unique_id] = ex
+00013e50: 7061 6e64 6564 5f74 696d 652c 2065 7870  panded_time, exp
+00013e60: 616e 6465 645f 696e 7465 6e73 6974 792c  anded_intensity,
+00013e70: 2078 665f 7361 6d70 6c65 2c20 6666 7474   xf_sample, fftt
+00013e80: 6f74 616c 5f73 616d 706c 650d 0a20 2020  otal_sample..   
+00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ea0: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
+00013eb0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00013ec0: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
+00013ed0: 655f 6964 5d20 3d20 2063 7572 7265 6e74  e_id] =  current
+00013ee0: 5f74 696d 652c 2063 7572 7265 6e74 5f63  _time, current_c
+00013ef0: 6c75 7374 6572 5f63 6c61 7373 2c20 6375  luster_class, cu
+00013f00: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
+00013f10: 6173 735f 7363 6f72 650d 0a20 2020 2020  ass_score..     
+00013f20: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00013f30: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
+00013f40: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
+00013f50: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00013f60: 5d20 3d20 6375 7272 656e 745f 7469 6d65  ] = current_time
+00013f70: 2c20 6375 7272 656e 745f 7a2c 2063 7572  , current_z, cur
+00013f80: 7265 6e74 5f79 2c20 6375 7272 656e 745f  rent_y, current_
+00013f90: 782c 2063 7572 7265 6e74 5f72 6164 6975  x, current_radiu
+00013fa0: 732c 2063 7572 7265 6e74 5f76 6f6c 756d  s, current_volum
+00013fb0: 652c 2063 7572 7265 6e74 5f65 6363 656e  e, current_eccen
+00013fc0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00013fd0: 7374 2c20 6375 7272 656e 745f 6563 6365  st, current_ecce
+00013fe0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+00013ff0: 636f 6e64 2c20 6375 7272 656e 745f 7375  cond, current_su
+00014000: 7266 6163 655f 6172 6561 2c20 6375 7272  rface_area, curr
+00014010: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
+00014020: 732c 2063 7572 7265 6e74 5f63 6c75 7374  s, current_clust
+00014030: 6572 5f63 6c61 7373 5f73 636f 7265 0d0a  er_class_score..
+00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014050: 2020 2075 6e69 7175 655f 6479 6e61 6d69     unique_dynami
+00014060: 635f 7072 6f70 6572 7469 6573 5f74 7261  c_properties_tra
+00014070: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00014080: 6971 7565 5f69 645d 203d 2063 7572 7265  ique_id] = curre
+00014090: 6e74 5f74 696d 652c 2063 7572 7265 6e74  nt_time, current
+000140a0: 5f73 7065 6564 2c20 6375 7272 656e 745f  _speed, current_
+000140b0: 6d6f 7469 6f6e 5f61 6e67 6c65 2c20 6375  motion_angle, cu
+000140c0: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
+000140d0: 6f6e 2c20 6375 7272 656e 745f 6469 7374  on, current_dist
+000140e0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+000140f0: 6375 7272 656e 745f 7261 6469 616c 5f61  current_radial_a
+00014100: 6e67 6c65 2c20 6375 7272 656e 745f 6365  ngle, current_ce
+00014110: 6c6c 5f61 7869 735f 6d61 736b 0d0a 2020  ll_axis_mask..  
+00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014130: 2073 656c 662e 756e 6971 7565 5f66 6674   self.unique_fft
+00014140: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
+00014150: 6b5f 6964 5d2e 7570 6461 7465 287b 6375  k_id].update({cu
+00014160: 7272 656e 745f 756e 6971 7565 5f69 643a  rrent_unique_id:
+00014170: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
+00014180: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
+00014190: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+000141a0: 5d7d 290d 0a20 2020 2020 2020 2020 2020  ]})..           
+000141b0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000141c0: 7175 655f 636c 7573 7465 725f 7072 6f70  que_cluster_prop
+000141d0: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
+000141e0: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
+000141f0: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
+00014200: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
+00014210: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
+00014220: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
+00014230: 7d29 0d0a 0d0a 2020 2020 2020 2020 2020  })....          
+00014240: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00014250: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
+00014260: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
+00014270: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
+00014280: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
+00014290: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+000142a0: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+000142b0: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
+000142c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000142d0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000142e0: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
+000142f0: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
+00014300: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
+00014310: 7175 655f 6964 3a75 6e69 7175 655f 6479  que_id:unique_dy
+00014320: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
+00014330: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00014340: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
+00014350: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014370: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
+00014380: 6469 6374 5f75 7064 6174 6528 7365 6c66  dict_update(self
+00014390: 2c20 756e 6971 7565 5f74 7261 636b 6c65  , unique_trackle
+000143a0: 745f 6964 733a 204c 6973 742c 2020 6365  t_ids: List,  ce
+000143b0: 6c6c 5f69 643a 2069 6e74 2c20 7472 6163  ll_id: int, trac
+000143c0: 6b5f 6964 3a20 696e 742c 2073 6f75 7263  k_id: int, sourc
+000143d0: 655f 6964 3a20 696e 742c 2074 6172 6765  e_id: int, targe
+000143e0: 745f 6964 3a20 696e 7429 3a0d 0a0d 0a20  t_id: int):.... 
+000143f0: 0d0a 2020 2020 2020 2020 6765 6e65 7261  ..        genera
+00014400: 7469 6f6e 5f69 6420 3d20 7365 6c66 2e67  tion_id = self.g
+00014410: 656e 6572 6174 696f 6e5f 6469 6374 5b63  eneration_dict[c
+00014420: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
+00014430: 2074 7261 636b 6c65 745f 6964 203d 2073   tracklet_id = s
+00014440: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
+00014450: 745b 6365 6c6c 5f69 645d 0d0a 0d0a 2020  t[cell_id]....  
+00014460: 2020 2020 2020 756e 6971 7565 5f69 6420        unique_id 
+00014470: 3d20 7374 7228 7472 6163 6b5f 6964 2920  = str(track_id) 
+00014480: 2b20 7374 7228 7365 6c66 2e6d 6178 5f74  + str(self.max_t
+00014490: 7261 636b 5f69 6429 202b 2073 7472 2867  rack_id) + str(g
+000144a0: 656e 6572 6174 696f 6e5f 6964 2920 2b20  eneration_id) + 
+000144b0: 7374 7228 7472 6163 6b6c 6574 5f69 6429  str(tracklet_id)
+000144c0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000144d0: 2020 2020 7665 635f 6d61 736b 203d 205b      vec_mask = [
+000144e0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+000144f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014500: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014510: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00014520: 645f 785f 6b65 795d 292c 2066 6c6f 6174  d_x_key]), float
+00014530: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014540: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014550: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00014560: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
+00014570: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
+00014580: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014590: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+000145a0: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
+000145b0: 656e 7472 6f69 645f 7a5f 6b65 795d 2920  entroid_z_key]) 
+000145c0: 5d0d 0a0d 0a20 2020 2020 2020 2076 6563  ]....        vec
+000145d0: 5f63 656c 6c20 3d20 5b66 6c6f 6174 2873  _cell = [float(s
+000145e0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000145f0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014600: 656c 6c5f 6964 295d 5b73 656c 662e 7870  ell_id)][self.xp
+00014610: 6f73 6964 5f6b 6579 5d29 202c 200d 0a20  osid_key]) , .. 
+00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014630: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00014640: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014650: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014660: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00014670: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
+00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014690: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+000146a0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+000146b0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000146c0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+000146d0: 2e7a 706f 7369 645f 6b65 795d 295d 0d0a  .zposid_key])]..
+000146e0: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
+000146f0: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
+00014700: 2876 6563 5f6d 6173 6b2c 2076 6563 5f63  (vec_mask, vec_c
+00014710: 656c 6c29 0d0a 0d0a 2020 2020 2020 2020  ell)....        
+00014720: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014730: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014740: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00014750: 287b 7365 6c66 2e72 6164 6961 6c5f 616e  ({self.radial_an
+00014760: 676c 655f 6b65 7920 3a20 616e 676c 657d  gle_key : angle}
+00014770: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+00014780: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00014790: 2075 6e69 7175 655f 7472 6163 6b6c 6574   unique_tracklet
+000147a0: 5f69 6473 2e61 7070 656e 6428 7374 7228  _ids.append(str(
+000147b0: 756e 6971 7565 5f69 6429 290d 0a20 2020  unique_id))..   
+000147c0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000147d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000147e0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+000147f0: 7064 6174 6528 7b73 656c 662e 636c 7573  pdate({self.clus
+00014800: 7465 7263 6c61 7373 5f6b 6579 203a 204e  terclass_key : N
+00014810: 6f6e 657d 290d 0a20 2020 2020 2020 2073  one})..        s
+00014820: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014830: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014840: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00014850: 7b73 656c 662e 636c 7573 7465 7273 636f  {self.clustersco
+00014860: 7265 5f6b 6579 203a 2030 7d29 0d0a 2020  re_key : 0})..  
+00014870: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00014880: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014890: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000148a0: 7570 6461 7465 287b 7365 6c66 2e75 6e69  update({self.uni
+000148b0: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
+000148c0: 756e 6971 7565 5f69 6429 7d29 0d0a 2020  unique_id)})..  
+000148d0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000148e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000148f0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00014900: 7570 6461 7465 287b 7365 6c66 2e74 7261  update({self.tra
+00014910: 636b 6c65 7469 645f 6b65 7920 3a20 7374  ckletid_key : st
+00014920: 7228 7472 6163 6b6c 6574 5f69 6429 7d29  r(tracklet_id)})
+00014930: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+00014940: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014950: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014960: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00014970: 662e 6765 6e65 7261 7469 6f6e 6964 5f6b  f.generationid_k
+00014980: 6579 203a 2073 7472 2867 656e 6572 6174  ey : str(generat
+00014990: 696f 6e5f 6964 297d 2920 0d0a 2020 2020  ion_id)}) ..    
+000149a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000149b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000149c0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000149d0: 6461 7465 287b 7365 6c66 2e74 7261 636b  date({self.track
+000149e0: 6964 5f6b 6579 203a 2073 7472 2874 7261  id_key : str(tra
+000149f0: 636b 5f69 6429 7d29 0d0a 2020 2020 2020  ck_id)})..      
+00014a00: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00014a10: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014a20: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00014a30: 7465 287b 7365 6c66 2e6d 6f74 696f 6e5f  te({self.motion_
+00014a40: 616e 676c 655f 6b65 7920 3a20 302e 307d  angle_key : 0.0}
+00014a50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00014a60: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014a70: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014a80: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00014a90: 662e 7370 6565 645f 6b65 7920 3a20 302e  f.speed_key : 0.
+00014aa0: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
+00014ab0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014ac0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014ad0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00014ae0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+00014af0: 5f6b 6579 203a 2030 2e30 7d29 0d0a 2020  _key : 0.0})..  
+00014b00: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00014b10: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014b20: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00014b30: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
+00014b40: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00014b50: 6972 7374 6b65 7920 3a20 4e6f 6e65 7d29  irstkey : None})
+00014b60: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00014b70: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014b80: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014b90: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014ba0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00014bb0: 6d70 5f73 6563 6f6e 646b 6579 203a 204e  mp_secondkey : N
+00014bc0: 6f6e 657d 290d 0a20 2020 2020 2020 2073  one})..        s
+00014bd0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014be0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014bf0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00014c00: 7b73 656c 662e 7375 7266 6163 655f 6172  {self.surface_ar
+00014c10: 6561 5f6b 6579 203a 204e 6f6e 657d 290d  ea_key : None}).
+00014c20: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00014c30: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014c40: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014c50: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00014c60: 6365 6c6c 6178 6973 5f6d 6173 6b5f 6b65  cellaxis_mask_ke
+00014c70: 7920 3a20 4e6f 6e65 7d29 0d0a 0d0a 2020  y : None})....  
+00014c80: 2020 2020 2020 6966 2073 6f75 7263 655f        if source_
+00014c90: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0d  id is not None:.
+00014ca0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014cb0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014cc0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014cd0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00014ce0: 656c 662e 6265 666f 7265 6964 5f6b 6579  elf.beforeid_key
+00014cf0: 203a 2069 6e74 2873 6f75 7263 655f 6964   : int(source_id
+00014d00: 297d 290d 0a20 2020 2020 2020 2020 2020  )})..           
+00014d10: 2076 6563 5f31 203d 205b 666c 6f61 7428   vec_1 = [float(
+00014d20: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014d30: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014d40: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
+00014d50: 706f 7369 645f 6b65 795d 2920 2d20 666c  posid_key]) - fl
+00014d60: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014d70: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014d80: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
+00014d90: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+00014da0: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
+00014db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014dc0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00014dd0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014de0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00014df0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00014e00: 5d29 202d 2066 6c6f 6174 2873 656c 662e  ]) - float(self.
+00014e10: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014e20: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
+00014e30: 655f 6964 295d 5b73 656c 662e 7970 6f73  e_id)][self.ypos
+00014e40: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
+00014e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e60: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
+00014e70: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014e80: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014e90: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
+00014ea0: 7369 645f 6b65 795d 2920 2d20 2066 6c6f  sid_key]) -  flo
+00014eb0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014ec0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014ed0: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
+00014ee0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00014ef0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+00014f00: 7065 6564 203d 206e 702e 7371 7274 286e  peed = np.sqrt(n
+00014f10: 702e 646f 7428 7665 635f 312c 2076 6563  p.dot(vec_1, vec
+00014f20: 5f31 2929 2f73 656c 662e 7463 616c 6962  _1))/self.tcalib
+00014f30: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+00014f40: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014f50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014f60: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00014f70: 6461 7465 287b 7365 6c66 2e73 7065 6564  date({self.speed
+00014f80: 5f6b 6579 203a 2073 7065 6564 7d29 0d0a  _key : speed})..
+00014f90: 0d0a 2020 2020 2020 2020 2020 2020 6d6f  ..            mo
+00014fa0: 7469 6f6e 5f61 6e67 6c65 203d 2061 6e67  tion_angle = ang
+00014fb0: 756c 6172 5f63 6861 6e67 6528 7665 635f  ular_change(vec_
+00014fc0: 6d61 736b 2c20 7665 635f 3129 0d0a 0d0a  mask, vec_1)....
+00014fd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014fe0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014ff0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015000: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015010: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
+00015020: 6b65 7920 3a20 6d6f 7469 6f6e 5f61 6e67  key : motion_ang
+00015030: 6c65 7d29 200d 0a0d 0a20 2020 2020 2020  le}) ....       
+00015040: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
+00015050: 6420 696e 2073 656c 662e 6564 6765 5f73  d in self.edge_s
+00015060: 6f75 7263 655f 6c6f 6f6b 7570 3a0d 0a20  ource_lookup:.. 
+00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015080: 2020 2070 7265 5f73 6f75 7263 655f 6964     pre_source_id
+00015090: 203d 2073 656c 662e 6564 6765 5f73 6f75   = self.edge_sou
+000150a0: 7263 655f 6c6f 6f6b 7570 5b73 6f75 7263  rce_lookup[sourc
+000150b0: 655f 6964 5d0d 0a20 2020 2020 2020 2020  e_id]..         
+000150c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150e0: 2076 6563 5f32 203d 205b 666c 6f61 7428   vec_2 = [float(
+000150f0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015100: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015110: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
+00015120: 706f 7369 645f 6b65 795d 2920 2d20 3220  posid_key]) - 2 
+00015130: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
+00015140: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015150: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
+00015160: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00015170: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
+00015180: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015190: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
+000151a0: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
+000151b0: 6c66 2e78 706f 7369 645f 6b65 795d 292c  lf.xposid_key]),
+000151c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000151d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000151e0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000151f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015200: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00015210: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+00015220: 202d 2032 202a 2066 6c6f 6174 2873 656c   - 2 * float(sel
+00015230: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015240: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
+00015250: 7263 655f 6964 295d 5b73 656c 662e 7970  rce_id)][self.yp
+00015260: 6f73 6964 5f6b 6579 5d29 202b 2066 6c6f  osid_key]) + flo
+00015270: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015280: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015290: 6e74 2870 7265 5f73 6f75 7263 655f 6964  nt(pre_source_id
+000152a0: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
+000152b0: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
+000152c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152d0: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
+000152e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000152f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015300: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
+00015310: 6b65 795d 2920 2d20 2032 202a 2066 6c6f  key]) -  2 * flo
+00015320: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015330: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015340: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
+00015350: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00015360: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
+00015370: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015380: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
+00015390: 7263 655f 6964 295d 5b73 656c 662e 7a70  rce_id)][self.zp
+000153a0: 6f73 6964 5f6b 6579 5d29 5d0d 0a20 2020  osid_key])]..   
+000153b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153c0: 2061 6363 203d 206e 702e 7371 7274 286e   acc = np.sqrt(n
+000153d0: 702e 646f 7428 7665 635f 322c 2076 6563  p.dot(vec_2, vec
+000153e0: 5f32 2929 2f73 656c 662e 7463 616c 6962  _2))/self.tcalib
+000153f0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+00015400: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015420: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00015430: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015440: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00015450: 7465 287b 7365 6c66 2e61 6363 656c 6572  te({self.acceler
+00015460: 6174 696f 6e5f 6b65 7920 3a20 6163 637d  ation_key : acc}
+00015470: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+00015480: 736f 7572 6365 5f69 6420 6973 204e 6f6e  source_id is Non
+00015490: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000154a0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000154b0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000154c0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+000154d0: 287b 7365 6c66 2e62 6566 6f72 6569 645f  ({self.beforeid_
+000154e0: 6b65 7920 3a20 4e6f 6e65 7d29 200d 0a20  key : None}) .. 
+000154f0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00015500: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+00015510: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00015520: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00015530: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015540: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015550: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015560: 7064 6174 6528 7b73 656c 662e 6166 7465  pdate({self.afte
+00015570: 7269 645f 6b65 7920 3a20 696e 7428 7461  rid_key : int(ta
+00015580: 7267 6574 5f69 6429 7d29 200d 0a20 2020  rget_id)}) ..   
+00015590: 2020 2020 2065 6c69 6620 7461 7267 6574       elif target
+000155a0: 5f69 6420 6973 204e 6f6e 653a 0d0a 2020  _id is None:..  
+000155b0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+000155c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000155d0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000155e0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+000155f0: 2e61 6674 6572 6964 5f6b 6579 203a 204e  .afterid_key : N
+00015600: 6f6e 657d 290d 0a20 2020 2020 2020 2020  one})..         
+00015610: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00015620: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015640: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00015650: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00015660: 2020 2020 6465 6620 5f74 656d 706f 7261      def _tempora
+00015670: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
+00015680: 6528 7365 6c66 293a 0d0a 2020 2020 0d0a  e(self):..    ..
+00015690: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+000156a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000156b0: 2e41 7474 7220 3d20 7b7d 0d0a 2020 2020  .Attr = {}..    
+000156c0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+000156d0: 7474 696d 6520 3d20 696e 7428 6d69 6e28  ttime = int(min(
+000156e0: 7365 6c66 2e41 6c6c 5661 6c75 6573 5b73  self.AllValues[s
+000156f0: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+00015700: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00015710: 2020 2020 656e 6474 696d 6520 3d20 696e      endtime = in
+00015720: 7428 6d61 7828 7365 6c66 2e41 6c6c 5661  t(max(self.AllVa
+00015730: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
+00015740: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
+00015750: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00015760: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015770: 662e 7469 6d65 203d 205b 5d0d 0a20 2020  f.time = []..   
+00015780: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015790: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+000157a0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
+000157b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000157c0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+000157d0: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
+000157e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000157f0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00015800: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
+00015810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015820: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00015830: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+00015840: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015850: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00015860: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00015870: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015880: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00015890: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
+000158a0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000158b0: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
+000158c0: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+000158d0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+000158e0: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+000158f0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015900: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015910: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
+00015920: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015930: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015940: 7469 635f 7661 725f 7370 6565 6420 3d20  tic_var_speed = 
 00015950: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
 00015960: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00015970: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
-00015980: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015990: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000159a0: 635f 7661 725f 7261 6469 7573 203d 205b  c_var_radius = [
-000159b0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000159c0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000159d0: 635f 6d65 616e 5f73 7065 6564 203d 205b  c_mean_speed = [
-000159e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000159f0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00015a00: 7661 725f 7370 6565 6420 3d20 5b5d 0d0a  var_speed = []..
-00015a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015a20: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00015a30: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
-00015a40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015a50: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f61  lf.mitotic_var_a
-00015a60: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-00015a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015a80: 6d69 746f 7469 635f 6d65 616e 5f64 6972  mitotic_mean_dir
-00015a90: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00015aa0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015ab0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00015ac0: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
-00015ad0: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00015ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015af0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00015b00: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00015b10: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00015b20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015b30: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00015b40: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00015b50: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015b60: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00015b70: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-00015b80: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-00015b90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015ba0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00015bb0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
-00015bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015bd0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015be0: 5f6d 6561 6e5f 6469 7370 5f79 203d 205b  _mean_disp_y = [
-00015bf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015c00: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015c10: 7469 635f 7661 725f 6469 7370 5f79 203d  tic_var_disp_y =
-00015c20: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015c30: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015c40: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00015c50: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00015c60: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015c70: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00015c80: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
-00015c90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015ca0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00015cb0: 6561 6e5f 7261 6469 7573 203d 205b 5d0d  ean_radius = [].
-00015cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015cd0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015ce0: 635f 7661 725f 7261 6469 7573 203d 205b  c_var_radius = [
-00015cf0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00015d00: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00015d10: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-00015d20: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015d30: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015d40: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
-00015d50: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
-00015d60: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015d70: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00015d80: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
-00015d90: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015da0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f61  on_mitotic_var_a
-00015db0: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-00015dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015dd0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00015de0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00015df0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00015e00: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015e10: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00015e20: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00015e30: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
-00015e40: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015e50: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00015e60: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00015e70: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-00015e80: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00015e90: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00015ea0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00015eb0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015ec0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00015ed0: 6c5f 6d65 616e 5f64 6973 705f 7a20 3d20  l_mean_disp_z = 
-00015ee0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00015ef0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00015f00: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 0d0a  _disp_z = []....
-00015f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f20: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00015f30: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00015f40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015f50: 616c 6c5f 7661 725f 6469 7370 5f79 203d  all_var_disp_y =
-00015f60: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015f70: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00015f80: 6d65 616e 5f64 6973 705f 7820 3d20 5b5d  mean_disp_x = []
-00015f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015fa0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00015fb0: 6973 705f 7820 3d20 5b5d 0d0a 0d0a 2020  isp_x = []....  
-00015fc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015fd0: 6c66 2e61 6c6c 5f6d 6561 6e5f 7261 6469  lf.all_mean_radi
-00015fe0: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-00015ff0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00016000: 6c5f 7661 725f 7261 6469 7573 203d 205b  l_var_radius = [
-00016010: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016020: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00016030: 616e 5f73 7065 6564 203d 205b 5d0d 0a20  an_speed = [].. 
-00016040: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016050: 656c 662e 616c 6c5f 7661 725f 7370 6565  elf.all_var_spee
-00016060: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 2020  d = []....      
-00016070: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00016080: 6c6c 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ll_mean_acc = []
-00016090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000160a0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f61    self.all_var_a
-000160b0: 6363 203d 205b 5d0d 0a0d 0a20 2020 2020  cc = []....     
-000160c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000160d0: 616c 6c5f 6d65 616e 5f64 6972 6563 7469  all_mean_directi
-000160e0: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-000160f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016100: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00016110: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00016120: 6520 3d20 5b5d 0d0a 0d0a 2020 2020 2020  e = []....      
-00016130: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00016140: 6c6c 5f6d 6561 6e5f 6469 7374 616e 6365  ll_mean_distance
-00016150: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00016160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016170: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00016180: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00016190: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000161a0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000161b0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-000161c0: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-000161d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000161e0: 6f6e 5f6d 6974 6f74 6963 5f63 6c75 7374  on_mitotic_clust
-000161f0: 6572 5f63 6c61 7373 203d 205b 5d0d 0a20  er_class = [].. 
-00016200: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016210: 656c 662e 616c 6c5f 636c 7573 7465 725f  elf.all_cluster_
-00016220: 636c 6173 7320 3d20 5b5d 0d0a 0d0a 2020  class = []....  
-00016230: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00016240: 6c5f 7370 6f74 735f 7472 6163 6b73 203d  l_spots_tracks =
-00016250: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00016260: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-00016270: 6e20 7365 6c66 2e75 6e69 7175 655f 7370  n self.unique_sp
-00016280: 6f74 5f70 726f 7065 7274 6965 732e 6974  ot_properties.it
-00016290: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-000162a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000162b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162c0: 2020 2020 2020 616c 6c5f 7370 6f74 7320        all_spots 
-000162d0: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
-000162e0: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
-000162f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016300: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00016310: 7472 6163 6b69 645f 6b65 7920 696e 2061  trackid_key in a
-00016320: 6c6c 5f73 706f 7473 3a0d 0a20 2020 2020  ll_spots:..     
-00016330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016340: 2020 2020 2061 6c6c 5f73 706f 7473 5f74       all_spots_t
-00016350: 7261 636b 735b 6b5d 203d 2061 6c6c 5f73  racks[k] = all_s
-00016360: 706f 7473 0d0a 2020 2020 2020 2020 2020  pots..          
-00016370: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00016380: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00016390: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-000163a0: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
-000163b0: 2020 2020 2020 2020 2020 7769 7468 2063            with c
-000163c0: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-000163d0: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
-000163e0: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
-000163f0: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
-00016400: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
-00016410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016420: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00016430: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00016440: 2069 2069 6e20 7471 646d 2872 616e 6765   i in tqdm(range
-00016450: 2873 7461 7274 7469 6d65 2c20 656e 6474  (starttime, endt
-00016460: 696d 6529 2c20 746f 7461 6c3d 656e 6474  ime), total=endt
-00016470: 696d 6520 2d20 7374 6172 7474 696d 6529  ime - starttime)
-00016480: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016490: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000164a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164b0: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
-000164c0: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
-000164d0: 7428 7365 6c66 2e5f 636f 6d70 7574 655f  t(self._compute_
-000164e0: 7465 6d70 6f72 616c 2c20 692c 2061 6c6c  temporal, i, all
-000164f0: 5f73 706f 7473 5f74 7261 636b 7329 290d  _spots_tracks)).
-00016500: 0a20 0d0a 2020 2020 2020 2020 2020 2020  . ..            
-00016510: 2020 2020 2020 2020 5b72 2e72 6573 756c          [r.resul
-00016520: 7428 2920 666f 7220 7220 696e 2063 6f6e  t() for r in con
-00016530: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-00016540: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-00016550: 7572 6573 295d 0d0a 0d0a 0d0a 2020 2020  ures)]......    
-00016560: 6465 6620 5f63 6f6d 7075 7465 5f74 656d  def _compute_tem
-00016570: 706f 7261 6c28 7365 6c66 2c20 692c 2061  poral(self, i, a
-00016580: 6c6c 5f73 706f 7473 5f74 7261 636b 7329  ll_spots_tracks)
-00016590: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
-000165a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000165b0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-000165c0: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-000165d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165e0: 6d69 746f 7469 635f 6469 7370 5f79 203d  mitotic_disp_y =
-000165f0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016600: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016610: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00016620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016630: 2020 6d69 746f 7469 635f 7261 6469 7573    mitotic_radius
-00016640: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016650: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016660: 6963 5f73 7065 6564 203d 205b 5d0d 0a20  ic_speed = [].. 
-00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016680: 2020 206d 6974 6f74 6963 5f61 6363 203d     mitotic_acc =
-00016690: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000166a0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-000166b0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000166c0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-000166d0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000166e0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-000166f0: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-00016700: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016710: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-00016720: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
-00016730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016740: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016750: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00016760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016770: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00016780: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00016790: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000167a0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-000167b0: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
+00015970: 6963 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ic_mean_acc = []
+00015980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015990: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+000159a0: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+000159b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000159c0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+000159d0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000159e0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+000159f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015a00: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
+00015a10: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+00015a20: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015a30: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015a40: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
+00015a50: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00015a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015a70: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00015a80: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00015a90: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+00015aa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015ab0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00015ac0: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
+00015ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ae0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00015af0: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
+00015b00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015b10: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00015b20: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
+00015b30: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015b40: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015b50: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00015b60: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+00015b70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015b80: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00015b90: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+00015ba0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015bb0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00015bc0: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
+00015bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015be0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015bf0: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
+00015c00: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00015c10: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00015c20: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+00015c30: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015c40: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015c50: 6e5f 6d69 746f 7469 635f 6d65 616e 5f73  n_mitotic_mean_s
+00015c60: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
+00015c70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015c80: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00015c90: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
+00015ca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015cb0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00015cc0: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
+00015cd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015ce0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00015cf0: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+00015d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015d10: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00015d20: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+00015d30: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
+00015d40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015d50: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00015d60: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+00015d70: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
+00015d80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015d90: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00015da0: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
+00015db0: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
+00015dc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015dd0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00015de0: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00015df0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+00015e00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015e10: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+00015e20: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
+00015e30: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00015e40: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
+00015e50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015e60: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+00015e70: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
+00015e80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015e90: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+00015ea0: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+00015eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015ec0: 616c 6c5f 6d65 616e 5f64 6973 705f 7820  all_mean_disp_x 
+00015ed0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015ee0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00015ef0: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
+00015f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015f10: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00015f20: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00015f30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015f40: 662e 616c 6c5f 7661 725f 7261 6469 7573  f.all_var_radius
+00015f50: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015f60: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00015f70: 6c5f 6d65 616e 5f73 7065 6564 203d 205b  l_mean_speed = [
+00015f80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015f90: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00015fa0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
+00015fb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015fc0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 6320  lf.all_mean_acc 
+00015fd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015fe0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00015ff0: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+00016000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016010: 656c 662e 616c 6c5f 6d65 616e 5f64 6972  elf.all_mean_dir
+00016020: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+00016030: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016040: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00016050: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+00016060: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
+00016070: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016080: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
+00016090: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+000160a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000160b0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+000160c0: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+000160d0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+000160e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000160f0: 662e 6d69 746f 7469 635f 636c 7573 7465  f.mitotic_cluste
+00016100: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
+00016110: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016120: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f63  lf.non_mitotic_c
+00016130: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
+00016140: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016150: 2020 2073 656c 662e 616c 6c5f 636c 7573     self.all_clus
+00016160: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
+00016170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016180: 2020 616c 6c5f 7370 6f74 735f 7472 6163    all_spots_trac
+00016190: 6b73 203d 207b 7d0d 0a20 2020 2020 2020  ks = {}..       
+000161a0: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
+000161b0: 7629 2069 6e20 7365 6c66 2e75 6e69 7175  v) in self.uniqu
+000161c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000161d0: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00016200: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
+00016210: 6f74 7320 3d20 7365 6c66 2e75 6e69 7175  ots = self.uniqu
+00016220: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016230: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
+00016240: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00016250: 656c 662e 7472 6163 6b69 645f 6b65 7920  elf.trackid_key 
+00016260: 696e 2061 6c6c 5f73 706f 7473 3a0d 0a20  in all_spots:.. 
+00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016280: 2020 2020 2020 2020 2061 6c6c 5f73 706f           all_spo
+00016290: 7473 5f74 7261 636b 735b 6b5d 203d 2061  ts_tracks[k] = a
+000162a0: 6c6c 5f73 706f 7473 0d0a 2020 2020 2020  ll_spots..      
+000162b0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+000162c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000162d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162e0: 6675 7475 7265 7320 3d20 5b5d 0d0a 2020  futures = []..  
+000162f0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00016300: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
+00016310: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
+00016320: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
+00016330: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
+00016340: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
+00016350: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+00016360: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00016370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016380: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
+00016390: 616e 6765 2873 7461 7274 7469 6d65 2c20  ange(starttime, 
+000163a0: 656e 6474 696d 6529 2c20 746f 7461 6c3d  endtime), total=
+000163b0: 656e 6474 696d 6520 2d20 7374 6172 7474  endtime - startt
+000163c0: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
+000163d0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000163e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163f0: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
+00016400: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
+00016410: 7562 6d69 7428 7365 6c66 2e5f 636f 6d70  ubmit(self._comp
+00016420: 7574 655f 7465 6d70 6f72 616c 2c20 692c  ute_temporal, i,
+00016430: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00016440: 7329 290d 0a20 0d0a 2020 2020 2020 2020  s)).. ..        
+00016450: 2020 2020 2020 2020 2020 2020 5b72 2e72              [r.r
+00016460: 6573 756c 7428 2920 666f 7220 7220 696e  esult() for r in
+00016470: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+00016480: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
+00016490: 2866 7574 7572 6573 295d 0d0a 0d0a 0d0a  (futures)]......
+000164a0: 2020 2020 6465 6620 5f63 6f6d 7075 7465      def _compute
+000164b0: 5f74 656d 706f 7261 6c28 7365 6c66 2c20  _temporal(self, 
+000164c0: 692c 2061 6c6c 5f73 706f 7473 5f74 7261  i, all_spots_tra
+000164d0: 636b 7329 3a20 2020 2020 2020 2020 2020  cks):           
+000164e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000164f0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016500: 6963 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ic_disp_z = []..
+00016510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016520: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00016530: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00016540: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016550: 6f74 6963 5f64 6973 705f 7820 3d20 5b5d  otic_disp_x = []
+00016560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016570: 2020 2020 2020 6d69 746f 7469 635f 7261        mitotic_ra
+00016580: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
+00016590: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000165a0: 6974 6f74 6963 5f73 7065 6564 203d 205b  itotic_speed = [
+000165b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000165c0: 2020 2020 2020 206d 6974 6f74 6963 5f61         mitotic_a
+000165d0: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
+000165e0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+000165f0: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
+00016600: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
+00016610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016620: 2020 6d69 746f 7469 635f 636c 7573 7465    mitotic_cluste
+00016630: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
+00016640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016650: 2020 6d69 746f 7469 635f 6469 7374 616e    mitotic_distan
+00016660: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+00016670: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00016680: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016690: 6f74 6963 5f64 6973 705f 7a20 3d20 5b5d  otic_disp_z = []
+000166a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000166b0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+000166c0: 635f 6469 7370 5f79 203d 205b 5d0d 0a20  c_disp_y = [].. 
+000166d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166e0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+000166f0: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
+00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016710: 6e6f 6e5f 6d69 746f 7469 635f 7261 6469  non_mitotic_radi
+00016720: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+00016730: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00016740: 5f6d 6974 6f74 6963 5f73 7065 6564 203d  _mitotic_speed =
+00016750: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016760: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016770: 6f74 6963 5f61 6363 203d 205b 5d0d 0a20  otic_acc = [].. 
+00016780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016790: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+000167a0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+000167b0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
 000167c0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000167d0: 6d69 746f 7469 635f 7261 6469 7573 203d  mitotic_radius =
-000167e0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000167f0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00016800: 6f74 6963 5f73 7065 6564 203d 205b 5d0d  otic_speed = [].
-00016810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016820: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016830: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00016840: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016850: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
-00016860: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00016870: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016880: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00016890: 7469 635f 636c 7573 7465 725f 636c 6173  tic_cluster_clas
-000168a0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-000168b0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000168c0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-000168d0: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-000168e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000168f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00016900: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00016910: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-00016920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016930: 616c 6c5f 6469 7370 5f79 203d 205b 5d0d  all_disp_y = [].
-00016940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016950: 2020 2020 2061 6c6c 5f64 6973 705f 7820       all_disp_x 
-00016960: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016970: 2020 2020 2020 2020 2020 616c 6c5f 7261            all_ra
-00016980: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-00016990: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000169a0: 6c6c 5f73 7065 6564 203d 205b 5d0d 0a20  ll_speed = [].. 
-000169b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169c0: 2020 2061 6c6c 5f61 6363 203d 205b 5d0d     all_acc = [].
-000169d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000169e0: 2020 2020 2061 6c6c 5f64 6972 6563 7469       all_directi
-000169f0: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00016a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016a10: 2020 2020 2020 616c 6c5f 636c 7573 7465        all_cluste
-00016a20: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
-00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a40: 2020 616c 6c5f 6469 7374 616e 6365 5f63    all_distance_c
-00016a50: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
-00016a60: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
-00016a70: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-00016a80: 6b2c 7629 2069 6e20 616c 6c5f 7370 6f74  k,v) in all_spot
-00016a90: 735f 7472 6163 6b73 2e69 7465 6d73 2829  s_tracks.items()
-00016aa0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016ab0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00016ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ad0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00016ae0: 7265 6e74 5f74 696d 6520 3d20 616c 6c5f  rent_time = all_
-00016af0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00016b00: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00016b10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016b20: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016b30: 6974 6f74 6963 203d 2061 6c6c 5f73 706f  itotic = all_spo
-00016b40: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00016b50: 662e 6469 7669 6469 6e67 5f6b 6579 5d0d  f.dividing_key].
-00016b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016b70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00016b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b90: 2020 2020 2020 2020 2020 6966 2069 203d            if i =
-00016ba0: 3d20 696e 7428 6375 7272 656e 745f 7469  = int(current_ti
-00016bb0: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
-00016bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bd0: 2020 2020 2020 2020 6966 206d 6974 6f74          if mitot
-00016be0: 6963 3a0d 0a20 2020 2020 2020 2020 2020  ic:..           
-00016bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c00: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016c10: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
-00016c20: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00016c30: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
-00016c40: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167d0: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+000167e0: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
+000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016800: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
+00016810: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00016820: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016830: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00016840: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00016850: 6c6c 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ll_disp_z = []..
+00016860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016870: 2020 2020 616c 6c5f 6469 7370 5f79 203d      all_disp_y =
+00016880: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016890: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+000168a0: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+000168b0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+000168c0: 6c5f 7261 6469 7573 203d 205b 5d0d 0a20  l_radius = [].. 
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168e0: 2020 2061 6c6c 5f73 7065 6564 203d 205b     all_speed = [
+000168f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016900: 2020 2020 2020 2061 6c6c 5f61 6363 203d         all_acc =
+00016910: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016920: 2020 2020 2020 2020 2061 6c6c 5f64 6972           all_dir
+00016930: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+00016940: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016950: 2020 2020 2020 2020 2020 616c 6c5f 636c            all_cl
+00016960: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
+00016970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016980: 2020 2020 2020 616c 6c5f 6469 7374 616e        all_distan
+00016990: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+000169a0: 5d0d 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020  ]..........     
+000169b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000169c0: 6f72 2028 6b2c 7629 2069 6e20 616c 6c5f  or (k,v) in all_
+000169d0: 7370 6f74 735f 7472 6163 6b73 2e69 7465  spots_tracks.ite
+000169e0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00016a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a20: 2063 7572 7265 6e74 5f74 696d 6520 3d20   current_time = 
+00016a30: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016a40: 5b6b 5d5b 7365 6c66 2e66 7261 6d65 6964  [k][self.frameid
+00016a50: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
+00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a70: 2020 206d 6974 6f74 6963 203d 2061 6c6c     mitotic = all
+00016a80: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00016a90: 5b73 656c 662e 6469 7669 6469 6e67 5f6b  [self.dividing_k
+00016aa0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+00016ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016ad0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016ae0: 2069 203d 3d20 696e 7428 6375 7272 656e   i == int(curren
+00016af0: 745f 7469 6d65 293a 0d0a 2020 2020 2020  t_time):..      
+00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b10: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00016b20: 6974 6f74 6963 3a0d 0a20 2020 2020 2020  itotic:..       
+00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b50: 206d 6974 6f74 6963 5f64 6973 705f 7a2e   mitotic_disp_z.
+00016b60: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00016b70: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00016b80: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
+00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bb0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016bc0: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
+00016bd0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00016be0: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+00016bf0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00016c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c10: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016c20: 6963 5f64 6973 705f 782e 6170 7065 6e64  ic_disp_x.append
+00016c30: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00016c40: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
+00016c50: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 00016c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c70: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
-00016c80: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00016c90: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00016ca0: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
-00016cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c80: 6d69 746f 7469 635f 7261 6469 7573 2e61  mitotic_radius.a
+00016c90: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00016ca0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e72  tracks[k][self.r
+00016cb0: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
 00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cd0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00016ce0: 6973 705f 782e 6170 7065 6e64 2861 6c6c  isp_x.append(all
-00016cf0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00016d00: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00016d10: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ce0: 2020 2020 206d 6974 6f74 6963 5f73 7065       mitotic_spe
+00016cf0: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
+00016d00: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00016d10: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
 00016d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d30: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00016d40: 7469 635f 7261 6469 7573 2e61 7070 656e  tic_radius.appen
-00016d50: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00016d60: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
-00016d70: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
-00016d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d40: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016d50: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
+00016d60: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00016d70: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+00016d80: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 00016d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016da0: 206d 6974 6f74 6963 5f73 7065 6564 2e61   mitotic_speed.a
-00016db0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00016dc0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
-00016dd0: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
-00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e00: 2020 2020 6d69 746f 7469 635f 6163 632e      mitotic_acc.
-00016e10: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00016e20: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00016e30: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-00016e40: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00016e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e60: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00016e70: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
-00016e80: 6368 616e 6765 2e61 7070 656e 6428 616c  change.append(al
-00016e90: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00016ea0: 5d5b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ][self.motion_an
-00016eb0: 676c 655f 6b65 795d 290d 0a20 2020 2020  gle_key])..     
-00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ee0: 2020 206d 6974 6f74 6963 5f64 6973 7461     mitotic_dista
-00016ef0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00016f00: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00016f10: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-00016f20: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00016f30: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f60: 6966 2073 656c 662e 636c 7573 7465 7263  if self.clusterc
-00016f70: 6c61 7373 5f6b 6579 2069 6e20 616c 6c5f  lass_key in all_
-00016f80: 7370 6f74 735f 7472 6163 6b73 5b6b 5d2e  spots_tracks[k].
-00016f90: 6b65 7973 2829 203a 0d0a 2020 2020 2020  keys() :..      
+00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016db0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+00016dc0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00016dd0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00016de0: 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74 696f  ks[k][self.motio
+00016df0: 6e5f 616e 676c 655f 6b65 795d 290d 0a20  n_angle_key]).. 
+00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e20: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00016e30: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00016e40: 6b2e 6170 7065 6e64 2861 6c6c 5f73 706f  k.append(all_spo
+00016e50: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00016e60: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+00016e70: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
+00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ea0: 2020 2020 6966 2073 656c 662e 636c 7573      if self.clus
+00016eb0: 7465 7263 6c61 7373 5f6b 6579 2069 6e20  terclass_key in 
+00016ec0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016ed0: 5b6b 5d2e 6b65 7973 2829 203a 0d0a 2020  [k].keys() :..  
+00016ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f00: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016f10: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
+00016f20: 7373 2e61 7070 656e 6428 616c 6c5f 7370  ss.append(all_sp
+00016f30: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00016f40: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
+00016f50: 6b65 795d 290d 0a0d 0a0d 0a20 2020 2020  key])......     
+00016f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016f80: 6e6f 7420 6d69 746f 7469 633a 0d0a 2020  not mitotic:..  
+00016f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fc0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016fd0: 5f63 6c75 7374 6572 5f63 6c61 7373 2e61  _cluster_class.a
-00016fe0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00016ff0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e63  tracks[k][self.c
-00017000: 6c75 7374 6572 636c 6173 735f 6b65 795d  lusterclass_key]
-00017010: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
-00017020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017030: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00017040: 6d69 746f 7469 633a 0d0a 2020 2020 2020  mitotic:..      
-00017050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fb0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00016fc0: 635f 6469 7370 5f7a 2e61 7070 656e 6428  c_disp_z.append(
+00016fd0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016fe0: 5b6b 5d5b 7365 6c66 2e7a 706f 7369 645f  [k][self.zposid_
+00016ff0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00017000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017010: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00017020: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00017030: 792e 6170 7065 6e64 2861 6c6c 5f73 706f  y.append(all_spo
+00017040: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017050: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
 00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00017080: 7370 5f7a 2e61 7070 656e 6428 616c 6c5f  sp_z.append(all_
-00017090: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-000170a0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-000170b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000170c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170d0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000170e0: 6974 6f74 6963 5f64 6973 705f 792e 6170  itotic_disp_y.ap
-000170f0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017100: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
-00017110: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00017120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017140: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017150: 6469 7370 5f78 2e61 7070 656e 6428 616c  disp_x.append(al
-00017160: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017170: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-00017180: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171a0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-000171b0: 5f6d 6974 6f74 6963 5f72 6164 6975 732e  _mitotic_radius.
-000171c0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-000171d0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-000171e0: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
-000171f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017210: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00017220: 635f 7370 6565 642e 6170 7065 6e64 2861  c_speed.append(a
-00017230: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017240: 6b5d 5b73 656c 662e 7370 6565 645f 6b65  k][self.speed_ke
-00017250: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017270: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017280: 5f6d 6974 6f74 6963 5f61 6363 2e61 7070  _mitotic_acc.app
-00017290: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000172a0: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
-000172b0: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
-000172c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172e0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-000172f0: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-00017300: 5f63 6861 6e67 652e 6170 7065 6e64 2861  _change.append(a
-00017310: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017320: 6b5d 5b73 656c 662e 6d6f 7469 6f6e 5f61  k][self.motion_a
-00017330: 6e67 6c65 5f6b 6579 5d29 0d0a 2020 2020  ngle_key])..    
-00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017360: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017370: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017380: 736b 2e61 7070 656e 6428 616c 6c5f 7370  sk.append(all_sp
-00017390: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-000173a0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-000173b0: 5f6d 6173 6b5f 6b65 795d 290d 0a20 2020  _mask_key])..   
-000173c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173e0: 2020 2020 2069 6620 7365 6c66 2e63 6c75       if self.clu
-000173f0: 7374 6572 636c 6173 735f 6b65 7920 696e  sterclass_key in
-00017400: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00017410: 735b 6b5d 2e6b 6579 7328 2920 3a0d 0a20  s[k].keys() :.. 
-00017420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017440: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00017450: 6e5f 6d69 746f 7469 635f 636c 7573 7465  n_mitotic_cluste
-00017460: 725f 636c 6173 732e 6170 7065 6e64 2861  r_class.append(a
-00017470: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017480: 6b5d 5b73 656c 662e 636c 7573 7465 7263  k][self.clusterc
-00017490: 6c61 7373 5f6b 6579 5d29 0d0a 0d0a 2020  lass_key])....  
+00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017080: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00017090: 7469 635f 6469 7370 5f78 2e61 7070 656e  tic_disp_x.appen
+000170a0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+000170b0: 6b73 5b6b 5d5b 7365 6c66 2e78 706f 7369  ks[k][self.xposi
+000170c0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170f0: 206e 6f6e 5f6d 6974 6f74 6963 5f72 6164   non_mitotic_rad
+00017100: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
+00017110: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017120: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
+00017130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017150: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00017160: 746f 7469 635f 7370 6565 642e 6170 7065  totic_speed.appe
+00017170: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017180: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
+00017190: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+000171a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171c0: 206e 6f6e 5f6d 6974 6f74 6963 5f61 6363   non_mitotic_acc
+000171d0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+000171e0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000171f0: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
+00017200: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017220: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00017230: 5f6d 6974 6f74 6963 5f64 6972 6563 7469  _mitotic_directi
+00017240: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+00017250: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017260: 636b 735b 6b5d 5b73 656c 662e 6d6f 7469  cks[k][self.moti
+00017270: 6f6e 5f61 6e67 6c65 5f6b 6579 5d29 0d0a  on_angle_key])..
+00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172a0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+000172b0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+000172c0: 6c5f 6d61 736b 2e61 7070 656e 6428 616c  l_mask.append(al
+000172d0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000172e0: 5d5b 7365 6c66 2e64 6973 7461 6e63 655f  ][self.distance_
+000172f0: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
+00017300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017320: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00017330: 2e63 6c75 7374 6572 636c 6173 735f 6b65  .clusterclass_ke
+00017340: 7920 696e 2061 6c6c 5f73 706f 7473 5f74  y in all_spots_t
+00017350: 7261 636b 735b 6b5d 2e6b 6579 7328 2920  racks[k].keys() 
+00017360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017390: 2020 6e6f 6e5f 6d69 746f 7469 635f 636c    non_mitotic_cl
+000173a0: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
+000173b0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+000173c0: 636b 735b 6b5d 5b73 656c 662e 636c 7573  cks[k][self.clus
+000173d0: 7465 7263 6c61 7373 5f6b 6579 5d29 0d0a  terclass_key])..
+000173e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017400: 2020 2020 616c 6c5f 6469 7370 5f7a 2e61      all_disp_z.a
+00017410: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017420: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e7a  tracks[k][self.z
+00017430: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017450: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017460: 6c6c 5f64 6973 705f 792e 6170 7065 6e64  ll_disp_y.append
+00017470: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017480: 735b 6b5d 5b73 656c 662e 7970 6f73 6964  s[k][self.yposid
+00017490: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174c0: 616c 6c5f 6469 7370 5f7a 2e61 7070 656e  all_disp_z.appen
-000174d0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000174e0: 6b73 5b6b 5d5b 7365 6c66 2e7a 706f 7369  ks[k][self.zposi
-000174f0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+000174b0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+000174c0: 7370 5f78 2e61 7070 656e 6428 616c 6c5f  sp_x.append(all_
+000174d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000174e0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+000174f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017510: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017520: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
-00017530: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017540: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-00017550: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017510: 2020 2020 2061 6c6c 5f72 6164 6975 732e       all_radius.
+00017520: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017530: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017540: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
+00017550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017570: 2020 2020 2020 616c 6c5f 6469 7370 5f78        all_disp_x
-00017580: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017590: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-000175a0: 2e78 706f 7369 645f 6b65 795d 290d 0a20  .xposid_key]).. 
+00017570: 616c 6c5f 7370 6565 642e 6170 7065 6e64  all_speed.append
+00017580: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017590: 735b 6b5d 5b73 656c 662e 7370 6565 645f  s[k][self.speed_
+000175a0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
 000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175d0: 2061 6c6c 5f72 6164 6975 732e 6170 7065   all_radius.appe
-000175e0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000175f0: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
-00017600: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
+000175c0: 2020 2020 2020 2020 2061 6c6c 5f61 6363           all_acc
+000175d0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+000175e0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000175f0: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
+00017600: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
 00017610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017620: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017630: 7370 6565 642e 6170 7065 6e64 2861 6c6c  speed.append(all
-00017640: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017650: 5b73 656c 662e 7370 6565 645f 6b65 795d  [self.speed_key]
-00017660: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017680: 2020 2020 2061 6c6c 5f61 6363 2e61 7070       all_acc.app
-00017690: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000176a0: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
-000176b0: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
-000176c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000176d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176e0: 2020 2061 6c6c 5f64 6972 6563 7469 6f6e     all_direction
-000176f0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-00017700: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017710: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
-00017720: 5f61 6e67 6c65 5f6b 6579 5d29 2020 200d  _angle_key])   .
-00017730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017750: 2020 2061 6c6c 5f64 6973 7461 6e63 655f     all_distance_
-00017760: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00017770: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017780: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
-00017790: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-000177a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000177b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177c0: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
-000177d0: 7573 7465 7263 6c61 7373 5f6b 6579 2069  usterclass_key i
-000177e0: 6e20 616c 6c5f 7370 6f74 735f 7472 6163  n all_spots_trac
-000177f0: 6b73 5b6b 5d2e 6b65 7973 2829 203a 0d0a  ks[k].keys() :..
-00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017820: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017830: 6c6c 5f63 6c75 7374 6572 5f63 6c61 7373  ll_cluster_class
-00017840: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017850: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017860: 2e63 6c75 7374 6572 636c 6173 735f 6b65  .clusterclass_ke
-00017870: 795d 2920 2020 200d 0a20 2020 2020 2020  y])    ..       
-00017880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178a0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-000178b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000178c0: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
-000178d0: 6e70 2e61 6273 286e 702e 6469 6666 286d  np.abs(np.diff(m
-000178e0: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
-000178f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017900: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00017910: 705f 7920 3d20 6e70 2e61 6273 286e 702e  p_y = np.abs(np.
-00017920: 6469 6666 286d 6974 6f74 6963 5f64 6973  diff(mitotic_dis
-00017930: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00017940: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00017950: 6963 5f64 6973 705f 7820 3d20 6e70 2e61  ic_disp_x = np.a
-00017960: 6273 286e 702e 6469 6666 286d 6974 6f74  bs(np.diff(mitot
-00017970: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
-00017980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017990: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-000179a0: 6973 705f 7a20 3d20 6e70 2e61 6273 286e  isp_z = np.abs(n
-000179b0: 702e 6469 6666 286e 6f6e 5f6d 6974 6f74  p.diff(non_mitot
-000179c0: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
-000179d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179e0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-000179f0: 705f 7920 3d20 6e70 2e61 6273 286e 702e  p_y = np.abs(np.
-00017a00: 6469 6666 286e 6f6e 5f6d 6974 6f74 6963  diff(non_mitotic
-00017a10: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
-00017a20: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017a30: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00017a40: 7820 3d20 6e70 2e61 6273 286e 702e 6469  x = np.abs(np.di
-00017a50: 6666 286e 6f6e 5f6d 6974 6f74 6963 5f64  ff(non_mitotic_d
-00017a60: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
-00017a70: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017a80: 6c6c 5f64 6973 705f 7a20 3d20 6e70 2e61  ll_disp_z = np.a
-00017a90: 6273 286e 702e 6469 6666 2861 6c6c 5f64  bs(np.diff(all_d
-00017aa0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
-00017ab0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017ac0: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
-00017ad0: 286e 702e 6469 6666 2861 6c6c 5f64 6973  (np.diff(all_dis
-00017ae0: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00017af0: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017b00: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
-00017b10: 702e 6469 6666 2861 6c6c 5f64 6973 705f  p.diff(all_disp_
-00017b20: 7829 290d 0a0d 0a0d 0a20 2020 2020 2020  x))......       
+00017620: 2020 2020 2020 2061 6c6c 5f64 6972 6563         all_direc
+00017630: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
+00017640: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017650: 7261 636b 735b 6b5d 5b73 656c 662e 6d6f  racks[k][self.mo
+00017660: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 5d29  tion_angle_key])
+00017670: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017690: 2020 2020 2020 2061 6c6c 5f64 6973 7461         all_dista
+000176a0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+000176b0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000176c0: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
+000176d0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+000176e0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017700: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00017710: 662e 636c 7573 7465 7263 6c61 7373 5f6b  f.clusterclass_k
+00017720: 6579 2069 6e20 616c 6c5f 7370 6f74 735f  ey in all_spots_
+00017730: 7472 6163 6b73 5b6b 5d2e 6b65 7973 2829  tracks[k].keys()
+00017740: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
+00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017770: 2020 2061 6c6c 5f63 6c75 7374 6572 5f63     all_cluster_c
+00017780: 6c61 7373 2e61 7070 656e 6428 616c 6c5f  lass.append(all_
+00017790: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000177a0: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
+000177b0: 735f 6b65 795d 2920 2020 200d 0a20 2020  s_key])    ..   
+000177c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177e0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+000177f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017800: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+00017810: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
+00017820: 6666 286d 6974 6f74 6963 5f64 6973 705f  ff(mitotic_disp_
+00017830: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+00017840: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00017850: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
+00017860: 286e 702e 6469 6666 286d 6974 6f74 6963  (np.diff(mitotic
+00017870: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
+00017880: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017890: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
+000178a0: 6e70 2e61 6273 286e 702e 6469 6666 286d  np.abs(np.diff(m
+000178b0: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+000178c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000178d0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+000178e0: 6963 5f64 6973 705f 7a20 3d20 6e70 2e61  ic_disp_z = np.a
+000178f0: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
+00017900: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
+00017910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017920: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00017930: 5f64 6973 705f 7920 3d20 6e70 2e61 6273  _disp_y = np.abs
+00017940: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
+00017950: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
+00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017970: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00017980: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
+00017990: 702e 6469 6666 286e 6f6e 5f6d 6974 6f74  p.diff(non_mitot
+000179a0: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
+000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179c0: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
+000179d0: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
+000179e0: 6c6c 5f64 6973 705f 7a29 290d 0a20 2020  ll_disp_z))..   
+000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a00: 2061 6c6c 5f64 6973 705f 7920 3d20 6e70   all_disp_y = np
+00017a10: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
+00017a20: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
+00017a30: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017a40: 6c6c 5f64 6973 705f 7820 3d20 6e70 2e61  ll_disp_x = np.a
+00017a50: 6273 286e 702e 6469 6666 2861 6c6c 5f64  bs(np.diff(all_d
+00017a60: 6973 705f 7829 290d 0a0d 0a0d 0a20 2020  isp_x))......   
+00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a90: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00017aa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017ab0: 7469 6d65 2e61 7070 656e 6428 6920 2a20  time.append(i * 
+00017ac0: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+00017ad0: 6e29 0d0a 0d0a 2020 2020 2020 2020 2020  n)....          
+00017ae0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017af0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
+00017b00: 6c61 7373 2e61 7070 656e 6428 6e70 2e61  lass.append(np.a
+00017b10: 7361 7272 6179 286d 6974 6f74 6963 5f63  sarray(mitotic_c
+00017b20: 6c75 7374 6572 5f63 6c61 7373 2929 0d0a  luster_class))..
 00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00017b60: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-00017b70: 2e61 7070 656e 6428 6920 2a20 7365 6c66  .append(i * self
-00017b80: 2e74 6361 6c69 6272 6174 696f 6e29 0d0a  .tcalibration)..
+00017b40: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00017b50: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
+00017b60: 7373 2e61 7070 656e 6428 6e70 2e61 7361  ss.append(np.asa
+00017b70: 7272 6179 286e 6f6e 5f6d 6974 6f74 6963  rray(non_mitotic
+00017b80: 5f63 6c75 7374 6572 5f63 6c61 7373 2929  _cluster_class))
 00017b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017ba0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017bb0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
-00017bc0: 2e61 7070 656e 6428 6e70 2e61 7361 7272  .append(np.asarr
-00017bd0: 6179 286d 6974 6f74 6963 5f63 6c75 7374  ay(mitotic_clust
-00017be0: 6572 5f63 6c61 7373 2929 0d0a 2020 2020  er_class))..    
-00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c00: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00017c10: 5f63 6c75 7374 6572 5f63 6c61 7373 2e61  _cluster_class.a
-00017c20: 7070 656e 6428 6e70 2e61 7361 7272 6179  ppend(np.asarray
-00017c30: 286e 6f6e 5f6d 6974 6f74 6963 5f63 6c75  (non_mitotic_clu
-00017c40: 7374 6572 5f63 6c61 7373 2929 0d0a 2020  ster_class))..  
-00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c60: 2020 7365 6c66 2e61 6c6c 5f63 6c75 7374    self.all_clust
-00017c70: 6572 5f63 6c61 7373 2e61 7070 656e 6428  er_class.append(
-00017c80: 6e70 2e61 7361 7272 6179 2861 6c6c 5f63  np.asarray(all_c
-00017c90: 6c75 7374 6572 5f63 6c61 7373 2929 0d0a  luster_class))..
-00017ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017cb0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017cc0: 6963 5f6d 6561 6e5f 6469 7370 5f7a 2e61  ic_mean_disp_z.a
-00017cd0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00017ce0: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
-00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d00: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017d10: 5f76 6172 5f64 6973 705f 7a2e 6170 7065  _var_disp_z.appe
-00017d20: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-00017d30: 635f 6469 7370 5f7a 2929 0d0a 0d0a 2020  c_disp_z))....  
-00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d50: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00017d60: 6561 6e5f 6469 7370 5f79 2e61 7070 656e  ean_disp_y.appen
-00017d70: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
-00017d80: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
-00017d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017da0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00017db0: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
-00017dc0: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-00017dd0: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-00017de0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017df0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00017e00: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
-00017e10: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
-00017e20: 7370 5f78 2929 0d0a 2020 2020 2020 2020  sp_x))..        
-00017e30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017e40: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-00017e50: 705f 782e 6170 7065 6e64 286e 702e 7374  p_x.append(np.st
-00017e60: 6428 6d69 746f 7469 635f 6469 7370 5f78  d(mitotic_disp_x
-00017e70: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00017e80: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017e90: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
-00017ea0: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
-00017eb0: 6e28 6d69 746f 7469 635f 7261 6469 7573  n(mitotic_radius
-00017ec0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00017ed0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00017ee0: 6f74 6963 5f76 6172 5f72 6164 6975 732e  otic_var_radius.
-00017ef0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
-00017f00: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-00017f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017f20: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017f30: 6963 5f6d 6561 6e5f 7370 6565 642e 6170  ic_mean_speed.ap
-00017f40: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00017f50: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
-00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f70: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00017f80: 6172 5f73 7065 6564 2e61 7070 656e 6428  ar_speed.append(
-00017f90: 6e70 2e73 7464 286d 6974 6f74 6963 5f73  np.std(mitotic_s
-00017fa0: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
-00017fb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017fc0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00017fd0: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
-00017fe0: 616e 286d 6974 6f74 6963 5f61 6363 2929  an(mitotic_acc))
-00017ff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018000: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018010: 6963 5f76 6172 5f61 6363 2e61 7070 656e  ic_var_acc.appen
-00018020: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018030: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
-00018040: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018050: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00018060: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018070: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
-00018080: 6e28 6d69 746f 7469 635f 6469 7265 6374  n(mitotic_direct
-00018090: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
-000180a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180b0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000180c0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-000180d0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
-000180e0: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-000180f0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00018100: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018110: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018120: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
-00018130: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00018140: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00018150: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-00018160: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
+00017ba0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f63        self.all_c
+00017bb0: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
+00017bc0: 656e 6428 6e70 2e61 7361 7272 6179 2861  end(np.asarray(a
+00017bd0: 6c6c 5f63 6c75 7374 6572 5f63 6c61 7373  ll_cluster_class
+00017be0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00017bf0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017c00: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00017c10: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
+00017c20: 6e28 6d69 746f 7469 635f 6469 7370 5f7a  n(mitotic_disp_z
+00017c30: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00017c40: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00017c50: 6f74 6963 5f76 6172 5f64 6973 705f 7a2e  otic_var_disp_z.
+00017c60: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+00017c70: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+00017c80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017c90: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00017ca0: 6963 5f6d 6561 6e5f 6469 7370 5f79 2e61  ic_mean_disp_y.a
+00017cb0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00017cc0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
+00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ce0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00017cf0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
+00017d00: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00017d10: 635f 6469 7370 5f79 2929 0d0a 0d0a 2020  c_disp_y))....  
+00017d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d30: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00017d40: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
+00017d50: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+00017d60: 635f 6469 7370 5f78 2929 0d0a 2020 2020  c_disp_x))..    
+00017d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d80: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00017d90: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+00017da0: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
+00017db0: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+00017dc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017dd0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00017de0: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+00017df0: 2e6d 6561 6e28 6d69 746f 7469 635f 7261  .mean(mitotic_ra
+00017e00: 6469 7573 2929 0d0a 2020 2020 2020 2020  dius))..        
+00017e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017e20: 2e6d 6974 6f74 6963 5f76 6172 5f72 6164  .mitotic_var_rad
+00017e30: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
+00017e40: 6428 6d69 746f 7469 635f 7261 6469 7573  d(mitotic_radius
+00017e50: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00017e60: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017e70: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
+00017e80: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
+00017e90: 286d 6974 6f74 6963 5f73 7065 6564 2929  (mitotic_speed))
+00017ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017eb0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00017ec0: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
+00017ed0: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+00017ee0: 6963 5f73 7065 6564 2929 0d0a 0d0a 2020  ic_speed))....  
+00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f00: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00017f10: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
+00017f20: 702e 6d65 616e 286d 6974 6f74 6963 5f61  p.mean(mitotic_a
+00017f30: 6363 2929 0d0a 2020 2020 2020 2020 2020  cc))..          
+00017f40: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017f50: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
+00017f60: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
+00017f70: 6f74 6963 5f61 6363 2929 0d0a 0d0a 2020  otic_acc))....  
+00017f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f90: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00017fa0: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
+00017fb0: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
+00017fc0: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+00017fd0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00017fe0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00017ff0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018000: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+00018010: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+00018020: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00018030: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00018040: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
+00018050: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018060: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00018070: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018080: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
+00018090: 6e28 6d69 746f 7469 635f 6469 7374 616e  n(mitotic_distan
+000180a0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180c0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+000180d0: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
+000180e0: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
+000180f0: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
+00018100: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018110: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018120: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018130: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00018140: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+00018150: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00018160: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
 00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018180: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00018190: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-000181a0: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
-000181b0: 6428 6d69 746f 7469 635f 6469 7374 616e  d(mitotic_distan
-000181c0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-000181d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000181e0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000181f0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00018200: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
-00018210: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00018220: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00018230: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018240: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018250: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
-00018260: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-00018270: 635f 6469 7370 5f7a 2929 0d0a 0d0a 2020  c_disp_z))....  
-00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018290: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000182a0: 6963 5f6d 6561 6e5f 6469 7370 5f79 2e61  ic_mean_disp_y.a
-000182b0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-000182c0: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-000182d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000182e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000182f0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00018300: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
-00018310: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-00018320: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-00018330: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018340: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018350: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
-00018360: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-00018370: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-00018380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018390: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-000183a0: 6f74 6963 5f76 6172 5f64 6973 705f 782e  otic_var_disp_x.
-000183b0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-000183c0: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
-000183d0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000183e0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000183f0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00018400: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-00018410: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018420: 635f 7261 6469 7573 2929 0d0a 2020 2020  c_radius))..    
-00018430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018440: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018450: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-00018460: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-00018470: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
-00018480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018490: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000184a0: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
-000184b0: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
-000184c0: 286e 6f6e 5f6d 6974 6f74 6963 5f73 7065  (non_mitotic_spe
-000184d0: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
-000184e0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000184f0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f73  on_mitotic_var_s
-00018500: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
-00018510: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f73  td(non_mitotic_s
-00018520: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
-00018530: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018540: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018550: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
-00018560: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
-00018570: 6963 5f61 6363 2929 0d0a 2020 2020 2020  ic_acc))..      
-00018580: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018590: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-000185a0: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
-000185b0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-000185c0: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
-000185d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000185e0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-000185f0: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
-00018600: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00018610: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018620: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
-00018630: 616e 6765 2929 0d0a 2020 2020 2020 2020  ange))..        
-00018640: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018650: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018660: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00018670: 6e67 652e 6170 7065 6e64 286e 702e 7374  nge.append(np.st
-00018680: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-00018690: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-000186a0: 2929 200d 0a0d 0a20 2020 2020 2020 2020  )) ....         
-000186b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000186c0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-000186d0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-000186e0: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
-000186f0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-00018700: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00018710: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
-00018720: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018730: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00018740: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018750: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-00018760: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
-00018770: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-00018780: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00018790: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000187a0: 6c5f 6d65 616e 5f64 6973 705f 7a2e 6170  l_mean_disp_z.ap
-000187b0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-000187c0: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
-000187d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000187e0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
-000187f0: 5f7a 2e61 7070 656e 6428 6e70 2e73 7464  _z.append(np.std
-00018800: 2861 6c6c 5f64 6973 705f 7a29 290d 0a0d  (all_disp_z))...
-00018810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018820: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018830: 616e 5f64 6973 705f 792e 6170 7065 6e64  an_disp_y.append
-00018840: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
-00018850: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00018860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018870: 616c 6c5f 7661 725f 6469 7370 5f79 2e61  all_var_disp_y.a
-00018880: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00018890: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
-000188a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188b0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-000188c0: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
-000188d0: 6d65 616e 2861 6c6c 5f64 6973 705f 7829  mean(all_disp_x)
-000188e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000188f0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018900: 7661 725f 6469 7370 5f78 2e61 7070 656e  var_disp_x.appen
-00018910: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
-00018920: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
-00018930: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018940: 662e 616c 6c5f 6d65 616e 5f72 6164 6975  f.all_mean_radiu
-00018950: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
-00018960: 2861 6c6c 5f72 6164 6975 7329 290d 0a20  (all_radius)).. 
-00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018980: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00018990: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-000189a0: 2e73 7464 2861 6c6c 5f72 6164 6975 7329  .std(all_radius)
-000189b0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000189c0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000189d0: 6c5f 6d65 616e 5f73 7065 6564 2e61 7070  l_mean_speed.app
-000189e0: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-000189f0: 7370 6565 6429 290d 0a20 2020 2020 2020  speed))..       
-00018a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018a10: 662e 616c 6c5f 7661 725f 7370 6565 642e  f.all_var_speed.
-00018a20: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-00018a30: 6c5f 7370 6565 6429 290d 0a0d 0a20 2020  l_speed))....   
-00018a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a50: 2073 656c 662e 616c 6c5f 6d65 616e 5f61   self.all_mean_a
-00018a60: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
-00018a70: 6e28 616c 6c5f 6163 6329 290d 0a20 2020  n(all_acc))..   
-00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a90: 2073 656c 662e 616c 6c5f 7661 725f 6163   self.all_var_ac
-00018aa0: 632e 6170 7065 6e64 286e 702e 7374 6428  c.append(np.std(
-00018ab0: 616c 6c5f 6163 6329 290d 0a0d 0a0d 0a0d  all_acc)).......
+00018180: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00018190: 5f76 6172 5f64 6973 705f 7a2e 6170 7065  _var_disp_z.appe
+000181a0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+000181b0: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+000181c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000181d0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000181e0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+000181f0: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
+00018200: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+00018210: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+00018220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018230: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00018240: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
+00018250: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00018260: 635f 6469 7370 5f79 2929 0d0a 0d0a 2020  c_disp_y))....  
+00018270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018280: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018290: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
+000182a0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+000182b0: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+000182c0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000182d0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000182e0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+000182f0: 705f 782e 6170 7065 6e64 286e 702e 7374  p_x.append(np.st
+00018300: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
+00018310: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+00018320: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018330: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00018340: 6561 6e5f 7261 6469 7573 2e61 7070 656e  ean_radius.appen
+00018350: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
+00018360: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
+00018370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018380: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00018390: 6f74 6963 5f76 6172 5f72 6164 6975 732e  otic_var_radius.
+000183a0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+000183b0: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
+000183c0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000183d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000183e0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+000183f0: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
+00018400: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
+00018410: 5f73 7065 6564 2929 0d0a 2020 2020 2020  _speed))..      
+00018420: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018430: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00018440: 6172 5f73 7065 6564 2e61 7070 656e 6428  ar_speed.append(
+00018450: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00018460: 6963 5f73 7065 6564 2929 0d0a 0d0a 2020  ic_speed))....  
+00018470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018480: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018490: 6963 5f6d 6561 6e5f 6163 632e 6170 7065  ic_mean_acc.appe
+000184a0: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+000184b0: 6974 6f74 6963 5f61 6363 2929 0d0a 2020  itotic_acc))..  
+000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184d0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+000184e0: 6963 5f76 6172 5f61 6363 2e61 7070 656e  ic_var_acc.appen
+000184f0: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
+00018500: 6f74 6963 5f61 6363 2929 0d0a 0d0a 2020  otic_acc))....  
+00018510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018520: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018530: 6963 5f6d 6561 6e5f 6469 7265 6374 696f  ic_mean_directio
+00018540: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00018550: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
+00018560: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+00018570: 6c5f 6368 616e 6765 2929 0d0a 2020 2020  l_change))..    
+00018580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018590: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+000185a0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
+000185b0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+000185c0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+000185d0: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+000185e0: 616e 6765 2929 200d 0a0d 0a20 2020 2020  ange)) ....     
+000185f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018600: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00018610: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
+00018620: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
+00018630: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+00018640: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+00018650: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+00018660: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018670: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00018680: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00018690: 6d61 736b 2e61 7070 656e 6428 6e70 2e73  mask.append(np.s
+000186a0: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
+000186b0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000186c0: 6b29 290d 0a0d 0a0d 0a20 2020 2020 2020  k))......       
+000186d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000186e0: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+000186f0: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
+00018700: 2861 6c6c 5f64 6973 705f 7a29 290d 0a20  (all_disp_z)).. 
+00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018720: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00018730: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+00018740: 2e73 7464 2861 6c6c 5f64 6973 705f 7a29  .std(all_disp_z)
+00018750: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018760: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018770: 6c5f 6d65 616e 5f64 6973 705f 792e 6170  l_mean_disp_y.ap
+00018780: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+00018790: 5f64 6973 705f 7929 290d 0a20 2020 2020  _disp_y))..     
+000187a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000187b0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+000187c0: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
+000187d0: 2861 6c6c 5f64 6973 705f 7929 290d 0a0d  (all_disp_y))...
+000187e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000187f0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00018800: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
+00018810: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
+00018820: 705f 7829 290d 0a20 2020 2020 2020 2020  p_x))..         
+00018830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018840: 616c 6c5f 7661 725f 6469 7370 5f78 2e61  all_var_disp_x.a
+00018850: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00018860: 5f64 6973 705f 7829 290d 0a0d 0a20 2020  _disp_x))....   
+00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018880: 2073 656c 662e 616c 6c5f 6d65 616e 5f72   self.all_mean_r
+00018890: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
+000188a0: 6d65 616e 2861 6c6c 5f72 6164 6975 7329  mean(all_radius)
+000188b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000188c0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+000188d0: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
+000188e0: 6428 6e70 2e73 7464 2861 6c6c 5f72 6164  d(np.std(all_rad
+000188f0: 6975 7329 290d 0a0d 0a20 2020 2020 2020  ius))....       
+00018900: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018910: 662e 616c 6c5f 6d65 616e 5f73 7065 6564  f.all_mean_speed
+00018920: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018930: 616c 6c5f 7370 6565 6429 290d 0a20 2020  all_speed))..   
+00018940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018950: 2073 656c 662e 616c 6c5f 7661 725f 7370   self.all_var_sp
+00018960: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
+00018970: 6428 616c 6c5f 7370 6565 6429 290d 0a0d  d(all_speed))...
+00018980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018990: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+000189a0: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
+000189b0: 2e6d 6561 6e28 616c 6c5f 6163 6329 290d  .mean(all_acc)).
+000189c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000189d0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+000189e0: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
+000189f0: 7374 6428 616c 6c5f 6163 6329 290d 0a0d  std(all_acc))...
+00018a00: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00018a10: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018a20: 6c5f 6d65 616e 5f64 6972 6563 7469 6f6e  l_mean_direction
+00018a30: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
+00018a40: 286e 702e 6d65 616e 2861 6c6c 5f64 6972  (np.mean(all_dir
+00018a50: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00018a60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018a70: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018a80: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
+00018a90: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
+00018aa0: 2e73 7464 2861 6c6c 5f64 6972 6563 7469  .std(all_directi
+00018ab0: 6f6e 616c 5f63 6861 6e67 6529 290d 0a0d  onal_change))...
 00018ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00018ad0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018ae0: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00018af0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00018b00: 6d65 616e 2861 6c6c 5f64 6972 6563 7469  mean(all_directi
-00018b10: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
+00018ae0: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
+00018af0: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
+00018b00: 6d65 616e 2861 6c6c 5f64 6973 7461 6e63  mean(all_distanc
+00018b10: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
 00018b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018b30: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00018b40: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018b50: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
-00018b60: 2861 6c6c 5f64 6972 6563 7469 6f6e 616c  (all_directional
-00018b70: 5f63 6861 6e67 6529 290d 0a0d 0a20 2020  _change))....   
+00018b40: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018b50: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
+00018b60: 2861 6c6c 5f64 6973 7461 6e63 655f 6365  (all_distance_ce
+00018b70: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
 00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b90: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00018ba0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00018bb0: 6b2e 6170 7065 6e64 286e 702e 6d65 616e  k.append(np.mean
-00018bc0: 2861 6c6c 5f64 6973 7461 6e63 655f 6365  (all_distance_ce
-00018bd0: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-00018be0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018bf0: 656c 662e 616c 6c5f 7661 725f 6469 7374  elf.all_var_dist
-00018c00: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00018c10: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00018c20: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018c30: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
-00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c50: 2020 200d 0a20 2020 2020 2020 200d 0a64     ..        ..d
-00018c60: 6566 2062 6f75 6e64 6172 795f 706f 696e  ef boundary_poin
-00018c70: 7473 286d 6173 6b2c 2078 6361 6c69 6272  ts(mask, xcalibr
-00018c80: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
-00018c90: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
-00018ca0: 6e29 3a0d 0a0d 0a20 2020 206e 6469 6d20  n):....    ndim 
-00018cb0: 3d20 6c65 6e28 6d61 736b 2e73 6861 7065  = len(mask.shape
-00018cc0: 290d 0a20 2020 2074 696d 6564 5f6d 6173  )..    timed_mas
-00018cd0: 6b20 3d20 7b7d 0d0a 2020 2020 6d61 736b  k = {}..    mask
-00018ce0: 203d 206d 6173 6b20 3e20 300d 0a20 2020   = mask > 0..   
-00018cf0: 206d 6173 6b20 3d20 6d61 736b 2e61 7374   mask = mask.ast
-00018d00: 7970 6528 2775 696e 7438 2729 0d0a 2020  ype('uint8')..  
-00018d10: 2020 2320 5958 2073 6861 7065 6420 6f62    # YX shaped ob
-00018d20: 6a65 6374 0d0a 2020 2020 6966 206e 6469  ject..    if ndi
-00018d30: 6d20 3d3d 2032 3a0d 0a20 2020 2020 2020  m == 2:..       
-00018d40: 200d 0a20 2020 2020 2020 2062 6f75 6e64   ..        bound
-00018d50: 6172 7920 3d20 6669 6e64 5f62 6f75 6e64  ary = find_bound
-00018d60: 6172 6965 7328 6d61 736b 290d 0a20 2020  aries(mask)..   
-00018d70: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
-00018d80: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
-00018d90: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
-00018da0: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
-00018db0: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-00018dc0: 6865 7265 2862 6f75 6e64 6172 7920 3e20  here(boundary > 
-00018dd0: 3029 0d0a 2020 2020 2020 2020 7265 616c  0)..        real
-00018de0: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
-00018df0: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
-00018e00: 6179 2869 6e64 6963 6573 2929 2e63 6f70  ay(indices)).cop
-00018e10: 7928 290d 0a0d 0a20 2020 2020 2020 2066  y()....        f
-00018e20: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-00018e30: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
-00018e40: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
-00018e50: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-00018e60: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
-00018e70: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
-00018e80: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00018e90: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-00018ea0: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
-00018eb0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-00018ec0: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
-00018ed0: 0d0a 2020 2020 2020 2020 7472 6565 203d  ..        tree =
-00018ee0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-00018ef0: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
-00018f00: 2020 2020 2020 2020 2320 5468 6973 206f          # This o
-00018f10: 626a 6563 7420 636f 6e74 6169 6e73 206c  bject contains l
-00018f20: 6973 7420 6f66 2061 6c6c 2074 6865 2070  ist of all the p
-00018f30: 6f69 6e74 7320 666f 7220 616c 6c20 7468  oints for all th
-00018f40: 6520 6c61 6265 6c73 2069 6e20 7468 6520  e labels in the 
-00018f50: 4d61 736b 2069 6d61 6765 2077 6974 6820  Mask image with 
-00018f60: 7468 6520 6c61 6265 6c20 6964 2061 6e64  the label id and
-00018f70: 2076 6f6c 756d 6520 6f66 2065 6163 6820   volume of each 
-00018f80: 6c61 6265 6c0d 0a20 2020 2020 2020 2074  label..        t
-00018f90: 696d 6564 5f6d 6173 6b5b 7374 7228 3029  imed_mask[str(0)
-00018fa0: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
-00018fb0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
-00018fc0: 6964 5d0d 0a0d 0a20 2020 2023 2054 5958  id]....    # TYX
-00018fd0: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
-00018fe0: 2020 2020 6966 206e 6469 6d20 3d3d 2033      if ndim == 3
-00018ff0: 3a0d 0a0d 0a0d 0a20 2020 2020 2020 2066  :......        f
-00019000: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
-00019010: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
-00019020: 5b30 5d29 293a 0d0a 2020 2020 2020 2020  [0])):..        
-00019030: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00019040: 2020 2020 2020 2020 2020 626f 756e 6461            bounda
-00019050: 7279 203d 2066 696e 645f 626f 756e 6461  ry = find_bounda
-00019060: 7269 6573 286d 6173 6b5b 692c 3a5d 290d  ries(mask[i,:]).
-00019070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019080: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
-00019090: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
-000190a0: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
-000190b0: 7279 2920 0d0a 2020 2020 2020 2020 2020  ry) ..          
-000190c0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-000190d0: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
-000190e0: 7920 3e20 3029 0d0a 2020 2020 2020 2020  y > 0)..        
-000190f0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-00019100: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
-00019110: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
-00019120: 6e64 6963 6573 2929 2e63 6f70 7928 290d  ndices)).copy().
-00019130: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00019140: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-00019150: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
-00019160: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
-00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019180: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00019190: 305d 203d 2072 6561 6c5f 696e 6469 6365  0] = real_indice
-000191a0: 735b 6a5d 5b30 5d20 2a20 7963 616c 6962  s[j][0] * ycalib
-000191b0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-000191c0: 2020 2020 2020 2020 2020 2020 7265 616c              real
-000191d0: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
-000191e0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-000191f0: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
-00019200: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-00019210: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-00019220: 7469 616c 2e63 4b44 5472 6565 2872 6561  tial.cKDTree(rea
-00019230: 6c5f 696e 6469 6365 7329 0d0a 0d0a 2020  l_indices)....  
-00019240: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00019250: 6d65 645f 6d61 736b 5b73 7472 2869 295d  med_mask[str(i)]
-00019260: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
-00019270: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
-00019280: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-00019290: 0d0a 2020 2020 2320 545a 5958 2073 6861  ..    # TZYX sha
-000192a0: 7065 6420 6f62 6a65 6374 0d0a 2020 2020  ped object..    
-000192b0: 6966 206e 6469 6d20 3d3d 2034 3a0d 0a20  if ndim == 4:.. 
-000192c0: 2020 2020 2020 2070 7269 6e74 2827 4d61         print('Ma
-000192d0: 736b 7320 6d61 6465 2069 6e74 6f20 6120  sks made into a 
-000192e0: 3444 2063 796c 696e 6465 722c 2075 7027  4D cylinder, up'
-000192f0: 290d 0a20 2020 2020 2020 2062 6f75 6e64  )..        bound
-00019300: 6172 7920 3d20 6e70 2e7a 6572 6f73 280d  ary = np.zeros(.
-00019310: 0a20 2020 2020 2020 2020 2020 205b 6d61  .            [ma
-00019320: 736b 2e73 6861 7065 5b30 5d2c 206d 6173  sk.shape[0], mas
-00019330: 6b2e 7368 6170 655b 315d 2c20 6d61 736b  k.shape[1], mask
-00019340: 2e73 6861 7065 5b32 5d2c 206d 6173 6b2e  .shape[2], mask.
-00019350: 7368 6170 655b 335d 5d0d 0a20 2020 2020  shape[3]]..     
-00019360: 2020 2029 0d0a 2020 2020 2020 2020 666f     )..        fo
-00019370: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
-00019380: 6d61 736b 2e73 6861 7065 5b30 5d29 3a0d  mask.shape[0]):.
-00019390: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-000193a0: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
-000193b0: 6172 795b 692c 3a5d 203d 2066 696e 645f  ary[i,:] = find_
-000193c0: 626f 756e 6461 7269 6573 286d 6173 6b5b  boundaries(mask[
-000193d0: 692c 3a5d 290d 0a20 2020 2020 2020 2020  i,:])..         
-000193e0: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
-000193f0: 6420 3d20 636f 6d70 7574 655f 6365 6e74  d = compute_cent
-00019400: 726f 6964 2862 6f75 6e64 6172 795b 692c  roid(boundary[i,
-00019410: 3a5d 2920 0d0a 2020 2020 2020 2020 2020  :]) ..          
-00019420: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-00019430: 6865 7265 2862 6f75 6e64 6172 795b 692c  here(boundary[i,
-00019440: 3a5d 203e 2030 290d 0a20 2020 2020 2020  :] > 0)..       
-00019450: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019460: 7320 3d20 6e70 2e74 7261 6e73 706f 7365  s = np.transpose
-00019470: 286e 702e 6173 6172 7261 7928 696e 6469  (np.asarray(indi
-00019480: 6365 7329 292e 636f 7079 2829 0d0a 0d0a  ces)).copy()....
-00019490: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000194a0: 6a20 696e 2072 616e 6765 2830 2c20 6c65  j in range(0, le
-000194b0: 6e28 7265 616c 5f69 6e64 6963 6573 2929  n(real_indices))
-000194c0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-000194d0: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-000194e0: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
-000194f0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-00019500: 202a 207a 6361 6c69 6272 6174 696f 6e0d   * zcalibration.
-00019510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019520: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019530: 735b 6a5d 5b31 5d20 3d20 7265 616c 5f69  s[j][1] = real_i
-00019540: 6e64 6963 6573 5b6a 5d5b 315d 202a 2079  ndices[j][1] * y
-00019550: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00019560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019570: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00019580: 5b32 5d20 3d20 7265 616c 5f69 6e64 6963  [2] = real_indic
-00019590: 6573 5b6a 5d5b 325d 202a 2078 6361 6c69  es[j][2] * xcali
-000195a0: 6272 6174 696f 6e0d 0a0d 0a20 2020 2020  bration....     
-000195b0: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
-000195c0: 6174 6961 6c2e 634b 4454 7265 6528 7265  atial.cKDTree(re
-000195d0: 616c 5f69 6e64 6963 6573 290d 0a20 2020  al_indices)..   
-000195e0: 2020 2020 2020 2020 2074 696d 6564 5f6d           timed_m
-000195f0: 6173 6b5b 7374 7228 6929 5d20 3d20 5b74  ask[str(i)] = [t
-00019600: 7265 652c 2069 6e64 6963 6573 2c20 7265  ree, indices, re
-00019610: 6769 6f6e 6365 6e74 726f 6964 5d0d 0a20  gioncentroid].. 
-00019620: 2020 2070 7269 6e74 2827 436f 6d70 7574     print('Comput
-00019630: 6564 2074 6865 2062 6f75 6e64 6172 7920  ed the boundary 
-00019640: 706f 696e 7473 2729 0d0a 0d0a 2020 2020  points')....    
-00019650: 7265 7475 726e 2074 696d 6564 5f6d 6173  return timed_mas
-00019660: 6b2c 2062 6f75 6e64 6172 7920 2020 2020  k, boundary     
-00019670: 2020 200d 0a0d 0a64 6566 2063 6f6d 7075     ....def compu
-00019680: 7465 5f63 656e 7472 6f69 6428 6269 6e61  te_centroid(bina
-00019690: 7279 5f69 6d61 6765 293a 0d0a 2020 2020  ry_image):..    
-000196a0: 2320 456e 7375 7265 2062 696e 6172 7920  # Ensure binary 
-000196b0: 696d 6167 6520 6973 2061 204e 756d 5079  image is a NumPy
-000196c0: 2061 7272 6179 0d0a 2020 2020 6269 6e61   array..    bina
-000196d0: 7279 5f69 6d61 6765 203d 206e 702e 6172  ry_image = np.ar
-000196e0: 7261 7928 6269 6e61 7279 5f69 6d61 6765  ray(binary_image
-000196f0: 290d 0a0d 0a20 2020 2077 6869 7465 5f70  )....    white_p
-00019700: 6978 656c 7320 3d20 6e70 2e77 6865 7265  ixels = np.where
-00019710: 2862 696e 6172 795f 696d 6167 6520 3d3d  (binary_image ==
-00019720: 2031 290d 0a20 2020 206e 756d 5f70 6978   1)..    num_pix
-00019730: 656c 7320 3d20 6c65 6e28 7768 6974 655f  els = len(white_
-00019740: 7069 7865 6c73 5b30 5d29 0d0a 0d0a 2020  pixels[0])....  
-00019750: 2020 2320 436f 6d70 7574 6520 7468 6520    # Compute the 
-00019760: 6365 6e74 726f 6964 206f 6620 7468 6520  centroid of the 
-00019770: 7768 6974 6520 7069 7865 6c73 2069 6e20  white pixels in 
-00019780: 7468 6520 626f 756e 6461 7279 2069 6d61  the boundary ima
-00019790: 6765 0d0a 2020 2020 6365 6e74 726f 6964  ge..    centroid
-000197a0: 203d 206e 702e 7a65 726f 7328 6269 6e61   = np.zeros(bina
-000197b0: 7279 5f69 6d61 6765 2e6e 6469 6d29 0d0a  ry_image.ndim)..
-000197c0: 2020 2020 666f 7220 6469 6d20 696e 2072      for dim in r
-000197d0: 616e 6765 2862 696e 6172 795f 696d 6167  ange(binary_imag
-000197e0: 652e 6e64 696d 293a 0d0a 2020 2020 2020  e.ndim):..      
-000197f0: 2020 6365 6e74 726f 6964 5b64 696d 5d20    centroid[dim] 
-00019800: 3d20 7768 6974 655f 7069 7865 6c73 5b64  = white_pixels[d
-00019810: 696d 5d2e 7375 6d28 2920 2f20 6e75 6d5f  im].sum() / num_
-00019820: 7069 7865 6c73 0d0a 0d0a 2020 2020 7265  pixels....    re
-00019830: 7475 726e 2063 656e 7472 6f69 640d 0a0d  turn centroid...
-00019840: 0a0d 0a0d 0a20 0d0a 0d0a 6465 6620 6765  ..... ....def ge
-00019850: 745f 6373 765f 6461 7461 2863 7376 293a  t_csv_data(csv):
-00019860: 0d0a 0d0a 2020 2020 2020 2020 6461 7461  ....        data
-00019870: 7365 7420 3d20 7064 2e72 6561 645f 6373  set = pd.read_cs
-00019880: 7628 0d0a 2020 2020 2020 2020 2020 2020  v(..            
-00019890: 6373 762c 2064 656c 696d 6974 6572 3d22  csv, delimiter="
-000198a0: 2c22 2c20 656e 636f 6469 6e67 3d22 756e  ,", encoding="un
-000198b0: 6963 6f64 655f 6573 6361 7065 222c 206c  icode_escape", l
-000198c0: 6f77 5f6d 656d 6f72 793d 4661 6c73 650d  ow_memory=False.
-000198d0: 0a20 2020 2020 2020 2029 5b33 3a5d 0d0a  .        )[3:]..
-000198e0: 2020 2020 2020 2020 6461 7461 7365 745f          dataset_
-000198f0: 696e 6465 7820 3d20 6461 7461 7365 742e  index = dataset.
-00019900: 696e 6465 780d 0a20 2020 2020 2020 2072  index..        r
-00019910: 6574 7572 6e20 6461 7461 7365 742c 2064  eturn dataset, d
-00019920: 6174 6173 6574 5f69 6e64 6578 0d0a 2020  ataset_index..  
-00019930: 2020 0d0a 6465 6620 6765 745f 7370 6f74    ..def get_spot
-00019940: 5f64 6174 6173 6574 2873 706f 745f 6461  _dataset(spot_da
-00019950: 7461 7365 742c 2074 7261 636b 5f61 6e61  taset, track_ana
-00019960: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
-00019970: 2078 6361 6c69 6272 6174 696f 6e2c 2079   xcalibration, y
-00019980: 6361 6c69 6272 6174 696f 6e2c 207a 6361  calibration, zca
-00019990: 6c69 6272 6174 696f 6e2c 2041 7474 7269  libration, Attri
-000199a0: 6275 7465 426f 786e 616d 652c 2064 6574  buteBoxname, det
-000199b0: 6563 7469 6f6e 6368 616e 6e65 6c29 3a0d  ectionchannel):.
-000199c0: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
-000199d0: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-000199e0: 2070 6f73 6978 203d 2074 7261 636b 5f61   posix = track_a
-000199f0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-00019a00: 735b 2270 6f73 6978 225d 0d0a 2020 2020  s["posix"]..    
-00019a10: 2020 2020 706f 7369 7920 3d20 7472 6163      posiy = trac
-00019a20: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00019a30: 6b65 7973 5b22 706f 7369 7922 5d0d 0a20  keys["posiy"].. 
-00019a40: 2020 2020 2020 2070 6f73 697a 203d 2074         posiz = t
-00019a50: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00019a60: 6f74 5f6b 6579 735b 2270 6f73 697a 225d  ot_keys["posiz"]
-00019a70: 0d0a 2020 2020 2020 2020 6672 616d 6520  ..        frame 
-00019a80: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-00019a90: 5f73 706f 745f 6b65 7973 5b22 6672 616d  _spot_keys["fram
-00019aa0: 6522 5d0d 0a20 2020 2020 2020 200d 0a20  e"]..        .. 
-00019ab0: 2020 2020 2020 204c 6f63 6174 696f 6e58         LocationX
-00019ac0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00019ad0: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-00019ae0: 6f73 6978 5d2e 6173 7479 7065 2822 666c  osix].astype("fl
-00019af0: 6f61 7422 2920 2f20 7863 616c 6962 7261  oat") / xcalibra
-00019b00: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-00019b10: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-00019b20: 2020 2020 2020 204c 6f63 6174 696f 6e59         LocationY
-00019b30: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00019b40: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-00019b50: 6f73 6979 5d2e 6173 7479 7065 2822 666c  osiy].astype("fl
-00019b60: 6f61 7422 2920 2f20 7963 616c 6962 7261  oat") / ycalibra
-00019b70: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-00019b80: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-00019b90: 2020 2020 2020 204c 6f63 6174 696f 6e5a         LocationZ
-00019ba0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00019bb0: 2020 7370 6f74 5f64 6174 6173 6574 5b70    spot_dataset[p
-00019bc0: 6f73 697a 5d2e 6173 7479 7065 2822 666c  osiz].astype("fl
-00019bd0: 6f61 7422 2920 2f20 7a63 616c 6962 7261  oat") / zcalibra
-00019be0: 7469 6f6e 0d0a 2020 2020 2020 2020 292e  tion..        ).
-00019bf0: 6173 7479 7065 2822 696e 7422 290d 0a20  astype("int").. 
-00019c00: 2020 2020 2020 204c 6f63 6174 696f 6e54         LocationT
-00019c10: 203d 2028 7370 6f74 5f64 6174 6173 6574   = (spot_dataset
-00019c20: 5b66 7261 6d65 5d2e 6173 7479 7065 2822  [frame].astype("
-00019c30: 666c 6f61 7422 2929 2e61 7374 7970 6528  float")).astype(
-00019c40: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-00019c50: 0d0a 0d0a 2020 2020 2020 2020 6967 6e6f  ....        igno
-00019c60: 7265 5f76 616c 7565 7320 3d20 5b74 7261  re_values = [tra
-00019c70: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00019c80: 5f6b 6579 735b 226d 6561 6e5f 696e 7465  _keys["mean_inte
-00019c90: 6e73 6974 7922 5d2c 7472 6163 6b5f 616e  nsity"],track_an
-00019ca0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00019cb0: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-00019cc0: 7922 5d5d 200d 0a20 2020 2020 2020 2066  y"]] ..        f
-00019cd0: 6f72 2028 6b2c 7629 2069 6e20 7472 6163  or (k,v) in trac
-00019ce0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00019cf0: 6b65 7973 2e69 7465 6d73 2829 3a0d 0a0d  keys.items():...
-00019d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019d10: 2069 6620 6465 7465 6374 696f 6e63 6861   if detectioncha
-00019d20: 6e6e 656c 203d 3d20 313a 0d0a 2020 2020  nnel == 1:..    
-00019d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d40: 2069 6620 6b20 3d3d 2022 6d65 616e 5f69   if k == "mean_i
-00019d50: 6e74 656e 7369 7479 5f63 6832 223a 0d0a  ntensity_ch2":..
-00019d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d70: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00019d80: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
-00019d90: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
-00019da0: 6e5f 696e 7465 6e73 6974 7922 5d0d 0a20  n_intensity"].. 
-00019db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019dc0: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
-00019dd0: 7565 735b 7661 6c75 655d 203d 2073 706f  ues[value] = spo
-00019de0: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
-00019df0: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-00019e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e10: 2020 2069 6620 6b20 3d3d 2022 746f 7461     if k == "tota
-00019e20: 6c5f 696e 7465 6e73 6974 795f 6368 3222  l_intensity_ch2"
-00019e30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019e40: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00019e50: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
-00019e60: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-00019e70: 746f 7461 6c5f 696e 7465 6e73 6974 7922  total_intensity"
-00019e80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00019e90: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-00019ea0: 6c56 616c 7565 735b 7661 6c75 655d 203d  lValues[value] =
-00019eb0: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
-00019ec0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-00019ed0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-00019ee0: 2020 2020 2020 2020 2020 2069 6620 7620             if v 
-00019ef0: 6e6f 7420 696e 2069 676e 6f72 655f 7661  not in ignore_va
-00019f00: 6c75 6573 3a0d 0a20 2020 2020 2020 2020  lues:..         
-00019f10: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00019f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f30: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-00019f40: 5b76 5d20 3d20 7370 6f74 5f64 6174 6173  [v] = spot_datas
-00019f50: 6574 5b76 5d2e 6173 7479 7065 2822 666c  et[v].astype("fl
-00019f60: 6f61 7422 290d 0a0d 0a20 2020 2020 2020  oat")....       
-00019f70: 2041 6c6c 5661 6c75 6573 5b70 6f73 6978   AllValues[posix
-00019f80: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
-00019f90: 6f6e 582c 3329 0d0a 2020 2020 2020 2020  onX,3)..        
-00019fa0: 416c 6c56 616c 7565 735b 706f 7369 795d  AllValues[posiy]
-00019fb0: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
-00019fc0: 6e59 2c33 290d 0a20 2020 2020 2020 2041  nY,3)..        A
-00019fd0: 6c6c 5661 6c75 6573 5b70 6f73 697a 5d20  llValues[posiz] 
-00019fe0: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
-00019ff0: 5a2c 3329 0d0a 2020 2020 2020 2020 416c  Z,3)..        Al
-0001a000: 6c56 616c 7565 735b 6672 616d 655d 203d  lValues[frame] =
-0001a010: 2072 6f75 6e64 284c 6f63 6174 696f 6e54   round(LocationT
-0001a020: 2c33 290d 0a20 2020 2020 2020 2041 7474  ,3)..        Att
-0001a030: 7269 6275 7465 6964 7320 3d20 5b5d 0d0a  ributeids = []..
-0001a040: 2020 2020 2020 2020 4174 7472 6962 7574          Attribut
-0001a050: 6569 6473 2e61 7070 656e 6428 4174 7472  eids.append(Attr
-0001a060: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
-0001a070: 2020 2020 2020 2066 6f72 2061 7474 7269         for attri
-0001a080: 6275 7465 6e61 6d65 2069 6e20 416c 6c56  butename in AllV
-0001a090: 616c 7565 732e 6b65 7973 2829 3a0d 0a20  alues.keys():.. 
-0001a0a0: 2020 2020 2020 2020 2020 2020 2041 7474               Att
-0001a0b0: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
-0001a0c0: 2861 7474 7269 6275 7465 6e61 6d65 2920  (attributename) 
-0001a0d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0001a0e0: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-0001a0f0: 2020 2020 2072 6574 7572 6e20 4174 7472       return Attr
-0001a100: 6962 7574 6569 6473 2c20 416c 6c56 616c  ibuteids, AllVal
-0001a110: 7565 7320 2020 2020 0d0a 2020 2020 0d0a  ues     ..    ..
-0001a120: 6465 6620 6765 745f 7472 6163 6b5f 6461  def get_track_da
-0001a130: 7461 7365 7428 7472 6163 6b5f 6461 7461  taset(track_data
-0001a140: 7365 742c 2074 7261 636b 5f61 6e61 6c79  set, track_analy
-0001a150: 7369 735f 7370 6f74 5f6b 6579 732c 2074  sis_spot_keys, t
-0001a160: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
-0001a170: 6163 6b5f 6b65 7973 2c20 5472 6163 6b41  ack_keys, TrackA
-0001a180: 7474 7269 6275 7465 426f 786e 616d 6529  ttributeBoxname)
-0001a190: 3a0d 0a0d 0a20 2020 2020 2020 2041 6c6c  :....        All
-0001a1a0: 5472 6163 6b56 616c 7565 7320 3d20 7b7d  TrackValues = {}
-0001a1b0: 0d0a 2020 2020 2020 2020 7472 6163 6b5f  ..        track_
-0001a1c0: 6964 203d 2074 7261 636b 5f61 6e61 6c79  id = track_analy
-0001a1d0: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
-0001a1e0: 7261 636b 5f69 6422 5d0d 0a20 2020 2020  rack_id"]..     
-0001a1f0: 2020 2054 6964 203d 2074 7261 636b 5f64     Tid = track_d
-0001a200: 6174 6173 6574 5b74 7261 636b 5f69 645d  ataset[track_id]
-0001a210: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a220: 0d0a 2020 2020 2020 200d 0a20 2020 2020  ..       ..     
-0001a230: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
-0001a240: 735b 7472 6163 6b5f 6964 5d20 3d20 5469  s[track_id] = Ti
-0001a250: 640d 0a20 2020 2020 200d 0a20 2020 2020  d..      ..     
-0001a260: 2020 2066 6f72 2028 6b2c 2076 2920 696e     for (k, v) in
-0001a270: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a280: 7472 6163 6b5f 6b65 7973 2e69 7465 6d73  track_keys.items
-0001a290: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
-0001a2a0: 2020 2020 2020 2078 203d 2074 7261 636b         x = track
-0001a2b0: 5f64 6174 6173 6574 5b76 5d2e 6173 7479  _dataset[v].asty
-0001a2c0: 7065 2822 666c 6f61 7422 290d 0a20 2020  pe("float")..   
-0001a2d0: 2020 2020 2020 2020 2020 2020 206d 696e               min
-0001a2e0: 7661 6c20 3d20 6d69 6e28 7829 0d0a 2020  val = min(x)..  
-0001a2f0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0001a300: 7876 616c 203d 206d 6178 2878 290d 0a0d  xval = max(x)...
-0001a310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a320: 2069 6620 6d69 6e76 616c 203e 2030 2061   if minval > 0 a
-0001a330: 6e64 206d 6178 7661 6c20 3c3d 2031 3a0d  nd maxval <= 1:.
-0001a340: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a350: 2020 2020 2020 2078 203d 2078 202b 2031         x = x + 1
-0001a360: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a370: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
-0001a380: 6573 5b6b 5d20 3d20 726f 756e 6428 782c  es[k] = round(x,
-0001a390: 2033 290d 0a0d 0a20 2020 2020 2020 2054   3)....        T
-0001a3a0: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-0001a3b0: 203d 205b 5d0d 0a20 2020 2020 2020 2054   = []..        T
-0001a3c0: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
-0001a3d0: 2e61 7070 656e 6428 5472 6163 6b41 7474  .append(TrackAtt
-0001a3e0: 7269 6275 7465 426f 786e 616d 6529 0d0a  ributeBoxname)..
-0001a3f0: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
-0001a400: 6962 7574 656e 616d 6520 696e 2074 7261  ibutename in tra
-0001a410: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
-0001a420: 6b5f 6b65 7973 2e6b 6579 7328 293a 0d0a  k_keys.keys():..
-0001a430: 2020 2020 2020 2020 2020 2020 5472 6163              Trac
-0001a440: 6b41 7474 7269 6275 7465 6964 732e 6170  kAttributeids.ap
-0001a450: 7065 6e64 2861 7474 7269 6275 7465 6e61  pend(attributena
-0001a460: 6d65 2920 2020 200d 0a20 2020 200d 0a20  me)    ..    .. 
-0001a470: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001a480: 6163 6b41 7474 7269 6275 7465 6964 732c  ackAttributeids,
-0001a490: 2041 6c6c 5472 6163 6b56 616c 7565 730d   AllTrackValues.
-0001a4a0: 0a20 2020 200d 0a64 6566 2067 6574 5f65  .    ..def get_e
-0001a4b0: 6467 6573 5f64 6174 6173 6574 2865 6467  dges_dataset(edg
-0001a4c0: 6573 5f64 6174 6173 6574 2c20 6564 6765  es_dataset, edge
-0001a4d0: 735f 6461 7461 7365 745f 696e 6465 782c  s_dataset_index,
-0001a4e0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a4f0: 7370 6f74 5f6b 6579 732c 2074 7261 636b  spot_keys, track
-0001a500: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
-0001a510: 6b65 7973 293a 0d0a 0d0a 2020 2020 2020  keys):....      
-0001a520: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
-0001a530: 203d 207b 7d0d 0a20 2020 2020 2020 2074   = {}..        t
-0001a540: 7261 636b 5f69 6420 3d20 7472 6163 6b5f  rack_id = track_
-0001a550: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001a560: 7973 5b22 7472 6163 6b5f 6964 225d 0d0a  ys["track_id"]..
-0001a570: 2020 2020 2020 2020 5469 6420 3d20 6564          Tid = ed
-0001a580: 6765 735f 6461 7461 7365 745b 7472 6163  ges_dataset[trac
-0001a590: 6b5f 6964 5d2e 6173 7479 7065 2822 666c  k_id].astype("fl
-0001a5a0: 6f61 7422 290d 0a20 2020 2020 2020 2069  oat")..        i
-0001a5b0: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
-0001a5c0: 6528 5469 6420 3d3d 2030 290d 0a20 2020  e(Tid == 0)..   
-0001a5d0: 2020 2020 206d 6178 7472 6163 6b5f 6964       maxtrack_id
-0001a5e0: 203d 206d 6178 2854 6964 290d 0a20 2020   = max(Tid)..   
-0001a5f0: 2020 2020 2063 6f6e 6469 7469 6f6e 5f69       condition_i
-0001a600: 6e64 6963 6573 203d 2065 6467 6573 5f64  ndices = edges_d
-0001a610: 6174 6173 6574 5f69 6e64 6578 5b69 6e64  ataset_index[ind
-0001a620: 6963 6573 5d0d 0a20 2020 2020 2020 2054  ices]..        T
-0001a630: 6964 5b63 6f6e 6469 7469 6f6e 5f69 6e64  id[condition_ind
-0001a640: 6963 6573 5d20 3d20 6d61 7874 7261 636b  ices] = maxtrack
-0001a650: 5f69 6420 2b20 310d 0a20 2020 2020 2020  _id + 1..       
-0001a660: 2041 6c6c 4564 6765 7356 616c 7565 735b   AllEdgesValues[
-0001a670: 7472 6163 6b5f 6964 5d20 3d20 5469 640d  track_id] = Tid.
-0001a680: 0a0d 0a20 2020 2020 2020 2066 6f72 206b  ...        for k
-0001a690: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
-0001a6a0: 6973 5f65 6467 6573 5f6b 6579 732e 7661  is_edges_keys.va
-0001a6b0: 6c75 6573 2829 3a0d 0a0d 0a20 2020 2020  lues():....     
-0001a6c0: 2020 2020 2020 2069 6620 6b20 213d 2074         if k != t
-0001a6d0: 7261 636b 5f69 643a 0d0a 2020 2020 2020  rack_id:..      
-0001a6e0: 2020 2020 2020 2020 2020 7820 3d20 6564            x = ed
-0001a6f0: 6765 735f 6461 7461 7365 745b 6b5d 2e61  ges_dataset[k].a
-0001a700: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001a710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a720: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
-0001a730: 5b6b 5d20 3d20 7820 2020 0d0a 2020 2020  [k] = x   ..    
-0001a740: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
-0001a750: 6574 7572 6e20 416c 6c45 6467 6573 5661  eturn AllEdgesVa
-0001a760: 6c75 6573 2020 200d 0a20 2020 200d 0a20  lues   ..    .. 
-0001a770: 2020 2020 2020 0d0a 2020 2020 0d0a 6465        ..    ..de
-0001a780: 6620 7363 616c 655f 7661 6c75 6528 782c  f scale_value(x,
-0001a790: 2073 6361 6c65 203d 2032 3535 202a 2032   scale = 255 * 2
-0001a7a0: 3535 293a 0d0a 0d0a 0d0a 2020 2020 2072  55):......     r
-0001a7b0: 6574 7572 6e20 7820 2a20 7363 616c 6520  eturn x * scale 
-0001a7c0: 2020 0d0a 2020 2020 0d0a 0d0a 0d0a 6465    ..    ......de
-0001a7d0: 6620 7072 6f62 5f73 6967 6d6f 6964 2878  f prob_sigmoid(x
-0001a7e0: 293a 0d0a 2020 2020 7265 7475 726e 2031  ):..    return 1
-0001a7f0: 202d 206d 6174 682e 6578 7028 2d78 290d   - math.exp(-x).
-0001a800: 0a0d 0a0d 0a64 6566 2061 6e67 756c 6172  .....def angular
-0001a810: 5f63 6861 6e67 6528 7665 635f 302c 2076  _change(vec_0, v
-0001a820: 6563 5f31 293a 0d0a 2020 2020 2020 2020  ec_1):..        
-0001a830: 0d0a 2020 2020 2020 2020 7665 635f 3020  ..        vec_0 
-0001a840: 3d20 7665 635f 3020 2f20 6e70 2e6c 696e  = vec_0 / np.lin
-0001a850: 616c 672e 6e6f 726d 2876 6563 5f30 290d  alg.norm(vec_0).
-0001a860: 0a20 2020 2020 2020 2076 6563 5f31 203d  .        vec_1 =
-0001a870: 2076 6563 5f31 202f 206e 702e 6c69 6e61   vec_1 / np.lina
-0001a880: 6c67 2e6e 6f72 6d28 7665 635f 3129 0d0a  lg.norm(vec_1)..
-0001a890: 2020 2020 2020 2020 616e 676c 6520 3d20          angle = 
-0001a8a0: 6e70 2e61 7263 636f 7328 6e70 2e63 6c69  np.arccos(np.cli
-0001a8b0: 7028 6e70 2e64 6f74 2876 6563 5f30 2c20  p(np.dot(vec_0, 
-0001a8c0: 7665 635f 3129 2c20 2d31 2e30 2c20 312e  vec_1), -1.0, 1.
-0001a8d0: 3029 290d 0a20 2020 2020 2020 2061 6e67  0))..        ang
-0001a8e0: 6c65 203d 2061 6e67 6c65 202a 2031 3830  le = angle * 180
-0001a8f0: 202f 206e 702e 7069 0d0a 2020 2020 2020   / np.pi..      
-0001a900: 2020 7265 7475 726e 2061 6e67 6c65 0d0a    return angle..
-0001a910: 2020 2020 200d 0a0d 0a64 6566 2065 7661       ....def eva
-0001a920: 6c5f 626f 6f6c 2876 616c 7565 293a 0d0a  l_bool(value):..
-0001a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a940: 2020 0d0a 2020 2020 2020 2020 6966 2076    ..        if v
-0001a950: 616c 7565 2020 3d3d 2027 5472 7565 273a  alue  == 'True':
-0001a960: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0001a970: 2020 2064 6976 5f6b 6579 203d 2054 7275     div_key = Tru
-0001a980: 650d 0a20 2020 2020 2020 2065 6c73 653a  e..        else:
-0001a990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a9a0: 2020 6469 765f 6b65 7920 3d20 4661 6c73    div_key = Fals
-0001a9b0: 6520 0d0a 0d0a 2020 2020 2020 2020 7265  e ....        re
-0001a9c0: 7475 726e 2064 6976 5f6b 6579 2020 2020  turn div_key    
-0001a9d0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-0001a9e0: 6465 6620 6368 6563 6b5f 616e 645f 7570  def check_and_up
-0001a9f0: 6461 7465 5f6d 6173 6b28 6d61 736b 2c69  date_mask(mask,i
-0001aa00: 6d61 6765 293a 0d0a 2020 2020 2020 200d  mage):..       .
-0001aa10: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0001aa20: 6d61 736b 2e73 6861 7065 2920 3c20 6c65  mask.shape) < le
-0001aa30: 6e28 696d 6167 652e 7368 6170 6529 3a0d  n(image.shape):.
-0001aa40: 0a20 2020 2020 2020 2020 2020 2075 7064  .            upd
-0001aa50: 6174 655f 6d61 736b 203d 206e 702e 7a65  ate_mask = np.ze
-0001aa60: 726f 7328 0d0a 2020 2020 2020 2020 2020  ros(..          
-0001aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa80: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
+00018b90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00018ba0: 200d 0a64 6566 2062 6f75 6e64 6172 795f   ..def boundary_
+00018bb0: 706f 696e 7473 286d 6173 6b2c 2078 6361  points(mask, xca
+00018bc0: 6c69 6272 6174 696f 6e2c 2079 6361 6c69  libration, ycali
+00018bd0: 6272 6174 696f 6e2c 207a 6361 6c69 6272  bration, zcalibr
+00018be0: 6174 696f 6e29 3a0d 0a0d 0a20 2020 206e  ation):....    n
+00018bf0: 6469 6d20 3d20 6c65 6e28 6d61 736b 2e73  dim = len(mask.s
+00018c00: 6861 7065 290d 0a20 2020 2074 696d 6564  hape)..    timed
+00018c10: 5f6d 6173 6b20 3d20 7b7d 0d0a 2020 2020  _mask = {}..    
+00018c20: 6d61 736b 203d 206d 6173 6b20 3e20 300d  mask = mask > 0.
+00018c30: 0a20 2020 206d 6173 6b20 3d20 6d61 736b  .    mask = mask
+00018c40: 2e61 7374 7970 6528 2775 696e 7438 2729  .astype('uint8')
+00018c50: 0d0a 2020 2020 2320 5958 2073 6861 7065  ..    # YX shape
+00018c60: 6420 6f62 6a65 6374 0d0a 2020 2020 6966  d object..    if
+00018c70: 206e 6469 6d20 3d3d 2032 3a0d 0a20 2020   ndim == 2:..   
+00018c80: 2020 2020 200d 0a20 2020 2020 2020 2062       ..        b
+00018c90: 6f75 6e64 6172 7920 3d20 6669 6e64 5f62  oundary = find_b
+00018ca0: 6f75 6e64 6172 6965 7328 6d61 736b 290d  oundaries(mask).
+00018cb0: 0a20 2020 2020 2020 2072 6567 696f 6e63  .        regionc
+00018cc0: 656e 7472 6f69 6420 3d20 2830 2c29 202b  entroid = (0,) +
+00018cd0: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
+00018ce0: 6428 626f 756e 6461 7279 2920 0d0a 2020  d(boundary) ..  
+00018cf0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+00018d00: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
+00018d10: 7920 3e20 3029 0d0a 2020 2020 2020 2020  y > 0)..        
+00018d20: 7265 616c 5f69 6e64 6963 6573 203d 206e  real_indices = n
+00018d30: 702e 7472 616e 7370 6f73 6528 6e70 2e61  p.transpose(np.a
+00018d40: 7361 7272 6179 2869 6e64 6963 6573 2929  sarray(indices))
+00018d50: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
+00018d60: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+00018d70: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
+00018d80: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
+00018d90: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+00018da0: 6963 6573 5b6a 5d5b 305d 203d 2072 6561  ices[j][0] = rea
+00018db0: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+00018dc0: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
+00018dd0: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00018de0: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
+00018df0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00018e00: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
+00018e10: 6f6e 0d0a 0d0a 2020 2020 2020 2020 7472  on....        tr
+00018e20: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
+00018e30: 5472 6565 2872 6561 6c5f 696e 6469 6365  Tree(real_indice
+00018e40: 7329 0d0a 2020 2020 2020 2020 2320 5468  s)..        # Th
+00018e50: 6973 206f 626a 6563 7420 636f 6e74 6169  is object contai
+00018e60: 6e73 206c 6973 7420 6f66 2061 6c6c 2074  ns list of all t
+00018e70: 6865 2070 6f69 6e74 7320 666f 7220 616c  he points for al
+00018e80: 6c20 7468 6520 6c61 6265 6c73 2069 6e20  l the labels in 
+00018e90: 7468 6520 4d61 736b 2069 6d61 6765 2077  the Mask image w
+00018ea0: 6974 6820 7468 6520 6c61 6265 6c20 6964  ith the label id
+00018eb0: 2061 6e64 2076 6f6c 756d 6520 6f66 2065   and volume of e
+00018ec0: 6163 6820 6c61 6265 6c0d 0a20 2020 2020  ach label..     
+00018ed0: 2020 2074 696d 6564 5f6d 6173 6b5b 7374     timed_mask[st
+00018ee0: 7228 3029 5d20 3d20 5b74 7265 652c 2069  r(0)] = [tree, i
+00018ef0: 6e64 6963 6573 2c20 7265 6769 6f6e 6365  ndices, regionce
+00018f00: 6e74 726f 6964 5d0d 0a0d 0a20 2020 2023  ntroid]....    #
+00018f10: 2054 5958 2073 6861 7065 6420 6f62 6a65   TYX shaped obje
+00018f20: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
+00018f30: 3d3d 2033 3a0d 0a0d 0a0d 0a20 2020 2020  == 3:......     
+00018f40: 2020 2066 6f72 2069 2069 6e20 7471 646d     for i in tqdm
+00018f50: 2872 616e 6765 2830 2c20 6d61 736b 2e73  (range(0, mask.s
+00018f60: 6861 7065 5b30 5d29 293a 0d0a 2020 2020  hape[0])):..    
+00018f70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00018f80: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+00018f90: 756e 6461 7279 203d 2066 696e 645f 626f  undary = find_bo
+00018fa0: 756e 6461 7269 6573 286d 6173 6b5b 692c  undaries(mask[i,
+00018fb0: 3a5d 290d 0a20 2020 2020 2020 2020 2020  :])..           
+00018fc0: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
+00018fd0: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
+00018fe0: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
+00018ff0: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
+00019000: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+00019010: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+00019020: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
+00019030: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00019040: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
+00019050: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
+00019060: 6179 2869 6e64 6963 6573 2929 2e63 6f70  ay(indices)).cop
+00019070: 7928 290d 0a0d 0a20 2020 2020 2020 2020  y()....         
+00019080: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00019090: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
+000190a0: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
+000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190c0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+000190d0: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
+000190e0: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
+000190f0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019110: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+00019120: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
+00019130: 735b 6a5d 5b31 5d20 2a20 7863 616c 6962  s[j][1] * xcalib
+00019140: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
+00019150: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
+00019160: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+00019170: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
+00019180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019190: 2020 7469 6d65 645f 6d61 736b 5b73 7472    timed_mask[str
+000191a0: 2869 295d 203d 205b 7472 6565 2c20 696e  (i)] = [tree, in
+000191b0: 6469 6365 732c 2072 6567 696f 6e63 656e  dices, regioncen
+000191c0: 7472 6f69 645d 0d0a 2020 2020 2020 2020  troid]..        
+000191d0: 2020 2020 0d0a 2020 2020 2320 545a 5958      ..    # TZYX
+000191e0: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
+000191f0: 2020 2020 6966 206e 6469 6d20 3d3d 2034      if ndim == 4
+00019200: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+00019210: 2827 4d61 736b 7320 6d61 6465 2069 6e74  ('Masks made int
+00019220: 6f20 6120 3444 2063 796c 696e 6465 722c  o a 4D cylinder,
+00019230: 2075 7027 290d 0a20 2020 2020 2020 2062   up')..        b
+00019240: 6f75 6e64 6172 7920 3d20 6e70 2e7a 6572  oundary = np.zer
+00019250: 6f73 280d 0a20 2020 2020 2020 2020 2020  os(..           
+00019260: 205b 6d61 736b 2e73 6861 7065 5b30 5d2c   [mask.shape[0],
+00019270: 206d 6173 6b2e 7368 6170 655b 315d 2c20   mask.shape[1], 
+00019280: 6d61 736b 2e73 6861 7065 5b32 5d2c 206d  mask.shape[2], m
+00019290: 6173 6b2e 7368 6170 655b 335d 5d0d 0a20  ask.shape[3]].. 
+000192a0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000192b0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+000192c0: 2830 2c20 6d61 736b 2e73 6861 7065 5b30  (0, mask.shape[0
+000192d0: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+000192e0: 200d 0a20 2020 2020 2020 2020 2020 2062   ..            b
+000192f0: 6f75 6e64 6172 795b 692c 3a5d 203d 2066  oundary[i,:] = f
+00019300: 696e 645f 626f 756e 6461 7269 6573 286d  ind_boundaries(m
+00019310: 6173 6b5b 692c 3a5d 290d 0a20 2020 2020  ask[i,:])..     
+00019320: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
+00019330: 7472 6f69 6420 3d20 636f 6d70 7574 655f  troid = compute_
+00019340: 6365 6e74 726f 6964 2862 6f75 6e64 6172  centroid(boundar
+00019350: 795b 692c 3a5d 2920 0d0a 2020 2020 2020  y[i,:]) ..      
+00019360: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+00019370: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
+00019380: 795b 692c 3a5d 203e 2030 290d 0a20 2020  y[i,:] > 0)..   
+00019390: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+000193a0: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
+000193b0: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
+000193c0: 696e 6469 6365 7329 292e 636f 7079 2829  indices)).copy()
+000193d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000193e0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+000193f0: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
+00019400: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
+00019410: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00019420: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+00019430: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00019440: 5d5b 305d 202a 207a 6361 6c69 6272 6174  ][0] * zcalibrat
+00019450: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00019460: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00019470: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
+00019480: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+00019490: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
+000194a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000194b0: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+000194c0: 735b 6a5d 5b32 5d20 3d20 7265 616c 5f69  s[j][2] = real_i
+000194d0: 6e64 6963 6573 5b6a 5d5b 325d 202a 2078  ndices[j][2] * x
+000194e0: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
+000194f0: 2020 2020 2020 2020 2020 2074 7265 6520             tree 
+00019500: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
+00019510: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
+00019520: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00019530: 6564 5f6d 6173 6b5b 7374 7228 6929 5d20  ed_mask[str(i)] 
+00019540: 3d20 5b74 7265 652c 2069 6e64 6963 6573  = [tree, indices
+00019550: 2c20 7265 6769 6f6e 6365 6e74 726f 6964  , regioncentroid
+00019560: 5d0d 0a20 2020 2070 7269 6e74 2827 436f  ]..    print('Co
+00019570: 6d70 7574 6564 2074 6865 2062 6f75 6e64  mputed the bound
+00019580: 6172 7920 706f 696e 7473 2729 0d0a 0d0a  ary points')....
+00019590: 2020 2020 7265 7475 726e 2074 696d 6564      return timed
+000195a0: 5f6d 6173 6b2c 2062 6f75 6e64 6172 7920  _mask, boundary 
+000195b0: 2020 2020 2020 200d 0a0d 0a64 6566 2063         ....def c
+000195c0: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
+000195d0: 6269 6e61 7279 5f69 6d61 6765 293a 0d0a  binary_image):..
+000195e0: 2020 2020 2320 456e 7375 7265 2062 696e      # Ensure bin
+000195f0: 6172 7920 696d 6167 6520 6973 2061 204e  ary image is a N
+00019600: 756d 5079 2061 7272 6179 0d0a 2020 2020  umPy array..    
+00019610: 6269 6e61 7279 5f69 6d61 6765 203d 206e  binary_image = n
+00019620: 702e 6172 7261 7928 6269 6e61 7279 5f69  p.array(binary_i
+00019630: 6d61 6765 290d 0a0d 0a20 2020 2077 6869  mage)....    whi
+00019640: 7465 5f70 6978 656c 7320 3d20 6e70 2e77  te_pixels = np.w
+00019650: 6865 7265 2862 696e 6172 795f 696d 6167  here(binary_imag
+00019660: 6520 3d3d 2031 290d 0a20 2020 206e 756d  e == 1)..    num
+00019670: 5f70 6978 656c 7320 3d20 6c65 6e28 7768  _pixels = len(wh
+00019680: 6974 655f 7069 7865 6c73 5b30 5d29 0d0a  ite_pixels[0])..
+00019690: 0d0a 2020 2020 2320 436f 6d70 7574 6520  ..    # Compute 
+000196a0: 7468 6520 6365 6e74 726f 6964 206f 6620  the centroid of 
+000196b0: 7468 6520 7768 6974 6520 7069 7865 6c73  the white pixels
+000196c0: 2069 6e20 7468 6520 626f 756e 6461 7279   in the boundary
+000196d0: 2069 6d61 6765 0d0a 2020 2020 6365 6e74   image..    cent
+000196e0: 726f 6964 203d 206e 702e 7a65 726f 7328  roid = np.zeros(
+000196f0: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
+00019700: 6d29 0d0a 2020 2020 666f 7220 6469 6d20  m)..    for dim 
+00019710: 696e 2072 616e 6765 2862 696e 6172 795f  in range(binary_
+00019720: 696d 6167 652e 6e64 696d 293a 0d0a 2020  image.ndim):..  
+00019730: 2020 2020 2020 6365 6e74 726f 6964 5b64        centroid[d
+00019740: 696d 5d20 3d20 7768 6974 655f 7069 7865  im] = white_pixe
+00019750: 6c73 5b64 696d 5d2e 7375 6d28 2920 2f20  ls[dim].sum() / 
+00019760: 6e75 6d5f 7069 7865 6c73 0d0a 0d0a 2020  num_pixels....  
+00019770: 2020 7265 7475 726e 2063 656e 7472 6f69    return centroi
+00019780: 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465  d........ ....de
+00019790: 6620 6765 745f 6373 765f 6461 7461 2863  f get_csv_data(c
+000197a0: 7376 293a 0d0a 0d0a 2020 2020 2020 2020  sv):....        
+000197b0: 6461 7461 7365 7420 3d20 7064 2e72 6561  dataset = pd.rea
+000197c0: 645f 6373 7628 0d0a 2020 2020 2020 2020  d_csv(..        
+000197d0: 2020 2020 6373 762c 2064 656c 696d 6974      csv, delimit
+000197e0: 6572 3d22 2c22 2c20 656e 636f 6469 6e67  er=",", encoding
+000197f0: 3d22 756e 6963 6f64 655f 6573 6361 7065  ="unicode_escape
+00019800: 222c 206c 6f77 5f6d 656d 6f72 793d 4661  ", low_memory=Fa
+00019810: 6c73 650d 0a20 2020 2020 2020 2029 5b33  lse..        )[3
+00019820: 3a5d 0d0a 2020 2020 2020 2020 6461 7461  :]..        data
+00019830: 7365 745f 696e 6465 7820 3d20 6461 7461  set_index = data
+00019840: 7365 742e 696e 6465 780d 0a20 2020 2020  set.index..     
+00019850: 2020 2072 6574 7572 6e20 6461 7461 7365     return datase
+00019860: 742c 2064 6174 6173 6574 5f69 6e64 6578  t, dataset_index
+00019870: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+00019880: 7370 6f74 5f64 6174 6173 6574 2873 706f  spot_dataset(spo
+00019890: 745f 6461 7461 7365 742c 2074 7261 636b  t_dataset, track
+000198a0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+000198b0: 6579 732c 2078 6361 6c69 6272 6174 696f  eys, xcalibratio
+000198c0: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
+000198d0: 207a 6361 6c69 6272 6174 696f 6e2c 2041   zcalibration, A
+000198e0: 7474 7269 6275 7465 426f 786e 616d 652c  ttributeBoxname,
+000198f0: 2064 6574 6563 7469 6f6e 6368 616e 6e65   detectionchanne
+00019900: 6c29 3a0d 0a20 2020 2020 2020 2041 6c6c  l):..        All
+00019910: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
+00019920: 2020 2020 2070 6f73 6978 203d 2074 7261       posix = tra
+00019930: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00019940: 5f6b 6579 735b 2270 6f73 6978 225d 0d0a  _keys["posix"]..
+00019950: 2020 2020 2020 2020 706f 7369 7920 3d20          posiy = 
+00019960: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00019970: 706f 745f 6b65 7973 5b22 706f 7369 7922  pot_keys["posiy"
+00019980: 5d0d 0a20 2020 2020 2020 2070 6f73 697a  ]..        posiz
+00019990: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+000199a0: 735f 7370 6f74 5f6b 6579 735b 2270 6f73  s_spot_keys["pos
+000199b0: 697a 225d 0d0a 2020 2020 2020 2020 6672  iz"]..        fr
+000199c0: 616d 6520 3d20 7472 6163 6b5f 616e 616c  ame = track_anal
+000199d0: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+000199e0: 6672 616d 6522 5d0d 0a20 2020 2020 2020  frame"]..       
+000199f0: 200d 0a20 2020 2020 2020 204c 6f63 6174   ..        Locat
+00019a00: 696f 6e58 203d 2028 0d0a 2020 2020 2020  ionX = (..      
+00019a10: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+00019a20: 6574 5b70 6f73 6978 5d2e 6173 7479 7065  et[posix].astype
+00019a30: 2822 666c 6f61 7422 2920 2f20 7863 616c  ("float") / xcal
+00019a40: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00019a50: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+00019a60: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+00019a70: 696f 6e59 203d 2028 0d0a 2020 2020 2020  ionY = (..      
+00019a80: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+00019a90: 6574 5b70 6f73 6979 5d2e 6173 7479 7065  et[posiy].astype
+00019aa0: 2822 666c 6f61 7422 2920 2f20 7963 616c  ("float") / ycal
+00019ab0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00019ac0: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+00019ad0: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+00019ae0: 696f 6e5a 203d 2028 0d0a 2020 2020 2020  ionZ = (..      
+00019af0: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+00019b00: 6574 5b70 6f73 697a 5d2e 6173 7479 7065  et[posiz].astype
+00019b10: 2822 666c 6f61 7422 2920 2f20 7a63 616c  ("float") / zcal
+00019b20: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00019b30: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+00019b40: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+00019b50: 696f 6e54 203d 2028 7370 6f74 5f64 6174  ionT = (spot_dat
+00019b60: 6173 6574 5b66 7261 6d65 5d2e 6173 7479  aset[frame].asty
+00019b70: 7065 2822 666c 6f61 7422 2929 2e61 7374  pe("float")).ast
+00019b80: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+00019b90: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00019ba0: 6967 6e6f 7265 5f76 616c 7565 7320 3d20  ignore_values = 
+00019bb0: 5b74 7261 636b 5f61 6e61 6c79 7369 735f  [track_analysis_
+00019bc0: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
+00019bd0: 696e 7465 6e73 6974 7922 5d2c 7472 6163  intensity"],trac
+00019be0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+00019bf0: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
+00019c00: 6e73 6974 7922 5d5d 200d 0a20 2020 2020  nsity"]] ..     
+00019c10: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+00019c20: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00019c30: 706f 745f 6b65 7973 2e69 7465 6d73 2829  pot_keys.items()
+00019c40: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+00019c50: 2020 2020 2069 6620 6465 7465 6374 696f       if detectio
+00019c60: 6e63 6861 6e6e 656c 203d 3d20 313a 0d0a  nchannel == 1:..
+00019c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c80: 2020 2020 2069 6620 6b20 3d3d 2022 6d65       if k == "me
+00019c90: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
+00019ca0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00019cb0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00019cc0: 616c 7565 203d 2074 7261 636b 5f61 6e61  alue = track_ana
+00019cd0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+00019ce0: 226d 6561 6e5f 696e 7465 6e73 6974 7922  "mean_intensity"
+00019cf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00019d00: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+00019d10: 6c56 616c 7565 735b 7661 6c75 655d 203d  lValues[value] =
+00019d20: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
+00019d30: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
+00019d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019d50: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
+00019d60: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+00019d70: 6368 3222 3a0d 0a20 2020 2020 2020 2020  ch2":..         
+00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d90: 2020 7661 6c75 6520 3d20 7472 6163 6b5f    value = track_
+00019da0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00019db0: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
+00019dc0: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
+00019dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019de0: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
+00019df0: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
+00019e00: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
+00019e10: 6174 2229 2020 2020 2020 200d 0a0d 0a20  at")       .... 
+00019e20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019e30: 6620 7620 6e6f 7420 696e 2069 676e 6f72  f v not in ignor
+00019e40: 655f 7661 6c75 6573 3a0d 0a20 2020 2020  e_values:..     
+00019e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e60: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00019e70: 2020 2020 2020 2020 2020 2041 6c6c 5661             AllVa
+00019e80: 6c75 6573 5b76 5d20 3d20 7370 6f74 5f64  lues[v] = spot_d
+00019e90: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
+00019ea0: 2822 666c 6f61 7422 290d 0a0d 0a20 2020  ("float")....   
+00019eb0: 2020 2020 2041 6c6c 5661 6c75 6573 5b70       AllValues[p
+00019ec0: 6f73 6978 5d20 3d20 726f 756e 6428 4c6f  osix] = round(Lo
+00019ed0: 6361 7469 6f6e 582c 3329 0d0a 2020 2020  cationX,3)..    
+00019ee0: 2020 2020 416c 6c56 616c 7565 735b 706f      AllValues[po
+00019ef0: 7369 795d 203d 2072 6f75 6e64 284c 6f63  siy] = round(Loc
+00019f00: 6174 696f 6e59 2c33 290d 0a20 2020 2020  ationY,3)..     
+00019f10: 2020 2041 6c6c 5661 6c75 6573 5b70 6f73     AllValues[pos
+00019f20: 697a 5d20 3d20 726f 756e 6428 4c6f 6361  iz] = round(Loca
+00019f30: 7469 6f6e 5a2c 3329 0d0a 2020 2020 2020  tionZ,3)..      
+00019f40: 2020 416c 6c56 616c 7565 735b 6672 616d    AllValues[fram
+00019f50: 655d 203d 2072 6f75 6e64 284c 6f63 6174  e] = round(Locat
+00019f60: 696f 6e54 2c33 290d 0a20 2020 2020 2020  ionT,3)..       
+00019f70: 2041 7474 7269 6275 7465 6964 7320 3d20   Attributeids = 
+00019f80: 5b5d 0d0a 2020 2020 2020 2020 4174 7472  []..        Attr
+00019f90: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
+00019fa0: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
+00019fb0: 290d 0a20 2020 2020 2020 2066 6f72 2061  )..        for a
+00019fc0: 7474 7269 6275 7465 6e61 6d65 2069 6e20  ttributename in 
+00019fd0: 416c 6c56 616c 7565 732e 6b65 7973 2829  AllValues.keys()
+00019fe0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00019ff0: 2041 7474 7269 6275 7465 6964 732e 6170   Attributeids.ap
+0001a000: 7065 6e64 2861 7474 7269 6275 7465 6e61  pend(attributena
+0001a010: 6d65 2920 2020 200d 0a20 2020 2020 2020  me)    ..       
+0001a020: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
+0001a030: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a040: 4174 7472 6962 7574 6569 6473 2c20 416c  Attributeids, Al
+0001a050: 6c56 616c 7565 7320 2020 2020 0d0a 2020  lValues     ..  
+0001a060: 2020 0d0a 6465 6620 6765 745f 7472 6163    ..def get_trac
+0001a070: 6b5f 6461 7461 7365 7428 7472 6163 6b5f  k_dataset(track_
+0001a080: 6461 7461 7365 742c 2074 7261 636b 5f61  dataset, track_a
+0001a090: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001a0a0: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
+0001a0b0: 735f 7472 6163 6b5f 6b65 7973 2c20 5472  s_track_keys, Tr
+0001a0c0: 6163 6b41 7474 7269 6275 7465 426f 786e  ackAttributeBoxn
+0001a0d0: 616d 6529 3a0d 0a0d 0a20 2020 2020 2020  ame):....       
+0001a0e0: 2041 6c6c 5472 6163 6b56 616c 7565 7320   AllTrackValues 
+0001a0f0: 3d20 7b7d 0d0a 2020 2020 2020 2020 7472  = {}..        tr
+0001a100: 6163 6b5f 6964 203d 2074 7261 636b 5f61  ack_id = track_a
+0001a110: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001a120: 735b 2274 7261 636b 5f69 6422 5d0d 0a20  s["track_id"].. 
+0001a130: 2020 2020 2020 2054 6964 203d 2074 7261         Tid = tra
+0001a140: 636b 5f64 6174 6173 6574 5b74 7261 636b  ck_dataset[track
+0001a150: 5f69 645d 2e61 7374 7970 6528 2266 6c6f  _id].astype("flo
+0001a160: 6174 2229 0d0a 2020 2020 2020 200d 0a20  at")..       .. 
+0001a170: 2020 2020 2020 2041 6c6c 5472 6163 6b56         AllTrackV
+0001a180: 616c 7565 735b 7472 6163 6b5f 6964 5d20  alues[track_id] 
+0001a190: 3d20 5469 640d 0a20 2020 2020 200d 0a20  = Tid..      .. 
+0001a1a0: 2020 2020 2020 2066 6f72 2028 6b2c 2076         for (k, v
+0001a1b0: 2920 696e 2074 7261 636b 5f61 6e61 6c79  ) in track_analy
+0001a1c0: 7369 735f 7472 6163 6b5f 6b65 7973 2e69  sis_track_keys.i
+0001a1d0: 7465 6d73 2829 3a0d 0a0d 0a20 2020 2020  tems():....     
+0001a1e0: 2020 2020 2020 2020 2020 2078 203d 2074             x = t
+0001a1f0: 7261 636b 5f64 6174 6173 6574 5b76 5d2e  rack_dataset[v].
+0001a200: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001a210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a220: 206d 696e 7661 6c20 3d20 6d69 6e28 7829   minval = min(x)
+0001a230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a240: 2020 6d61 7876 616c 203d 206d 6178 2878    maxval = max(x
+0001a250: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0001a260: 2020 2020 2069 6620 6d69 6e76 616c 203e       if minval >
+0001a270: 2030 2061 6e64 206d 6178 7661 6c20 3c3d   0 and maxval <=
+0001a280: 2031 3a0d 0a0d 0a20 2020 2020 2020 2020   1:....         
+0001a290: 2020 2020 2020 2020 2020 2078 203d 2078             x = x
+0001a2a0: 202b 2031 0d0a 0d0a 2020 2020 2020 2020   + 1....        
+0001a2b0: 2020 2020 2020 2020 416c 6c54 7261 636b          AllTrack
+0001a2c0: 5661 6c75 6573 5b6b 5d20 3d20 726f 756e  Values[k] = roun
+0001a2d0: 6428 782c 2033 290d 0a0d 0a20 2020 2020  d(x, 3)....     
+0001a2e0: 2020 2054 7261 636b 4174 7472 6962 7574     TrackAttribut
+0001a2f0: 6569 6473 203d 205b 5d0d 0a20 2020 2020  eids = []..     
+0001a300: 2020 2054 7261 636b 4174 7472 6962 7574     TrackAttribut
+0001a310: 6569 6473 2e61 7070 656e 6428 5472 6163  eids.append(Trac
+0001a320: 6b41 7474 7269 6275 7465 426f 786e 616d  kAttributeBoxnam
+0001a330: 6529 0d0a 2020 2020 2020 2020 666f 7220  e)..        for 
+0001a340: 6174 7472 6962 7574 656e 616d 6520 696e  attributename in
+0001a350: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a360: 7472 6163 6b5f 6b65 7973 2e6b 6579 7328  track_keys.keys(
+0001a370: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001a380: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001a390: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
+0001a3a0: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
+0001a3b0: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+0001a3c0: 6e20 5472 6163 6b41 7474 7269 6275 7465  n TrackAttribute
+0001a3d0: 6964 732c 2041 6c6c 5472 6163 6b56 616c  ids, AllTrackVal
+0001a3e0: 7565 730d 0a20 2020 200d 0a64 6566 2067  ues..    ..def g
+0001a3f0: 6574 5f65 6467 6573 5f64 6174 6173 6574  et_edges_dataset
+0001a400: 2865 6467 6573 5f64 6174 6173 6574 2c20  (edges_dataset, 
+0001a410: 6564 6765 735f 6461 7461 7365 745f 696e  edges_dataset_in
+0001a420: 6465 782c 2074 7261 636b 5f61 6e61 6c79  dex, track_analy
+0001a430: 7369 735f 7370 6f74 5f6b 6579 732c 2074  sis_spot_keys, t
+0001a440: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
+0001a450: 6765 735f 6b65 7973 293a 0d0a 0d0a 2020  ges_keys):....  
+0001a460: 2020 2020 2020 416c 6c45 6467 6573 5661        AllEdgesVa
+0001a470: 6c75 6573 203d 207b 7d0d 0a20 2020 2020  lues = {}..     
+0001a480: 2020 2074 7261 636b 5f69 6420 3d20 7472     track_id = tr
+0001a490: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+0001a4a0: 745f 6b65 7973 5b22 7472 6163 6b5f 6964  t_keys["track_id
+0001a4b0: 225d 0d0a 2020 2020 2020 2020 5469 6420  "]..        Tid 
+0001a4c0: 3d20 6564 6765 735f 6461 7461 7365 745b  = edges_dataset[
+0001a4d0: 7472 6163 6b5f 6964 5d2e 6173 7479 7065  track_id].astype
+0001a4e0: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
+0001a4f0: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
+0001a500: 7768 6572 6528 5469 6420 3d3d 2030 290d  where(Tid == 0).
+0001a510: 0a20 2020 2020 2020 206d 6178 7472 6163  .        maxtrac
+0001a520: 6b5f 6964 203d 206d 6178 2854 6964 290d  k_id = max(Tid).
+0001a530: 0a20 2020 2020 2020 2063 6f6e 6469 7469  .        conditi
+0001a540: 6f6e 5f69 6e64 6963 6573 203d 2065 6467  on_indices = edg
+0001a550: 6573 5f64 6174 6173 6574 5f69 6e64 6578  es_dataset_index
+0001a560: 5b69 6e64 6963 6573 5d0d 0a20 2020 2020  [indices]..     
+0001a570: 2020 2054 6964 5b63 6f6e 6469 7469 6f6e     Tid[condition
+0001a580: 5f69 6e64 6963 6573 5d20 3d20 6d61 7874  _indices] = maxt
+0001a590: 7261 636b 5f69 6420 2b20 310d 0a20 2020  rack_id + 1..   
+0001a5a0: 2020 2020 2041 6c6c 4564 6765 7356 616c       AllEdgesVal
+0001a5b0: 7565 735b 7472 6163 6b5f 6964 5d20 3d20  ues[track_id] = 
+0001a5c0: 5469 640d 0a0d 0a20 2020 2020 2020 2066  Tid....        f
+0001a5d0: 6f72 206b 2069 6e20 7472 6163 6b5f 616e  or k in track_an
+0001a5e0: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
+0001a5f0: 732e 7661 6c75 6573 2829 3a0d 0a0d 0a20  s.values():.... 
+0001a600: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+0001a610: 213d 2074 7261 636b 5f69 643a 0d0a 2020  != track_id:..  
+0001a620: 2020 2020 2020 2020 2020 2020 2020 7820                x 
+0001a630: 3d20 6564 6765 735f 6461 7461 7365 745b  = edges_dataset[
+0001a640: 6b5d 2e61 7374 7970 6528 2266 6c6f 6174  k].astype("float
+0001a650: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
+0001a660: 2020 2020 2020 416c 6c45 6467 6573 5661        AllEdgesVa
+0001a670: 6c75 6573 5b6b 5d20 3d20 7820 2020 0d0a  lues[k] = x   ..
+0001a680: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001a690: 2020 2072 6574 7572 6e20 416c 6c45 6467     return AllEdg
+0001a6a0: 6573 5661 6c75 6573 2020 200d 0a20 2020  esValues   ..   
+0001a6b0: 200d 0a20 2020 2020 2020 0d0a 2020 2020   ..       ..    
+0001a6c0: 0d0a 6465 6620 7363 616c 655f 7661 6c75  ..def scale_valu
+0001a6d0: 6528 782c 2073 6361 6c65 203d 2032 3535  e(x, scale = 255
+0001a6e0: 202a 2032 3535 293a 0d0a 0d0a 0d0a 2020   * 255):......  
+0001a6f0: 2020 2072 6574 7572 6e20 7820 2a20 7363     return x * sc
+0001a700: 616c 6520 2020 0d0a 2020 2020 0d0a 0d0a  ale   ..    ....
+0001a710: 0d0a 6465 6620 7072 6f62 5f73 6967 6d6f  ..def prob_sigmo
+0001a720: 6964 2878 293a 0d0a 2020 2020 7265 7475  id(x):..    retu
+0001a730: 726e 2031 202d 206d 6174 682e 6578 7028  rn 1 - math.exp(
+0001a740: 2d78 290d 0a0d 0a0d 0a64 6566 2061 6e67  -x)......def ang
+0001a750: 756c 6172 5f63 6861 6e67 6528 7665 635f  ular_change(vec_
+0001a760: 302c 2076 6563 5f31 293a 0d0a 2020 2020  0, vec_1):..    
+0001a770: 2020 2020 0d0a 2020 2020 2020 2020 7665      ..        ve
+0001a780: 635f 3020 3d20 7665 635f 3020 2f20 6e70  c_0 = vec_0 / np
+0001a790: 2e6c 696e 616c 672e 6e6f 726d 2876 6563  .linalg.norm(vec
+0001a7a0: 5f30 290d 0a20 2020 2020 2020 2076 6563  _0)..        vec
+0001a7b0: 5f31 203d 2076 6563 5f31 202f 206e 702e  _1 = vec_1 / np.
+0001a7c0: 6c69 6e61 6c67 2e6e 6f72 6d28 7665 635f  linalg.norm(vec_
+0001a7d0: 3129 0d0a 2020 2020 2020 2020 616e 676c  1)..        angl
+0001a7e0: 6520 3d20 6e70 2e61 7263 636f 7328 6e70  e = np.arccos(np
+0001a7f0: 2e63 6c69 7028 6e70 2e64 6f74 2876 6563  .clip(np.dot(vec
+0001a800: 5f30 2c20 7665 635f 3129 2c20 2d31 2e30  _0, vec_1), -1.0
+0001a810: 2c20 312e 3029 290d 0a20 2020 2020 2020  , 1.0))..       
+0001a820: 2061 6e67 6c65 203d 2061 6e67 6c65 202a   angle = angle *
+0001a830: 2031 3830 202f 206e 702e 7069 0d0a 2020   180 / np.pi..  
+0001a840: 2020 2020 2020 7265 7475 726e 2061 6e67        return ang
+0001a850: 6c65 0d0a 2020 2020 200d 0a0d 0a64 6566  le..     ....def
+0001a860: 2065 7661 6c5f 626f 6f6c 2876 616c 7565   eval_bool(value
+0001a870: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001a880: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001a890: 6966 2076 616c 7565 2020 3d3d 2027 5472  if value  == 'Tr
+0001a8a0: 7565 273a 200d 0a20 2020 2020 2020 2020  ue': ..         
+0001a8b0: 2020 2020 2020 2064 6976 5f6b 6579 203d         div_key =
+0001a8c0: 2054 7275 650d 0a20 2020 2020 2020 2065   True..        e
+0001a8d0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0001a8e0: 2020 2020 2020 6469 765f 6b65 7920 3d20        div_key = 
+0001a8f0: 4661 6c73 6520 0d0a 0d0a 2020 2020 2020  False ....      
+0001a900: 2020 7265 7475 726e 2064 6976 5f6b 6579    return div_key
+0001a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a920: 0d0a 0d0a 6465 6620 6368 6563 6b5f 616e  ....def check_an
+0001a930: 645f 7570 6461 7465 5f6d 6173 6b28 6d61  d_update_mask(ma
+0001a940: 736b 2c69 6d61 6765 293a 0d0a 2020 2020  sk,image):..    
+0001a950: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+0001a960: 6c65 6e28 6d61 736b 2e73 6861 7065 2920  len(mask.shape) 
+0001a970: 3c20 6c65 6e28 696d 6167 652e 7368 6170  < len(image.shap
+0001a980: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+0001a990: 2075 7064 6174 655f 6d61 736b 203d 206e   update_mask = n
+0001a9a0: 702e 7a65 726f 7328 0d0a 2020 2020 2020  p.zeros(..      
+0001a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9c0: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+0001a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9e0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
+0001a9f0: 6861 7065 5b30 5d2c 0d0a 2020 2020 2020  hape[0],..      
+0001aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa10: 2020 2020 2020 2020 2020 696d 6167 652e            image.
+0001aa20: 7368 6170 655b 315d 2c0d 0a20 2020 2020  shape[1],..     
+0001aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa40: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+0001aa50: 2e73 6861 7065 5b32 5d2c 0d0a 2020 2020  .shape[2],..    
+0001aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa70: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+0001aa80: 652e 7368 6170 655b 335d 2c0d 0a20 2020  e.shape[3],..   
 0001aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aaa0: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
-0001aab0: 5b30 5d2c 0d0a 2020 2020 2020 2020 2020  [0],..          
-0001aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aad0: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
-0001aae0: 655b 315d 2c0d 0a20 2020 2020 2020 2020  e[1],..         
-0001aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab00: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001ab10: 7065 5b32 5d2c 0d0a 2020 2020 2020 2020  pe[2],..        
-0001ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab30: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001ab40: 6170 655b 335d 2c0d 0a20 2020 2020 2020  ape[3],..       
-0001ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab60: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-0001ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab80: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-0001ab90: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
-0001aba0: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
-0001abb0: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
-0001abc0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0001abd0: 6e20 7261 6e67 6528 302c 2075 7064 6174  n range(0, updat
-0001abe0: 655f 6d61 736b 2e73 6861 7065 5b31 5d29  e_mask.shape[1])
-0001abf0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-0001ac00: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-0001ac10: 6d61 736b 5b69 2c20 6a2c 203a 2c20 3a5d  mask[i, j, :, :]
-0001ac20: 203d 206d 6173 6b5b 692c 203a 2c20 3a5d   = mask[i, :, :]
-0001ac30: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0001ac40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ac50: 2075 7064 6174 655f 6d61 736b 203d 206d   update_mask = m
-0001ac60: 6173 6b0d 0a0d 0a20 2020 2020 2020 2072  ask....        r
-0001ac70: 6574 7572 6e20 7570 6461 7465 5f6d 6173  eturn update_mas
-0001ac80: 6b20 2020 2020 2020 200d 0a20 2020 2020  k        ..     
-0001ac90: 2020 0d0a                                  ..
+0001aaa0: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aac0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0001aad0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0001aae0: 6528 302c 2075 7064 6174 655f 6d61 736b  e(0, update_mask
+0001aaf0: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
+0001ab00: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001ab10: 206a 2069 6e20 7261 6e67 6528 302c 2075   j in range(0, u
+0001ab20: 7064 6174 655f 6d61 736b 2e73 6861 7065  pdate_mask.shape
+0001ab30: 5b31 5d29 3a0d 0a0d 0a20 2020 2020 2020  [1]):....       
+0001ab40: 2020 2020 2020 2020 2020 2020 2075 7064               upd
+0001ab50: 6174 655f 6d61 736b 5b69 2c20 6a2c 203a  ate_mask[i, j, :
+0001ab60: 2c20 3a5d 203d 206d 6173 6b5b 692c 203a  , :] = mask[i, :
+0001ab70: 2c20 3a5d 0d0a 2020 2020 2020 2020 656c  , :]..        el
+0001ab80: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0001ab90: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
+0001aba0: 203d 206d 6173 6b0d 0a0d 0a20 2020 2020   = mask....     
+0001abb0: 2020 2072 6574 7572 6e20 7570 6461 7465     return update
+0001abc0: 5f6d 6173 6b20 2020 2020 2020 200d 0a20  _mask        .. 
+0001abd0: 2020 2020 2020 0d0a                            ..
```

### Comparing `napatrackmater-3.3.8/napatrackmater/Trackvector.py` & `napatrackmater-3.3.9/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater/__init__.py` & `napatrackmater-3.3.9/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater/clustering.py` & `napatrackmater-3.3.9/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.3.9/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater/fate_mapping.py` & `napatrackmater-3.3.9/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater/pretrained.py` & `napatrackmater-3.3.9/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.3.9/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.3.8
+Version: 3.3.9
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.3.8/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.3.9/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.3.8/setup.py` & `napatrackmater-3.3.9/setup.py`

 * *Files identical despite different names*

