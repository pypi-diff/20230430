# Comparing `tmp/apollo-sdk-0.1.1.tar.gz` & `tmp/apollo-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-sdk-0.1.1.tar", last modified: Wed Apr 26 04:43:49 2023, max compression
+gzip compressed data, was "apollo-sdk-0.1.2.tar", last modified: Sun Apr 30 05:04:52 2023, max compression
```

## Comparing `apollo-sdk-0.1.1.tar` & `apollo-sdk-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,58 @@
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-04-26 04:43:49.653666 apollo-sdk-0.1.1/
--rw-r--r--   0 adrianbrown   (501) staff       (20)     3793 2023-04-26 04:08:42.000000 apollo-sdk-0.1.1/LICENSE
--rw-r--r--   0 adrianbrown   (501) staff       (20)      582 2023-04-26 04:43:49.653502 apollo-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 adrianbrown   (501) staff       (20)     4186 2023-04-26 04:30:58.000000 apollo-sdk-0.1.1/README.md
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-04-26 04:43:49.652395 apollo-sdk-0.1.1/apollo/
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1401 2023-04-26 04:08:42.000000 apollo-sdk-0.1.1/apollo/__init__.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     3700 2023-04-26 04:08:42.000000 apollo-sdk-0.1.1/apollo/client.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1489 2023-04-26 04:08:42.000000 apollo-sdk-0.1.1/apollo/const.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     4284 2023-04-26 04:08:42.000000 apollo-sdk-0.1.1/apollo/exceptions.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1377 2023-04-26 04:08:42.000000 apollo-sdk-0.1.1/apollo/manager.py
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1205 2023-04-26 04:08:42.000000 apollo-sdk-0.1.1/apollo/resource.py
-drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-04-26 04:43:49.653295 apollo-sdk-0.1.1/apollo_sdk.egg-info/
--rw-r--r--   0 adrianbrown   (501) staff       (20)      582 2023-04-26 04:43:49.000000 apollo-sdk-0.1.1/apollo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 adrianbrown   (501) staff       (20)      305 2023-04-26 04:43:49.000000 apollo-sdk-0.1.1/apollo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 adrianbrown   (501) staff       (20)        1 2023-04-26 04:43:49.000000 apollo-sdk-0.1.1/apollo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 adrianbrown   (501) staff       (20)      266 2023-04-26 04:43:49.000000 apollo-sdk-0.1.1/apollo_sdk.egg-info/requires.txt
--rw-r--r--   0 adrianbrown   (501) staff       (20)        7 2023-04-26 04:43:49.000000 apollo-sdk-0.1.1/apollo_sdk.egg-info/top_level.txt
--rw-r--r--   0 adrianbrown   (501) staff       (20)       38 2023-04-26 04:43:49.653716 apollo-sdk-0.1.1/setup.cfg
--rw-r--r--   0 adrianbrown   (501) staff       (20)     1800 2023-04-26 04:43:45.000000 apollo-sdk-0.1.1/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.850677 apollo-sdk-0.1.2/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.1.2/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)      632 2023-04-30 05:04:52.850828 apollo-sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5509 2023-04-29 17:42:09.000000 apollo-sdk-0.1.2/README.md
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.846342 apollo-sdk-0.1.2/apollo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1403 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3608 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/client.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.846472 apollo-sdk-0.1.2/apollo/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.847013 apollo-sdk-0.1.2/apollo/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.847175 apollo-sdk-0.1.2/apollo/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.847333 apollo-sdk-0.1.2/apollo/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.847460 apollo-sdk-0.1.2/apollo/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848002 apollo-sdk-0.1.2/apollo/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1375 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/manager.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848154 apollo-sdk-0.1.2/apollo/models/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848281 apollo-sdk-0.1.2/apollo/models/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848414 apollo-sdk-0.1.2/apollo/models/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/google/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848561 apollo-sdk-0.1.2/apollo/models/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848708 apollo-sdk-0.1.2/apollo/models/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/models/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1194 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848846 apollo-sdk-0.1.2/apollo/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.848967 apollo-sdk-0.1.2/apollo/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.849516 apollo-sdk-0.1.2/apollo/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      859 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1155 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      888 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.849745 apollo-sdk-0.1.2/apollo/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.2/apollo/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-04-30 05:04:52.850537 apollo-sdk-0.1.2/apollo_sdk.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      632 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1087 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      266 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        7 2023-04-30 05:04:52.000000 apollo-sdk-0.1.2/apollo_sdk.egg-info/top_level.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      103 2023-04-30 05:04:52.851122 apollo-sdk-0.1.2/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1899 2023-04-30 05:04:44.000000 apollo-sdk-0.1.2/setup.py
```

### Comparing `apollo-sdk-0.1.1/LICENSE` & `apollo-sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.1/PKG-INFO` & `apollo-sdk-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Build automated decision making workflows. Aggregate your LLMs all into one place and build from there using one api.
+Home-page: https://github.com/apolloapi/apolloapi
 Author: Apollo API, Inc.
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `apollo-sdk-0.1.1/README.md` & `apollo-sdk-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -30,233 +30,316 @@
 000001d0: 2074 6865 2064 6574 6563 7469 6f6e 206f   the detection o
 000001e0: 6620 6861 726d 2069 6e20 696d 6167 6573  f harm in images
 000001f0: 2c20 7669 6465 6f73 2c20 6175 6469 6f20  , videos, audio 
 00000200: 616e 6420 7465 7874 2e0a 3c2f 6469 763e  and text..</div>
 00000210: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
 00000220: 6572 223e 0a20 2020 203c 6272 202f 3e0a  er">.    <br />.
 00000230: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000240: 7073 3a2f 2f61 706f 6c6c 6f61 7069 2e69  ps://apolloapi.i
-00000250: 6f22 2072 656c 3d22 646f 666f 6c6c 6f77  o" rel="dofollow
-00000260: 223e 3c73 7472 6f6e 673e 446f 6373 2063  "><strong>Docs c
-00000270: 6f6d 696e 6720 736f 6f6e 20c2 bb3c 2f73  oming soon ..</s
-00000280: 7472 6f6e 673e 3c2f 613e 0a20 2020 203c  trong></a>.    <
-00000290: 6272 202f 3e0a 0a20 203c 6272 2f3e 0a20  br />..  <br/>. 
-000002a0: 2020 203c 212d 2d20 3c61 2068 7265 663d     <!-- <a href=
-000002b0: 2268 7474 7073 3a2f 2f64 6f63 732e 6e61  "https://docs.na
-000002c0: 6e67 6f2e 6465 7622 3e45 7861 6d70 6c65  ngo.dev">Example
-000002d0: 733c 2f61 3e20 2d2d 3e0a 2020 2020 3c61  s</a> -->.    <a
-000002e0: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
-000002f0: 7777 2e61 706f 6c6c 6f61 7069 2e69 6f2f  ww.apolloapi.io/
-00000300: 223e 4a6f 696e 2074 6865 2077 6169 746c  ">Join the waitl
-00000310: 6973 743c 2f61 3e0a 2020 2020 c2b7 0a20  ist</a>.    ... 
-00000320: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00000330: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000340: 706f 6c6c 6f61 7069 2f61 706f 6c6c 6f61  polloapi/apolloa
-00000350: 7069 2f69 7373 7565 7322 3e52 6570 6f72  pi/issues">Repor
-00000360: 7420 4275 673c 2f61 3e0a 2020 2020 c2b7  t Bug</a>.    ..
-00000370: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00000380: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
-00000390: 2f5a 5548 3766 3741 7a55 5922 3e43 6f6d  /ZUH7f7AzUY">Com
-000003a0: 6d75 6e69 7479 2044 6973 636f 7264 3c2f  munity Discord</
-000003b0: 613e 0a3c 2f70 3e0a 0a23 2320 e2ad 9020  a>.</p>..## ... 
-000003c0: 4361 6e20 796f 7520 7368 6f77 206d 6520  Can you show me 
-000003d0: 616e 2065 7861 6d70 6c65 3f0a 0a49 6e20  an example?..In 
-000003e0: 796f 7572 2063 6f64 6520 796f 7520 6361  your code you ca
-000003f0: 6e20 7772 6974 653a 0a0a 6060 6074 730a  n write:..```ts.
-00000400: 4170 6f6c 6c6f 2e63 6f6e 6e65 6374 2827  Apollo.connect('
-00000410: 706f 7374 6772 6573 3a2f 2f75 7365 726e  postgres://usern
-00000420: 616d 653a 7061 7373 776f 7264 4068 6f73  ame:password@hos
-00000430: 746e 616d 2e2e 2e27 2c20 2e2e 2e29 202f  tnam...', ...) /
-00000440: 2f20 5374 6172 7473 2073 796e 6369 6e67  / Starts syncing
-00000450: 2063 6f6e 7465 6e74 2066 6f72 6576 6572   content forever
-00000460: 210a 0a41 706f 6c6c 6f2e 7573 6528 274f  !..Apollo.use('O
-00000470: 7065 6e41 4927 2c20 226d 6f64 6572 6174  penAI', "moderat
-00000480: 696f 6e22 2c20 2e2e 2e29 202f 2f20 436f  ion", ...) // Co
-00000490: 6e6e 6563 7420 746f 2065 7869 7374 696e  nnect to existin
-000004a0: 6720 7072 6f76 6964 6572 7321 0a0a 4170  g providers!..Ap
-000004b0: 6f6c 6c6f 2e72 756c 6528 2750 6872 6173  ollo.rule('Phras
-000004c0: 6531 272c 2027 3e3d 272c 2027 302e 3827  e1', '>=', '0.8'
-000004d0: 2920 2f2f 2043 7265 6174 6520 6375 7374  ) // Create cust
-000004e0: 6f6d 2072 756c 6573 210a 0a41 706f 6c6c  om rules!..Apoll
-000004f0: 6f2e 7573 6528 2741 706f 6c6c 6f27 2c20  o.use('Apollo', 
-00000500: 2276 696f 6c65 6e63 6522 2c20 2e2e 2e29  "violence", ...)
-00000510: 202f 2f20 436f 6e6e 6563 7420 7769 7468   // Connect with
-00000520: 206f 7572 2069 6e74 6572 6e61 6c20 6d6f   our internal mo
-00000530: 6465 6c73 210a 0a2f 2f20 4465 7465 6374  dels!..// Detect
-00000540: 2062 6164 2061 6374 6f72 7320 6174 2073   bad actors at s
-00000550: 6361 6c65 210a 4170 6f6c 6c6f 2e64 6574  cale!.Apollo.det
-00000560: 6563 7449 6d61 6765 2827 496d 6167 6531  ectImage('Image1
-00000570: 272c 2027 636f 6e74 6169 6e73 272c 2027  ', 'contains', '
-00000580: 5645 5259 5f4c 494b 454c 5927 2920 2f2f  VERY_LIKELY') //
-00000590: 2049 6d61 6765 2041 6e61 6c79 7369 732f   Image Analysis/
-000005a0: 4f43 520a 4170 6f6c 6c6f 2e64 6574 6563  OCR.Apollo.detec
-000005b0: 7453 7065 6563 6828 2741 7564 696f 3127  tSpeech('Audio1'
-000005c0: 2c20 2763 6f6e 7461 696e 7327 2c20 2755  , 'contains', 'U
-000005d0: 4e4c 494b 454c 5927 2920 2f2f 2041 7564  NLIKELY') // Aud
-000005e0: 696f 2050 726f 6365 7373 696e 670a 4170  io Processing.Ap
-000005f0: 6f6c 6c6f 2e64 6574 6563 7456 6964 656f  ollo.detectVideo
-00000600: 2827 5669 6465 6f31 272c 2027 636f 6e74  ('Video1', 'cont
-00000610: 6169 6e73 272c 2027 504f 5353 4942 4c45  ains', 'POSSIBLE
-00000620: 2729 202f 2f20 5669 6465 6f20 416e 616c  ') // Video Anal
-00000630: 7973 6973 0a41 706f 6c6c 6f2e 6465 7465  ysis.Apollo.dete
-00000640: 6374 5465 7874 2827 5068 7261 7365 3127  ctText('Phrase1'
-00000650: 2c20 2763 6f6e 7461 696e 7327 2c20 2755  , 'contains', 'U
-00000660: 4e4b 4e4f 574e 2729 202f 2f20 5465 7874  NKNOWN') // Text
-00000670: 2041 6e61 6c79 7369 730a 0a60 6060 0a0a   Analysis..```..
-00000680: 4170 6f6c 6c6f 2074 6865 6e20 7461 6b65  Apollo then take
-00000690: 7320 6361 7265 206f 663a 0a0a 2d20 4465  s care of:..- De
-000006a0: 7465 6374 696e 6720 7265 616c 2d74 696d  tecting real-tim
-000006b0: 6520 6368 616e 6765 7320 696e 2075 7365  e changes in use
-000006c0: 7220 6578 7065 7269 656e 6365 0a2d 2041  r experience.- A
-000006d0: 7574 6f6d 6174 6564 2064 6574 6563 7469  utomated detecti
-000006e0: 6f6e 2061 6761 696e 7374 2069 6d61 6765  on against image
-000006f0: 2c20 7669 6465 6f2c 2061 7564 696f 206f  , video, audio o
-00000700: 7220 7465 7874 0a2d 2043 6f6e 6e65 6374  r text.- Connect
-00000710: 696e 6720 706f 6c69 6379 2074 6f20 7072  ing policy to pr
-00000720: 6f64 7563 740a 2d20 4d61 6b69 6e67 2073  oduct.- Making s
-00000730: 7572 6520 796f 7572 2069 6e74 6567 7261  ure your integra
-00000740: 7469 6f6e 2069 7320 726f 6275 7374 2c20  tion is robust, 
-00000750: 736f 2079 6f75 206e 6576 6572 2061 6761  so you never aga
-00000760: 696e 2068 6176 6520 746f 2077 6f72 7279  in have to worry
-00000770: 2061 626f 7574 2073 7475 636b 2f73 7461   about stuck/sta
-00000780: 6c65 2064 6174 6120 6f72 2066 616c 7365  le data or false
-00000790: 2d70 6f73 6974 6976 6573 0a0a 2323 20f0  -positives..## .
-000007a0: 9fa7 91e2 808d f09f 92bb 2043 6f6f 6c2c  .......... Cool,
-000007b0: 2077 6861 7420 6361 6e20 4920 6275 696c   what can I buil
-000007c0: 6420 7769 7468 2069 743f 0a0a 2d20 5472  d with it?..- Tr
-000007d0: 7573 7420 2620 5361 6665 7479 2074 6561  ust & Safety tea
-000007e0: 6d73 2069 6e20 636f 6d70 616e 6965 7320  ms in companies 
-000007f0: 7573 6520 4170 6f6c 6c6f 2074 6f20 2a2a  use Apollo to **
-00000800: 6275 696c 6420 6e61 7469 7665 2069 6e2d  build native in-
-00000810: 6170 7020 636f 6e6e 6563 7469 6f6e 732a  app connections*
-00000820: 2a20 7265 6c61 7465 6420 746f 2061 6374  * related to act
-00000830: 6976 6520 7265 7370 6f6e 7365 2c20 636f  ive response, co
-00000840: 6e74 656e 7420 6d6f 6465 7261 7469 6f6e  ntent moderation
-00000850: 2c20 6672 6175 6420 6465 7465 6374 696f  , fraud detectio
-00000860: 6e2c 2065 7463 2e0a 2d20 536f 6d65 202a  n, etc..- Some *
-00000870: 2a61 7574 6f6d 6174 6520 7468 6569 7220  *automate their 
-00000880: 7065 7273 6f6e 616c 206c 6976 6573 2a2a  personal lives**
-00000890: 2077 6974 6820 4170 6f6c 6c6f 2062 7920   with Apollo by 
-000008a0: 696e 7465 6772 6174 696e 6720 6167 6169  integrating agai
-000008b0: 6e73 7420 6469 7363 6f72 6420 636f 6d6d  nst discord comm
-000008c0: 756e 6974 6965 7320 6f72 206f 7468 6572  unities or other
-000008d0: 2064 6563 656e 7472 616c 697a 6564 206e   decentralized n
-000008e0: 6574 776f 726b 7320 666f 7220 7361 6665  etworks for safe
-000008f0: 7479 0a2d 2041 706f 6c6c 6f20 6361 6e20  ty.- Apollo can 
-00000900: 6865 6c70 2079 6f75 202a 2a71 7569 636b  help you **quick
-00000910: 6c79 2062 7569 6c64 2074 7275 7374 2a2a  ly build trust**
-00000920: 2066 6f72 2068 6f62 6279 2070 726f 6a65   for hobby proje
-00000930: 6374 732c 2063 6f6d 6d75 6e69 7469 6573  cts, communities
-00000940: 206f 7220 6275 7369 6e65 7373 0a0a 2323   or business..##
-00000950: 20f0 9f9a 8020 496e 7465 7265 7374 696e   .... Interestin
-00000960: 672c 2068 6f77 2063 616e 2049 2074 7279  g, how can I try
-00000970: 2069 743f 0a0a 4c65 7427 7320 7365 7475   it?..Let's setu
-00000980: 7020 796f 7572 2066 6972 7374 2049 6e74  p your first Int
-00000990: 6567 7261 7469 6f6e 2069 6e20 3220 6d69  egration in 2 mi
-000009a0: 6e75 7465 7321 0a0a 4974 2077 696c 6c20  nutes!..It will 
-000009b0: 7075 6c6c 2066 726f 6d20 796f 7572 206c  pull from your l
-000009c0: 6f63 616c 2064 6174 6162 6173 6520 2861  ocal database (a
-000009d0: 6e64 206b 6565 7020 6974 2069 6e20 7379  nd keep it in sy
-000009e0: 6e63 292e 0a0a 5465 7374 2073 656e 6469  nc)...Test sendi
-000009f0: 6e67 2079 6f75 7220 636f 6e74 656e 7420  ng your content 
-00000a00: 746f 206f 7572 2041 5049 210a 0a2e 2e2e  to our API!.....
-00000a10: 616e 6420 6372 6561 7465 2061 2049 6e74  and create a Int
-00000a20: 6567 7261 7469 6f6e 2077 6974 6820 6120  egration with a 
-00000a30: 7369 6d70 6c65 2063 6f6d 6d61 6e64 3a0a  simple command:.
-00000a40: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
-00000a50: 7461 6c6c 0a60 6060 0a0a 6060 6070 7974  tall.```..```pyt
-00000a60: 686f 6e0a 0a60 6060 0a0a 5468 6174 2773  hon..```..That's
-00000a70: 2061 6c6c 2069 7420 7461 6b65 7321 0a0a   all it takes!..
-00000a80: 5468 6174 2773 2061 6c6c 2069 7420 7461  That's all it ta
-00000a90: 6b65 7321 2059 6f75 2063 616e 2063 6865  kes! You can che
-00000aa0: 636b 206f 7574 205b 7468 6520 6c69 7374  ck out [the list
-00000ab0: 206f 6620 616c 6c20 506f 6bc3 a96d 6f6e   of all Pok..mon
-00000ac0: 7320 696e 2079 6f75 7220 6c6f 6361 6c20  s in your local 
-00000ad0: 6461 7461 6261 7365 5d28 6874 7470 3a2f  database](http:/
-00000ae0: 2f6c 6f63 616c 686f 7374 3a38 3038 302f  /localhost:8080/
-00000af0: 3f70 6773 716c 3d6e 616e 676f 2d64 6226  ?pgsql=nango-db&
-00000b00: 7573 6572 6e61 6d65 3d6e 616e 676f 2664  username=nango&d
-00000b10: 623d 6e61 6e67 6f26 6e73 3d70 7562 6c69  b=nango&ns=publi
-00000b20: 6326 7365 6c65 6374 3d5f 6e61 6e67 6f5f  c&select=_nango_
-00000b30: 7261 7729 2028 7061 7373 776f 7264 2069  raw) (password i
-00000b40: 7320 606e 616e 676f 6029 2e0a 0a49 6e20  s `nango`)...In 
-00000b50: 7072 6163 7469 6365 2c20 796f 7520 7072  practice, you pr
-00000b60: 6f62 6162 6c79 2077 616e 7420 746f 2075  obably want to u
-00000b70: 7365 206f 6e65 206f 6620 6f75 7220 6e61  se one of our na
-00000b80: 7469 7665 2053 444b 7320 746f 2069 6e74  tive SDKs to int
-00000b90: 6572 6163 7420 7769 7468 2041 706f 6c6c  eract with Apoll
-00000ba0: 6f27 7320 4150 4920 6f72 2075 7365 206f  o's API or use o
-00000bb0: 7572 2063 7573 746f 6d20 6272 6f77 7365  ur custom browse
-00000bc0: 7220 636c 6965 6e74 2073 6f20 796f 7520  r client so you 
-00000bd0: 646f 6e74 2068 6176 6520 746f 2077 7269  dont have to wri
-00000be0: 7465 2063 6f64 652e 0a0a 6060 606a 730a  te code...```js.
-00000bf0: 696d 706f 7274 207b 204e 616e 676f 207d  import { Nango }
-00000c00: 2066 726f 6d20 2240 6e61 6e67 6f68 712f   from "@nangohq/
-00000c10: 6e6f 6465 2d63 6c69 656e 7422 3b0a 6c65  node-client";.le
-00000c20: 7420 636f 6e66 6967 203d 207b 0a20 2072  t config = {.  r
-00000c30: 6573 706f 6e73 655f 7061 7468 3a20 2272  esponse_path: "r
-00000c40: 6573 756c 7473 222c 202f 2f20 5468 6520  esults", // The 
-00000c50: 7061 7468 2074 6f20 7468 6520 506f 6bc3  path to the Pok.
-00000c60: a96d 6f6e 7320 6f62 6a65 6374 7320 696e  .mons objects in
-00000c70: 2074 6865 2072 6573 706f 6e73 652e 0a20   the response.. 
-00000c80: 2070 6167 696e 675f 7572 6c5f 7061 7468   paging_url_path
-00000c90: 3a20 226e 6578 7422 2c20 2f2f 2054 6865  : "next", // The
-00000ca0: 2070 6174 6820 746f 2074 6865 206e 6578   path to the nex
-00000cb0: 7420 7061 6765 2773 2075 726c 2069 6e20  t page's url in 
-00000cc0: 7468 6520 7265 7370 6f6e 7365 2e0a 7d3b  the response..};
-00000cd0: 0a61 7761 6974 204e 616e 676f 2e73 796e  .await Nango.syn
-00000ce0: 6328 2268 7474 7073 3a2f 2f70 6f6b 6561  c("https://pokea
-00000cf0: 7069 2e63 6f2f 6170 692f 7632 2f70 6f6b  pi.co/api/v2/pok
-00000d00: 656d 6f6e 222c 2063 6f6e 6669 6729 3b0a  emon", config);.
-00000d10: 6060 600a 0a23 2320 436f 6e74 7269 6275  ```..## Contribu
-00000d20: 7469 6e67 0a0a 2323 2320 f09f 93a6 2070  ting..### .... p
-00000d30: 7265 2d63 6f6d 6d69 7420 636f 6e66 6967  re-commit config
-00000d40: 0a0a 436c 6f6e 6520 7468 6520 7265 706f  ..Clone the repo
-00000d50: 2061 6e64 2073 7461 7274 2041 706f 6c6c   and start Apoll
-00000d60: 6f20 6c6f 6361 6c6c 792e 2e2e 0a0a 6060  o locally.....``
-00000d70: 6062 6173 680a 6769 7420 636c 6f6e 6520  `bash.git clone 
-00000d80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000d90: 6f6d 2f61 706f 6c6c 6f61 7069 2f61 706f  om/apolloapi/apo
-00000da0: 6c6c 6f61 7069 2e67 6974 0a63 6420 6170  lloapi.git.cd ap
-00000db0: 6f6c 6c6f 6170 6920 2626 2070 7974 686f  olloapi && pytho
-00000dc0: 6e33 202d 6d20 7665 6e76 2065 6e76 2026  n3 -m venv env &
-00000dd0: 2620 736f 7572 6365 2065 6e76 2f62 696e  & source env/bin
-00000de0: 2f61 6374 6976 6174 6520 2626 2070 6970  /activate && pip
-00000df0: 2069 6e73 7461 6c6c 202d 7220 7265 7175   install -r requ
-00000e00: 6972 656d 656e 7473 2e74 7874 0a60 6060  irements.txt.```
-00000e10: 0a0a 2d20 4166 7465 7220 696e 7374 616c  ..- After instal
-00000e20: 6c69 6e67 2073 7973 7465 6d20 6465 7065  ling system depe
-00000e30: 6e64 656e 6369 6573 2062 6520 7375 7265  ndencies be sure
-00000e40: 2074 6f20 696e 7374 616c 6c20 7072 652d   to install pre-
-00000e50: 636f 6d6d 6974 2066 6f72 206c 696e 7420  commit for lint 
-00000e60: 6368 6563 6b73 0a0a 6060 6062 6173 680a  checks..```bash.
-00000e70: 7069 7020 696e 7374 616c 6c20 7072 652d  pip install pre-
-00000e80: 636f 6d6d 6974 0a0a 7072 652d 636f 6d6d  commit..pre-comm
-00000e90: 6974 2069 6e73 7461 6c6c 0a0a 7072 652d  it install..pre-
-00000ea0: 636f 6d6d 6974 2072 756e 202d 2d61 6c6c  commit run --all
-00000eb0: 2d66 696c 6573 0a60 6060 0a0a 2323 20f0  -files.```..## .
-00000ec0: 9f94 8d20 4e65 6174 2c20 4920 776f 756c  ... Neat, I woul
-00000ed0: 6420 6c69 6b65 2074 6f20 6c65 6172 6e20  d like to learn 
-00000ee0: 6d6f 7265 0a0a e2ad 9020 466f 6c6c 6f77  more..... Follow
-00000ef0: 206f 7572 2064 6576 656c 6f70 6d65 6e74   our development
-00000f00: 2062 7920 7374 6172 7269 6e67 2075 7320   by starring us 
-00000f10: 6865 7265 206f 6e20 4769 7448 7562 20e2  here on GitHub .
-00000f20: ad90 0a0a 3c21 2d2d 202d 2045 7870 6c6f  ....<!-- - Explo
-00000f30: 7265 2073 6f6d 6520 5b52 6561 6c20 776f  re some [Real wo
-00000f40: 726c 6420 6578 616d 706c 6573 5d28 6874  rld examples](ht
-00000f50: 7470 733a 2f2f 7777 772e 7468 6562 7269  tps://www.thebri
-00000f60: 6566 6e65 7773 6c65 7474 6572 2e63 6f6d  efnewsletter.com
-00000f70: 2920 2d2d 3e0a 0a2d 2053 6861 7265 2066  ) -->..- Share f
-00000f80: 6565 6462 6163 6b20 6f72 2061 736b 2071  eedback or ask q
-00000f90: 7565 7374 696f 6e73 206f 6e20 7468 6520  uestions on the 
-00000fa0: 5b44 6973 636f 7264 2063 6f6d 6d75 6e69  [Discord communi
-00000fb0: 7479 5d28 6874 7470 733a 2f2f 6469 7363  ty](https://disc
-00000fc0: 6f72 642e 6767 2f5a 5548 3766 3741 7a55  ord.gg/ZUH7f7AzU
-00000fd0: 5929 0a2d 205b 4368 6174 2077 6974 6820  Y).- [Chat with 
-00000fe0: 6120 6d65 6d62 6572 206f 6620 7468 6520  a member of the 
-00000ff0: 7465 616d 5d28 6874 7470 733a 2f2f 6170  team](https://ap
-00001000: 6f6c 6c6f 6170 692e 696f 2920 f09f 918b  olloapi.io) ....
-00001010: 0a2d 2043 6865 636b 206f 7572 205b 626c  .- Check our [bl
-00001020: 6f67 206f 6e20 5472 7573 7420 2620 5361  og on Trust & Sa
-00001030: 6665 7479 5d28 6874 7470 733a 2f2f 7777  fety](https://ww
-00001040: 772e 7468 6562 7269 6566 6e65 7773 6c65  w.thebriefnewsle
-00001050: 7474 6572 2e63 6f6d 290a                 tter.com).
+00000240: 7073 3a2f 2f61 706f 6c6c 6f61 7069 2d64  ps://apolloapi-d
+00000250: 6f63 2e76 6572 6365 6c2e 6170 702f 2220  oc.vercel.app/" 
+00000260: 7265 6c3d 2264 6f66 6f6c 6c6f 7722 3e3c  rel="dofollow"><
+00000270: 7374 726f 6e67 3e44 6f63 7320 c2bb 3c2f  strong>Docs ..</
+00000280: 7374 726f 6e67 3e3c 2f61 3e0a 2020 2020  strong></a>.    
+00000290: 3c62 7220 2f3e 0a0a 2020 3c62 722f 3e0a  <br />..  <br/>.
+000002a0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+000002b0: 7073 3a2f 2f61 706f 6c6c 6f61 7069 2d64  ps://apolloapi-d
+000002c0: 6f63 2e76 6572 6365 6c2e 6170 702f 223e  oc.vercel.app/">
+000002d0: 4578 616d 706c 6573 3c2f 613e 0a20 2020  Examples</a>.   
+000002e0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000002f0: 2f2f 7777 772e 6170 6f6c 6c6f 6170 692e  //www.apolloapi.
+00000300: 696f 2f22 3e4a 6f69 6e20 7468 6520 7761  io/">Join the wa
+00000310: 6974 6c69 7374 3c2f 613e 0a20 2020 20c2  itlist</a>.    .
+00000320: b70a 2020 2020 3c61 2068 7265 663d 2268  ..    <a href="h
+00000330: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000340: 6d2f 6170 6f6c 6c6f 6170 692f 6170 6f6c  m/apolloapi/apol
+00000350: 6c6f 6170 692f 6973 7375 6573 223e 5265  loapi/issues">Re
+00000360: 706f 7274 2042 7567 3c2f 613e 0a20 2020  port Bug</a>.   
+00000370: 20c2 b70a 2020 2020 3c61 2068 7265 663d   ...    <a href=
+00000380: 2268 7474 7073 3a2f 2f64 6973 636f 7264  "https://discord
+00000390: 2e67 672f 5a55 4837 6637 417a 5559 223e  .gg/ZUH7f7AzUY">
+000003a0: 436f 6d6d 756e 6974 7920 4469 7363 6f72  Community Discor
+000003b0: 643c 2f61 3e0a 3c2f 703e 0a0a 2323 20e2  d</a>.</p>..## .
+000003c0: ad90 2043 616e 2079 6f75 2073 686f 7720  .. Can you show 
+000003d0: 6d65 2061 6e20 6578 616d 706c 653f 0a0a  me an example?..
+000003e0: 496e 2079 6f75 7220 636f 6465 2079 6f75  In your code you
+000003f0: 2063 616e 2077 7269 7465 3a0a 0a60 6060   can write:..```
+00000400: 7473 0a41 706f 6c6c 6f2e 636f 6e6e 6563  ts.Apollo.connec
+00000410: 7428 2770 6f73 7467 7265 733a 2f2f 7573  t('postgres://us
+00000420: 6572 6e61 6d65 3a70 6173 7377 6f72 6440  ername:password@
+00000430: 686f 7374 6e61 6d2e 2e2e 272c 202e 2e2e  hostnam...', ...
+00000440: 2920 2f2f 2053 7461 7274 7320 7379 6e63  ) // Starts sync
+00000450: 696e 6720 636f 6e74 656e 7420 666f 7265  ing content fore
+00000460: 7665 7221 0a0a 4170 6f6c 6c6f 2e75 7365  ver!..Apollo.use
+00000470: 2827 4f70 656e 4149 272c 2022 6d6f 6465  ('OpenAI', "mode
+00000480: 7261 7469 6f6e 222c 202e 2e2e 2920 2f2f  ration", ...) //
+00000490: 2043 6f6e 6e65 6374 2074 6f20 6578 6973   Connect to exis
+000004a0: 7469 6e67 2070 726f 7669 6465 7273 210a  ting providers!.
+000004b0: 0a41 706f 6c6c 6f2e 7275 6c65 2827 5068  .Apollo.rule('Ph
+000004c0: 7261 7365 3127 2c20 273e 3d27 2c20 2730  rase1', '>=', '0
+000004d0: 2e38 2729 202f 2f20 4372 6561 7465 2063  .8') // Create c
+000004e0: 7573 746f 6d20 7275 6c65 7321 0a0a 4170  ustom rules!..Ap
+000004f0: 6f6c 6c6f 2e75 7365 2827 4170 6f6c 6c6f  ollo.use('Apollo
+00000500: 272c 2022 7669 6f6c 656e 6365 222c 202e  ', "violence", .
+00000510: 2e2e 2920 2f2f 2043 6f6e 6e65 6374 2077  ..) // Connect w
+00000520: 6974 6820 6f75 7220 696e 7465 726e 616c  ith our internal
+00000530: 206d 6f64 656c 7321 0a0a 2f2f 2044 6574   models!..// Det
+00000540: 6563 7420 6261 6420 6163 746f 7273 2061  ect bad actors a
+00000550: 7420 7363 616c 6521 0a41 706f 6c6c 6f2e  t scale!.Apollo.
+00000560: 6465 7465 6374 496d 6167 6528 2749 6d61  detectImage('Ima
+00000570: 6765 3127 2c20 2763 6f6e 7461 696e 7327  ge1', 'contains'
+00000580: 2c20 2756 4552 595f 4c49 4b45 4c59 2729  , 'VERY_LIKELY')
+00000590: 202f 2f20 496d 6167 6520 416e 616c 7973   // Image Analys
+000005a0: 6973 2f4f 4352 0a41 706f 6c6c 6f2e 6465  is/OCR.Apollo.de
+000005b0: 7465 6374 5370 6565 6368 2827 4175 6469  tectSpeech('Audi
+000005c0: 6f31 272c 2027 636f 6e74 6169 6e73 272c  o1', 'contains',
+000005d0: 2027 554e 4c49 4b45 4c59 2729 202f 2f20   'UNLIKELY') // 
+000005e0: 4175 6469 6f20 5072 6f63 6573 7369 6e67  Audio Processing
+000005f0: 0a41 706f 6c6c 6f2e 6465 7465 6374 5669  .Apollo.detectVi
+00000600: 6465 6f28 2756 6964 656f 3127 2c20 2763  deo('Video1', 'c
+00000610: 6f6e 7461 696e 7327 2c20 2750 4f53 5349  ontains', 'POSSI
+00000620: 424c 4527 2920 2f2f 2056 6964 656f 2041  BLE') // Video A
+00000630: 6e61 6c79 7369 730a 4170 6f6c 6c6f 2e64  nalysis.Apollo.d
+00000640: 6574 6563 7454 6578 7428 2750 6872 6173  etectText('Phras
+00000650: 6531 272c 2027 636f 6e74 6169 6e73 272c  e1', 'contains',
+00000660: 2027 554e 4b4e 4f57 4e27 2920 2f2f 2054   'UNKNOWN') // T
+00000670: 6578 7420 416e 616c 7973 6973 0a0a 6060  ext Analysis..``
+00000680: 600a 0a41 706f 6c6c 6f20 7468 656e 2074  `..Apollo then t
+00000690: 616b 6573 2063 6172 6520 6f66 3a0a 0a2d  akes care of:..-
+000006a0: 2044 6574 6563 7469 6e67 2072 6561 6c2d   Detecting real-
+000006b0: 7469 6d65 2063 6861 6e67 6573 2069 6e20  time changes in 
+000006c0: 7573 6572 2065 7870 6572 6965 6e63 650a  user experience.
+000006d0: 2d20 4175 746f 6d61 7465 6420 6465 7465  - Automated dete
+000006e0: 6374 696f 6e20 6167 6169 6e73 7420 696d  ction against im
+000006f0: 6167 652c 2076 6964 656f 2c20 6175 6469  age, video, audi
+00000700: 6f20 6f72 2074 6578 740a 2d20 436f 6e6e  o or text.- Conn
+00000710: 6563 7469 6e67 2070 6f6c 6963 7920 746f  ecting policy to
+00000720: 2070 726f 6475 6374 0a2d 204d 616b 696e   product.- Makin
+00000730: 6720 7375 7265 2079 6f75 7220 696e 7465  g sure your inte
+00000740: 6772 6174 696f 6e20 6973 2072 6f62 7573  gration is robus
+00000750: 742c 2073 6f20 796f 7520 6e65 7665 7220  t, so you never 
+00000760: 6167 6169 6e20 6861 7665 2074 6f20 776f  again have to wo
+00000770: 7272 7920 6162 6f75 7420 7374 7563 6b2f  rry about stuck/
+00000780: 7374 616c 6520 6461 7461 206f 7220 6661  stale data or fa
+00000790: 6c73 652d 706f 7369 7469 7665 730a 0a23  lse-positives..#
+000007a0: 2320 f09f a791 e280 8df0 9f92 bb20 436f  # ........... Co
+000007b0: 6f6c 2c20 7768 6174 2063 616e 2049 2062  ol, what can I b
+000007c0: 7569 6c64 2077 6974 6820 6974 3f0a 0a2d  uild with it?..-
+000007d0: 2054 7275 7374 2026 2053 6166 6574 7920   Trust & Safety 
+000007e0: 7465 616d 7320 696e 2063 6f6d 7061 6e69  teams in compani
+000007f0: 6573 2075 7365 2041 706f 6c6c 6f20 746f  es use Apollo to
+00000800: 202a 2a62 7569 6c64 206e 6174 6976 6520   **build native 
+00000810: 696e 2d61 7070 2063 6f6e 6e65 6374 696f  in-app connectio
+00000820: 6e73 2a2a 2072 656c 6174 6564 2074 6f20  ns** related to 
+00000830: 6163 7469 7665 2072 6573 706f 6e73 652c  active response,
+00000840: 2063 6f6e 7465 6e74 206d 6f64 6572 6174   content moderat
+00000850: 696f 6e2c 2066 7261 7564 2064 6574 6563  ion, fraud detec
+00000860: 7469 6f6e 2c20 6574 632e 0a2d 2053 6f6d  tion, etc..- Som
+00000870: 6520 2a2a 6175 746f 6d61 7465 2074 6865  e **automate the
+00000880: 6972 2070 6572 736f 6e61 6c20 6c69 7665  ir personal live
+00000890: 732a 2a20 7769 7468 2041 706f 6c6c 6f20  s** with Apollo 
+000008a0: 6279 2069 6e74 6567 7261 7469 6e67 2061  by integrating a
+000008b0: 6761 696e 7374 2064 6973 636f 7264 2063  gainst discord c
+000008c0: 6f6d 6d75 6e69 7469 6573 206f 7220 6f74  ommunities or ot
+000008d0: 6865 7220 6465 6365 6e74 7261 6c69 7a65  her decentralize
+000008e0: 6420 6e65 7477 6f72 6b73 2066 6f72 2073  d networks for s
+000008f0: 6166 6574 790a 2d20 4170 6f6c 6c6f 2063  afety.- Apollo c
+00000900: 616e 2068 656c 7020 796f 7520 2a2a 7175  an help you **qu
+00000910: 6963 6b6c 7920 6275 696c 6420 7472 7573  ickly build trus
+00000920: 742a 2a20 666f 7220 686f 6262 7920 7072  t** for hobby pr
+00000930: 6f6a 6563 7473 2c20 636f 6d6d 756e 6974  ojects, communit
+00000940: 6965 7320 6f72 2062 7573 696e 6573 730a  ies or business.
+00000950: 0a23 2320 f09f 9a80 2049 6e74 6572 6573  .## .... Interes
+00000960: 7469 6e67 2c20 686f 7720 6361 6e20 4920  ting, how can I 
+00000970: 7472 7920 6974 3f0a 0a4c 6574 2773 2073  try it?..Let's s
+00000980: 6574 7570 2079 6f75 7220 6669 7273 7420  etup your first 
+00000990: 496e 7465 6772 6174 696f 6e20 696e 2032  Integration in 2
+000009a0: 206d 696e 7574 6573 210a 0a49 7420 7769   minutes!..It wi
+000009b0: 6c6c 2070 756c 6c20 6672 6f6d 2079 6f75  ll pull from you
+000009c0: 7220 6c6f 6361 6c20 6461 7461 6261 7365  r local database
+000009d0: 2028 616e 6420 6b65 6570 2069 7420 696e   (and keep it in
+000009e0: 2073 796e 6329 2e0a 0a54 6f20 7374 6172   sync)...To star
+000009f0: 743a 0a0a 6060 6062 6173 680a 2320 696e  t:..```bash.# in
+00000a00: 7374 616c 6c20 7468 6520 636c 692d 746f  stall the cli-to
+00000a10: 6f6c 6b69 740a 7069 7020 696e 7374 616c  olkit.pip instal
+00000a20: 6c20 6170 6f6c 6c6f 2d73 646b 0a0a 2320  l apollo-sdk..# 
+00000a30: 656e 7465 7220 6120 7079 7468 6f6e 2072  enter a python r
+00000a40: 6570 6c20 6f72 2063 7265 6174 6520 6120  epl or create a 
+00000a50: 7079 7468 6f6e 2066 696c 652c 2075 7020  python file, up 
+00000a60: 746f 2079 6f75 2120 2872 6570 6c20 6973  to you! (repl is
+00000a70: 2065 6173 6965 7374 290a 7079 7468 6f6e   easiest).python
+00000a80: 330a 6060 600a 0a60 6060 7079 7468 6f6e  3.```..```python
+00000a90: 0a23 2069 6d70 6f72 7420 7468 6520 7061  .# import the pa
+00000aa0: 636b 6167 650a 6672 6f6d 2061 706f 6c6c  ckage.from apoll
+00000ab0: 6f2e 636c 6965 6e74 2069 6d70 6f72 7420  o.client import 
+00000ac0: 4170 6f6c 6c6f 0a0a 2320 7379 6e63 2064  Apollo..# sync d
+00000ad0: 6174 6120 6672 6f6d 2079 6f75 7220 6461  ata from your da
+00000ae0: 7461 6261 7365 2069 6e73 7461 6e63 650a  tabase instance.
+00000af0: 2320 2877 6520 7375 7070 6f72 7420 7375  # (we support su
+00000b00: 7061 6261 7365 2061 7420 7468 6520 6375  pabase at the cu
+00000b10: 7272 656e 7420 6d6f 6d65 6e74 206f 7220  rrent moment or 
+00000b20: 706f 7374 6772 6573 716c 2076 6961 2075  postgresql via u
+00000b30: 7269 2066 6f72 6d61 7429 0a41 706f 6c6c  ri format).Apoll
+00000b40: 6f2e 636f 6e6e 6563 7428 2270 6f73 7467  o.connect("postg
+00000b50: 7265 733a 2f2f 7573 6572 6e61 6d65 3a70  res://username:p
+00000b60: 6173 7377 6f72 6440 686f 7374 6e61 6d65  assword@hostname
+00000b70: 3a70 6f72 742f 6461 7461 6261 7365 5f6e  :port/database_n
+00000b80: 616d 6522 290a 0a23 2049 6620 796f 7520  ame")..# If you 
+00000b90: 7761 6e74 2074 6f20 7465 7374 206f 7574  want to test out
+00000ba0: 206f 7065 7261 7469 6f6e 206f 6e20 796f   operation on yo
+00000bb0: 7572 2065 7874 6572 6e61 6c20 636f 6e6e  ur external conn
+00000bc0: 6563 7469 6f6e 0a41 706f 6c6c 6f2e 6665  ection.Apollo.fe
+00000bd0: 7463 685f 7461 626c 6573 2829 0a41 706f  tch_tables().Apo
+00000be0: 6c6c 6f2e 7175 6572 7928 2264 6573 6322  llo.query("desc"
+00000bf0: 2c20 2274 6162 6c65 222c 2022 636f 6c75  , "table", "colu
+00000c00: 6d6e 2229 0a60 6060 0a0a 5465 7374 2073  mn").```..Test s
+00000c10: 656e 6469 6e67 2079 6f75 7220 636f 6e74  ending your cont
+00000c20: 656e 7420 746f 206f 7572 2041 5049 210a  ent to our API!.
+00000c30: 0a2e 2e2e 616e 6420 6372 6561 7465 2061  ....and create a
+00000c40: 2077 6f72 6b66 6c6f 7720 7769 7468 2061   workflow with a
+00000c50: 2073 696d 706c 6520 636f 6d6d 616e 643a   simple command:
+00000c60: 0a0a 6060 6070 7974 686f 6e0a 2320 696d  ..```python.# im
+00000c70: 706f 7274 2074 6865 2070 6163 6b61 6765  port the package
+00000c80: 0a66 726f 6d20 6170 6f6c 6c6f 2e63 6c69  .from apollo.cli
+00000c90: 656e 7420 696d 706f 7274 2041 706f 6c6c  ent import Apoll
+00000ca0: 6f0a 0a23 2055 7365 206f 7572 2063 7573  o..# Use our cus
+00000cb0: 746f 6d20 6d6f 6465 6c20 746f 2074 6573  tom model to tes
+00000cc0: 7420 6275 696c 6469 6e67 2064 6563 6973  t building decis
+00000cd0: 696f 6e73 0a41 706f 6c6c 6f2e 7573 6528  ions.Apollo.use(
+00000ce0: 2241 706f 6c6c 6f22 290a 0a23 2057 6520  "Apollo")..# We 
+00000cf0: 7375 7070 6f72 7420 7669 6465 6f2c 2073  support video, s
+00000d00: 7065 6563 682c 2069 6d61 6765 2061 6e64  peech, image and
+00000d10: 2074 6578 742e 2054 7279 2074 6578 7421   text. Try text!
+00000d20: 0a41 706f 6c6c 6f2e 6465 7465 6374 5465  .Apollo.detectTe
+00000d30: 7874 2822 5068 7261 7365 3122 2c20 2263  xt("Phrase1", "c
+00000d40: 6f6e 7461 696e 7322 2c20 2254 6872 6561  ontains", "Threa
+00000d50: 7473 2229 0a60 6060 0a0a 5468 6174 2773  ts").```..That's
+00000d60: 2061 6c6c 2069 7420 7461 6b65 7321 0a0a   all it takes!..
+00000d70: 5468 6174 2773 2061 6c6c 2069 7420 7461  That's all it ta
+00000d80: 6b65 7321 2059 6f75 2063 616e 2063 6865  kes! You can che
+00000d90: 636b 206f 7574 205b 6d6f 7265 206f 6e20  ck out [more on 
+00000da0: 6f75 7220 6e6f 7469 6f6e 2070 6167 655d  our notion page]
+00000db0: 2868 7474 7073 3a2f 2f63 6c6f 7564 6775  (https://cloudgu
+00000dc0: 7275 6162 2e6e 6f74 696f 6e2e 7369 7465  ruab.notion.site
+00000dd0: 2f41 706f 6c6c 6f2d 6535 6533 3437 3734  /Apollo-e5e34774
+00000de0: 3563 3165 3433 3739 3864 3834 3964 3739  5c1e43798d849d79
+00000df0: 6363 6539 3061 6261 292e 0a0a 496e 2070  cce90aba)...In p
+00000e00: 7261 6374 6963 652c 2079 6f75 2070 726f  ractice, you pro
+00000e10: 6261 626c 7920 7761 6e74 2074 6f20 7573  bably want to us
+00000e20: 6520 6f6e 6520 6f66 206f 7572 206e 6174  e one of our nat
+00000e30: 6976 6520 5344 4b73 2074 6f20 696e 7465  ive SDKs to inte
+00000e40: 7261 6374 2077 6974 6820 4170 6f6c 6c6f  ract with Apollo
+00000e50: 2773 2041 5049 206f 7220 7573 6520 6f75  's API or use ou
+00000e60: 7220 6375 7374 6f6d 2062 726f 7773 6572  r custom browser
+00000e70: 2063 6c69 656e 7420 736f 2079 6f75 2064   client so you d
+00000e80: 6f6e 7420 6861 7665 2074 6f20 7772 6974  ont have to writ
+00000e90: 6520 636f 6465 2e20 4966 2073 6f2c 2070  e code. If so, p
+00000ea0: 696e 6720 7573 2061 7420 6164 7269 616e  ing us at adrian
+00000eb0: 4061 706f 6c6c 6f61 7069 2e69 6f21 0a0a  @apolloapi.io!..
+00000ec0: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00000ed0: 0a23 2323 20f0 9f93 a620 7072 652d 636f  .### .... pre-co
+00000ee0: 6d6d 6974 2063 6f6e 6669 670a 0a41 7320  mmit config..As 
+00000ef0: 616e 206f 7065 6e20 736f 7572 6365 2070  an open source p
+00000f00: 726f 6a65 6374 2c20 4170 6f6c 6c6f 2077  roject, Apollo w
+00000f10: 656c 636f 6d65 7320 636f 6e74 7269 6275  elcomes contribu
+00000f20: 7469 6f6e 7320 6672 6f6d 2074 6865 2063  tions from the c
+00000f30: 6f6d 6d75 6e69 7479 2061 7420 6c61 7267  ommunity at larg
+00000f40: 652e 2054 6869 7320 6973 6ee2 8099 7420  e. This isn...t 
+00000f50: 616e 2065 7868 6175 7374 6976 6520 7265  an exhaustive re
+00000f60: 6665 7265 6e63 6520 616e 6420 6973 2061  ference and is a
+00000f70: 206c 6976 696e 6720 646f 6375 6d65 6e74   living document
+00000f80: 2073 7562 6a65 6374 2074 6f20 6368 616e   subject to chan
+00000f90: 6765 2061 7320 6e65 6564 6564 2077 6865  ge as needed whe
+00000fa0: 6e20 7468 6520 7072 6f6a 6563 7420 666f  n the project fo
+00000fb0: 726d 616c 697a 6573 2061 6e79 2070 7261  rmalizes any pra
+00000fc0: 6374 6963 6520 6f72 2070 6174 7465 726e  ctice or pattern
+00000fd0: 2e0a 0a43 6c6f 6e65 2074 6865 2072 6570  ...Clone the rep
+00000fe0: 6f20 616e 6420 7374 6172 7420 4170 6f6c  o and start Apol
+00000ff0: 6c6f 206c 6f63 616c 6c79 2e2e 2e0a 0a60  lo locally.....`
+00001000: 6060 6261 7368 0a67 6974 2063 6c6f 6e65  ``bash.git clone
+00001010: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00001020: 636f 6d2f 6170 6f6c 6c6f 6170 692f 6170  com/apolloapi/ap
+00001030: 6f6c 6c6f 6170 692e 6769 740a 6364 2061  olloapi.git.cd a
+00001040: 706f 6c6c 6f61 7069 2026 2620 7079 7468  polloapi && pyth
+00001050: 6f6e 3320 2d6d 2076 656e 7620 656e 7620  on3 -m venv env 
+00001060: 2626 2073 6f75 7263 6520 656e 762f 6269  && source env/bi
+00001070: 6e2f 6163 7469 7661 7465 2026 2620 7069  n/activate && pi
+00001080: 7020 696e 7374 616c 6c20 2d72 2072 6571  p install -r req
+00001090: 7569 7265 6d65 6e74 732e 7478 740a 6060  uirements.txt.``
+000010a0: 600a 0a2d 2041 6674 6572 2069 6e73 7461  `..- After insta
+000010b0: 6c6c 696e 6720 7379 7374 656d 2064 6570  lling system dep
+000010c0: 656e 6465 6e63 6965 7320 6265 2073 7572  endencies be sur
+000010d0: 6520 746f 2069 6e73 7461 6c6c 2070 7265  e to install pre
+000010e0: 2d63 6f6d 6d69 7420 666f 7220 6c69 6e74  -commit for lint
+000010f0: 2063 6865 636b 730a 0a60 6060 6261 7368   checks..```bash
+00001100: 0a70 6970 2069 6e73 7461 6c6c 2070 7265  .pip install pre
+00001110: 2d63 6f6d 6d69 740a 0a70 7265 2d63 6f6d  -commit..pre-com
+00001120: 6d69 7420 696e 7374 616c 6c0a 0a70 7265  mit install..pre
+00001130: 2d63 6f6d 6d69 7420 7275 6e20 2d2d 616c  -commit run --al
+00001140: 6c2d 6669 6c65 730a 6060 600a 0a41 706f  l-files.```..Apo
+00001150: 6c6c 6f20 7573 6573 2063 6f6d 6d69 7420  llo uses commit 
+00001160: 6d65 7373 6167 6573 2066 6f72 2061 7574  messages for aut
+00001170: 6f6d 6174 6564 2067 656e 6572 6174 696f  omated generatio
+00001180: 6e20 6f66 2070 726f 6a65 6374 2063 6861  n of project cha
+00001190: 6e67 656c 6f67 2e20 466f 7220 6576 6572  ngelog. For ever
+000011a0: 7920 7075 6c6c 2072 6571 7565 7374 2077  y pull request w
+000011b0: 6520 7265 7175 6573 7420 636f 6e74 7269  e request contri
+000011c0: 6275 746f 7273 2074 6f20 6265 2063 6f6d  butors to be com
+000011d0: 706c 6961 6e74 2077 6974 6820 7468 6520  pliant with the 
+000011e0: 666f 6c6c 6f77 696e 6720 636f 6d6d 6974  following commit
+000011f0: 206d 6573 7361 6765 206e 6f74 6174 696f   message notatio
+00001200: 6e2e 0a0a 6060 600a 3c74 7970 653e 3a20  n...```.<type>: 
+00001210: 3c73 756d 6d61 7279 3e0a 0a3c 626f 6479  <summary>..<body
+00001220: 3e0a 6060 600a 0a41 6363 6570 7465 6420  >.```..Accepted 
+00001230: 603c 7479 7065 3e60 2076 616c 7565 733a  `<type>` values:
+00001240: 0a2d 206e 6577 203d 206e 6577 6c79 2069  .- new = newly i
+00001250: 6d70 6c65 6d65 6e74 6564 2075 7365 722d  mplemented user-
+00001260: 6661 6369 6e67 2066 6561 7475 7265 730a  facing features.
+00001270: 2d20 6368 6720 3d20 6368 616e 6765 7320  - chg = changes 
+00001280: 696e 2065 7869 7374 696e 6720 7573 6572  in existing user
+00001290: 2d66 6163 696e 6720 6665 6174 7572 6573  -facing features
+000012a0: 0a2d 2066 6978 203d 2075 7365 722d 6661  .- fix = user-fa
+000012b0: 6369 6e67 2062 7567 6669 7865 730a 2d20  cing bugfixes.- 
+000012c0: 6f74 6820 3d20 6f74 6865 7220 6368 616e  oth = other chan
+000012d0: 6765 7320 7768 6963 6820 7573 6572 7320  ges which users 
+000012e0: 7368 6f75 6c64 206b 6e6f 7720 6162 6f75  should know abou
+000012f0: 740a 2d20 6465 7620 3d20 616e 7920 6465  t.- dev = any de
+00001300: 7665 6c6f 7065 722d 6661 6369 6e67 2063  veloper-facing c
+00001310: 6861 6e67 6573 2c20 7265 6761 7264 6c65  hanges, regardle
+00001320: 7373 206f 6620 6e65 772f 6368 672f 6669  ss of new/chg/fi
+00001330: 7820 7374 6174 7573 0a0a 2323 2323 2053  x status..#### S
+00001340: 756d 6d61 7279 2028 5468 6520 6669 7273  ummary (The firs
+00001350: 7420 6c69 6e65 290a 0a54 6865 2066 6972  t line)..The fir
+00001360: 7374 206c 696e 6520 7368 6f75 6c64 206e  st line should n
+00001370: 6f74 2062 6520 6c6f 6e67 6572 2074 6861  ot be longer tha
+00001380: 6e20 3735 2063 6861 7261 6374 6572 732c  n 75 characters,
+00001390: 2074 6865 2073 6563 6f6e 6420 6c69 6e65   the second line
+000013a0: 2069 7320 616c 7761 7973 2062 6c61 6e6b   is always blank
+000013b0: 2061 6e64 206f 7468 6572 206c 696e 6573   and other lines
+000013c0: 2073 686f 756c 6420 6265 2077 7261 7070   should be wrapp
+000013d0: 6564 2061 7420 3830 2063 6861 7261 6374  ed at 80 charact
+000013e0: 6572 732e 0a0a 2323 20f0 9f94 8d20 4e65  ers...## .... Ne
+000013f0: 6174 2c20 4920 776f 756c 6420 6c69 6b65  at, I would like
+00001400: 2074 6f20 6c65 6172 6e20 6d6f 7265 0a0a   to learn more..
+00001410: e2ad 9020 466f 6c6c 6f77 206f 7572 2064  ... Follow our d
+00001420: 6576 656c 6f70 6d65 6e74 2062 7920 7374  evelopment by st
+00001430: 6172 7269 6e67 2075 7320 6865 7265 206f  arring us here o
+00001440: 6e20 4769 7448 7562 20e2 ad90 0a0a 2d20  n GitHub .....- 
+00001450: 5368 6172 6520 6665 6564 6261 636b 206f  Share feedback o
+00001460: 7220 6173 6b20 7175 6573 7469 6f6e 7320  r ask questions 
+00001470: 6f6e 2074 6865 205b 4469 7363 6f72 6420  on the [Discord 
+00001480: 636f 6d6d 756e 6974 795d 2868 7474 7073  community](https
+00001490: 3a2f 2f64 6973 636f 7264 2e67 672f 5a55  ://discord.gg/ZU
+000014a0: 4837 6637 417a 5559 290a 2d20 5b43 6861  H7f7AzUY).- [Cha
+000014b0: 7420 7769 7468 2061 206d 656d 6265 7220  t with a member 
+000014c0: 6f66 2074 6865 2074 6561 6d5d 2868 7474  of the team](htt
+000014d0: 7073 3a2f 2f61 706f 6c6c 6f61 7069 2e69  ps://apolloapi.i
+000014e0: 6f29 20f0 9f91 8b0a 2d20 4368 6563 6b20  o) .....- Check 
+000014f0: 6f75 7220 5b62 6c6f 6720 6f6e 2054 7275  our [blog on Tru
+00001500: 7374 2026 2053 6166 6574 795d 2868 7474  st & Safety](htt
+00001510: 7073 3a2f 2f77 7777 2e74 6865 6272 6965  ps://www.thebrie
+00001520: 666e 6577 736c 6574 7465 722e 636f 6d29  fnewsletter.com)
+00001530: 0a2d 204c 6f6f 6b20 6174 206f 7572 2064  .- Look at our d
+00001540: 6f63 7320 6f6e 2068 6f77 2074 6f20 6765  ocs on how to ge
+00001550: 7420 7374 6172 7465 6420 5b68 6572 6521  t started [here!
+00001560: 5d28 6874 7470 733a 2f2f 6170 6f6c 6c6f  ](https://apollo
+00001570: 6170 692d 646f 632e 7665 7263 656c 2e61  api-doc.vercel.a
+00001580: 7070 2f29 0a                             pp/).
```

### Comparing `apollo-sdk-0.1.1/apollo/__init__.py` & `apollo-sdk-0.1.2/apollo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from django.utils.module_loading import import_string
 
 
 def get_supabase_client(connection_string) -> AbstractSupabaseClient:
     client = import_string(SUPABASE_CLIENT_CLASS)
     return client(connection_string)
 
+
 def get_firebase_client(service_account_key) -> AbstractFirebaseClient:
     client = import_string(FIREBASE_CLIENT_CLASS)
     return client(service_account_key)
 
+
 def get_json_client() -> AbstractRestClient:
     client = import_string(REST_CLIENT_CLASS)
     return client
```

### Comparing `apollo-sdk-0.1.1/apollo/client.py` & `apollo-sdk-0.1.2/apollo/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,19 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from apollo.resource import General
 from apollo.exceptions import ExecutionError, EmptyResultsWarning
 
 import itertools
-import json
 
 
 class Apollo(General):
-   
     @classmethod
-    def set_context(cls, query_type, table, col):   
+    def set_context(cls, query_type, table, col):
         # oldest order
         if query_type == "asc":
             cls._context[
                 query_type
             ] = f"SELECT * FROM {table} ORDER BY {col} ASC LIMIT 100;"
 
         # newest
@@ -39,21 +37,21 @@
         return cls._context[query_type]
 
     # fetch all available tables
     @classmethod
     def fetch_tables(cls):
         """
         Fetch all the tables for your external resource using Apollo
-        
+
         Args:
         None
-        
+
         Returns:
         list: All the available tables for your resource
-        
+
         Next steps:
         [Success]: Run a query with query
         """
         try:
             response = cls.psql_curs.execute(cls._context["all_tables"])
         except Exception as err:
             raise ExecutionError(err)
@@ -61,20 +59,20 @@
         return list(itertools.chain.from_iterable(response))
 
     # # execute a sql query
     @classmethod
     def query(cls, query_type, table, col):
         """
         Query your external resource using Apollo
-        
+
         Args:
         query_type (str): The sort order for your query
         table (str): The table to query
         col (str): The column to sort by
-        
+
         Returns:
         dict: result of query
         """
         query_string = cls.set_context(query_type, table, col)
 
         try:
             response = cls.psql_curs.execute(query_string)
@@ -83,38 +81,38 @@
 
         return cls._manager.convert_dict(response)
 
     @classmethod
     def connect(cls, db_url, *args, **kwargs):
         """
         Sync data with Apollo to begin building decision trees
-        
+
         Args:
         db_url (str): The database URL to connect to
-        
+
         Returns:
         str: A message indicating that the connection was successful
-        
+
         Next steps:
-        [Success]: Syncing data to Apollo, next steps below; 
+        [Success]: Syncing data to Apollo, next steps below;
             1. Apollo.fetch_tables()
             2. Apollo.query([desc/asc], [table], [column])
         """
         cls.psql_curs = cls._manager.connect_to_prefix(db_url)
         return "Syncing data with Apollo"
-    
+
     @classmethod
     def use(cls, provider, *args, **kwargs):
-        if provider == 'Apollo':
+        if provider == "Apollo":
             cls.model = "Apollo"
             return f"Connected to {provider} provider, using Safety model"
         else:
             return f"Provider {provider} not found"
-    
+
     @classmethod
     def detectText(cls, text, operator, threshold):
         if cls.model:
             print(cls.model)
             conn = cls._service_manager.connect()
-            return conn.make_https_request({'rule': f"{text} {operator} {threshold}"})
+            return conn.make_https_request({"rule": f"{text} {operator} {threshold}"})
         else:
             return "No provider connected"
```

### Comparing `apollo-sdk-0.1.1/apollo/const.py` & `apollo-sdk-0.1.2/apollo/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 
 
 # Supabase support
 SUPABASE_CLIENT_CLASS = os.environ.get(
     "SUPABASE_CLIENT_CLASS", "apollo.database.supabase.SupabaseClient"
 )
 
-# Firebase support 
+# Firebase support
 FIREBASE_CLIENT_CLASS = os.environ.get(
     "FIREBASE_CLIENT_CLASS", "apollo.database.firebase.FirebaseClient"
 )
 
 # Service client
-REST_CLIENT_CLASS = os.environ.get("REST_CLIENT_CLASS", "apollo.service.json.RestClient")
+REST_CLIENT_CLASS = os.environ.get(
+    "REST_CLIENT_CLASS", "apollo.service.json.RestClient"
+)
 
 # Hard code sql queries to prevent injection
 QUERY_CONTEXT = {
     "asc": "",
     "desc": "",
     "all_tables": "select table_name from information_schema.tables where table_schema='public'",
 }
 
 # Test account for firebase
-TEST_ACCOUNT = os.environ.get(
-    "test_account", None
-)
+TEST_ACCOUNT = os.environ.get("test_account", None)
 
-# Service SDK test token, THIS IS PUBLIC 
-test_token = os.environ.get("test_token", "81ecfd535e2d0c402bc84be64f31edcbed643d3e")
+# Service SDK test token, THIS IS PUBLIC
+test_token = os.environ.get("test_token", "81ecfd535e2d0c402bc84be64f31edcbed643d3e")
```

### Comparing `apollo-sdk-0.1.1/apollo/exceptions.py` & `apollo-sdk-0.1.2/apollo/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,44 +9,41 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+
 class SDKException(Exception):
     """The base exception class for all exceptions this library raises."""
+
     def __init__(self, message=None):
         message = self.__class__.__name__ if message is None else message
         super(Exception, self).__init__(message)
 
 
 class AuthorizationFailure(SDKException):
     """Cannot authorize API client."""
-    pass
 
 
 class EndpointException(SDKException):
     """Something is rotten in Service Catalog."""
-    pass
 
 
 class EndpointNotFound(EndpointException):
     """Could not find requested endpoint in Service Catalog."""
-    pass
 
 
 class EmptyCatalog(EndpointNotFound):
     """The service catalog is empty."""
-    pass
 
 
 class NoMatchingPlugin(SDKException):
     """No matching plugins could be created with the provided parameters."""
-    pass
 
 
 class InvalidResponse(SDKException):
     """The response from the server is not valid for this request."""
 
     def __init__(self, response):
         super(InvalidResponse, self).__init__()
@@ -57,25 +54,22 @@
     def __init__(self, message, details=None):
         super(HttpException, self).__init__(message)
         self.details = details
 
 
 class MethodNotSupported(SDKException):
     """The resource does not support this operation type."""
-    pass
 
 
 class ResourceNotFound(SDKException):
     """The requested resource was not found."""
-    pass
 
 
 class DuplicateResource(SDKException):
     """More than one resource exists with that name."""
-    pass
 
 
 class FirebaseConnectionError(Exception):
     """
     There was an error connecting to the firebase client.
     """
 
@@ -96,15 +90,15 @@
     def __init__(self, obj, message="Unable to reach the postgres client"):
         self.obj = obj
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
         return f"{self.obj} [ERR] - {self.message}"
-    
+
 
 class PostgresExecutionError(Exception):
     """
     There was an error connecting to the postgres client.
     """
 
     def __init__(self, obj, message="You're missing a connection string"):
@@ -147,16 +141,14 @@
 
 
 class EmptyResultsWarning(Exception):
     """
     There were no results found.
     """
 
-    def __init__(
-        self, obj, message="Empty query results detected"
-    ):
+    def __init__(self, obj, message="Empty query results detected"):
         self.obj = obj
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
-        return f"{self.obj} -> {self.message}"
+        return f"{self.obj} -> {self.message}"
```

### Comparing `apollo-sdk-0.1.1/apollo/manager.py` & `apollo-sdk-0.1.2/apollo/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from apollo import get_supabase_client, get_firebase_client, get_json_client
 from apollo.exceptions import EmptyResultsWarning
 
+
 class PostgresConnectionManager:
     @staticmethod
     def connect_to_prefix(uri):
         return get_supabase_client(uri)
 
     @staticmethod
     def convert_dict(items):
@@ -34,13 +35,13 @@
         return vector
 
 
 class FirebaseConnectionManager:
     @staticmethod
     def connect_to_prefix(service_account_key):
         return get_firebase_client(service_account_key)
-    
+
 
 class JSONConnectionManager:
     @staticmethod
     def connect():
-        return get_json_client()
+        return get_json_client()
```

### Comparing `apollo-sdk-0.1.1/apollo/resource.py` & `apollo-sdk-0.1.2/apollo/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,36 +9,41 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from apollo.manager import PostgresConnectionManager, FirebaseConnectionManager, JSONConnectionManager
+from apollo.manager import (
+    PostgresConnectionManager,
+    FirebaseConnectionManager,
+    JSONConnectionManager,
+)
 from apollo.const import QUERY_CONTEXT
 
+
 class Postgres:
-    
+
     # Specific sql queries
     _context = QUERY_CONTEXT
-    
+
     # Database utility class
     _manager = PostgresConnectionManager()
-    
+
     # curosr instance
     psql_curs = None
-    
+
 
 class Firebase:
     pass
 
 
 class JSON:
-    
+
     # Service utility class
     _service_manager = JSONConnectionManager()
-    
- 
+
+
 class General(Postgres, JSON):
-    
+
     # Current LLM to be used
     model = None
```

### Comparing `apollo-sdk-0.1.1/apollo_sdk.egg-info/PKG-INFO` & `apollo-sdk-0.1.2/apollo_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: apollo-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Build automated decision making workflows. Aggregate your LLMs all into one place and build from there using one api.
+Home-page: https://github.com/apolloapi/apolloapi
 Author: Apollo API, Inc.
 Author-email: adrbrownx@gmail.com
 License: Elastic License v2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `apollo-sdk-0.1.1/setup.py` & `apollo-sdk-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,44 +10,46 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="apollo-sdk",
-    version="0.1.1",
+    version="0.1.2",
     description="Build automated decision making workflows. Aggregate your LLMs all into one place and build from there using one api.",
     author="Apollo API, Inc.",
     author_email="adrbrownx@gmail.com",
-    packages=["apollo"],
-    license='Elastic License v2',
+    packages=find_packages(),
+    # package_dir={'': ''},
+    url="https://github.com/apolloapi/apolloapi",
+    license="Elastic License v2",
     install_requires=[
-        'Django==4.1.2',
-        'firebase-admin==6.1.0',
-        'grpcio==1.53.0',
-        'httplib2==0.21.0',
-        'protobuf==4.22.3',
-        'psycopg2-binary==2.9.6',
-        'python-dotenv==1.0.0',
-        'psycopg==3.1.6',
-        'requests==2.28.1',
-        'psycopg2==2.9.3',
-        'pytest==7.2.0',
-        'PyJWT==2.6.0',
-        'requests==2.28.1',
-        'six==1.16.0',
-        'sqlparse==0.4.3',
-        'urllib3==1.26.13',
+        "Django==4.1.2",
+        "firebase-admin==6.1.0",
+        "grpcio==1.53.0",
+        "httplib2==0.21.0",
+        "protobuf==4.22.3",
+        "psycopg2-binary==2.9.6",
+        "python-dotenv==1.0.0",
+        "psycopg==3.1.6",
+        "requests==2.28.1",
+        "psycopg2==2.9.3",
+        "pytest==7.2.0",
+        "PyJWT==2.6.0",
+        "requests==2.28.1",
+        "six==1.16.0",
+        "sqlparse==0.4.3",
+        "urllib3==1.26.13",
     ],
     classifiers=[
-        'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
-)
+)
```

