# Comparing `tmp/rankgun-1.0.1.tar.gz` & `tmp/rankgun-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankgun-1.0.1.tar", last modified: Sat Jul 23 00:58:29 2022, max compression
+gzip compressed data, was "rankgun-2.0.0.tar", last modified: Sun Apr 30 14:49:36 2023, max compression
```

## Comparing `rankgun-1.0.1.tar` & `rankgun-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-07-23 00:58:29.195421 rankgun-1.0.1/
--rw-rw-rw-   0        0        0    35857 2022-07-18 17:16:24.000000 rankgun-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      514 2022-07-23 00:58:29.196423 rankgun-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       87 2022-07-22 00:50:37.000000 rankgun-1.0.1/README.md
--rw-rw-rw-   0        0        0      108 2022-07-18 17:13:00.000000 rankgun-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      582 2022-07-23 00:58:29.243424 rankgun-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-23 00:58:28.800419 rankgun-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-07-23 00:58:28.936419 rankgun-1.0.1/src/rankgun/
--rw-rw-rw-   0        0        0     2165 2022-07-23 00:21:13.000000 rankgun-1.0.1/src/rankgun/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-23 00:58:29.188426 rankgun-1.0.1/src/rankgun.egg-info/
--rw-rw-rw-   0        0        0      514 2022-07-23 00:58:28.000000 rankgun-1.0.1/src/rankgun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2022-07-23 00:58:28.000000 rankgun-1.0.1/src/rankgun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-23 00:58:28.000000 rankgun-1.0.1/src/rankgun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-07-23 00:58:28.000000 rankgun-1.0.1/src/rankgun.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-23 00:58:28.000000 rankgun-1.0.1/src/rankgun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:49:36.745821 rankgun-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35852 2023-04-30 14:49:25.000000 rankgun-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-30 14:49:36.745821 rankgun-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-30 14:49:25.000000 rankgun-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 14:49:25.000000 rankgun-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-30 14:49:36.745821 rankgun-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:49:36.745821 rankgun-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:49:36.745821 rankgun-2.0.0/src/rankgun/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-30 14:49:25.000000 rankgun-2.0.0/src/rankgun/__innit__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:49:36.745821 rankgun-2.0.0/src/rankgun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-30 14:49:36.000000 rankgun-2.0.0/src/rankgun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 14:49:36.000000 rankgun-2.0.0/src/rankgun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:49:36.000000 rankgun-2.0.0/src/rankgun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 14:49:36.000000 rankgun-2.0.0/src/rankgun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 14:49:36.000000 rankgun-2.0.0/src/rankgun.egg-info/top_level.txt
```

### Comparing `rankgun-1.0.1/LICENSE` & `rankgun-2.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
     Rankgun
-    Copyright (C) CookieHax
+    Copyright (C) Noah-Haf
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU Affero General Public License as
     published by the Free Software Foundation version 3.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Affero General Public License for more details.
 
     You should have received a copy of the GNU Affero General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
-    
+
                         GNU AFFERO GENERAL PUBLIC LICENSE
                        Version 3, 19 November 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
```

### Comparing `rankgun-1.0.1/setup.cfg` & `rankgun-2.0.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2072 616e 6b67 756e 0d0a 7665 7273   = rankgun..vers
-00000020: 696f 6e20 3d20 312e 302e 310d 0a61 7574  ion = 1.0.1..aut
-00000030: 686f 7220 3d20 436f 6f6b 6965 5f44 6576  hor = Cookie_Dev
-00000040: 580d 0a61 7574 686f 725f 656d 6169 6c20  X..author_email 
-00000050: 3d20 526f 626c 6f78 436f 6f6b 6965 5f44  = RobloxCookie_D
-00000060: 6576 5840 6f75 746c 6f6f 6b2e 636f 6d0d  evX@outlook.com.
-00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2068  .description = h
-00000080: 7474 7073 3a2f 2f72 616e 6b67 756e 2e77  ttps://rankgun.w
-00000090: 6f72 6b73 0d0a 6c6f 6e67 5f64 6573 6372  orks..long_descr
-000000a0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
-000000b0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
-000000c0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
-000000d0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
-000000e0: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
-000000f0: 7474 7073 3a2f 2f72 616e 6b67 756e 2e77  ttps://rankgun.w
-00000100: 6f72 6b73 0d0a 636c 6173 7369 6669 6572  orks..classifier
-00000110: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
-00000120: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000130: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-00000140: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000150: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-00000160: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-00000170: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000180: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-00000190: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-000001a0: 6972 203d 200d 0a09 3d20 7372 630d 0a69  ir = ...= src..i
-000001b0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-000001c0: 3d20 0d0a 0972 6571 7565 7374 730d 0a09  = ...requests...
-000001d0: 6173 796e 6369 6f0d 0a70 7974 686f 6e5f  asyncio..python_
-000001e0: 7265 7175 6972 6573 203d 203e 3d33 2e36  requires = >=3.6
-000001f0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000200: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000210: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
-00000220: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000230: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000240: 2030 0d0a 0d0a                            0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7261 6e6b 6775 6e0a 7665 7273 696f  = rankgun.versio
+00000020: 6e20 3d20 322e 302e 300a 6175 7468 6f72  n = 2.0.0.author
+00000030: 203d 204e 6f61 682d 4861 660a 6175 7468   = Noah-Haf.auth
+00000040: 6f72 5f65 6d61 696c 203d 2052 6f62 6c6f  or_email = Roblo
+00000050: 7843 6f6f 6b69 655f 4465 7658 406f 7574  xCookie_DevX@out
+00000060: 6c6f 6f6b 2e63 6f6d 0a64 6573 6372 6970  look.com.descrip
+00000070: 7469 6f6e 203d 2068 7474 7073 3a2f 2f72  tion = https://r
+00000080: 616e 6b67 756e 2e77 6f72 6b73 0a6c 6f6e  ankgun.works.lon
+00000090: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+000000a0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640a  file: README.md.
+000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000c0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000d0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 7572  text/markdown.ur
+000000e0: 6c20 3d20 6874 7470 733a 2f2f 7261 6e6b  l = https://rank
+000000f0: 6775 6e2e 776f 726b 730a 636c 6173 7369  gun.works.classi
+00000100: 6669 6572 7320 3d20 0a09 5072 6f67 7261  fiers = ..Progra
+00000110: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000120: 3a20 5079 7468 6f6e 203a 3a20 330a 094c  : Python :: 3..L
+00000130: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000140: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000150: 6365 6e73 650a 094f 7065 7261 7469 6e67  cense..Operating
+00000160: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000170: 6465 7065 6e64 656e 740a 0a5b 6f70 7469  dependent..[opti
+00000180: 6f6e 735d 0a70 6163 6b61 6765 5f64 6972  ons].package_dir
+00000190: 203d 200a 093d 2073 7263 0a69 6e73 7461   = ..= src.insta
+000001a0: 6c6c 5f72 6571 7569 7265 7320 3d20 0a09  ll_requires = ..
+000001b0: 7265 7175 6573 7473 0a09 6173 796e 6369  requests..asynci
+000001c0: 6f0a 7079 7468 6f6e 5f72 6571 7569 7265  o.python_require
+000001d0: 7320 3d20 3e3d 332e 360a 0a5b 6f70 7469  s = >=3.6..[opti
+000001e0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+000001f0: 645d 0a77 6865 7265 203d 2073 7263 0a0a  d].where = src..
+00000200: 5b65 6767 5f69 6e66 6f5d 0a74 6167 5f62  [egg_info].tag_b
+00000210: 7569 6c64 203d 200a 7461 675f 6461 7465  uild = .tag_date
+00000220: 203d 2030 0a0a                            = 0..
```

